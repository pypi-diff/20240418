# Comparing `tmp/flow360-24.2.2.tar.gz` & `tmp/flow360-24.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-24.2.2.tar", max compression
+gzip compressed data, was "flow360-24.2.3.tar", max compression
```

## Comparing `flow360-24.2.2.tar` & `flow360-24.2.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    26526 2024-04-11 12:21:01.934429 flow360-24.2.2/LICENSE
--rw-r--r--   0        0        0     3514 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/__init__.py
--rw-r--r--   0        0        0     5665 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/accounts_utils.py
--rw-r--r--   0        0        0       54 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2590 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/app.py
--rw-r--r--   0        0        0      580 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/dict_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3683 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     2579 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/requests.py
--rw-r--r--   0        0        0     1191 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0    12039 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      262 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/security.py
--rw-r--r--   0        0        0     1076 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/utils.py
--rw-r--r--   0        0        0      223 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/webbrowser.py
--rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/__init__.py
--rw-r--r--   0        0        0    30720 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/case.py
--rw-r--r--   0        0        0     3907 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/compress_upload.py
--rw-r--r--   0        0        0      142 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/__init__.py
--rw-r--r--   0        0        0     9264 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/boundaries.py
--rw-r--r--   0        0        0     8474 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/conversions.py
--rw-r--r--   0        0        0      438 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/exposed_units.py
--rw-r--r--   0        0        0     4394 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/flow360_fields.py
--rw-r--r--   0        0        0     2428 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/flow360_legacy.py
--rw-r--r--   0        0        0    29693 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/flow360_output.py
--rw-r--r--   0        0        0    66368 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0     1065 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/initial_condition.py
--rw-r--r--   0        0        0    45016 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     1337 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/params_utils.py
--rw-r--r--   0        0        0     3069 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/physical_properties.py
--rw-r--r--   0        0        0    26021 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0     5400 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/time_stepping.py
--rw-r--r--   0        0        0    11560 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/turbulence_quantities.py
--rw-r--r--   0        0        0    37382 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/unit_system.py
--rw-r--r--   0        0        0     2748 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/updater.py
--rw-r--r--   0        0        0    19271 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/validations.py
--rw-r--r--   0        0        0     8065 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/volume_zones.py
--rw-r--r--   0        0        0     5547 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/folder.py
--rw-r--r--   0        0        0      860 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/interfaces.py
--rw-r--r--   0        0        0      221 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6891 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/meshing/params.py
--rw-r--r--   0        0        0    20417 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/resource_base.py
--rw-r--r--   0        0        0    28333 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/results/case_results.py
--rw-r--r--   0        0        0     9401 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2291 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/types.py
--rw-r--r--   0        0        0     4601 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/utils.py
--rw-r--r--   0        0        0     3246 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/validator.py
--rw-r--r--   0        0        0    25053 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     3407 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/environment.py
--rw-r--r--   0        0        0     2036 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/error_messages.py
--rw-r--r--   0        0        0      384 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/__init__.py
--rw-r--r--   0        0        0     3877 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      446 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      291 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5356 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157799 2024-04-11 12:21:01.946429 flow360-24.2.2/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1157977 2024-04-11 12:21:01.950429 flow360-24.2.2/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1157978 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      431 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      431 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/bet_line.py
--rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence/Flow360Mesh.json
--rw-r--r--   0        0        0     1596 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence/flow360.json
--rw-r--r--   0        0        0      372 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence.py
--rw-r--r--   0        0        0     1430 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      372 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder.py
--rw-r--r--   0        0        0      383 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/monitors.py
--rw-r--r--   0        0        0     3115 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/monitors_and_slices/flow360.json
--rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0      925 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     1444 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/Flow360Mesh.json
--rw-r--r--   0        0        0      427 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      390 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing.py
--rw-r--r--   0        0        0      415 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing_user_defined_dynamics.py
--rw-r--r--   0        0        0     2744 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      346 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     2056 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/exceptions.py
--rw-r--r--   0        0        0      293 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/file_path.py
--rw-r--r--   0        0        0      924 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/flags.py
--rw-r--r--   0        0        0      791 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/global_exception_handler.py
--rw-r--r--   0        0        0    11894 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/log.py
--rw-r--r--   0        0        0    11310 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/services.py
--rw-r--r--   0        0        0     1255 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/solver_version.py
--rw-r--r--   0        0        0      944 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/units.py
--rw-r--r--   0        0        0     3652 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/user_config.py
--rw-r--r--   0        0        0      206 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/utils.py
--rw-r--r--   0        0        0       40 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/version.py
--rw-r--r--   0        0        0     3823 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/version_check.py
--rw-r--r--   0        0        0     1645 2024-04-11 12:21:20.038686 flow360-24.2.2/pyproject.toml
--rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 flow360-24.2.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-18 18:47:11.185594 flow360-24.2.3/LICENSE
+-rw-r--r--   0        0        0     3514 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/__init__.py
+-rw-r--r--   0        0        0     5665 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/accounts_utils.py
+-rw-r--r--   0        0        0       54 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2590 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cli/app.py
+-rw-r--r--   0        0        0      580 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cli/dict_utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3683 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     2579 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/requests.py
+-rw-r--r--   0        0        0     1191 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0    12039 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      262 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/security.py
+-rw-r--r--   0        0        0     1076 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/utils.py
+-rw-r--r--   0        0        0      223 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/cloud/webbrowser.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/__init__.py
+-rw-r--r--   0        0        0    30720 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/case.py
+-rw-r--r--   0        0        0     3907 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/compress_upload.py
+-rw-r--r--   0        0        0      142 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/constants.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/__init__.py
+-rw-r--r--   0        0        0     9264 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/boundaries.py
+-rw-r--r--   0        0        0     8474 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/conversions.py
+-rw-r--r--   0        0        0      438 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/exposed_units.py
+-rw-r--r--   0        0        0     4394 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/flow360_fields.py
+-rw-r--r--   0        0        0     2428 2024-04-18 18:47:11.185594 flow360-24.2.3/flow360/component/flow360_params/flow360_legacy.py
+-rw-r--r--   0        0        0    29693 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/flow360_output.py
+-rw-r--r--   0        0        0    66368 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0     1065 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/initial_condition.py
+-rw-r--r--   0        0        0    45016 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     1337 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/params_utils.py
+-rw-r--r--   0        0        0     3069 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/physical_properties.py
+-rw-r--r--   0        0        0    26021 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0     5400 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/time_stepping.py
+-rw-r--r--   0        0        0    11560 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/turbulence_quantities.py
+-rw-r--r--   0        0        0    37382 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/unit_system.py
+-rw-r--r--   0        0        0     2748 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/updater.py
+-rw-r--r--   0        0        0    19271 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/validations.py
+-rw-r--r--   0        0        0     8065 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/flow360_params/volume_zones.py
+-rw-r--r--   0        0        0     5547 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/folder.py
+-rw-r--r--   0        0        0      860 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/interfaces.py
+-rw-r--r--   0        0        0      221 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6891 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0    20417 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    28333 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/results/case_results.py
+-rw-r--r--   0        0        0     9401 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2291 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/types.py
+-rw-r--r--   0        0        0     4601 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/utils.py
+-rw-r--r--   0        0        0     3246 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/validator.py
+-rw-r--r--   0        0        0    25053 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     3407 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/environment.py
+-rw-r--r--   0        0        0     2036 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/error_messages.py
+-rw-r--r--   0        0        0      384 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     3877 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      446 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      291 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5356 2024-04-18 18:47:11.189594 flow360-24.2.3/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157799 2024-04-18 18:47:11.197594 flow360-24.2.3/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1157977 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1157978 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      431 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      431 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0       63 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/convergence/Flow360Mesh.json
+-rw-r--r--   0        0        0     1596 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/convergence/flow360.json
+-rw-r--r--   0        0        0      372 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/convergence.py
+-rw-r--r--   0        0        0     1430 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      372 2024-04-18 18:47:11.201594 flow360-24.2.3/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0      383 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/monitors.py
+-rw-r--r--   0        0        0     3115 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/monitors_and_slices/flow360.json
+-rw-r--r--   0        0        0       63 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0      925 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     1444 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0       63 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/release-22.3.3.0ge/Flow360Mesh.json
+-rw-r--r--   0        0        0      427 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      390 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0      415 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/om6wing_user_defined_dynamics.py
+-rw-r--r--   0        0        0     2744 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      346 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     2056 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/exceptions.py
+-rw-r--r--   0        0        0      293 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/file_path.py
+-rw-r--r--   0        0        0      924 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/flags.py
+-rw-r--r--   0        0        0      791 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/global_exception_handler.py
+-rw-r--r--   0        0        0    11894 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/log.py
+-rw-r--r--   0        0        0    11310 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/services.py
+-rw-r--r--   0        0        0     1255 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/solver_version.py
+-rw-r--r--   0        0        0      944 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/units.py
+-rw-r--r--   0        0        0     3652 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/user_config.py
+-rw-r--r--   0        0        0      206 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/utils.py
+-rw-r--r--   0        0        0       40 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/version.py
+-rw-r--r--   0        0        0     3823 2024-04-18 18:47:11.205594 flow360-24.2.3/flow360/version_check.py
+-rw-r--r--   0        0        0     1645 2024-04-18 18:47:32.413452 flow360-24.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 flow360-24.2.3/PKG-INFO
```

### Comparing `flow360-24.2.2/LICENSE` & `flow360-24.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/__init__.py` & `flow360-24.2.3/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/accounts_utils.py` & `flow360-24.2.3/flow360/accounts_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cli/app.py` & `flow360-24.2.3/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cli/dict_utils.py` & `flow360-24.2.3/flow360/cli/dict_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cloud/http_util.py` & `flow360-24.2.3/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cloud/requests.py` & `flow360-24.2.3/flow360/cloud/requests.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cloud/rest_api.py` & `flow360-24.2.3/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cloud/s3_utils.py` & `flow360-24.2.3/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/cloud/utils.py` & `flow360-24.2.3/flow360/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/case.py` & `flow360-24.2.3/flow360/component/case.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/compress_upload.py` & `flow360-24.2.3/flow360/component/compress_upload.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/boundaries.py` & `flow360-24.2.3/flow360/component/flow360_params/boundaries.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/conversions.py` & `flow360-24.2.3/flow360/component/flow360_params/conversions.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/flow360_fields.py` & `flow360-24.2.3/flow360/component/flow360_params/flow360_fields.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/flow360_legacy.py` & `flow360-24.2.3/flow360/component/flow360_params/flow360_legacy.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/flow360_output.py` & `flow360-24.2.3/flow360/component/flow360_params/flow360_output.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/flow360_params.py` & `flow360-24.2.3/flow360/component/flow360_params/flow360_params.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/initial_condition.py` & `flow360-24.2.3/flow360/component/flow360_params/initial_condition.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/params_base.py` & `flow360-24.2.3/flow360/component/flow360_params/params_base.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/params_utils.py` & `flow360-24.2.3/flow360/component/flow360_params/params_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/physical_properties.py` & `flow360-24.2.3/flow360/component/flow360_params/physical_properties.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/solvers.py` & `flow360-24.2.3/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/time_stepping.py` & `flow360-24.2.3/flow360/component/flow360_params/time_stepping.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/turbulence_quantities.py` & `flow360-24.2.3/flow360/component/flow360_params/turbulence_quantities.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/unit_system.py` & `flow360-24.2.3/flow360/component/flow360_params/unit_system.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/updater.py` & `flow360-24.2.3/flow360/component/flow360_params/updater.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/validations.py` & `flow360-24.2.3/flow360/component/flow360_params/validations.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/flow360_params/volume_zones.py` & `flow360-24.2.3/flow360/component/flow360_params/volume_zones.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/folder.py` & `flow360-24.2.3/flow360/component/folder.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/interfaces.py` & `flow360-24.2.3/flow360/component/interfaces.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/meshing/params.py` & `flow360-24.2.3/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/resource_base.py` & `flow360-24.2.3/flow360/component/resource_base.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/results/case_results.py` & `flow360-24.2.3/flow360/component/results/case_results.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/surface_mesh.py` & `flow360-24.2.3/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/types.py` & `flow360-24.2.3/flow360/component/types.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/utils.py` & `flow360-24.2.3/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/validator.py` & `flow360-24.2.3/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/component/volume_mesh.py` & `flow360-24.2.3/flow360/component/volume_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/environment.py` & `flow360-24.2.3/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/error_messages.py` & `flow360-24.2.3/flow360/error_messages.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/actuatorDisk/flow360.json` & `flow360-24.2.3/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/airplane/geometry.csm` & `flow360-24.2.3/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/airplane/surface_params.json` & `flow360-24.2.3/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/airplane/volume_params.json` & `flow360-24.2.3/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/base_test_case.py` & `flow360-24.2.3/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/betDisk/flow360.json` & `flow360-24.2.3/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/betLine/flow360.json` & `flow360-24.2.3/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-24.2.3/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/convergence/flow360.json` & `flow360-24.2.3/flow360/examples/convergence/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/cylinder/flow360.json` & `flow360-24.2.3/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-24.2.3/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/monitors_and_slices/flow360.json` & `flow360-24.2.3/flow360/examples/monitors_and_slices/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/om6wing/case.yaml` & `flow360-24.2.3/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/om6wing/flow360.json` & `flow360-24.2.3/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-24.2.3/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/flow360.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-24.2.3/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/exceptions.py` & `flow360-24.2.3/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/flags.py` & `flow360-24.2.3/flow360/flags.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/global_exception_handler.py` & `flow360-24.2.3/flow360/global_exception_handler.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/log.py` & `flow360-24.2.3/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/services.py` & `flow360-24.2.3/flow360/services.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/solver_version.py` & `flow360-24.2.3/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/units.py` & `flow360-24.2.3/flow360/units.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/user_config.py` & `flow360-24.2.3/flow360/user_config.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/flow360/version_check.py` & `flow360-24.2.3/flow360/version_check.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.2/pyproject.toml` & `flow360-24.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "flow360"
-version = "v24.2.2"
+version = "v24.2.3"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = "^1.10.0"
+pydantic = "^1.10.8"
 pytest = "^7.1.2"
 click = "^8.1.3"
 toml = "^0.10.2"
 requests = "^2.28.1"
 boto3 = "^1.24.63"
 numpy = [{ python = "^3.7", version = "^1.19.0" },
     { python = "^3.8", version = "^1.20.0" },
```

### Comparing `flow360-24.2.2/PKG-INFO` & `flow360-24.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 24.2.2
+Version: 24.2.3
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: numpy (>=1.19.0,<2.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: numpy (>=1.20.0,<2.0.0) ; python_version >= "3.8" and python_version < "4.0"
 Requires-Dist: numpy (>=1.23.0,<2.0.0) ; python_version >= "3.9" and python_version < "4.0"
 Requires-Dist: numpy (>=1.26.0,<2.0.0) ; python_version >= "3.12" and python_version < "4.0"
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: unyt (>=2.8.0,<3.0.0) ; python_version >= "3.7" and python_version < "4.0"
 Requires-Dist: unyt (>=2.9.5,<3.0.0) ; python_version >= "3.8" and python_version < "4.0"
```

