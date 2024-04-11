# Comparing `tmp/flow360-24.2.1.tar.gz` & `tmp/flow360-24.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow360-24.2.1.tar", max compression
+gzip compressed data, was "flow360-24.2.2.tar", max compression
```

## Comparing `flow360-24.2.1.tar` & `flow360-24.2.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0    26526 2024-03-21 12:04:45.205216 flow360-24.2.1/LICENSE
--rw-r--r--   0        0        0     3514 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/__init__.py
--rw-r--r--   0        0        0     5665 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/accounts_utils.py
--rw-r--r--   0        0        0       54 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cli/__init__.py
--rw-r--r--   0        0        0     2590 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cli/app.py
--rw-r--r--   0        0        0      580 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cli/dict_utils.py
--rw-r--r--   0        0        0        0 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/__init__.py
--rw-r--r--   0        0        0     3683 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/http_util.py
--rw-r--r--   0        0        0     2579 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/requests.py
--rw-r--r--   0        0        0     1191 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/rest_api.py
--rw-r--r--   0        0        0    12039 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/s3_utils.py
--rw-r--r--   0        0        0      262 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/security.py
--rw-r--r--   0        0        0     1076 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/utils.py
--rw-r--r--   0        0        0      223 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/cloud/webbrowser.py
--rw-r--r--   0        0        0        0 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/component/__init__.py
--rw-r--r--   0        0        0    30720 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/component/case.py
--rw-r--r--   0        0        0     3907 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/component/compress_upload.py
--rw-r--r--   0        0        0      142 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/component/constants.py
--rw-r--r--   0        0        0        0 2024-03-21 12:04:45.205216 flow360-24.2.1/flow360/component/flow360_params/__init__.py
--rw-r--r--   0        0        0     9236 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/boundaries.py
--rw-r--r--   0        0        0     8474 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/conversions.py
--rw-r--r--   0        0        0      438 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/exposed_units.py
--rw-r--r--   0        0        0     4394 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/flow360_fields.py
--rw-r--r--   0        0        0     2428 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/flow360_legacy.py
--rw-r--r--   0        0        0    29575 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/flow360_output.py
--rw-r--r--   0        0        0    62851 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/flow360_params.py
--rw-r--r--   0        0        0     1065 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/initial_condition.py
--rw-r--r--   0        0        0    44136 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/params_base.py
--rw-r--r--   0        0        0     1337 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/params_utils.py
--rw-r--r--   0        0        0     3069 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/physical_properties.py
--rw-r--r--   0        0        0    26021 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/solvers.py
--rw-r--r--   0        0        0     5400 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/time_stepping.py
--rw-r--r--   0        0        0     9076 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/turbulence_quantities.py
--rw-r--r--   0        0        0    37382 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/unit_system.py
--rw-r--r--   0        0        0     2748 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/updater.py
--rw-r--r--   0        0        0    19271 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/validations.py
--rw-r--r--   0        0        0     8065 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/flow360_params/volume_zones.py
--rw-r--r--   0        0        0     5547 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/folder.py
--rw-r--r--   0        0        0      860 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/interfaces.py
--rw-r--r--   0        0        0      221 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/meshing/__init__.py
--rw-r--r--   0        0        0     6891 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/meshing/params.py
--rw-r--r--   0        0        0    20417 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/resource_base.py
--rw-r--r--   0        0        0    27817 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/results/case_results.py
--rw-r--r--   0        0        0     9401 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/surface_mesh.py
--rw-r--r--   0        0        0     2291 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/types.py
--rw-r--r--   0        0        0     4601 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/utils.py
--rw-r--r--   0        0        0     3246 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/validator.py
--rw-r--r--   0        0        0    25053 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/component/volume_mesh.py
--rw-r--r--   0        0        0     3407 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/environment.py
--rw-r--r--   0        0        0     2036 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/error_messages.py
--rw-r--r--   0        0        0      384 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/__init__.py
--rw-r--r--   0        0        0     3877 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/actuatorDisk/flow360.json
--rw-r--r--   0        0        0      446 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/actuator_disk.py
--rw-r--r--   0        0        0    24017 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/airplane/geometry.csm
--rw-r--r--   0        0        0      675 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/airplane/surface_params.json
--rw-r--r--   0        0        0     3702 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/airplane/volume_params.json
--rw-r--r--   0        0        0      291 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/airplane.py
--rw-r--r--   0        0        0     5356 2024-03-21 12:04:45.209216 flow360-24.2.1/flow360/examples/base_test_case.py
--rw-r--r--   0        0        0  1157799 2024-03-21 12:04:45.217216 flow360-24.2.1/flow360/examples/betDisk/flow360.json
--rw-r--r--   0        0        0  1157977 2024-03-21 12:04:45.221216 flow360-24.2.1/flow360/examples/betLine/flow360.json
--rw-r--r--   0        0        0  1157978 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      431 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/bet_disk.py
--rw-r--r--   0        0        0      431 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/bet_line.py
--rw-r--r--   0        0        0       63 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/convergence/Flow360Mesh.json
--rw-r--r--   0        0        0     1596 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/convergence/flow360.json
--rw-r--r--   0        0        0      372 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/convergence.py
--rw-r--r--   0        0        0     1430 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/cylinder/flow360.json
--rw-r--r--   0        0        0     1492 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0      372 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/cylinder.py
--rw-r--r--   0        0        0      383 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/monitors.py
--rw-r--r--   0        0        0     3115 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/monitors_and_slices/flow360.json
--rw-r--r--   0        0        0       63 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/Flow360Mesh.json
--rw-r--r--   0        0        0      925 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/case.yaml
--rw-r--r--   0        0        0     1444 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/flow360.json
--rw-r--r--   0        0        0       63 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/release-22.3.3.0ge/Flow360Mesh.json
--rw-r--r--   0        0        0      427 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
--rw-r--r--   0        0        0     2305 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
--rw-r--r--   0        0        0      390 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing.py
--rw-r--r--   0        0        0      415 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/om6wing_user_defined_dynamics.py
--rw-r--r--   0        0        0     2744 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/flow360.json
--rw-r--r--   0        0        0      913 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/flow360mesh.json
--rw-r--r--   0        0        0     3379 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
--rw-r--r--   0        0        0     3376 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
--rw-r--r--   0        0        0     1177 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
--rw-r--r--   0        0        0      346 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/examples/rotating_spheres.py
--rw-r--r--   0        0        0     2056 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/exceptions.py
--rw-r--r--   0        0        0      293 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/file_path.py
--rw-r--r--   0        0        0      924 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/flags.py
--rw-r--r--   0        0        0      791 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/global_exception_handler.py
--rw-r--r--   0        0        0    11894 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/log.py
--rw-r--r--   0        0        0    11148 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/services.py
--rw-r--r--   0        0        0     1255 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/solver_version.py
--rw-r--r--   0        0        0      944 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/units.py
--rw-r--r--   0        0        0     3652 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/user_config.py
--rw-r--r--   0        0        0      206 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/utils.py
--rw-r--r--   0        0        0       40 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/version.py
--rw-r--r--   0        0        0     3823 2024-03-21 12:04:45.225216 flow360-24.2.1/flow360/version_check.py
--rw-r--r--   0        0        0     1645 2024-03-21 12:05:02.605009 flow360-24.2.1/pyproject.toml
--rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 flow360-24.2.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-11 12:21:01.934429 flow360-24.2.2/LICENSE
+-rw-r--r--   0        0        0     3514 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/__init__.py
+-rw-r--r--   0        0        0     5665 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/accounts_utils.py
+-rw-r--r--   0        0        0       54 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/__init__.py
+-rw-r--r--   0        0        0     2590 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/app.py
+-rw-r--r--   0        0        0      580 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cli/dict_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/__init__.py
+-rw-r--r--   0        0        0     3683 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/http_util.py
+-rw-r--r--   0        0        0     2579 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/requests.py
+-rw-r--r--   0        0        0     1191 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/rest_api.py
+-rw-r--r--   0        0        0    12039 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/s3_utils.py
+-rw-r--r--   0        0        0      262 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/security.py
+-rw-r--r--   0        0        0     1076 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/utils.py
+-rw-r--r--   0        0        0      223 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/cloud/webbrowser.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/__init__.py
+-rw-r--r--   0        0        0    30720 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/case.py
+-rw-r--r--   0        0        0     3907 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/compress_upload.py
+-rw-r--r--   0        0        0      142 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/__init__.py
+-rw-r--r--   0        0        0     9264 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/boundaries.py
+-rw-r--r--   0        0        0     8474 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/conversions.py
+-rw-r--r--   0        0        0      438 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/exposed_units.py
+-rw-r--r--   0        0        0     4394 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/flow360_fields.py
+-rw-r--r--   0        0        0     2428 2024-04-11 12:21:01.934429 flow360-24.2.2/flow360/component/flow360_params/flow360_legacy.py
+-rw-r--r--   0        0        0    29693 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/flow360_output.py
+-rw-r--r--   0        0        0    66368 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/flow360_params.py
+-rw-r--r--   0        0        0     1065 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/initial_condition.py
+-rw-r--r--   0        0        0    45016 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/params_base.py
+-rw-r--r--   0        0        0     1337 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/params_utils.py
+-rw-r--r--   0        0        0     3069 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/physical_properties.py
+-rw-r--r--   0        0        0    26021 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/solvers.py
+-rw-r--r--   0        0        0     5400 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/time_stepping.py
+-rw-r--r--   0        0        0    11560 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/turbulence_quantities.py
+-rw-r--r--   0        0        0    37382 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/unit_system.py
+-rw-r--r--   0        0        0     2748 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/updater.py
+-rw-r--r--   0        0        0    19271 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/validations.py
+-rw-r--r--   0        0        0     8065 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/flow360_params/volume_zones.py
+-rw-r--r--   0        0        0     5547 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/folder.py
+-rw-r--r--   0        0        0      860 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/interfaces.py
+-rw-r--r--   0        0        0      221 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/meshing/__init__.py
+-rw-r--r--   0        0        0     6891 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/meshing/params.py
+-rw-r--r--   0        0        0    20417 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/resource_base.py
+-rw-r--r--   0        0        0    28333 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/results/case_results.py
+-rw-r--r--   0        0        0     9401 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/surface_mesh.py
+-rw-r--r--   0        0        0     2291 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/types.py
+-rw-r--r--   0        0        0     4601 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/utils.py
+-rw-r--r--   0        0        0     3246 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/validator.py
+-rw-r--r--   0        0        0    25053 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/component/volume_mesh.py
+-rw-r--r--   0        0        0     3407 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/environment.py
+-rw-r--r--   0        0        0     2036 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/error_messages.py
+-rw-r--r--   0        0        0      384 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/__init__.py
+-rw-r--r--   0        0        0     3877 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/actuatorDisk/flow360.json
+-rw-r--r--   0        0        0      446 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/actuator_disk.py
+-rw-r--r--   0        0        0    24017 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/geometry.csm
+-rw-r--r--   0        0        0      675 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/surface_params.json
+-rw-r--r--   0        0        0     3702 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane/volume_params.json
+-rw-r--r--   0        0        0      291 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/airplane.py
+-rw-r--r--   0        0        0     5356 2024-04-11 12:21:01.938428 flow360-24.2.2/flow360/examples/base_test_case.py
+-rw-r--r--   0        0        0  1157799 2024-04-11 12:21:01.946429 flow360-24.2.2/flow360/examples/betDisk/flow360.json
+-rw-r--r--   0        0        0  1157977 2024-04-11 12:21:01.950429 flow360-24.2.2/flow360/examples/betLine/flow360.json
+-rw-r--r--   0        0        0  1157978 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      431 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/bet_disk.py
+-rw-r--r--   0        0        0      431 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/bet_line.py
+-rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence/Flow360Mesh.json
+-rw-r--r--   0        0        0     1596 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence/flow360.json
+-rw-r--r--   0        0        0      372 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/convergence.py
+-rw-r--r--   0        0        0     1430 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder/flow360.json
+-rw-r--r--   0        0        0     1492 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0      372 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/cylinder.py
+-rw-r--r--   0        0        0      383 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/monitors.py
+-rw-r--r--   0        0        0     3115 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/monitors_and_slices/flow360.json
+-rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/Flow360Mesh.json
+-rw-r--r--   0        0        0      925 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/case.yaml
+-rw-r--r--   0        0        0     1444 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/flow360.json
+-rw-r--r--   0        0        0       63 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/Flow360Mesh.json
+-rw-r--r--   0        0        0      427 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/case.yaml
+-rw-r--r--   0        0        0     2305 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json
+-rw-r--r--   0        0        0      390 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing.py
+-rw-r--r--   0        0        0      415 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/om6wing_user_defined_dynamics.py
+-rw-r--r--   0        0        0     2744 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/flow360.json
+-rw-r--r--   0        0        0      913 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/flow360mesh.json
+-rw-r--r--   0        0        0     3379 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json
+-rw-r--r--   0        0        0     3376 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json
+-rw-r--r--   0        0        0     1177 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json
+-rw-r--r--   0        0        0      346 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/examples/rotating_spheres.py
+-rw-r--r--   0        0        0     2056 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/exceptions.py
+-rw-r--r--   0        0        0      293 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/file_path.py
+-rw-r--r--   0        0        0      924 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/flags.py
+-rw-r--r--   0        0        0      791 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/global_exception_handler.py
+-rw-r--r--   0        0        0    11894 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/log.py
+-rw-r--r--   0        0        0    11310 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/services.py
+-rw-r--r--   0        0        0     1255 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/solver_version.py
+-rw-r--r--   0        0        0      944 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/units.py
+-rw-r--r--   0        0        0     3652 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/user_config.py
+-rw-r--r--   0        0        0      206 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/utils.py
+-rw-r--r--   0        0        0       40 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/version.py
+-rw-r--r--   0        0        0     3823 2024-04-11 12:21:01.954429 flow360-24.2.2/flow360/version_check.py
+-rw-r--r--   0        0        0     1645 2024-04-11 12:21:20.038686 flow360-24.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 flow360-24.2.2/PKG-INFO
```

### Comparing `flow360-24.2.1/LICENSE` & `flow360-24.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/__init__.py` & `flow360-24.2.2/flow360/__init__.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/accounts_utils.py` & `flow360-24.2.2/flow360/accounts_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cli/app.py` & `flow360-24.2.2/flow360/cli/app.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cli/dict_utils.py` & `flow360-24.2.2/flow360/cli/dict_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cloud/http_util.py` & `flow360-24.2.2/flow360/cloud/http_util.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cloud/requests.py` & `flow360-24.2.2/flow360/cloud/requests.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cloud/rest_api.py` & `flow360-24.2.2/flow360/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cloud/s3_utils.py` & `flow360-24.2.2/flow360/cloud/s3_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/cloud/utils.py` & `flow360-24.2.2/flow360/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/case.py` & `flow360-24.2.2/flow360/component/case.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/compress_upload.py` & `flow360-24.2.2/flow360/component/compress_upload.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/boundaries.py` & `flow360-24.2.2/flow360/component/flow360_params/boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     )
 
 
 class BoundaryWithTurbulenceQuantities(Boundary, metaclass=ABCMeta):
     """Turbulence Quantities on Boundaries"""
 
     turbulence_quantities: Optional[TurbulenceQuantitiesType] = pd.Field(
-        alias="turbulenceQuantities"
+        alias="turbulenceQuantities", discriminator="model_type"
     )
 
 
 class NoSlipWall(Boundary):
     """No slip wall boundary"""
 
     type: Literal["NoSlipWall"] = pd.Field("NoSlipWall", const=True)
@@ -98,15 +98,15 @@
     Example
     -------
     >>> heatFluxWall = HeatFluxWall(heatFlux=-0.01, velocity=(0, 0, 0))
     """
 
     type: Literal["HeatFluxWall"] = pd.Field("HeatFluxWall", const=True)
     heat_flux: Union[float, StrictStr] = pd.Field(alias="heatFlux", options=["Value", "Expression"])
-    velocity: Optional[BoundaryVelocityType] = pd.Field(alias="velocity")
+    velocity: Optional[BoundaryVelocityType] = pd.Field(alias="Velocity")
 
 
 class SubsonicOutflowPressure(BoundaryWithTurbulenceQuantities):
     """SubsonicOutflowPressure boundary"""
 
     type: Literal["SubsonicOutflowPressure"] = pd.Field("SubsonicOutflowPressure", const=True)
     static_pressure_ratio: PositiveFloat = pd.Field(alias="staticPressureRatio")
```

### Comparing `flow360-24.2.1/flow360/component/flow360_params/conversions.py` & `flow360-24.2.2/flow360/component/flow360_params/conversions.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/flow360_fields.py` & `flow360-24.2.2/flow360/component/flow360_params/flow360_fields.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/flow360_legacy.py` & `flow360-24.2.2/flow360/component/flow360_params/flow360_legacy.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/flow360_output.py` & `flow360-24.2.2/flow360/component/flow360_params/flow360_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     animation_frequency_time_average: Optional[PositiveAndNegOneInt] = pd.Field(
         alias="animationFrequencyTimeAverage", options=["Static", "Animated"], default=-1
     )
     animation_frequency_time_average_offset: Optional[int] = pd.Field(
         alias="animationFrequencyTimeAverageOffset", default=0
     )
     start_average_integration_step: Optional[NonNegativeAndNegOneInt] = pd.Field(
-        alias="startAverageIntegrationStep", default=-1
+        alias="startAverageIntegrationStep", default=-1, options=["From step", "No averaging"]
     )
 
     # Temporarily disabled until solver-side support for new animation format is introduced
     """
     animation_settings: Optional[AnimationSettingsExtended] = pd.Field(alias="animationSettings")
 
     # pylint: disable=unused-argument
@@ -626,15 +626,15 @@
         fields = get_output_fields(
             self,
             [],
             allowed=get_field_values(CommonFieldNames) + get_field_values(SurfaceFieldNames),
         )
 
         if self.output_fields is not None:
-            fields += self.output_fields
+            fields = list(set(fields + self.output_fields))
 
         model = {
             "animationFrequency": self.animation_frequency,
             "animationFrequencyOffset": self.animation_frequency_offset,
             "animationFrequencyTimeAverage": self.animation_frequency_time_average,
             "animationFrequencyTimeAverageOffset": self.animation_frequency_time_average_offset,
             "computeTimeAverages": self.compute_time_averages,
@@ -669,15 +669,15 @@
 
     def update_model(self) -> Flow360BaseModel:
         fields = get_output_fields(
             self, [], allowed=get_field_values(CommonFieldNames) + get_field_values(SliceFieldNames)
         )
 
         if self.output_fields is not None:
-            fields += self.output_fields
+            fields = list(set(fields + self.output_fields))
 
         model = {
             "animationFrequency": self.animation_frequency,
             "animationFrequencyOffset": self.animation_frequency_offset,
             "outputFormat": self.output_format,
             "outputFields": fields,
         }
@@ -720,17 +720,15 @@
         fields = get_output_fields(
             self,
             ["write_single_file", "write_distributed_file"],
             allowed=get_field_values(CommonFieldNames) + get_field_values(VolumeFieldNames),
         )
 
         if self.output_fields is not None:
-            for item in self.output_fields:
-                if item not in fields:
-                    fields.append(item)
+            fields = list(set(fields + self.output_fields))
 
         model = {
             "animationFrequency": self.animation_frequency,
             "animationFrequencyOffset": self.animation_frequency_offset,
             "animationFrequencyTimeAverage": self.animation_frequency_time_average,
             "animationFrequencyTimeAverageOffset": self.animation_frequency_time_average_offset,
             "computeTimeAverages": self.compute_time_averages,
@@ -752,14 +750,17 @@
 
     def update_model(self):
         fields = get_output_fields(
             self,
             [],
             allowed=get_field_values(CommonFieldNames),
         )
+        if self.output_fields is not None:
+            fields = list(set(fields + self.output_fields))
+
         model = {
             "animationFrequency": self.animation_frequency,
             "animationFrequencyOffset": self.animation_frequency_offset,
             "outputFormat": self.output_format,
             "isoSurfaces": self.iso_surfaces,
             "outputFields": fields,
         }
```

### Comparing `flow360-24.2.1/flow360/component/flow360_params/flow360_params.py` & `flow360-24.2.2/flow360/component/flow360_params/flow360_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 )
 from .time_stepping import (
     BaseTimeStepping,
     SteadyTimeStepping,
     TimeStepping,
     UnsteadyTimeStepping,
 )
-from .turbulence_quantities import TurbulenceQuantitiesType
+from .turbulence_quantities import TurbulenceQuantities, TurbulenceQuantitiesType
 from .unit_system import (
     AngularVelocityType,
     AreaType,
     CGS_unit_system,
     CGSUnitSystem,
     DensityType,
     DimensionedType,
@@ -531,19 +531,16 @@
 
     model_type: str
     alpha: Optional[float] = pd.Field(alias="alphaAngle", default=0, displayed="Alpha angle [deg]")
     beta: Optional[float] = pd.Field(alias="betaAngle", default=0, displayed="Beta angle [deg]")
     turbulent_viscosity_ratio: Optional[NonNegativeFloat] = pd.Field(
         alias="turbulentViscosityRatio"
     )
-    ## Legacy update pending.
-    ## The validation for turbulenceQuantities (make sure we have correct combinations, maybe in root validator)
-    ## is also pending. TODO
     turbulence_quantities: Optional[TurbulenceQuantitiesType] = pd.Field(
-        alias="turbulenceQuantities"
+        alias="turbulenceQuantities", discriminator="model_type"
     )
 
     # pylint: disable=missing-class-docstring,too-few-public-methods
     class Config(Flow360BaseModel.Config):
         conflicting_fields = [
             Conflicts(field1="turbulent_viscosity_ratio", field2="turbulence_quantities")
         ]
@@ -555,16 +552,18 @@
     :class: Freestream component using Mach number
     """
 
     model_type: Literal["FromMach"] = pd.Field("FromMach", alias="modelType", const=True)
     Mach: PositiveFloat = pd.Field(displayed="Mach number")
     Mach_ref: Optional[PositiveFloat] = pd.Field(alias="MachRef", displayed="Reference Mach number")
     mu_ref: PositiveFloat = pd.Field(alias="muRef", displayed="Dynamic viscosity [non-dim]")
-    temperature: Union[Literal[-1], PositiveFloat] = pd.Field(
-        alias="Temperature", displayed="Temperature [K]"
+    temperature: Union[PositiveFloat, Literal[-1]] = pd.Field(
+        alias="Temperature",
+        displayed="Temperature [K]",
+        options=["Temperature [K]", "Constant temperature"],
     )
 
     # pylint: disable=arguments-differ, unused-argument
     def to_solver(self, params: Flow360Params, **kwargs) -> FreestreamFromMach:
         """
         returns configuration object in flow360 units system
         """
@@ -578,18 +577,20 @@
 
     model_type: Literal["FromMachReynolds"] = pd.Field(
         "FromMachReynolds", alias="modelType", const=True
     )
     Mach: PositiveFloat = pd.Field(displayed="Mach number")
     Mach_ref: Optional[PositiveFloat] = pd.Field(alias="MachRef", displayed="Reference Mach number")
     Reynolds: Union[pd.confloat(gt=0, allow_inf_nan=False), Literal["inf"]] = pd.Field(
-        displayed="Reynolds number"
+        displayed="Reynolds number", options=["Reynolds", "Reynolds = inf"]
     )
-    temperature: Union[Literal[-1], PositiveFloat] = pd.Field(
-        alias="Temperature", displayed="Temperature [K]"
+    temperature: Union[PositiveFloat, Literal[-1]] = pd.Field(
+        alias="Temperature",
+        displayed="Temperature [K]",
+        options=["Temperature [K]", "Constant temperature"],
     )
 
     # pylint: disable=arguments-differ, unused-argument
     def to_solver(self, params: Flow360Params, **kwargs) -> FreestreamFromMach:
         """
         returns configuration object in flow360 units system
         """
@@ -601,16 +602,18 @@
     :class: Zero velocity freestream component
     """
 
     model_type: Literal["ZeroMach"] = pd.Field("ZeroMach", alias="modelType", const=True)
     Mach: Literal[0] = pd.Field(0, const=True, displayed="Mach number")
     Mach_ref: pd.confloat(gt=1.0e-12) = pd.Field(alias="MachRef", displayed="Reference Mach number")
     mu_ref: PositiveFloat = pd.Field(alias="muRef", displayed="Dynamic viscosity [non-dim]")
-    temperature: Union[Literal[-1], PositiveFloat] = pd.Field(
-        alias="Temperature", displayed="Temperature [K]"
+    temperature: Union[PositiveFloat, Literal[-1]] = pd.Field(
+        alias="Temperature",
+        displayed="Temperature [K]",
+        options=["Temperature [K]", "Constant temperature"],
     )
 
     # pylint: disable=arguments-differ, unused-argument
     def to_solver(self, params: Flow360Params, **kwargs) -> ZeroFreestream:
         """
         returns configuration object in flow360 units system
         """
@@ -1414,14 +1417,51 @@
     mu_ref: Optional[PositiveFloat] = pd.Field(alias="muRef")
     temperature: Union[Literal[-1], PositiveFloat] = pd.Field(alias="Temperature")
     alpha: Optional[float] = pd.Field(alias="alphaAngle")
     beta: Optional[float] = pd.Field(alias="betaAngle", default=0)
     turbulent_viscosity_ratio: Optional[NonNegativeFloat] = pd.Field(
         alias="turbulentViscosityRatio"
     )
+    turbulence_quantities: Optional[TurbulenceQuantitiesType] = pd.Field(
+        alias="turbulenceQuantities"
+    )
+
+    def __init__(self, *args, **kwargs):
+        with Flow360UnitSystem(verbose=False):
+            # Try to add discriminators to turbulence quantities,
+            class _TurbulenceQuantityTempModel(pd.BaseModel):
+                field: TurbulenceQuantitiesType = pd.Field(discriminator="model_type")
+
+            options = [
+                "TurbulentViscosityRatio",
+                "TurbulentKineticEnergy",
+                "TurbulentIntensity",
+                "TurbulentLengthScale",
+                "ModifiedTurbulentViscosityRatio",
+                "ModifiedTurbulentViscosity",
+                "SpecificDissipationRateAndTurbulentKineticEnergy",
+                "TurbulentViscosityRatioAndTurbulentKineticEnergy",
+                "TurbulentLengthScaleAndTurbulentKineticEnergy",
+                "TurbulentIntensityAndSpecificDissipationRate",
+                "TurbulentIntensityAndTurbulentViscosityRatio",
+                "TurbulentIntensityAndTurbulentLengthScale",
+                "SpecificDissipationRateAndTurbulentViscosityRatio",
+                "SpecificDissipationRateAndTurbulentLengthScale",
+                "TurbulentViscosityRatioAndTurbulentLengthScale",
+            ]
+
+            tq = kwargs.get("turbulenceQuantities")
+            if tq is not None and tq.get("modelType") is None:
+                model = {"field": tq}
+                model = try_add_discriminator(
+                    model, "field/modelType", options, _TurbulenceQuantityTempModel
+                )
+                kwargs["turbulenceQuantities"] = model["field"]
+
+            super().__init__(*args, **kwargs)
 
     def update_model(self) -> Flow360BaseModel:
         class _FreestreamTempModel(pd.BaseModel):
             """Helper class used to create
             the correct freestream from dict data"""
 
             field: FreestreamType = pd.Field(discriminator="model_type")
@@ -1430,14 +1470,16 @@
             "field": {
                 "alphaAngle": self.alpha,
                 "betaAngle": self.beta,
                 "turbulentViscosityRatio": self.turbulent_viscosity_ratio,
             }
         }
 
+        try_set(model["field"], "turbulenceQuantities", self.turbulence_quantities)
+
         # Set velocity
         if self.comments is not None:
             if self.comments.get("freestreamMeterPerSecond") is not None:
                 # pylint: disable=no-member
                 velocity = self.comments["freestreamMeterPerSecond"] * u.m / u.s
                 try_set(model["field"], "velocity", velocity)
             elif (
@@ -1600,14 +1642,46 @@
 
 
 class BoundariesLegacy(Boundaries):
     """Legacy Boundaries class"""
 
     def __init__(self, *args, **kwargs):
         with Flow360UnitSystem(verbose=False):
+            # Try to add discriminators to every
+            # boundary that has turbulence quantities,
+            class _TurbulenceQuantityTempModel(pd.BaseModel):
+                field: TurbulenceQuantitiesType = pd.Field(discriminator="model_type")
+
+            options = [
+                "TurbulentViscosityRatio",
+                "TurbulentKineticEnergy",
+                "TurbulentIntensity",
+                "TurbulentLengthScale",
+                "ModifiedTurbulentViscosityRatio",
+                "ModifiedTurbulentViscosity",
+                "SpecificDissipationRateAndTurbulentKineticEnergy",
+                "TurbulentViscosityRatioAndTurbulentKineticEnergy",
+                "TurbulentLengthScaleAndTurbulentKineticEnergy",
+                "TurbulentIntensityAndSpecificDissipationRate",
+                "TurbulentIntensityAndTurbulentViscosityRatio",
+                "TurbulentIntensityAndTurbulentLengthScale",
+                "SpecificDissipationRateAndTurbulentViscosityRatio",
+                "SpecificDissipationRateAndTurbulentLengthScale",
+                "TurbulentViscosityRatioAndTurbulentLengthScale",
+            ]
+
+            for value in kwargs.values():
+                tq = value.get("turbulenceQuantities")
+                if tq is not None and tq.get("modelType") is None:
+                    model = {"field": tq}
+                    model = try_add_discriminator(
+                        model, "field/modelType", options, _TurbulenceQuantityTempModel
+                    )
+                    value["turbulenceQuantities"] = model["field"]
+
             super().__init__(*args, **kwargs)
 
 
 class VolumeZonesLegacy(VolumeZones):
     """Legacy VolumeZones class"""
 
     def __init__(self, *args, **kwargs):
```

### Comparing `flow360-24.2.1/flow360/component/flow360_params/initial_condition.py` & `flow360-24.2.2/flow360/component/flow360_params/initial_condition.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/params_base.py` & `flow360-24.2.2/flow360/component/flow360_params/params_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1236,14 +1236,30 @@
             root_schema["additionalProperties"] = schema
         else:
             root_schema["additionalProperties"]["oneOf"] = []
             for model in models:
                 schema = model.flow360_schema()
                 root_schema["additionalProperties"]["oneOf"].append(schema)
 
+        if cls.SchemaConfig.displayed is not None:
+            root_schema["displayed"] = cls.SchemaConfig.displayed
+        for item in cls.SchemaConfig.exclude_fields:
+            cls._schema_remove(root_schema, item.split("/"))
+        for item in cls.SchemaConfig.optional_objects:
+            cls._schema_generate_optional(root_schema, item.split("/"))
+        if cls.SchemaConfig.swap_fields is not None:
+            for key, value in cls.SchemaConfig.swap_fields.items():
+                value["title"] = root_schema["properties"][key]["title"]
+                displayed = root_schema["properties"][key].get("displayed")
+                if displayed is not None:
+                    value["displayed"] = displayed
+                root_schema["properties"][key] = value
+        cls._schema_swap_key(root_schema, "title", "displayed")
+        cls._schema_clean(root_schema)
+
         definitions = {}
 
         cls._collect_all_definitions(root_schema, definitions)
 
         if definitions:
             root_schema["definitions"] = definitions
```

### Comparing `flow360-24.2.1/flow360/component/flow360_params/params_utils.py` & `flow360-24.2.2/flow360/component/flow360_params/params_utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/physical_properties.py` & `flow360-24.2.2/flow360/component/flow360_params/physical_properties.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/solvers.py` & `flow360-24.2.2/flow360/component/flow360_params/solvers.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/time_stepping.py` & `flow360-24.2.2/flow360/component/flow360_params/time_stepping.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/turbulence_quantities.py` & `flow360-24.2.2/flow360/component/flow360_params/turbulence_quantities.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 """
 Turbulence quantities parameters
 """
 
 # pylint: disable=unused-import
 from abc import ABCMeta
-from typing import Optional, Union
+from typing import Literal, Optional, Union
 
 import pydantic as pd
 
 from ..types import NonNegativeFloat, PositiveFloat
 from .params_base import Flow360BaseModel
 
 
 class TurbulentKineticEnergy(Flow360BaseModel):
     """
     turbulentKineticEnergy : non-dimensional [`C_inf^2`]
         Turbulent kinetic energy. Applicable only when using SST model.
     """
 
+    model_type: Literal["TurbulentKineticEnergy"] = pd.Field(
+        "TurbulentKineticEnergy", alias="modelType", const=True
+    )
     turbulent_kinetic_energy: Optional[NonNegativeFloat] = pd.Field(alias="turbulentKineticEnergy")
 
 
 class TurbulentIntensity(Flow360BaseModel):
     """
     turbulentIntensity : non-dimensional [`-`]
         Turbulent intensity. Applicable only when using SST model.
         This is related to turbulent kinetic energy as:
         `turbulentKineticEnergy = 1.5*pow(U_ref * turbulentIntensity, 2)`.
         Note the use of the freestream velocity U_ref instead of C_inf.
     """
 
+    model_type: Literal["TurbulentIntensity"] = pd.Field(
+        "TurbulentIntensity", alias="modelType", const=True
+    )
     turbulent_intensity: Optional[NonNegativeFloat] = pd.Field(alias="turbulentIntensity")
 
 
 class _SpecificDissipationRate(Flow360BaseModel, metaclass=ABCMeta):
     """
     specificDissipationRate : non-dimensional [`C_inf/L_gridUnit`]
         Turbulent specific dissipation rate. Applicable only when using SST model.
     """
 
+    model_type: Literal["SpecificDissipationRate"] = pd.Field(
+        "SpecificDissipationRate", alias="modelType", const=True
+    )
     specific_dissipation_rate: Optional[NonNegativeFloat] = pd.Field(
         alias="specificDissipationRate"
     )
 
 
 class TurbulentViscosityRatio(Flow360BaseModel):
     """
     turbulentViscosityRatio : non-dimensional [`-`]
         The ratio of turbulent eddy viscosity over the freestream viscosity. Applicable for both SA and SST model.
     """
 
+    model_type: Literal["TurbulentViscosityRatio"] = pd.Field(
+        "TurbulentViscosityRatio", alias="modelType", const=True
+    )
     turbulent_viscosity_ratio: Optional[NonNegativeFloat] = pd.Field(
         alias="turbulentViscosityRatio"
     )
 
 
 class TurbulentLengthScale(Flow360BaseModel, metaclass=ABCMeta):
     """
@@ -61,83 +73,110 @@
         The turbulent length scale is an estimation of the size of the eddies that are modeled/not resolved.
         Applicable only when using SST model. This is related to the turbulent kinetic energy and turbulent
         specific dissipation rate as: `L_T = sqrt(k)/(pow(beta_0^*, 0.25)*w)` where `L_T` is turbulent length scale,
         `k` is turbulent kinetic energy, `beta_0^*` is 0.09 and `w` is turbulent specific dissipation rate.
         Applicable only when using SST model.
     """
 
+    model_type: Literal["TurbulentLengthScale"] = pd.Field(
+        "TurbulentLengthScale", alias="modelType", const=True
+    )
     turbulent_length_scale: Optional[PositiveFloat] = pd.Field(alias="turbulentLengthScale")
 
 
 class ModifiedTurbulentViscosityRatio(Flow360BaseModel):
     """
     modifiedTurbulentViscosityRatio : non-dimensional [`-`]
         The ratio of modified turbulent eddy viscosity (SA) over the freestream viscosity.
         Applicable only when using SA model.
     """
 
+    model_type: Literal["ModifiedTurbulentViscosityRatio"] = pd.Field(
+        "ModifiedTurbulentViscosityRatio", alias="modelType", const=True
+    )
     modified_turbulent_viscosity_ratio: Optional[PositiveFloat] = pd.Field(
         alias="modifiedTurbulentViscosityRatio"
     )
 
 
 class ModifiedTurbulentViscosity(Flow360BaseModel):
     """
     modifiedTurbulentViscosity : non-dimensional [`C_inf*L_gridUnit`]
         The modified turbulent eddy viscosity (SA). Applicable only when using SA model.
     """
 
+    model_type: Literal["ModifiedTurbulentViscosity"] = pd.Field(
+        "ModifiedTurbulentViscosity", alias="modelType", const=True
+    )
     modified_turbulent_viscosity: Optional[PositiveFloat] = pd.Field(
         alias="modifiedTurbulentViscosity"
     )
 
 
 # pylint: disable=missing-class-docstring
 class SpecificDissipationRateAndTurbulentKineticEnergy(
     _SpecificDissipationRate, TurbulentKineticEnergy
 ):
-    pass
+    model_type: Literal["SpecificDissipationRateAndTurbulentKineticEnergy"] = pd.Field(
+        "SpecificDissipationRateAndTurbulentKineticEnergy", alias="modelType", const=True
+    )
 
 
 class TurbulentViscosityRatioAndTurbulentKineticEnergy(
     TurbulentViscosityRatio, TurbulentKineticEnergy
 ):
-    pass
+    model_type: Literal["TurbulentViscosityRatioAndTurbulentKineticEnergy"] = pd.Field(
+        "TurbulentViscosityRatioAndTurbulentKineticEnergy", alias="modelType", const=True
+    )
 
 
 class TurbulentLengthScaleAndTurbulentKineticEnergy(TurbulentLengthScale, TurbulentKineticEnergy):
-    pass
+    model_type: Literal["TurbulentLengthScaleAndTurbulentKineticEnergy"] = pd.Field(
+        "TurbulentLengthScaleAndTurbulentKineticEnergy", alias="modelType", const=True
+    )
 
 
 class TurbulentIntensityAndSpecificDissipationRate(TurbulentIntensity, _SpecificDissipationRate):
-    pass
+    model_type: Literal["TurbulentIntensityAndSpecificDissipationRate"] = pd.Field(
+        "TurbulentIntensityAndSpecificDissipationRate", alias="modelType", const=True
+    )
 
 
 class TurbulentIntensityAndTurbulentViscosityRatio(TurbulentIntensity, TurbulentViscosityRatio):
-    pass
+    model_type: Literal["TurbulentIntensityAndTurbulentViscosityRatio"] = pd.Field(
+        "TurbulentIntensityAndTurbulentViscosityRatio", alias="modelType", const=True
+    )
 
 
 class TurbulentIntensityAndTurbulentLengthScale(TurbulentIntensity, TurbulentLengthScale):
-    pass
+    model_type: Literal["TurbulentIntensityAndTurbulentLengthScale"] = pd.Field(
+        "TurbulentIntensityAndTurbulentLengthScale", alias="modelType", const=True
+    )
 
 
 class SpecificDissipationRateAndTurbulentViscosityRatio(
     _SpecificDissipationRate, TurbulentViscosityRatio
 ):
-    pass
+    model_type: Literal["SpecificDissipationRateAndTurbulentViscosityRatio"] = pd.Field(
+        "SpecificDissipationRateAndTurbulentViscosityRatio", alias="modelType", const=True
+    )
 
 
 class SpecificDissipationRateAndTurbulentLengthScale(
     _SpecificDissipationRate, TurbulentLengthScale
 ):
-    pass
+    model_type: Literal["SpecificDissipationRateAndTurbulentLengthScale"] = pd.Field(
+        "SpecificDissipationRateAndTurbulentLengthScale", alias="modelType", const=True
+    )
 
 
 class TurbulentViscosityRatioAndTurbulentLengthScale(TurbulentViscosityRatio, TurbulentLengthScale):
-    pass
+    model_type: Literal["TurbulentViscosityRatioAndTurbulentLengthScale"] = pd.Field(
+        "TurbulentViscosityRatioAndTurbulentLengthScale", alias="modelType", const=True
+    )
 
 
 # pylint: enable=missing-class-docstring
 
 TurbulenceQuantitiesType = Union[
     TurbulentViscosityRatio,
     TurbulentKineticEnergy,
```

### Comparing `flow360-24.2.1/flow360/component/flow360_params/unit_system.py` & `flow360-24.2.2/flow360/component/flow360_params/unit_system.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/updater.py` & `flow360-24.2.2/flow360/component/flow360_params/updater.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/validations.py` & `flow360-24.2.2/flow360/component/flow360_params/validations.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/flow360_params/volume_zones.py` & `flow360-24.2.2/flow360/component/flow360_params/volume_zones.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/folder.py` & `flow360-24.2.2/flow360/component/folder.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/interfaces.py` & `flow360-24.2.2/flow360/component/interfaces.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/meshing/params.py` & `flow360-24.2.2/flow360/component/meshing/params.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/resource_base.py` & `flow360-24.2.2/flow360/component/resource_base.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/results/case_results.py` & `flow360-24.2.2/flow360/component/results/case_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,14 +579,30 @@
                         self._udd_names.append(name)
                         self._udds[name] = UserDefinedDynamicsCSVModel(remote_file_name=filename)
                         # pylint: disable=protected-access
                         self._udds[name]._download_method = self._download_method
 
         return self._udd_names
 
+    def download(self, to_folder: str = ".", overwrite: bool = False):
+        """
+        Download all udd files to the specified location.
+
+        Parameters
+        ----------
+        to_folder : str, optional
+            The folder where the file will be downloaded.
+        overwrite : bool, optional
+            Flag indicating whether to overwrite existing files.
+        """
+
+        self.udd_names
+        for udd in self._udds.values():
+            udd.download(to_folder=to_folder, overwrite=overwrite)
+
     def get_udd_by_name(self, name: str) -> UserDefinedDynamicsCSVModel:
         """
         Get user-defined dynamics by name.
 
         Parameters
         ----------
         name : str
```

### Comparing `flow360-24.2.1/flow360/component/surface_mesh.py` & `flow360-24.2.2/flow360/component/surface_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/types.py` & `flow360-24.2.2/flow360/component/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     return Annotated[UnionType, pd.Field(discriminator=TYPE_TAG_STR)]
 
 
 PositiveFloat = pd.PositiveFloat
 NonNegativeFloat = pd.NonNegativeFloat
 PositiveInt = pd.PositiveInt
 NonNegativeInt = pd.NonNegativeInt
-NonNegativeAndNegOneInt = Union[Literal[-1], pd.NonNegativeInt]
-PositiveAndNegOneInt = Union[Literal[-1], pd.PositiveInt]
+NonNegativeAndNegOneInt = Union[pd.NonNegativeInt, Literal[-1]]
+PositiveAndNegOneInt = Union[pd.PositiveInt, Literal[-1]]
 Size = Tuple[PositiveFloat, PositiveFloat, PositiveFloat]
 MomentLengthType = Tuple[PositiveFloat, PositiveFloat, PositiveFloat]
 BoundaryVelocityType = Tuple[Union[float, str], Union[float, str], Union[float, str]]
 List2D = List[List[float]]
 
 # we use tuple for fixed length lists, beacause List is a mutable, variable length structure
 Coordinate = Tuple[float, float, float]
```

### Comparing `flow360-24.2.1/flow360/component/utils.py` & `flow360-24.2.2/flow360/component/utils.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/validator.py` & `flow360-24.2.2/flow360/component/validator.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/component/volume_mesh.py` & `flow360-24.2.2/flow360/component/volume_mesh.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/environment.py` & `flow360-24.2.2/flow360/environment.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/error_messages.py` & `flow360-24.2.2/flow360/error_messages.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/actuatorDisk/flow360.json` & `flow360-24.2.2/flow360/examples/actuatorDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/airplane/geometry.csm` & `flow360-24.2.2/flow360/examples/airplane/geometry.csm`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/airplane/surface_params.json` & `flow360-24.2.2/flow360/examples/airplane/surface_params.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/airplane/volume_params.json` & `flow360-24.2.2/flow360/examples/airplane/volume_params.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/base_test_case.py` & `flow360-24.2.2/flow360/examples/base_test_case.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/betDisk/flow360.json` & `flow360-24.2.2/flow360/examples/betDisk/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/betLine/flow360.json` & `flow360-24.2.2/flow360/examples/betLine/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/betLine/release-21.3.3.0ge/flow360.json` & `flow360-24.2.2/flow360/examples/betLine/release-21.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/convergence/flow360.json` & `flow360-24.2.2/flow360/examples/convergence/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/cylinder/flow360.json` & `flow360-24.2.2/flow360/examples/cylinder/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json` & `flow360-24.2.2/flow360/examples/cylinder/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/monitors_and_slices/flow360.json` & `flow360-24.2.2/flow360/examples/monitors_and_slices/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/om6wing/case.yaml` & `flow360-24.2.2/flow360/examples/om6wing/case.yaml`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/om6wing/flow360.json` & `flow360-24.2.2/flow360/examples/om6wing/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json` & `flow360-24.2.2/flow360/examples/om6wing/release-22.3.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/flow360.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/flow360mesh.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/release-21.4.1.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json` & `flow360-24.2.2/flow360/examples/rotatingSpheres/release-22.1.3.0ge/flow360mesh.json`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/exceptions.py` & `flow360-24.2.2/flow360/exceptions.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/flags.py` & `flow360-24.2.2/flow360/flags.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/global_exception_handler.py` & `flow360-24.2.2/flow360/global_exception_handler.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/log.py` & `flow360-24.2.2/flow360/log.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/services.py` & `flow360-24.2.2/flow360/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,16 +282,17 @@
 def validate_flow360_params_model(params_as_dict, unit_system_name):
     """
     Validate a params dict against the pydantic model
     """
 
     unit_system = init_unit_system(unit_system_name)
 
-    # removing _add properties as these are only used in WebUI
+    # removing _add and _temp properties as these are only used in WebUI
     params_as_dict = remove_properties_with_prefix(params_as_dict, "_add")
+    params_as_dict = remove_properties_with_prefix(params_as_dict, "_temp")
     params_as_dict = remove_dimensioned_type_none_leaves(params_as_dict)
 
     params_as_dict["unitSystem"] = unit_system.dict()
 
     remove_empty_entries(params_as_dict, exclude=["boundaries"])
 
     values, fields_set, validation_errors = pd.validate_model(Flow360Params, params_as_dict)
@@ -337,14 +338,15 @@
 
 def handle_case_submit(params_as_dict, unit_system_name):
     """
     Handles case submit. Performs pydantic validation, converts units to solver units, and exports JSON representation.
     """
     unit_system = init_unit_system(unit_system_name)
     params_as_dict = remove_properties_with_prefix(params_as_dict, "_add")
+    params_as_dict = remove_properties_with_prefix(params_as_dict, "_temp")
     params_as_dict = remove_dimensioned_type_none_leaves(params_as_dict)
 
     with unit_system:
         params = Flow360Params(**params_as_dict)
 
     solver_json = params.flow360_json()
     solver_dict = json.loads(solver_json)
```

### Comparing `flow360-24.2.1/flow360/solver_version.py` & `flow360-24.2.2/flow360/solver_version.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/units.py` & `flow360-24.2.2/flow360/units.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/user_config.py` & `flow360-24.2.2/flow360/user_config.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/flow360/version_check.py` & `flow360-24.2.2/flow360/version_check.py`

 * *Files identical despite different names*

### Comparing `flow360-24.2.1/pyproject.toml` & `flow360-24.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flow360"
-version = "v24.2.1"
+version = "v24.2.2"
 description = ""
 authors = ["Flexcompute <support@flexcompute.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 pydantic = "^1.10.0"
 pytest = "^7.1.2"
```

### Comparing `flow360-24.2.1/PKG-INFO` & `flow360-24.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flow360
-Version: 24.2.1
+Version: 24.2.2
 Summary: 
 Author: Flexcompute
 Author-email: support@flexcompute.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

