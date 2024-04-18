# Comparing `tmp/pdm_backend-2.2.0.tar.gz` & `tmp/pdm_backend-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_backend-2.2.0.tar", last modified: Sun Apr 14 07:54:48 2024, max compression
+gzip compressed data, was "pdm_backend-2.2.1.tar", last modified: Thu Apr 18 03:32:59 2024, max compression
```

## Comparing `pdm_backend-2.2.0.tar` & `pdm_backend-2.2.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
--rw-r--r--   0        0        0     1067 2024-04-14 07:54:30.319984 pdm_backend-2.2.0/LICENSE
--rw-r--r--   0        0        0     1711 2024-04-14 07:54:30.319984 pdm_backend-2.2.0/README.md
--rw-r--r--   0        0        0     2326 2024-04-14 07:54:48.572017 pdm_backend-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3286 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      197 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      496 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     9590 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2676 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0    10347 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5292 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8208 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/markers.py
--rw-r--r--   0        0        0    33036 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/metadata.py
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     2933 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39824 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18950 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     5268 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16256 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1113 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    20891 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/py.typed
--rw-r--r--   0        0        0     1072 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/LICENSE
--rw-r--r--   0        0        0      396 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0       26 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/py.typed
--rw-r--r--   0        0        0     1072 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/LICENSE
--rw-r--r--   0        0        0      177 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/__init__.py
--rw-r--r--   0        0        0     6132 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/_writer.py
--rw-r--r--   0        0        0       26 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/py.typed
--rw-r--r--   0        0        0       73 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/_vendor/vendor.txt
--rw-r--r--   0        0        0    12629 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/base.py
--rw-r--r--   0        0        0     9872 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/config.py
--rw-r--r--   0        0        0     3674 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/editable.py
--rw-r--r--   0        0        0      452 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/exceptions.py
--rw-r--r--   0        0        0      108 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/__init__.py
--rw-r--r--   0        0        0     4593 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/base.py
--rw-r--r--   0        0        0     6459 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/setuptools.py
--rw-r--r--   0        0        0     5296 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/version/__init__.py
--rw-r--r--   0        0        0    10153 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/hooks/version/scm.py
--rw-r--r--   0        0        0     1037 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/intree.py
--rw-r--r--   0        0        0    14959 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/macosx_platform.py
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/py.typed
--rw-r--r--   0        0        0     3050 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/sdist.py
--rw-r--r--   0        0        0     1381 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/structures.py
--rw-r--r--   0        0        0     8985 2024-04-14 07:54:30.323984 pdm_backend-2.2.0/src/pdm/backend/utils.py
--rw-r--r--   0        0        0    11818 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/src/pdm/backend/wheel.py
--rw-r--r--   0        0        0       72 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0      929 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/conftest.py
--rw-r--r--   0        0        0      856 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/hook_class.py
--rw-r--r--   0        0        0      599 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/hook_module.py
--rw-r--r--   0        0        0      599 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/hooks/local_hook.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/LICENSE
--rw-r--r--   0        0        0      138 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
--rw-r--r--   0        0        0      234 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
--rw-r--r--   0        0        0      558 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
--rw-r--r--   0        0        0      478 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/LICENSE
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/my_package/__init__.py
--rw-r--r--   0        0        0      478 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
--rw-r--r--   0        0        0      138 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pdm.lock
--rw-r--r--   0        0        0      230 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pdm_build.py
--rw-r--r--   0        0        0      554 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/LICENSE
--rw-r--r--   0        0        0       26 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      379 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
--rw-r--r--   0        0        0      433 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/LICENSE
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/README.md
--rw-r--r--   0        0        0      407 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-metadata-test/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       60 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      402 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/README.md
--rw-r--r--   0        0        0      406 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-license/src/foo_module.py
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/README.md
-lrwxr-xr-x   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
--rw-r--r--   0        0        0      330 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-no-version/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/data_out.json
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pdm.lock
--rw-r--r--   0        0        0      555 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/single_module.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/data_out.json
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pdm.lock
--rw-r--r--   0        0        0      642 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt
--rwxr-xr-x   0        0        0       32 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/single_module.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/README.md
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
--rw-r--r--   0        0        0      574 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/README.md
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
--rw-r--r--   0        0        0     7700 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock
--rw-r--r--   0        0        0      513 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/data.json
--rwxr-xr-x   0        0        0        0 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/my_package/executable
--rw-r--r--   0        0        0     2461 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      598 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0     4259 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      604 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/README.md
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
--rw-r--r--   0        0        0        3 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
--rw-r--r--   0        0        0      464 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-pep420-package/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/LICENSE
--rw-r--r--   0        0        0      277 2024-04-14 07:54:30.327984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/my_build.py
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
--rw-r--r--   0        0        0      138 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
--rw-r--r--   0        0        0      549 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
--rw-r--r--   0        0        0       26 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/README.md
--rw-r--r--   0        0        0      413 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/data_out.json
--rw-r--r--   0        0        0      500 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/single_module.py
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      395 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/README.md
--rw-r--r--   0        0        0      406 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
--rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
--rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/.gitignore
--rw-r--r--   0        0        0       12 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/LICENSE
--rw-r--r--   0        0        0       24 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/README.md
--rw-r--r--   0        0        0       36 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/foo/__init__.py
--rw-r--r--   0        0        0      369 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/pyproject.toml
--rw-r--r--   0        0        0      156 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/fixtures/projects/demo-using-scm/version.py
--rw-r--r--   0        0        0    20060 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_api.py
--rw-r--r--   0        0        0     5324 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_file_finder.py
--rw-r--r--   0        0        0     1632 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_hooks.py
--rw-r--r--   0        0        0     3058 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_metadata.py
--rw-r--r--   0        0        0      748 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     1176 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/test_wheel.py
--rw-r--r--   0        0        0      318 2024-04-14 07:54:30.331984 pdm_backend-2.2.0/tests/testutils.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdm_backend-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1711 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/README.md
+-rw-r--r--   0        0        0     2326 2024-04-18 03:32:59.568298 pdm_backend-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3286 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      496 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     9590 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2676 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10347 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    33036 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     2933 2024-04-18 03:32:51.168273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39824 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18950 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     5268 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16256 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1113 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    21011 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/LICENSE
+-rw-r--r--   0        0        0      396 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/py.typed
+-rw-r--r--   0        0        0     1072 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/LICENSE
+-rw-r--r--   0        0        0      177 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/__init__.py
+-rw-r--r--   0        0        0     6132 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/_writer.py
+-rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/py.typed
+-rw-r--r--   0        0        0       70 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/_vendor/vendor.txt
+-rw-r--r--   0        0        0    12629 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/base.py
+-rw-r--r--   0        0        0     9872 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/config.py
+-rw-r--r--   0        0        0     3674 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/editable.py
+-rw-r--r--   0        0        0      452 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/exceptions.py
+-rw-r--r--   0        0        0      108 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/__init__.py
+-rw-r--r--   0        0        0     4593 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/base.py
+-rw-r--r--   0        0        0     6459 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/setuptools.py
+-rw-r--r--   0        0        0     5296 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/version/__init__.py
+-rw-r--r--   0        0        0    10153 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/hooks/version/scm.py
+-rw-r--r--   0        0        0     1037 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/intree.py
+-rw-r--r--   0        0        0    14959 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/macosx_platform.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/py.typed
+-rw-r--r--   0        0        0     3050 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/sdist.py
+-rw-r--r--   0        0        0     1381 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/structures.py
+-rw-r--r--   0        0        0     8985 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/utils.py
+-rw-r--r--   0        0        0    12797 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/src/pdm/backend/wheel.py
+-rw-r--r--   0        0        0       72 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      929 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      856 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/hook_class.py
+-rw-r--r--   0        0        0      599 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/hook_module.py
+-rw-r--r--   0        0        0      599 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/hooks/local_hook.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/LICENSE
+-rw-r--r--   0        0        0      138 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pdm.lock
+-rw-r--r--   0        0        0      234 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pdm_build.py
+-rw-r--r--   0        0        0      558 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/src/my_package/hellomodule.c
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/LICENSE
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/my_package/__init__.py
+-rw-r--r--   0        0        0      478 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/my_package/hellomodule.c
+-rw-r--r--   0        0        0      138 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pdm.lock
+-rw-r--r--   0        0        0      230 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pdm_build.py
+-rw-r--r--   0        0        0      554 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/LICENSE
+-rw-r--r--   0        0        0       26 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      379 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/foo/my_package/data.json
+-rw-r--r--   0        0        0      433 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-explicit-package-dir/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/README.md
+-rw-r--r--   0        0        0      407 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-metadata-test/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       60 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      402 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/README.md
+-rw-r--r--   0        0        0      406 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-license/src/foo_module.py
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/anothername.toml -> pyproject.toml
+-rw-r--r--   0        0        0      330 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-no-version/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.172273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pdm.lock
+-rw-r--r--   0        0        0      555 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pdm.lock
+-rw-r--r--   0        0        0      642 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt
+-rwxr-xr-x   0        0        0       32 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/scripts/data/my_script.sh
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/README.md
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_a.json
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/my_package/data/data_inner/data_b.json
+-rw-r--r--   0        0        0      574 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/README.md
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/my_package/data.json
+-rw-r--r--   0        0        0     7700 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock
+-rw-r--r--   0        0        0      513 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/tests/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/data.json
+-rwxr-xr-x   0        0        0        0 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/my_package/executable
+-rw-r--r--   0        0        0     2461 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      598 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0     4259 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      604 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/README.md
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/foo/my_package/data.json
+-rw-r--r--   0        0        0      464 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-pep420-package/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/LICENSE
+-rw-r--r--   0        0        0      277 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/my_build.py
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/my_package/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pdm.lock
+-rw-r--r--   0        0        0      549 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/README.md
+-rw-r--r--   0        0        0      413 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-reuse-spec/src/foo_module.py
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/data_out.json
+-rw-r--r--   0        0        0      500 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package-include/sub/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      395 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/README.md
+-rw-r--r--   0        0        0      406 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/pyproject.toml
+-rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-src-pymodule/src/foo_module.py
+-rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/.gitignore
+-rw-r--r--   0        0        0       12 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/LICENSE
+-rw-r--r--   0        0        0       24 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/README.md
+-rw-r--r--   0        0        0       36 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/foo/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/fixtures/projects/demo-using-scm/version.py
+-rw-r--r--   0        0        0    21084 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_api.py
+-rw-r--r--   0        0        0     5324 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_file_finder.py
+-rw-r--r--   0        0        0     1632 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_hooks.py
+-rw-r--r--   0        0        0     3058 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_metadata.py
+-rw-r--r--   0        0        0      748 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1176 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/test_wheel.py
+-rw-r--r--   0        0        0      318 2024-04-18 03:32:51.176273 pdm_backend-2.2.1/tests/testutils.py
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 pdm_backend-2.2.1/PKG-INFO
```

### Comparing `pdm_backend-2.2.0/LICENSE` & `pdm_backend-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/README.md` & `pdm_backend-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/pyproject.toml` & `pdm_backend-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "importlib-metadata>=3.6; python_version < \"3.10\"",
 ]
-version = "2.2.0"
+version = "2.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/pdm-project/pdm-backend"
 Repository = "https://github.com/pdm-project/pdm-backend"
```

### Comparing `pdm_backend-2.2.0/src/pdm/backend/__init__.py` & `pdm_backend-2.2.1/src/pdm/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.APACHE` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/LICENSE.BSD` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_elffile.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_manylinux.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_musllinux.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_parser.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_structures.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/_tokenizer.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/markers.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/metadata.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/requirements.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/specifiers.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/tags.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/utils.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/packaging/version.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/LICENSE` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/pyproject_metadata/__init__.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/pyproject_metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 import collections
 import copy
 import dataclasses
 import email.utils
 import os
 import os.path
 import pathlib
+import sys
 import typing
 
 
 if typing.TYPE_CHECKING:
     from collections.abc import Mapping
     from typing import Any
 
     from pdm.backend._vendor.packaging.requirements import Requirement
 
+    if sys.version_info < (3, 11):
+        from typing_extensions import Self
+    else:
+        from typing import Self
+
 import pdm.backend._vendor.packaging.markers as pkg_markers
 import pdm.backend._vendor.packaging.requirements as pkg_requirements
 import pdm.backend._vendor.packaging.specifiers as pkg_specifiers
 import pdm.backend._vendor.packaging.utils as pkg_utils
 import pdm.backend._vendor.packaging.version as pkg_version
 
 
-__version__ = '0.8.0rc1'
+__version__ = '0.8.0'
 
 KNOWN_METADATA_VERSIONS = {'2.1', '2.2', '2.3'}
 
 
 class ConfigurationError(Exception):
     '''Error in the backend metadata.'''
     def __init__(self, msg: str, *, key: str | None = None):
@@ -200,30 +206,30 @@
 
     @classmethod
     def from_pyproject(
         cls,
         data: Mapping[str, Any],
         project_dir: str | os.PathLike[str] = os.path.curdir,
         metadata_version: str | None = None,
-    ) -> StandardMetadata:
+    ) -> Self:
         fetcher = DataFetcher(data)
         project_dir = pathlib.Path(project_dir)
 
         if 'project' not in fetcher:
             msg = 'Section "project" missing in pyproject.toml'
             raise ConfigurationError(msg)
 
         dynamic = fetcher.get_list('project.dynamic')
         if 'name' in dynamic:
             msg = 'Unsupported field "name" in "project.dynamic"'
             raise ConfigurationError(msg)
 
         for field in dynamic:
             if field in data['project']:
-                msg = f'Field "project.{field}" declared as dynamic in but is defined'
+                msg = f'Field "project.{field}" declared as dynamic in "project.dynamic" but is defined'
                 raise ConfigurationError(msg)
 
         name = fetcher.get_str('project.name')
         if not name:
             msg = 'Field "project.name" missing'
             raise ConfigurationError(msg)
 
@@ -231,19 +237,18 @@
         requires_python_string = fetcher.get_str('project.requires-python')
         version = pkg_version.Version(version_string) if version_string else None
 
         if version is None and 'version' not in dynamic:
             msg = 'Field "project.version" missing and "version" not specified in "project.dynamic"'
             raise ConfigurationError(msg)
 
-        # Description can't be multiline
+        # Description fills Summary, which cannot be multiline
+        # However, throwing an error isn't backward compatible,
+        # so leave it up to the users for now.
         description = fetcher.get_str('project.description')
-        if description and '\n' in description:
-            msg = 'The description must be a single line'
-            raise ConfigurationError(msg)
 
         if metadata_version and metadata_version not in KNOWN_METADATA_VERSIONS:
             msg = f'The metadata_version must be one of {KNOWN_METADATA_VERSIONS} or None (default)'
             raise ConfigurationError(msg)
 
         return cls(
             name,
```

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/LICENSE` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_parser.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli/_re.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/LICENSE` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/_vendor/tomli_w/_writer.py` & `pdm_backend-2.2.1/src/pdm/backend/_vendor/tomli_w/_writer.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/base.py` & `pdm_backend-2.2.1/src/pdm/backend/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/config.py` & `pdm_backend-2.2.1/src/pdm/backend/config.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/editable.py` & `pdm_backend-2.2.1/src/pdm/backend/editable.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/hooks/base.py` & `pdm_backend-2.2.1/src/pdm/backend/hooks/base.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/hooks/setuptools.py` & `pdm_backend-2.2.1/src/pdm/backend/hooks/setuptools.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/hooks/version/__init__.py` & `pdm_backend-2.2.1/src/pdm/backend/hooks/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/hooks/version/scm.py` & `pdm_backend-2.2.1/src/pdm/backend/hooks/version/scm.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/intree.py` & `pdm_backend-2.2.1/src/pdm/backend/intree.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/macosx_platform.py` & `pdm_backend-2.2.1/src/pdm/backend/macosx_platform.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/sdist.py` & `pdm_backend-2.2.1/src/pdm/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/structures.py` & `pdm_backend-2.2.1/src/pdm/backend/structures.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/utils.py` & `pdm_backend-2.2.1/src/pdm/backend/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/src/pdm/backend/wheel.py` & `pdm_backend-2.2.1/src/pdm/backend/wheel.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import zipfile
 from base64 import urlsafe_b64encode
 from pathlib import Path
 from typing import IO, Any, Iterable, Mapping, NamedTuple, cast
 
 from pdm.backend._vendor.packaging import tags
 from pdm.backend._vendor.packaging.specifiers import SpecifierSet
-from pdm.backend._vendor.packaging.utils import canonicalize_name
+from pdm.backend._vendor.packaging.utils import _build_tag_regex, canonicalize_name
 from pdm.backend.base import Builder
 from pdm.backend.hooks import Context
 from pdm.backend.hooks.setuptools import SetuptoolsBuildHook
 from pdm.backend.structures import FileMap
 from pdm.backend.utils import (
     get_abi_tag,
     get_platform,
@@ -42,14 +42,16 @@
 WHEEL_FILE_FORMAT = """\
 Wheel-Version: 1.0
 Generator: pdm-backend ({version})
 Root-Is-Purelib: {is_purelib}
 Tag: {tag}
 """
 
+BUILD_TAG_FORMAT = "Build: {build_number}"
+
 # Fix the date time for reproducible builds
 try:
     _env_date = time.gmtime(int(os.environ["SOURCE_DATE_EPOCH"]))[:6]
 except (ValueError, KeyError):
     ZIPINFO_DATE_TIME = (2016, 1, 1, 0, 0, 0)
 else:
     if _env_date[0] < 1980:
@@ -73,14 +75,15 @@
     hooks = Builder.hooks + [SetuptoolsBuildHook()]
 
     def __init__(
         self, location: str | Path, config_settings: Mapping[str, Any] | None = None
     ) -> None:
         super().__init__(location, config_settings)
         self.__tag: str | None = None
+        self.__build_number: str | None = None
 
     def scheme_path(self, name: str, relative: str) -> str:
         if name not in SCHEME_NAMES:
             raise ValueError(
                 f"Unknown scheme name {name!r}, must be one of {SCHEME_NAMES}"
             )
         return f"{self.name_version}.data/{name}/{relative}"
@@ -152,36 +155,58 @@
 
         with os.fdopen(fd, "w+b") as fp:
             with zipfile.ZipFile(fp, "w", compression=zipfile.ZIP_DEFLATED) as zf:
                 for rel_path, full_path in files:
                     records.append(self._add_file_to_zip(zf, rel_path, full_path))
                 self._write_record(zf, records)
 
-        target = context.dist_dir / f"{self.name_version}-{self.tag}.whl"
+        name_version = self.name_version
+        if self.build_number:
+            name_version = f"{name_version}-{self.build_number}"
+
+        target = context.dist_dir / f"{name_version}-{self.tag}.whl"
         if target.exists():
             target.unlink()
         shutil.move(temp_name, target)
         return target
 
     @property
     def name_version(self) -> str:
         name = to_filename(canonicalize_name(self.config.metadata["name"]))
         version = to_filename(safe_version(self.config.metadata["version"]))
         return f"{name}-{version}"
 
     @property
+    def build_number(self) -> str | None:
+        if not self.__build_number:
+            self.__build_number = self._get_build_number()
+        return self.__build_number
+
+    @property
     def dist_info_name(self) -> str:
         return f"{self.name_version}.dist-info"
 
     @property
     def tag(self) -> str:
         if self.__tag is None:
             self.__tag = self._get_tag()
         return self.__tag
 
+    def _get_build_number(self) -> str | None:
+        cmd = "--build-number"
+        if cmd not in self.config_settings:
+            return None
+        build_number = self.config_settings[cmd]
+        if not _build_tag_regex.match(build_number):
+            raise ValueError(
+                f"Invalid build number: {build_number}, please refer to PEP 427"
+            )
+
+        return build_number
+
     def _get_tag(self) -> str:
         impl, abi, platform = self._get_platform_tags()
         is_purelib = self.config.build_config.is_purelib
         if not is_purelib:
             if not platform:
                 platform = get_platform(self.location / "build")
             if not impl:
@@ -272,20 +297,23 @@
 
     def _write_wheel_file(self, fp: IO[str], is_purelib: bool) -> None:
         try:
             version = get_version("pdm-backend")
         except ModuleNotFoundError:
             version = "0.0.0+local"
 
-        fp.write(
-            WHEEL_FILE_FORMAT.format(
-                is_purelib=str(is_purelib).lower(), tag=self.tag, version=version
-            )
+        wheel_metadata = WHEEL_FILE_FORMAT.format(
+            is_purelib=str(is_purelib).lower(), tag=self.tag, version=version
         )
 
+        if self.build_number:
+            wheel_metadata = f"{wheel_metadata}{BUILD_TAG_FORMAT.format(build_number=self.build_number)}"
+
+        fp.write(wheel_metadata)
+
     def _write_entry_points(
         self, fp: IO[str], entry_points: dict[str, dict[str, str]]
     ) -> None:
         for group_name in sorted(entry_points):
             fp.write(f"[{group_name}]\n")
             for name, value in sorted(entry_points[group_name].items()):
                 fp.write(f"{name} = {value}\n")
```

### Comparing `pdm_backend-2.2.0/tests/conftest.py` & `pdm_backend-2.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/hooks/hook_class.py` & `pdm_backend-2.2.1/tests/fixtures/hooks/hook_class.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/hooks/hook_module.py` & `pdm_backend-2.2.1/tests/fixtures/hooks/hook_module.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/hooks/local_hook.py` & `pdm_backend-2.2.1/tests/fixtures/hooks/local_hook.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension-in-src/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-cextension/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-cextension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pdm.lock` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include-error/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pdm.lock` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-include/requirements_simple.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-include/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-deep-path/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pdm.lock` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package-with-tests/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package-with-tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pdm.lock` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-package/requirements_simple.txt` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-package/requirements_simple.txt`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml` & `pdm_backend-2.2.1/tests/fixtures/projects/demo-purelib-with-build/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/test_api.py` & `pdm_backend-2.2.1/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,40 @@
 
     for name in ("pyproject.toml", "LICENSE"):
         assert name not in zip_names
 
     assert "demo_module-0.1.0.dist-info/licenses/LICENSE" in zip_names
 
 
+@pytest.mark.parametrize("name", ["demo-module"])
+def test_build_single_module_with_build_number(dist: Path) -> None:
+    build_number = "20231241"
+    wheel_name = api.build_wheel(
+        dist.as_posix(),
+        config_settings={"--build-number": build_number},
+    )
+    assert wheel_name == f"demo_module-0.1.0-{build_number}-py3-none-any.whl"
+    with zipfile.ZipFile(dist / wheel_name) as zf:
+        wheel_metadata = email.message_from_bytes(
+            zf.read("demo_module-0.1.0.dist-info/WHEEL")
+        )
+        assert wheel_metadata["Build"] == build_number
+
+
+@pytest.mark.parametrize("name", ["demo-module"])
+def test_build_single_module_without_build_number(dist: Path) -> None:
+    wheel_name = api.build_wheel(dist.as_posix())
+    assert wheel_name == "demo_module-0.1.0-py3-none-any.whl"
+    with zipfile.ZipFile(dist / wheel_name) as zf:
+        wheel_metadata = email.message_from_bytes(
+            zf.read("demo_module-0.1.0.dist-info/WHEEL")
+        )
+        assert "Build" not in wheel_metadata
+
+
 @pytest.mark.parametrize("name", ["demo-package"])
 def test_build_package(dist: Path) -> None:
     wheel_name = api.build_wheel(dist.as_posix())
     sdist_name = api.build_sdist(dist.as_posix())
     assert sdist_name == "demo_package-0.1.0.tar.gz"
     assert wheel_name == "demo_package-0.1.0-py2.py3-none-any.whl"
```

### Comparing `pdm_backend-2.2.0/tests/test_file_finder.py` & `pdm_backend-2.2.1/tests/test_file_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/test_hooks.py` & `pdm_backend-2.2.1/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/test_metadata.py` & `pdm_backend-2.2.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/test_utils.py` & `pdm_backend-2.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/tests/test_wheel.py` & `pdm_backend-2.2.1/tests/test_wheel.py`

 * *Files identical despite different names*

### Comparing `pdm_backend-2.2.0/PKG-INFO` & `pdm_backend-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-backend
-Version: 2.2.0
+Version: 2.2.1
 Summary: The build backend used by PDM that supports latest packaging standards
 Keywords: packaging,PEP 517,build
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm-backend Version: 2.2.0 Summary: The build
+Metadata-Version: 2.1 Name: pdm-backend Version: 2.2.1 Summary: The build
 backend used by PDM that supports latest packaging standards Keywords:
 packaging,PEP 517,build Author-Email: Frost Ming
 frostming.com> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

