# Comparing `tmp/ansys_dpf_composites-0.4.0.tar.gz` & `tmp/ansys_dpf_composites-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_dpf_composites-0.4.0.tar", max compression
+gzip compressed data, was "ansys_dpf_composites-0.4.1.tar", max compression
```

## Comparing `ansys_dpf_composites-0.4.0.tar` & `ansys_dpf_composites-0.4.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0      356 2024-02-21 08:31:14.209572 ansys_dpf_composites-0.4.0/AUTHORS
--rw-r--r--   0        0        0     1096 2024-02-21 08:31:14.209572 ansys_dpf_composites-0.4.0/LICENSE
--rw-r--r--   0        0        0     6099 2024-02-21 08:31:14.209572 ansys_dpf_composites-0.4.0/README.rst
--rw-r--r--   0        0        0     3807 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1904 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/__init__.py
--rw-r--r--   0        0        0     1908 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_factory.py
--rw-r--r--   0        0        0    34138 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_impl.py
--rw-r--r--   0        0        0    28165 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_impl_2023r2.py
--rw-r--r--   0        0        0     9883 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_indexer.py
--rw-r--r--   0        0        0    13857 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_sampling_point_helpers.py
--rw-r--r--   0        0        0     1291 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_typing_helper.py
--rw-r--r--   0        0        0    18687 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/composite_model.py
--rw-r--r--   0        0        0     2288 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/composite_scope.py
--rw-r--r--   0        0        0     2216 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/constants.py
--rw-r--r--   0        0        0    23304 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/data_sources.py
--rw-r--r--   0        0        0     8373 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/example_helper/__init__.py
--rw-r--r--   0        0        0     2255 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/__init__.py
--rw-r--r--   0        0        0     5451 2024-02-21 08:31:14.213572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
--rw-r--r--   0        0        0     2509 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_core_failure.py
--rw-r--r--   0        0        0     8020 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_cuntze.py
--rw-r--r--   0        0        0     3615 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
--rw-r--r--   0        0        0     3269 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
--rw-r--r--   0        0        0     4226 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_failure_mode_enum.py
--rw-r--r--   0        0        0     4401 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_hashin.py
--rw-r--r--   0        0        0     1784 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_hoffman.py
--rw-r--r--   0        0        0     5207 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_larc.py
--rw-r--r--   0        0        0    10028 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_max_strain.py
--rw-r--r--   0        0        0     5859 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_max_stress.py
--rw-r--r--   0        0        0    10337 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_puck.py
--rw-r--r--   0        0        0     2346 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
--rw-r--r--   0        0        0     3055 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
--rw-r--r--   0        0        0     1795 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
--rw-r--r--   0        0        0     1783 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
--rw-r--r--   0        0        0     3478 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_von_mises.py
--rw-r--r--   0        0        0     2214 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/__init__.py
--rw-r--r--   0        0        0     5697 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
--rw-r--r--   0        0        0     1552 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_enums.py
--rw-r--r--   0        0        0    25212 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_layup_info.py
--rw-r--r--   0        0        0     2635 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_reference_surface.py
--rw-r--r--   0        0        0     5295 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/material_operators.py
--rw-r--r--   0        0        0     9846 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/material_properties.py
--rw-r--r--   0        0        0     4952 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/ply_wise_data.py
--rw-r--r--   0        0        0        0 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/py.typed
--rw-r--r--   0        0        0    12135 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/result_definition.py
--rw-r--r--   0        0        0    25055 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point.py
--rw-r--r--   0        0        0    22353 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point_2023r2.py
--rw-r--r--   0        0        0    13895 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point_types.py
--rw-r--r--   0        0        0     7542 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/select_indices.py
--rw-r--r--   0        0        0     1952 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/__init__.py
--rw-r--r--   0        0        0     4497 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
--rw-r--r--   0        0        0     5274 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_load_plugin.py
--rw-r--r--   0        0        0     4641 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_upload_files_to_server.py
--rw-r--r--   0        0        0     2762 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_versions.py
--rw-r--r--   0        0        0     3063 2024-02-21 08:31:14.217572 ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/unit_system.py
--rw-r--r--   0        0        0     8862 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      356 2024-04-18 14:57:22.175720 ansys_dpf_composites-0.4.1/AUTHORS
+-rw-r--r--   0        0        0     1096 2024-04-18 14:57:22.175720 ansys_dpf_composites-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6099 2024-04-18 14:57:22.175720 ansys_dpf_composites-0.4.1/README.rst
+-rw-r--r--   0        0        0     3820 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1904 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_factory.py
+-rw-r--r--   0        0        0    34916 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_impl.py
+-rw-r--r--   0        0        0    28016 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_impl_2023r2.py
+-rw-r--r--   0        0        0     9883 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_indexer.py
+-rw-r--r--   0        0        0    13857 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_sampling_point_helpers.py
+-rw-r--r--   0        0        0     1291 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_typing_helper.py
+-rw-r--r--   0        0        0    18687 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/composite_model.py
+-rw-r--r--   0        0        0     2288 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/composite_scope.py
+-rw-r--r--   0        0        0     2216 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/constants.py
+-rw-r--r--   0        0        0    23304 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/data_sources.py
+-rw-r--r--   0        0        0     8373 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/example_helper/__init__.py
+-rw-r--r--   0        0        0     2255 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/__init__.py
+-rw-r--r--   0        0        0     5451 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py
+-rw-r--r--   0        0        0     2509 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_core_failure.py
+-rw-r--r--   0        0        0     8020 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_cuntze.py
+-rw-r--r--   0        0        0     3615 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py
+-rw-r--r--   0        0        0     3269 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py
+-rw-r--r--   0        0        0     4226 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_failure_mode_enum.py
+-rw-r--r--   0        0        0     4401 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_hashin.py
+-rw-r--r--   0        0        0     1784 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_hoffman.py
+-rw-r--r--   0        0        0     5207 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_larc.py
+-rw-r--r--   0        0        0    10028 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_max_strain.py
+-rw-r--r--   0        0        0     5859 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_max_stress.py
+-rw-r--r--   0        0        0    10337 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_puck.py
+-rw-r--r--   0        0        0     2346 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py
+-rw-r--r--   0        0        0     3055 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py
+-rw-r--r--   0        0        0     1795 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py
+-rw-r--r--   0        0        0     1783 2024-04-18 14:57:22.179720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py
+-rw-r--r--   0        0        0     3478 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_von_mises.py
+-rw-r--r--   0        0        0     2214 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/__init__.py
+-rw-r--r--   0        0        0     5697 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py
+-rw-r--r--   0        0        0     1552 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_enums.py
+-rw-r--r--   0        0        0    25212 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_layup_info.py
+-rw-r--r--   0        0        0     2635 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_reference_surface.py
+-rw-r--r--   0        0        0     5295 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/material_operators.py
+-rw-r--r--   0        0        0     9846 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/material_properties.py
+-rw-r--r--   0        0        0     4952 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/ply_wise_data.py
+-rw-r--r--   0        0        0        0 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/py.typed
+-rw-r--r--   0        0        0    12135 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/result_definition.py
+-rw-r--r--   0        0        0    25055 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point.py
+-rw-r--r--   0        0        0    22353 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point_2023r2.py
+-rw-r--r--   0        0        0    13895 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point_types.py
+-rw-r--r--   0        0        0     7542 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/select_indices.py
+-rw-r--r--   0        0        0     1952 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/__init__.py
+-rw-r--r--   0        0        0     4497 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py
+-rw-r--r--   0        0        0     5274 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_load_plugin.py
+-rw-r--r--   0        0        0     4641 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_upload_files_to_server.py
+-rw-r--r--   0        0        0     2926 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_versions.py
+-rw-r--r--   0        0        0     3063 2024-04-18 14:57:22.183720 ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/unit_system.py
+-rw-r--r--   0        0        0     8875 1970-01-01 00:00:00.000000 ansys_dpf_composites-0.4.1/PKG-INFO
```

### Comparing `ansys_dpf_composites-0.4.0/LICENSE` & `ansys_dpf_composites-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/README.rst` & `ansys_dpf_composites-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/pyproject.toml` & `ansys_dpf_composites-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 # Check https://python-poetry.org/docs/pyproject/ for all available sections
 name = "ansys-dpf-composites"
-version = "0.4.0"
+version = "0.4.1"
 description = "Post-processing of composite structures based on Ansys DPF"
 license = "MIT"
 authors = ["ANSYS, Inc. <ansys.support@ansys.com>"]
 maintainers = ["PyAnsys developers <pyansys.maintainers@ansys.com>"]
 readme = "README.rst"
 repository = "https://github.com/ansys/pydpf-composites"
 documentation = "https://composites.dpf.docs.pyansys.com"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [
     { include = "ansys", from = "src" },
 ]
```

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/__init__.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_factory.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_factory.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_impl.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 from .layup_info.material_operators import MaterialOperators, get_material_operators
 from .layup_info.material_properties import MaterialProperty, get_constant_property_dict
 from .result_definition import FailureMeasureEnum
 from .sampling_point import SamplingPointNew
 from .server_helpers import (
     upload_continuous_fiber_composite_files_to_server,
     version_equal_or_later,
+    version_older_than,
 )
 from .unit_system import get_unit_system
 
 
 def _deprecated_composite_definition_label(func: Callable[..., Any]) -> Any:
     """Emit a warning when the deprecated ``composite_definition_label`` is used."""
     function_arg = "composite_definition_label"
@@ -494,52 +495,63 @@
                 add_default_data_op.run()
 
             # It is important to evaluate the field here, otherwise the merge operator detects
             # the workflow as changed if upstream operator inputs change
             min_container = minmax_el_op.outputs.field_min()
             max_container = minmax_el_op.outputs.field_max()
 
-            converter_op = dpf.Operator("composite::failure_measure_converter")
-            converter_op.inputs.fields_container(min_container)
-            converter_op.inputs.measure_type(measure.value)
-            converter_op.run()
-
-            converter_op.inputs.fields_container(max_container)
-            converter_op.run()
-
             min_merger.connect(merge_index, min_container)
             max_merger.connect(merge_index, max_container)
             merge_index = merge_index + 1
 
         if merge_index == 0:
             raise RuntimeError("No output is generated! Check the scope (element and ply IDs).")
 
         if self._supports_reference_surface_operators():
+            overall_max_container = max_merger.outputs.merged_fields_container()
+
             self._map_to_reference_surface_operator.inputs.min_container(
                 min_merger.outputs.merged_fields_container()
             )
-            self._map_to_reference_surface_operator.inputs.max_container(
-                max_merger.outputs.merged_fields_container()
+            self._map_to_reference_surface_operator.inputs.max_container(overall_max_container)
+
+            ref_surface_max_container = (
+                self._map_to_reference_surface_operator.outputs.max_container()
             )
 
-            if measure == FailureMeasureEnum.INVERSE_RESERVE_FACTOR:
-                return _merge_containers(
-                    max_merger.outputs.merged_fields_container(),
-                    self._map_to_reference_surface_operator.outputs.max_container(),
-                )
-            else:
-                return _merge_containers(
-                    min_merger.outputs.merged_fields_container(),
-                    self._map_to_reference_surface_operator.outputs.min_container(),
-                )
+            converter_op = dpf.Operator("composite::failure_measure_converter")
+            converter_op.inputs.measure_type(measure.value)
+            converter_op.inputs.fields_container(overall_max_container)
+            converter_op.run()
+            converter_op.inputs.fields_container(ref_surface_max_container)
+            converter_op.run()
+
+            if version_older_than(self._server, "8.2"):
+                # For versions before 8.2, the Reference Surface suffix
+                # is not correctly preserved by the failure_measure_converter
+                # We add the suffix manually here.
+                for field in ref_surface_max_container:
+                    if (
+                        field.name.startswith("IRF")
+                        or field.name.startswith("SF")
+                        or field.name.startswith("SM")
+                    ):
+                        assert not field.name.endswith(REF_SURFACE_NAME)
+                        # Set name in field definition, because setting
+                        # the name directly is not supported for older dpf versions
+                        field_definition = field.field_definition
+                        field_definition.name = field_definition.name + " " + REF_SURFACE_NAME
+
+            return _merge_containers(overall_max_container, ref_surface_max_container)
         else:
-            if measure == FailureMeasureEnum.INVERSE_RESERVE_FACTOR:
-                return max_merger.outputs.merged_fields_container()
-            else:
-                return min_merger.outputs.merged_fields_container()
+            converter_op = dpf.Operator("composite::failure_measure_converter")
+            converter_op.inputs.measure_type(measure.value)
+            converter_op.inputs.fields_container(max_merger.outputs.merged_fields_container())
+            converter_op.run()
+            return max_container
 
     @_deprecated_composite_definition_label
     def get_sampling_point(
         self,
         combined_criterion: CombinedFailureCriterion,
         element_id: int,
         time: Optional[float] = None,
```

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_composite_model_impl_2023r2.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_composite_model_impl_2023r2.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,18 +332,15 @@
             measure=measure.value,
         )
         failure_operator = dpf.Operator("composite::composite_failure_operator")
         failure_operator.inputs.unit_system(self._unit_system)
 
         failure_operator.inputs.result_definition(rd.to_json())
 
-        if measure == FailureMeasureEnum.INVERSE_RESERVE_FACTOR:
-            return failure_operator.outputs.fields_containerMax()
-        else:
-            return failure_operator.outputs.fields_containerMin()
+        return failure_operator.outputs.fields_containerMax()
 
     def get_sampling_point(
         self,
         combined_criterion: CombinedFailureCriterion,
         element_id: int,
         time: Optional[float] = None,
         composite_definition_label: Optional[str] = None,
```

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_indexer.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_indexer.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_sampling_point_helpers.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_sampling_point_helpers.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/_typing_helper.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/_typing_helper.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/composite_model.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/composite_model.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/composite_scope.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/composite_scope.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/constants.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/data_sources.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/data_sources.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/example_helper/__init__.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/example_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/__init__.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_combined_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_core_failure.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_core_failure.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_cuntze.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_cuntze.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_face_sheet_wrinkling.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_failure_criterion_base.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_failure_mode_enum.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_failure_mode_enum.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_hashin.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_hashin.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_hoffman.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_hoffman.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_larc.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_larc.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_max_strain.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_max_strain.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_max_stress.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_max_stress.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_puck.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_puck.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_quadratic_failure_criterion.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_shear_crimping.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_tsai_hill.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_tsai_wu.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/failure_criteria/_von_mises.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/failure_criteria/_von_mises.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/__init__.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_add_layup_info_to_mesh.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_enums.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_enums.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_layup_info.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_layup_info.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/_reference_surface.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/_reference_surface.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/material_operators.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/material_operators.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/layup_info/material_properties.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/layup_info/material_properties.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/ply_wise_data.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/ply_wise_data.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/result_definition.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/result_definition.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point_2023r2.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point_2023r2.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/sampling_point_types.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/sampling_point_types.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/select_indices.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/select_indices.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/__init__.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_connect_to_or_start_server.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_load_plugin.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_load_plugin.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_upload_files_to_server.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_upload_files_to_server.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/server_helpers/_versions.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/server_helpers/_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,19 @@
     ),
     "8.0": _DpfVersionInfo(
         "8.0",
         "2024 R2 pre 0",
         "DPF Composites: reference surface support and \
                                                    section data from RST",
     ),
+    "8.2": _DpfVersionInfo(
+        "8.2",
+        "2024 R2 pre 2",
+        "DPF Composites: Failure measure conversion preserves Reference Surface suffix",
+    ),
 }
 
 
 def _check_key(ver: str) -> None:
     if ver not in _DPF_VERSIONS.keys():
         msg = ", ".join([f"{index}:{ver.server_version}" for index, ver in _DPF_VERSIONS.items()])
         raise RuntimeError(f"Invalid key `{ver}`. Allowed values are {msg}.")
```

### Comparing `ansys_dpf_composites-0.4.0/src/ansys/dpf/composites/unit_system.py` & `ansys_dpf_composites-0.4.1/src/ansys/dpf/composites/unit_system.py`

 * *Files identical despite different names*

### Comparing `ansys_dpf_composites-0.4.0/PKG-INFO` & `ansys_dpf_composites-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ansys-dpf-composites
-Version: 0.4.0
+Version: 0.4.1
 Summary: Post-processing of composite structures based on Ansys DPF
 Home-page: https://github.com/ansys/pydpf-composites
 License: MIT
 Author: ANSYS, Inc.
 Author-email: ansys.support@ansys.com
 Maintainer: PyAnsys developers
 Maintainer-email: pyansys.maintainers@ansys.com
 Requires-Python: >=3.9,<3.13
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

