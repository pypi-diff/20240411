# Comparing `tmp/gearpy-0.7.0.tar.gz` & `tmp/gearpy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gearpy-0.7.0.tar", last modified: Tue Apr  9 19:55:48 2024, max compression
+gzip compressed data, was "gearpy-0.7.1.tar", last modified: Wed Apr 10 18:28:13 2024, max compression
```

## Comparing `gearpy-0.7.0.tar` & `gearpy-0.7.1.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-09 19:55:48.000000 gearpy-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-09 19:55:37.000000 gearpy-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/mechanical_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31110 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/dc_motor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/flywheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/mechanical_objects/gear_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/gear_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44171 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/helical_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/mating_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/mechanical_object_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41309 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/spur_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    34264 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/worm_gear.py
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/mechanical_objects/worm_wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/motor_control/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/motor_control_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/pwm_control.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/motor_control/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/constant_pwm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/reach_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/rules_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/start_limit_current.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/motor_control/rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55448 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/powertrain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/absolute_rotary_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/amperometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/sensor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/tachometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/sensors/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/units/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/unit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    89909 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/units/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17524 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20123 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy/utils/stop_condition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/operator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-09 19:55:37.000000 gearpy-0.7.0/gearpy/utils/stop_condition/stop_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-09 19:55:48.000000 gearpy-0.7.0/gearpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:55:47.000000 gearpy-0.7.0/gearpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:55:48.000000 gearpy-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-09 19:55:37.000000 gearpy-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.707033 gearpy-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 18:28:04.000000 gearpy-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-04-10 18:28:13.707033 gearpy-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-04-10 18:28:04.000000 gearpy-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.695033 gearpy-0.7.1/gearpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.699033 gearpy-0.7.1/gearpy/mechanical_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31114 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/dc_motor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/flywheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.699033 gearpy-0.7.1/gearpy/mechanical_objects/gear_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/gear_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/gear_data/lewis_factor_table.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/gear_data/worm_gear_and_wheel_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    44175 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/helical_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/mating_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/mechanical_object_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41313 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/spur_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34268 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/worm_gear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37366 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/mechanical_objects/worm_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.699033 gearpy-0.7.1/gearpy/motor_control/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/motor_control_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/pwm_control.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.699033 gearpy-0.7.1/gearpy/motor_control/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/constant_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/reach_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/rules_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/start_limit_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/start_proportional_to_angular_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/motor_control/rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55457 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/powertrain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.703033 gearpy-0.7.1/gearpy/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/absolute_rotary_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/amperometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/sensor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/tachometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/sensors/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.703033 gearpy-0.7.1/gearpy/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/units/unit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89149 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.703033 gearpy-0.7.1/gearpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20109 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.703033 gearpy-0.7.1/gearpy/utils/stop_condition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/stop_condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/stop_condition/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/stop_condition/operator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-10 18:28:04.000000 gearpy-0.7.1/gearpy/utils/stop_condition/stop_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:28:13.703033 gearpy-0.7.1/gearpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-04-10 18:28:13.000000 gearpy-0.7.1/gearpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-10 18:28:13.000000 gearpy-0.7.1/gearpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:28:13.000000 gearpy-0.7.1/gearpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 18:28:13.000000 gearpy-0.7.1/gearpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 18:28:13.000000 gearpy-0.7.1/gearpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-10 18:28:04.000000 gearpy-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:28:13.707033 gearpy-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-10 18:28:04.000000 gearpy-0.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gearpy-0.7.0/README.rst` & `gearpy-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/dc_motor.py` & `gearpy-0.7.1/gearpy/mechanical_objects/dc_motor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Current, InertiaMoment, Torque, UnitBase
 from .mechanical_object_base import RotatingObject, MotorBase
-from typing import Dict, List, Union, Optional
+from typing import Optional
 
 
 class DCMotor(MotorBase):
     r""":py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` object.
 
     Attributes
     ----------
@@ -614,15 +615,15 @@
     def electric_current(self, electric_current: Current):
         if not isinstance(electric_current, Current):
             raise TypeError(f"Parameter 'electric_current' must be an instance of {Current.__name__!r}.")
 
         self.__electric_current = electric_current
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the DC motor. Each time variable is stored as a dictionary key-value pair. The available
         time variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
@@ -658,15 +659,15 @@
             self.time_variables['electric current'].append(self.electric_current)
         if 'pwm' not in self.time_variables.keys():
             self.time_variables['pwm'] = [self.pwm]
         else:
             self.time_variables['pwm'].append(self.pwm)
 
     @property
-    def pwm(self) -> Union[float, int]:
+    def pwm(self) -> float | int:
         """Pulse Width Modulation duty cycle of the supply voltage of the DC motor. \n
         It must be a :py:class:`float` or an :py:class:`int` within ``-1`` and ``1``. \n
         In general the duty cycle can be between ``0`` and ``1``, but :py:attr:`pwm` can be between ``-1`` and ``1``, in
         order to take into account the voltage sign with respect to the direction of rotation:
 
         - if :py:attr:`pwm` is positive, then the supply voltage pushes the motor to rotate in the `positive` direction,
         - if :py:attr:`pwm` is negative, then the supply voltage pushes the motor to rotate in the `negative` direction,
@@ -694,15 +695,15 @@
 
            :py:meth:`compute_torque` \n
            :py:meth:`compute_electric_current`
         """
         return self.__pwm
 
     @pwm.setter
-    def pwm(self, pwm: Union[float, int]):
+    def pwm(self, pwm: float | int):
         if not isinstance(pwm, float) and not isinstance(pwm, int):
             raise TypeError("Parameter 'pwm' must be a float or an integer.")
 
         if (pwm > 1) or (pwm < -1):
             raise ValueError("Pulse Width Modulation (PWM) must be within -1 and 1.")
 
         self.__pwm = pwm
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/flywheel.py` & `gearpy-0.7.1/gearpy/mechanical_objects/flywheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, InertiaMoment, Torque, UnitBase
 from .mechanical_object_base import RotatingObject
-from typing import Dict, List, Union
 
 
 class Flywheel(RotatingObject):
     r""":py:class:`Flywheel <gearpy.mechanical_objects.flywheel.Flywheel>` object.
 
     Attributes
     ----------
@@ -309,15 +309,15 @@
 
         if master_gear_ratio <= 0:
             raise ValueError("Parameter 'master_gear_ratio' must be positive.")
 
         self.__master_gear_ratio = master_gear_ratio
 
     @property
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         """Efficiency of the fixed joint between the flywheel and its driving rotating object. Since the relation
         between the flywheel and its neighbor elements in the powertrain elements is always a fixed joint, the
         efficiency is always equal to ``1`` and cannot be overwritten. \n
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
@@ -342,15 +342,15 @@
            ``TypeError``
                If :py:attr:`inertia_moment` is not an instance of
                :py:class:`InertiaMoment <gearpy.units.units.InertiaMoment>`.
         """
         return super().inertia_moment
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the flywheel. Each time variable is stored as a dictionary key-value pair. The available
         time variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/helical_gear.py` & `gearpy-0.7.1/gearpy/mechanical_objects/helical_gear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
     Stress, Time, Torque, UnitBase
 from math import sqrt, atan
 from .mechanical_object_base import RotatingObject, lewis_factor_function, Role
 from .mating_roles import MatingMaster, MatingSlave
 from .spur_gear import SpurGear
-from typing import Callable, Dict, List, Union, Optional
+from typing import Callable, Optional
 
 
 class HelicalGear(SpurGear):
     r""":py:class:`HelicalGear <gearpy.mechanical_objects.helical_gear.HelicalGear>` object.
 
     Attributes
     ----------
@@ -412,15 +413,15 @@
         return super().master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
         super(HelicalGear, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
 
     @property
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float` or an
         :py:class:`int` within ``0`` and ``1``. \n
         To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
         :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
@@ -434,15 +435,15 @@
                If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
            ``ValueError``
                If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return super().master_gear_efficiency
 
     @master_gear_efficiency.setter
-    def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
+    def master_gear_efficiency(self, master_gear_efficiency: float | int):
         super(HelicalGear, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
 
     @property
     def mating_role(self) -> Role:
         """Role of the gear in the gear mating. \n
         If the gear drives the mate one, then it is the "master" gear and its role is
         :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is the "slave" one
@@ -947,15 +948,15 @@
         return super().external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
         super(HelicalGear, type(self)).external_torque.fset(self, external_torque)
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
         variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/mechanical_object_base.py` & `gearpy-0.7.1/gearpy/mechanical_objects/mechanical_object_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
 from . import gear_data
 from gearpy.units import Angle, AngularPosition, AngularSpeed, AngularAcceleration, Force, InertiaMoment, Length, \
                          Stress, Time, Torque, UnitBase
 from importlib import resources as imp_resources
 from inspect import signature
 import pandas as pd
 from scipy.interpolate import interp1d
-from typing import Callable, Dict, List, Union
+from typing import Callable
 
 
 LEWIS_FACTOR_DATA_FILE = (imp_resources.files(gear_data) / 'lewis_factor_table.csv')
 LEWIS_FACTOR_DATA = pd.read_csv(LEWIS_FACTOR_DATA_FILE)
 MINIMUM_TEETH_NUMBER = LEWIS_FACTOR_DATA.loc[LEWIS_FACTOR_DATA.index[0], 'Number of teeth']
 lewis_factor_function = interp1d(x = LEWIS_FACTOR_DATA['Number of teeth'],
                                  y = LEWIS_FACTOR_DATA['Lewis Factor'],
@@ -183,15 +184,15 @@
     @property
     @abstractmethod
     def inertia_moment(self) -> InertiaMoment:
         return self.__inertia_moment
 
     @property
     @abstractmethod
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         return self.__time_variables
 
     @abstractmethod
     def update_time_variables(self):
         self.__time_variables['angular position'].append(self.__angular_position)
         self.__time_variables['angular speed'].append(self.__angular_speed)
         self.__time_variables['angular acceleration'].append(self.__angular_acceleration)
@@ -428,20 +429,20 @@
         if master_gear_ratio <= 0:
             raise ValueError("Parameter 'master_gear_ratio' must be positive.")
 
         self.__master_gear_ratio = master_gear_ratio
 
     @property
     @abstractmethod
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         return self.__master_gear_efficiency
 
     @master_gear_efficiency.setter
     @abstractmethod
-    def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
+    def master_gear_efficiency(self, master_gear_efficiency: float | int):
         if not isinstance(master_gear_efficiency, float) and not isinstance(master_gear_efficiency, int):
             raise TypeError("Parameter 'master_gear_efficiency' must be a float or an integer.")
 
         if master_gear_efficiency > 1 or master_gear_efficiency < 0:
             raise ValueError("Parameter 'master_gear_efficiency' must be within 0 and 1.")
 
         self.__master_gear_efficiency = master_gear_efficiency
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/spur_gear.py` & `gearpy-0.7.1/gearpy/mechanical_objects/spur_gear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
     Stress, Time, Torque, UnitBase
 from math import sqrt
 from .mechanical_object_base import RotatingObject, GearBase, lewis_factor_function, Role
 from .mating_roles import MatingMaster, MatingSlave
-from typing import Callable, Dict, List, Union, Optional
+from typing import Callable, Optional
 
 
 class SpurGear(GearBase):
     r""":py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` object.
 
     Attributes
     ----------
@@ -345,15 +346,15 @@
         return super().master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
         super(SpurGear, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
 
     @property
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float` or an
         :py:class:`int` within ``0`` and ``1``. \n
         To set this property use :py:func:`add_gear_mating <gearpy.utils.relations.add_gear_mating>` or
         :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
@@ -367,15 +368,15 @@
                If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
            ``ValueError``
                If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return super().master_gear_efficiency
 
     @master_gear_efficiency.setter
-    def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
+    def master_gear_efficiency(self, master_gear_efficiency: float | int):
         super(SpurGear, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
 
     @property
     def mating_role(self) -> Role:
         """Role of the gear in the gear mating. \n
         If the gear drives the mate one, then it is the "master" gear and its role is
         :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is the "slave" one
@@ -871,15 +872,15 @@
         return super().external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
         super(SpurGear, type(self)).external_torque.fset(self, external_torque)
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
         variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/worm_gear.py` & `gearpy-0.7.1/gearpy/mechanical_objects/worm_gear.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
                          Time, Torque, UnitBase
 from inspect import signature
 from .mating_roles import MatingMaster, MatingSlave
 from .mechanical_object_base import RotatingObject, Role, WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES, \
                                     worm_gear_and_wheel_maximum_helix_angle_function
-from typing import Callable, Dict, List, Union, Optional
+from typing import Callable, Optional
 
 
 class WormGear(RotatingObject):
     r""":py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` object.
 
     Attributes
     ----------
@@ -377,15 +378,15 @@
 
         if master_gear_ratio <= 0:
             raise ValueError("Parameter 'master_gear_ratio' must be positive.")
 
         self.__master_gear_ratio = master_gear_ratio
 
     @property
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float` or an
         :py:class:`int` within ``0`` and ``1``. \n
         To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
         :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
@@ -399,15 +400,15 @@
                If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
            ``ValueError``
                If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return self.__master_gear_efficiency
 
     @master_gear_efficiency.setter
-    def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
+    def master_gear_efficiency(self, master_gear_efficiency: float | int):
         if not isinstance(master_gear_efficiency, float) and not isinstance(master_gear_efficiency, int):
             raise TypeError("Parameter 'master_gear_efficiency' must be a float or an integer.")
 
         if master_gear_efficiency > 1 or master_gear_efficiency < 0:
             raise ValueError("Parameter 'master_gear_efficiency' must be within 0 and 1.")
 
         self.__master_gear_efficiency = master_gear_efficiency
@@ -720,15 +721,15 @@
         for parameter in ['angular_position', 'angular_speed', 'time']:
             if parameter not in sig.parameters.keys():
                 raise KeyError(f"Function 'external_torque' misses parameter {parameter!r}.")
 
         self.__external_torque = external_torque
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the gear. Each time variable is stored as a dictionary key-value pair. The available time
         variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
```

### Comparing `gearpy-0.7.0/gearpy/mechanical_objects/worm_wheel.py` & `gearpy-0.7.1/gearpy/mechanical_objects/worm_wheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
 from gearpy.units import AngularPosition, AngularSpeed, AngularAcceleration, Angle, Force, InertiaMoment, Length, \
                          Stress, Time, Torque, UnitBase
 from math import pi
 from .mechanical_object_base import RotatingObject, Role, WORM_GEAR_AND_WHEEL_AVAILABLE_PRESSURE_ANGLES, \
                                     worm_gear_and_wheel_maximum_helix_angle_function, worm_wheel_lewis_factor_function
 from .mating_roles import MatingMaster, MatingSlave
 from .helical_gear import HelicalGear
-from typing import Callable, Dict, List, Union, Optional
+from typing import Callable, Optional
 
 
 class WormWheel(HelicalGear):
     r""":py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>` object.
 
     Attributes
     ----------
@@ -378,15 +379,15 @@
         return super().master_gear_ratio
 
     @master_gear_ratio.setter
     def master_gear_ratio(self, master_gear_ratio: float):
         super(WormWheel, type(self)).master_gear_ratio.fset(self, master_gear_ratio)
 
     @property
-    def master_gear_efficiency(self) -> Union[float, int]:
+    def master_gear_efficiency(self) -> float | int:
         """Efficiency of the gear mating between the gear and its driving gear. It must be a :py:class:`float`  or an
         :py:class:`int` within ``0`` and ``1``. \n
         To set this property use :py:func:`add_worm_gear_mating <gearpy.utils.relations.add_worm_gear_mating>` or
         :py:func:`add_fixed_joint <gearpy.utils.relations.add_fixed_joint>`.
 
         Returns
         -------
@@ -400,15 +401,15 @@
                If :py:attr:`master_gear_efficiency` is not a :py:class:`float` or an :py:class:`int`.
            ``ValueError``
                If :py:attr:`master_gear_efficiency` is not within ``0`` and ``1``.
         """
         return super().master_gear_efficiency
 
     @master_gear_efficiency.setter
-    def master_gear_efficiency(self, master_gear_efficiency: Union[float, int]):
+    def master_gear_efficiency(self, master_gear_efficiency: float | int):
         super(WormWheel, type(self)).master_gear_efficiency.fset(self, master_gear_efficiency)
 
     @property
     def mating_role(self) -> Role:
         """Role of the gear in the gear mating. \n
         If the gear drives the mate one, then it is the "master" gear and its role is
         :py:class:`MatingMaster <gearpy.mechanical_objects.mating_roles.MatingMaster>`, otherwise it is
@@ -801,15 +802,15 @@
         return super().external_torque
 
     @external_torque.setter
     def external_torque(self, external_torque: Callable[[AngularPosition, AngularSpeed, Time], Torque]):
         super(WormWheel, type(self)).external_torque.fset(self, external_torque)
 
     @property
-    def time_variables(self) -> Dict[str, List[UnitBase]]:
+    def time_variables(self) -> dict[str, list[UnitBase]]:
         """Time variables of the worm wheel. Each time variable is stored as a dictionary key-value pair. The available
         time variables are:
 
         - :py:attr:`angular_position`: ``'angular position'``,
         - :py:attr:`angular_speed`: ``'angular speed'``,
         - :py:attr:`angular_acceleration`: ``'angular acceleration'``,
         - :py:attr:`torque`: ``'torque'``,
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/motor_control_base.py` & `gearpy-0.7.1/gearpy/motor_control/motor_control_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/motor_control/pwm_control.py` & `gearpy-0.7.1/gearpy/motor_control/pwm_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from __future__ import annotations
 from gearpy.powertrain import Powertrain
 from .motor_control_base import MotorControlBase
 from gearpy.motor_control.rules.rules_base import RuleBase
-from typing import Union
 
 
 class PWMControl(MotorControlBase):
     r""":py:class:`PWMControl <gearpy.motor_control.pwm_control.PWMControl>` object.
 
     Attributes
     ----------
@@ -109,9 +109,9 @@
             pwm = [self._saturate_pwm(pwm_value) for pwm_value in pwm_values if pwm_value is not None][0]
         else:
             pwm = 1
 
         self.__powertrain.elements[0].pwm = pwm
 
     @staticmethod
-    def _saturate_pwm(pwm) -> Union[float, int]:
+    def _saturate_pwm(pwm) -> float | int:
         return min(max(pwm, -1), 1)
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/constant_pwm.py` & `gearpy-0.7.1/gearpy/motor_control/rules/constant_pwm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from __future__ import annotations
 from gearpy.sensors import Timer
 from gearpy.powertrain import Powertrain
 from gearpy.motor_control.rules.rules_base import RuleBase
-from typing import Union
 
 
 class ConstantPWM(RuleBase):
     """:py:class:`ConstantPWM <gearpy.motor_control.rules.constant_pwm.ConstantPWM>` object. \n
     It can be used to make a gradual start of the ``powertrain``'s motion, in order to avoid a peak in the
     ``powertrain``'s DC motor absorbed electric current. \n
     It checks whether the ``timer`` is active and, if so, it sets the ``pwm`` of ``powertrain`` motor to the constant
@@ -32,15 +32,15 @@
 
        :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`
     """
 
     def __init__(self,
                  timer: Timer,
                  powertrain: Powertrain,
-                 target_pwm_value: Union[float, int]):
+                 target_pwm_value: float | int):
         super().__init__()
 
         if not isinstance(timer, Timer):
             raise TypeError(f"Parameter 'timer' must be an instance of {Timer.__name__!r}.")
 
         if not isinstance(powertrain, Powertrain):
             raise TypeError(f"Parameter 'powertrain' must be an instance of {Powertrain.__name__!r}.")
@@ -51,15 +51,15 @@
         if (target_pwm_value < -1) or (target_pwm_value > 1):
             raise ValueError("Parameter 'target_pwm_value' must be within -1 and 1.")
 
         self.__timer = timer
         self.__powertrain = powertrain
         self.__target_pwm_value = target_pwm_value
 
-    def apply(self) -> Union[None, float, int]:
+    def apply(self) -> None | float | int:
         r"""It checks if ``timer`` is active and, if so, it returns the ``pwm`` to apply to the ``powertrain`` motor,
         equal to ``target_pwm_value``.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int` or :py:obj:`None`
             PWM value to apply to the motor, equal to ``target_pwm_value``.
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/reach_angular_position.py` & `gearpy-0.7.1/gearpy/motor_control/rules/reach_angular_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import MotorBase, RotatingObject
 from gearpy.sensors import AbsoluteRotaryEncoder
 from gearpy.powertrain import Powertrain
 from gearpy.units import AngularPosition, Angle
 from gearpy.motor_control.rules.rules_base import RuleBase
-from typing import Union
 from .utils import _compute_static_error
 
 
 class ReachAngularPosition(RuleBase):
     """:py:class:`ReachAngularPosition <gearpy.motor_control.rules.reach_angular_position.ReachAngularPosition>` object. \n
     It can be used to make the ``encoder``'s ``target`` reach a ``target_angular_position`` within a ``braking_angle``.
 
@@ -69,15 +69,15 @@
             raise TypeError(f"Parameter 'braking_angle' must be an instance of {Angle.__name__!r}.")
 
         self.__encoder = encoder
         self.__powertrain = powertrain
         self.__target_angular_position = target_angular_position
         self.__braking_angle = braking_angle
 
-    def apply(self) -> Union[None, float, int]:
+    def apply(self) -> None | float | int:
         """It computes the ``pwm`` to apply to the ``powertrain``'s DC motor in order to reach a 
         ``target_angular_position`` by the ``target`` rotating object of the ``encoder``, within a specific
         ``braking_angle``.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int` or :py:obj:`None`
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/rules_base.py` & `gearpy-0.7.1/gearpy/motor_control/rules/rules_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/start_limit_current.py` & `gearpy-0.7.1/gearpy/motor_control/rules/start_limit_current.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import DCMotor
 from gearpy.sensors import AbsoluteRotaryEncoder, Tachometer
 from gearpy.units import AngularPosition, Current
 import numpy as np
 from gearpy.motor_control.rules.rules_base import RuleBase
-from typing import Union
 
 
 class StartLimitCurrent(RuleBase):
     """:py:class:`StartLimitCurrent <gearpy.motor_control.rules.start_limit_current.StartLimitCurrent>` object. \n
     It can be used to make a gradual start of the powertrain's motion and limit the ``motor`` absorbed electric
     current to be lower than or equal to a ``limit_electric_current`` value. It computes a ``pwm`` to apply to the
     ``motor`` up until the ``encoder``'s ``target``'s ``angular_position`` equals ``target_angular_position``. \n
@@ -73,15 +73,15 @@
 
         self.__encoder = encoder
         self.__tachometer = tachometer
         self.__motor = motor
         self.__limit_electric_current = limit_electric_current
         self.__target_angular_position = target_angular_position
 
-    def apply(self) -> Union[None, float, int]:
+    def apply(self) -> None | float | int:
         r"""It computes the ``pwm`` to apply to the ``motor`` in order to limit its absorbed electric current to be
         lower or equal to ``limit_electric_current``, until the ``encoder``'s ``target`` rotating object's
         ``angular_position`` equals the ``target_angular_position``.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int` or :py:obj:`None`
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/start_proportional_to_angular_position.py` & `gearpy-0.7.1/gearpy/motor_control/rules/start_proportional_to_angular_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import MotorBase, RotatingObject
 from gearpy.sensors import AbsoluteRotaryEncoder
 from gearpy.powertrain import Powertrain
 from gearpy.units import AngularPosition
 from gearpy.motor_control.rules.rules_base import RuleBase
-from typing import Union, Optional
+from typing import Optional
 from .utils import _compute_pwm_min
 
 
 class StartProportionalToAngularPosition(RuleBase):
     """:py:class:`StartProportionalToAngularPosition <gearpy.motor_control.rules.start_proportional_to_angular_position.StartProportionalToAngularPosition>` object. \n
     It can be used to make a gradual start of the ``powertrain``'s motion, in order to avoid a peak in the
     ``powertrain``'s DC motor absorbed electric current. \n
@@ -51,15 +52,15 @@
        :py:attr:`DCMotor.pwm <gearpy.mechanical_objects.dc_motor.DCMotor.pwm>`
     """
 
     def __init__(self,
                  encoder: AbsoluteRotaryEncoder,
                  powertrain: Powertrain,
                  target_angular_position: AngularPosition,
-                 pwm_min_multiplier: Union[float, int],
+                 pwm_min_multiplier: float | int,
                  pwm_min: Optional[float] = None):
         super().__init__()
 
         if not isinstance(encoder, AbsoluteRotaryEncoder):
             raise TypeError(f"Parameter 'encoder' must be an instance of {AbsoluteRotaryEncoder.__name__!r}.")
 
         if not isinstance(powertrain, Powertrain):
@@ -95,15 +96,15 @@
 
         self.__encoder = encoder
         self.__powertrain = powertrain
         self.__target_angular_position = target_angular_position
         self.__pwm_min_multiplier = pwm_min_multiplier
         self.__pwm_min = pwm_min
 
-    def apply(self) -> Union[None, float, int]:
+    def apply(self) -> None | float | int:
         """It computes the ``pwm`` to apply to the ``powertrain`` motor, proportional to the ``encoder``'s ``target``
         ``angular_position`` until it reaches the ``target_angular_position``.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int` or :py:obj:`None`
             PWM value to apply to the motor, proportional to the ``encoder``'s ``target`` ``angular_position``.
```

### Comparing `gearpy-0.7.0/gearpy/motor_control/rules/utils.py` & `gearpy-0.7.1/gearpy/motor_control/rules/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import SpurGear
 from gearpy.powertrain import Powertrain
 from gearpy.units import AngularPosition, Angle
-from typing import Union
 
 
-def _compute_static_error(braking_angle: Angle, powertrain: Powertrain) -> Union[Angle, AngularPosition]:
+def _compute_static_error(braking_angle: Angle, powertrain: Powertrain) -> Angle | AngularPosition:
     maximum_torque = powertrain.elements[0].maximum_torque
     load_torque = powertrain.elements[0].load_torque
 
     powertrain_efficiency = 1
     for element in powertrain.elements:
         if isinstance(element, SpurGear):
             powertrain_efficiency *= element.master_gear_efficiency
@@ -17,15 +17,15 @@
         static_error = ((load_torque/maximum_torque)/powertrain_efficiency)*braking_angle
     else:
         static_error = AngularPosition(0, 'rad')
 
     return static_error
 
 
-def _compute_pwm_min(powertrain: Powertrain) -> Union[float, int]:
+def _compute_pwm_min(powertrain: Powertrain) -> float | int:
     maximum_torque = powertrain.elements[0].maximum_torque
     if powertrain.elements[0].time_variables['load torque']:
         load_torque = powertrain.elements[0].time_variables['load torque'][0]
     else:
         load_torque = powertrain.elements[0].load_torque
     no_load_electric_current = powertrain.elements[0].no_load_electric_current
     maximum_electric_current = powertrain.elements[0].maximum_electric_current
```

### Comparing `gearpy-0.7.0/gearpy/powertrain.py` & `gearpy-0.7.1/gearpy/powertrain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
 from collections import Counter
 from gearpy.mechanical_objects import MotorBase, RotatingObject, GearBase, WormGear
 from gearpy.units import Time
 from gearpy.utils import export_time_variables
 import matplotlib.pyplot as plt
 import pandas as pd
 import os
 from scipy.interpolate import interp1d
-from typing import List, Tuple, Union, Optional
+from typing import Optional
 
 
 VARIABLES_SORT_ORDER = {'angular position': 0, 'angular speed': 1, 'angular acceleration': 2, 'torque': 3,
                         'driving torque': 4, 'load torque': 5, 'tangential force': 6, 'bending stress': 7,
                         'contact stress': 8, 'electric current': 9, 'pwm': 10}
 
 
@@ -75,15 +76,15 @@
         self.__self_locking = False
         for element in self.elements:
             if isinstance(element, WormGear):
                 if element.self_locking:
                     self.__self_locking = True
 
     @property
-    def elements(self) -> Tuple[RotatingObject]:
+    def elements(self) -> tuple[RotatingObject]:
         """Rotating objects in the powertrain. \n
         The first element is the driving motor, the next elements are in order, from the closest to the farthest from
         the motor. Each element is driven by the previous one and it drives the following one.
 
         Returns
         -------
         :py:class:`tuple`
@@ -98,15 +99,15 @@
            :py:class:`SpurGear <gearpy.mechanical_objects.spur_gear.SpurGear>` \n
            :py:class:`WormGear <gearpy.mechanical_objects.worm_gear.WormGear>` \n
            :py:class:`WormWheel <gearpy.mechanical_objects.worm_wheel.WormWheel>`
         """
         return self.__elements
 
     @property
-    def time(self) -> List[Time]:
+    def time(self) -> list[Time]:
         """List of the simulated time steps. \n
         During computation, the solver appends a simulated time step to this list at each iteration. \n
         Every element of this list must be an instance of :py:class:`Time <gearpy.units.units.Time>`.
 
         Returns
         -------
         :py:class:`list`
@@ -200,15 +201,15 @@
                             element.contact_stress = element.time_variables['contact stress'][0]
 
             for variable in element.time_variables.keys():
                 element.time_variables[variable] = []
 
     def snapshot(self,
                  target_time: Time,
-                 variables: Optional[List[str]] = None,
+                 variables: Optional[list[str]] = None,
                  angular_position_unit: Optional[str] = 'rad',
                  angular_speed_unit: Optional[str] = 'rad/s',
                  angular_acceleration_unit: Optional[str] = 'rad/s^2',
                  torque_unit: Optional[str] = 'Nm',
                  driving_torque_unit: Optional[str] = 'Nm',
                  load_torque_unit: Optional[str] = 'Nm',
                  force_unit: Optional[str] = 'N',
@@ -446,16 +447,16 @@
         if print_data:
             print(f'Mechanical Powertrain Status at Time = {target_time}')
             print(data.to_string())
 
         return data
 
     def plot(self,
-             elements: Optional[List[Union[RotatingObject, str]]] = None,
-             variables: Optional[List[str]] = None,
+             elements: Optional[list[RotatingObject | str]] = None,
+             variables: Optional[list[str]] = None,
              angular_position_unit: Optional[str] = 'rad',
              angular_speed_unit: Optional[str] = 'rad/s',
              angular_acceleration_unit: Optional[str] = 'rad/s^2',
              torque_unit: Optional[str] = 'Nm',
              force_unit: Optional[str] = 'N',
              stress_unit: Optional[str] = 'MPa',
              current_unit: Optional[str] = 'A',
```

### Comparing `gearpy-0.7.0/gearpy/sensors/absolute_rotary_encoder.py` & `gearpy-0.7.1/gearpy/sensors/absolute_rotary_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import RotatingObject
 from gearpy.units import AngularPosition
 from .sensor_base import SensorBase
-from typing import Optional, Union
+from typing import Optional
 
 
 class AbsoluteRotaryEncoder(SensorBase):
     r""":py:class:`AbsoluteRotaryEncoder <gearpy.sensors.absolute_rotary_encoder.AbsoluteRotaryEncoder>` object.
 
     Attributes
     ----------
@@ -38,15 +39,15 @@
 
            ``TypeError``
                If :py:attr:`target` is not an instance of
                :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__target
 
-    def get_value(self, unit: Optional[str] = None) -> Union[AngularPosition, float, int]:
+    def get_value(self, unit: Optional[str] = None) -> AngularPosition | float | int:
         """It gets the angular position of the :py:attr:`target` rotating object. \n
         If a ``unit`` is set, then it converts the angular position to that unit and returns only the numerical value as
         float or integer.
 
         Parameters
         ----------
         ``unit`` : :py:class:`str`, optional
```

### Comparing `gearpy-0.7.0/gearpy/sensors/amperometer.py` & `gearpy-0.7.1/gearpy/sensors/amperometer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import MotorBase
 from gearpy.units import Current
 from .sensor_base import SensorBase
-from typing import Optional, Union
+from typing import Optional
 
 
 class Amperometer(SensorBase):
     r""":py:class:`Amperometer <gearpy.sensors.amperometer.Amperometer>` object.
 
     Attributes
     ----------
@@ -41,15 +42,15 @@
 
            ``TypeError``
                If :py:attr:`target` is not an instance of
                :py:class:`MotorBase <gearpy.mechanical_objects.mechanical_object_base.MotorBase>`.
         """
         return self.__target
 
-    def get_value(self, unit: Optional[str] = None) -> Union[Current, float, int]:
+    def get_value(self, unit: Optional[str] = None) -> Current | float | int:
         """It gets the electric current of the :py:attr:`target` motor object. \n
         If a ``unit`` is set, then it converts the electric current to that unit and returns only the numerical value
         as float or integer.
 
         Parameters
         ----------
         ``unit`` : :py:class:`str`, optional
```

### Comparing `gearpy-0.7.0/gearpy/sensors/sensor_base.py` & `gearpy-0.7.1/gearpy/sensors/sensor_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
 from gearpy.mechanical_objects import RotatingObject
 from gearpy.units import UnitBase
-from typing import Union
 
 
 class SensorBase(ABC):
     """:py:class:`SensorBase <gearpy.sensors.sensor_base.SensorBase>` object. \n
     Abstract base class for creating sensor objects.
 
     .. admonition:: See Also
@@ -17,8 +17,8 @@
     """
 
     @property
     @abstractmethod
     def target(self) -> RotatingObject: ...
 
     @abstractmethod
-    def get_value(self) -> Union[UnitBase, float, int]: ...
+    def get_value(self) -> UnitBase | float | int: ...
```

### Comparing `gearpy-0.7.0/gearpy/sensors/tachometer.py` & `gearpy-0.7.1/gearpy/sensors/tachometer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import RotatingObject
 from gearpy.units import AngularSpeed
 from .sensor_base import SensorBase
-from typing import Optional, Union
+from typing import Optional
 
 
 class Tachometer(SensorBase):
     r""":py:class:`Tachometer <gearpy.sensors.tachometer.Tachometer>` object.
 
     Attributes
     ----------
@@ -38,15 +39,15 @@
 
            ``TypeError``
                If :py:attr:`target` is not an instance of
                :py:class:`RotatingObject <gearpy.mechanical_objects.mechanical_object_base.RotatingObject>`.
         """
         return self.__target
 
-    def get_value(self, unit: Optional[str] = None) -> Union[AngularSpeed, float, int]:
+    def get_value(self, unit: Optional[str] = None) -> AngularSpeed | float | int:
         """It gets the angular speed of the :py:attr:`target` rotating object. \n
         If a ``unit`` is set, then it converts the angular speed to that unit and returns only the numerical value as
         float or integer.
 
         Parameters
         ----------
         ``unit`` : :py:class:`str`, optional
```

### Comparing `gearpy-0.7.0/gearpy/sensors/timer.py` & `gearpy-0.7.1/gearpy/sensors/timer.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/solver.py` & `gearpy-0.7.1/gearpy/solver.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/units/unit_base.py` & `gearpy-0.7.1/gearpy/units/unit_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
 from math import fabs
-from typing import Union
 
 
 COMPARISON_TOLERANCE = 1e-12
 
 
 class UnitBase(ABC):
     """:py:class:`UnitBase <gearpy.units.unit_base.UnitBase>` object. \n
@@ -27,15 +27,15 @@
        :py:class:`TimeInterval <gearpy.units.units.TimeInterval>` \n
        :py:class:`Torque <gearpy.units.units.Torque>`
     """
 
     __UNITS = {}
 
     @abstractmethod
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         if not isinstance(value, float) and not isinstance(value, int):
             raise TypeError("Parameter 'value' must be a float or an integer.")
 
         if not isinstance(unit, str):
             raise TypeError("Parameter 'unit' must be a string.")
 
     def __repr__(self):
@@ -46,95 +46,95 @@
 
     def __abs__(self):
         return self.__class__(abs(self.value), self.unit)
 
     def __neg__(self):
         return self.__class__(-self.value, self.unit)
 
-    def __add__(self, other: 'UnitBase') -> None:
+    def __add__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'It is not allowed to sum a {self.__class__.__name__} and a {other.__class__.__name__}.')
 
         return self.__class__(value = self.value + other.to(self.unit).value, unit = self.unit)
 
-    def __sub__(self, other: 'UnitBase') -> None:
+    def __sub__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'It is not allowed to subtract a {other.__class__.__name__} '
                             f'from a {self.__class__.__name__}.')
 
         try:
             return self.__class__(value = self.value - other.to(self.unit).value, unit = self.unit)
         except ValueError:
             if self.value - other.to(self.unit).value <= 0:
                 raise ValueError('Cannot perform the subtraction because the result is negative or null.')
 
     @abstractmethod
-    def __mul__(self, other: Union[float, int]) -> None: ...
+    def __mul__(self, other: float | int) -> None: ...
 
     @abstractmethod
-    def __rmul__(self, other: Union[float, int]) -> None: ...
+    def __rmul__(self, other: float | int) -> None: ...
 
     @abstractmethod
-    def __truediv__(self, other: Union['UnitBase', float, int]) -> None:
+    def __truediv__(self, other: UnitBase | float | int) -> None:
         if not isinstance(other, UnitBase) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide a Unit by a {other.__class__.__name__}.')
 
         if isinstance(other, UnitBase):
             if other.value == 0:
                 raise ZeroDivisionError('It is not allowed to divide a Unit by zero.')
         else:
             if other == 0:
                 raise ZeroDivisionError('It is not allowed to divide a Unit by zero.')
 
-    def __eq__(self, other: 'UnitBase') -> None:
+    def __eq__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value == other.value
         else:
             return fabs(self.value - other.to(self.unit).value) < COMPARISON_TOLERANCE
 
-    def __ne__(self, other: 'UnitBase') -> None:
+    def __ne__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value != other.value
         else:
             return fabs(self.value - other.to(self.unit).value) > COMPARISON_TOLERANCE
 
-    def __gt__(self, other: 'UnitBase') -> None:
+    def __gt__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value > other.value
         else:
             return self.value - other.to(self.unit).value > COMPARISON_TOLERANCE
 
-    def __ge__(self, other: 'UnitBase') -> None:
+    def __ge__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value >= other.value
         else:
             return self.value - other.to(self.unit).value >= -COMPARISON_TOLERANCE
 
-    def __lt__(self, other: 'UnitBase') -> None:
+    def __lt__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value < other.value
         else:
             return self.value - other.to(self.unit).value < -COMPARISON_TOLERANCE
 
-    def __le__(self, other: 'UnitBase') -> None:
+    def __le__(self, other: UnitBase) -> None:
         if not isinstance(other, self.__class__) and not issubclass(self.__class__, other.__class__):
             raise TypeError(f'Cannot compare {self.__class__.__name__} and {other.__class__.__name__}.')
 
         if self.unit == other.unit:
             return self.value <= other.value
         else:
             return self.value - other.to(self.unit).value <= COMPARISON_TOLERANCE
```

### Comparing `gearpy-0.7.0/gearpy/units/units.py` & `gearpy-0.7.1/gearpy/units/units.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 from math import pi, sin, cos, tan
-from typing import Union, Optional
+from typing import Optional
 from .unit_base import UnitBase
 
 
 class AngularPosition(UnitBase):
     r""":py:class:`AngularPosition <gearpy.units.units.AngularPosition>` object.
 
     Attributes
@@ -28,56 +29,56 @@
 
     __UNITS = {'rad': 1,
                'deg': pi/180,
                'arcmin': pi/180/60,
                'arcsec': pi/180/60/60,
                'rot': 2*pi}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'AngularPosition':
+    def __mul__(self, other: float | int) -> AngularPosition:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return AngularPosition(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'AngularPosition':
+    def __rmul__(self, other: float | int) -> AngularPosition:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return AngularPosition(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['AngularPosition', float, int]) -> Union['AngularPosition', float]:
+    def __truediv__(self, other: AngularPosition | float | int) -> AngularPosition | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, AngularPosition) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, AngularPosition):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularPosition(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Angular position numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Angular position numerical value.
 
@@ -111,15 +112,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'AngularPosition':
+    def to(self, target_unit: str, inplace: bool = False) -> AngularPosition:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -182,45 +183,45 @@
         if inplace:
             self.__value = target_value
             self.__unit = target_unit
             return self
         else:
             return AngularPosition(value = target_value, unit = target_unit)
 
-    def sin(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def sin(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the sine of the angular position at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the sine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
         :py:class:`float`
             Computed sine of the angular position.
         """
         return sin(2*pi*frequency*self.to('rad').value)
 
-    def cos(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def cos(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the cosine of the angular position at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the cosine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
         :py:class:`float`
             Computed cosine of the angular position.
         """
         return cos(2*pi*frequency*self.to('rad').value)
 
-    def tan(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def tan(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the tangent of the angular position at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the tangent. Default is :math:`\frac{1}{2 \pi}`.
 
@@ -251,65 +252,65 @@
         It computes the sine of the angle at a given frequency.
     :py:meth:`cos`
         It computes the cosine of the angle at a given frequency.
     :py:meth:`tan`
         It computes the tangent of the angle at a given frequency.
     """
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if value < 0:
             raise ValueError("Parameter 'value' must be positive or null.")
 
         self.__value = value
         self.__unit = unit
 
-    def __add__(self, other: Union['AngularPosition', 'Angle']) -> Union['AngularPosition', 'Angle']:
+    def __add__(self, other: AngularPosition | Angle) -> AngularPosition | Angle:
         super().__add__(other = other)
 
         if isinstance(other, Angle):
             return Angle(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
         else:
             return AngularPosition(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
 
-    def __sub__(self, other: Union['AngularPosition', 'Angle']) -> Union['AngularPosition', 'Angle']:
+    def __sub__(self, other: AngularPosition | Angle) -> AngularPosition | Angle:
         super().__sub__(other = other)
 
         if isinstance(other, Angle):
             return Angle(value = self.__value - other.to(self.__unit).value, unit = self.__unit)
         else:
             return AngularPosition(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
 
-    def __mul__(self, other: Union[float, int]) -> 'Angle':
+    def __mul__(self, other: float | int) -> Angle:
         super().__mul__(other = other)
 
         if other < 0:
             raise ValueError('Cannot perform a multiplication by a negative number.')
 
         return Angle(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Angle':
+    def __rmul__(self, other: float | int) -> Angle:
         super().__rmul__(other = other)
 
         if other < 0:
             raise ValueError('Cannot perform a multiplication by a negative number.')
 
         return Angle(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['AngularPosition', float, int]) -> Union['AngularPosition', float]:
+    def __truediv__(self, other: AngularPosition | float | int) -> AngularPosition | float:
         super().__truediv__(other = other)
 
         if isinstance(other, AngularPosition):
             return self.__value/other.to(self.__unit).value
         else:
             return Angle(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Angle numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive or
         null.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Angle numerical value.
@@ -346,15 +347,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return super().unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Angle':
+    def to(self, target_unit: str, inplace: bool = False) -> Angle:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -408,45 +409,45 @@
         if inplace:
             self.__value = converted.value
             self.__unit = converted.unit
             return self
         else:
             return Angle(value = converted.value, unit = converted.unit)
 
-    def sin(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def sin(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the sine of the angle at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the sine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
         :py:class:`float`
             Computed sine of the angle.
         """
         return super().sin(frequency = frequency)
 
-    def cos(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def cos(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the cosine of the angle at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the cosine. Default is :math:`\frac{1}{2 \pi}`.
 
         Returns
         -------
         :py:class:`float`
             Computed cosine of the angle.
         """
         return super().cos(frequency = frequency)
 
-    def tan(self, frequency: Optional[Union[float, int]] = 1/2/pi) -> float:
+    def tan(self, frequency: Optional[float | int] = 1/2/pi) -> float:
         r"""It computes the tangent of the angle at a given frequency.
 
         Parameters
         ----------
         ``frequency`` : :py:class:`float` or :py:class:`int`, optional
             Frequency to multiply by before computing the tangent. Default is :math:`\frac{1}{2 \pi}`.
 
@@ -481,61 +482,61 @@
                'deg/s': pi/180,
                'deg/min': pi/180/60,
                'deg/h': pi/180/60/60,
                'rps': 2*pi,
                'rpm': 2*pi/60,
                'rph': 2*pi/60/60}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union['Time', float, int]) -> Union['AngularPosition', 'AngularSpeed']:
+    def __mul__(self, other: Time | float | int) -> AngularPosition | AngularSpeed:
         super().__mul__(other = other)
 
         if not isinstance(other, Time) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Time):
             return AngularPosition(value = self.to('rad/s').value*other.to('sec').value, unit = 'rad')
         else:
             return AngularSpeed(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union['Time', float, int]) -> Union['AngularPosition', 'AngularSpeed']:
+    def __rmul__(self, other: Time | float | int) -> AngularPosition | AngularSpeed:
         super().__rmul__(other = other)
 
         if not isinstance(other, Time) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by a '
                             f'{self.__class__.__name__}.')
 
         if isinstance(other, Time):
             return AngularPosition(value = self.to('rad/s').value*other.to('sec').value, unit = 'rad')
         else:
             return AngularSpeed(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['AngularSpeed', float, int]) -> Union['AngularSpeed', float]:
+    def __truediv__(self, other: AngularSpeed | float | int) -> AngularSpeed | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, AngularSpeed) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide a {self.__class__.__name__} by a {other.__class__.__name__}.')
 
         if isinstance(other, AngularSpeed):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularSpeed(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Angular speed numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Angular speed numerical value.
 
@@ -573,15 +574,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'AngularSpeed':
+    def to(self, target_unit: str, inplace: bool = False) -> AngularSpeed:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -667,62 +668,62 @@
         measurement.
     """
 
     __UNITS = {'rad/s^2': 1,
                'deg/s^2': pi/180,
                'rot/s^2': 2*pi}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union['Time', float, int]) -> Union['AngularAcceleration', 'AngularSpeed']:
+    def __mul__(self, other: Time | float | int) -> AngularAcceleration | AngularSpeed:
         super().__mul__(other = other)
 
         if not isinstance(other, Time) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Time):
             return AngularSpeed(value = self.to('rad/s^2').value*other.to('sec').value, unit = 'rad/s')
         else:
             return AngularAcceleration(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union['Time', float, int]) -> Union['AngularAcceleration', 'AngularSpeed']:
+    def __rmul__(self, other: Time | float | int) -> AngularAcceleration | AngularSpeed:
         super().__rmul__(other = other)
 
         if not isinstance(other, Time) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         if isinstance(other, Time):
             return AngularSpeed(value = self.to('rad/s^2').value*other.to('sec').value, unit = 'rad/s')
         else:
             return AngularAcceleration(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['AngularAcceleration', float, int]) -> Union['AngularAcceleration', float]:
+    def __truediv__(self, other: AngularAcceleration | float | int) -> AngularAcceleration | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, AngularAcceleration) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, AngularAcceleration):
             return self.__value/other.to(self.__unit).value
         else:
             return AngularAcceleration(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Angular acceleration numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Angular acceleration numerical value.
 
@@ -754,15 +755,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'AngularAcceleration':
+    def to(self, target_unit: str, inplace: bool = False) -> AngularAcceleration:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -853,65 +854,65 @@
                'kgcm^2': 1e-4,
                'kgmm^2': 1e-6,
                'gm^2': 1e-3,
                'gdm^2': 1e-5,
                'gcm^2': 1e-7,
                'gmm^2': 1e-9}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         if value <= 0:
             raise ValueError("Parameter 'value' must be positive.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'InertiaMoment':
+    def __mul__(self, other: float | int) -> InertiaMoment:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if other <= 0:
             raise ValueError('Cannot perform a multiplication by a negative number or by zero.')
 
         return InertiaMoment(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'InertiaMoment':
+    def __rmul__(self, other: float | int) -> InertiaMoment:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         if other <= 0:
             raise ValueError('Cannot perform a multiplication by a negative number or by zero.')
 
         return InertiaMoment(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['InertiaMoment', float, int]) -> Union['InertiaMoment', float]:
+    def __truediv__(self, other: InertiaMoment | float | int) -> InertiaMoment | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, InertiaMoment) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, InertiaMoment):
             return self.__value/other.to(self.__unit).value
         else:
             return InertiaMoment(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Moment of inertia numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be
         positive.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Moment of inertia numerical value.
@@ -951,15 +952,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'InertiaMoment':
+    def to(self, target_unit: str, inplace: bool = False) -> InertiaMoment:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1059,44 +1060,44 @@
                'kgfcm': 9.80665e-2,
                'kgfmm': 9.80665e-3,
                'gfm': 9.80665e-3,
                'gfdm': 9.80665e-4,
                'gfcm': 9.80665e-5,
                'gfmm': 9.80665e-6}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'Torque':
+    def __mul__(self, other: float | int) -> Torque:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return Torque(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Torque':
+    def __rmul__(self, other: float | int) -> Torque:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by a '
                             f'{self.__class__.__name__}.')
 
         return Torque(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['InertiaMoment', 'Length', 'Torque', float, int]) \
-            -> Union['AngularAcceleration', 'Force', float, 'Torque']:
+    def __truediv__(self, other: InertiaMoment | Length | Torque | float | int) \
+            -> AngularAcceleration | Force | float | Torque:
         super().__truediv__(other = other)
 
         if not isinstance(other, InertiaMoment) and not isinstance(other, Length) and not isinstance(other, Torque) \
                 and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide a {self.__class__.__name__} by a {other.__class__.__name__}.')
 
         if isinstance(other, InertiaMoment):
@@ -1105,15 +1106,15 @@
             return Force(value = self.to('Nm').value/other.to('m').value, unit = 'N')
         elif isinstance(other, Torque):
             return self.__value/other.to(self.__unit).value
         else:
             return Torque(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Torque numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Torque numerical value.
 
@@ -1159,15 +1160,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Torque':
+    def to(self, target_unit: str, inplace: bool = False) -> Torque:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1254,69 +1255,68 @@
     """
 
     __UNITS = {'sec': 1,
                'min': 60,
                'hour': 60*60,
                'ms': 1e-3}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union['AngularAcceleration', 'AngularSpeed', float, int]) \
-            -> Union['AngularPosition', 'AngularSpeed', 'Time']:
+    def __mul__(self, other: AngularAcceleration | AngularSpeed | float | int) -> AngularPosition | AngularSpeed | Time:
         super().__mul__(other = other)
 
         if not isinstance(other, AngularAcceleration) and not isinstance(other, AngularSpeed) \
                 and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, AngularAcceleration):
             return AngularSpeed(value = self.to('sec').value*other.to('rad/s^2').value, unit = 'rad/s')
         elif isinstance(other, AngularSpeed):
             return AngularPosition(value = self.to('sec').value*other.to('rad/s').value, unit = 'rad')
         else:
             return Time(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union['AngularAcceleration', 'AngularSpeed', float, int]) \
-            -> Union['AngularPosition', 'AngularSpeed', 'Time']:
+    def __rmul__(self, other: AngularAcceleration | AngularSpeed | float | int) \
+            -> AngularPosition | AngularSpeed | Time:
         super().__rmul__(other = other)
 
         if not isinstance(other, AngularAcceleration) and not isinstance(other, AngularSpeed) \
                 and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by a '
                             f'{self.__class__.__name__}.')
 
         if isinstance(other, AngularAcceleration):
             return AngularSpeed(value = self.to('sec').value*other.to('rad/s^2').value, unit = 'rad/s')
         elif isinstance(other, AngularSpeed):
             return AngularPosition(value = self.to('sec').value*other.to('rad/s').value, unit = 'rad')
         else:
             return Time(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Time', float, int]) -> Union['Time', float]:
+    def __truediv__(self, other: Time | float | int) -> Time | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Time) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide a {self.__class__.__name__} by a {other.__class__.__name__}.')
 
         if isinstance(other, Time):
             return self.__value/other.to(self.__unit).value
         else:
             return Time(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Time numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Time numerical value.
 
@@ -1349,15 +1349,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Time':
+    def to(self, target_unit: str, inplace: bool = False) -> Time:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1438,65 +1438,65 @@
     Methods
     -------
     :py:meth:`to`
         It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement.
     """
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if value <= 0:
             raise ValueError("Parameter 'value' must be positive.")
 
         self.__value = value
         self.__unit = unit
 
-    def __add__(self, other: Union['Time', 'TimeInterval']) -> Union['Time', 'TimeInterval']:
+    def __add__(self, other: Time | TimeInterval) -> Time | TimeInterval:
         super().__add__(other = other)
 
         if isinstance(other, TimeInterval):
             return TimeInterval(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
         else:
             return Time(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
 
-    def __sub__(self, other: Union['Time', 'TimeInterval']) -> Union['Time', 'TimeInterval']:
+    def __sub__(self, other: Time | TimeInterval) -> Time | TimeInterval:
         super().__sub__(other = other)
 
         if isinstance(other, TimeInterval):
             return TimeInterval(value = self.__value - other.to(self.__unit).value, unit = self.__unit)
         else:
             return Time(value = self.__value + other.to(self.__unit).value, unit = self.__unit)
 
-    def __mul__(self, other: Union[float, int]) -> 'TimeInterval':
+    def __mul__(self, other: float | int) -> TimeInterval:
         super().__mul__(other = other)
 
         if other <= 0:
             raise ValueError('Cannot perform a multiplication by a negative number or by zero.')
 
         return TimeInterval(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'TimeInterval':
+    def __rmul__(self, other: float | int) -> TimeInterval:
         super().__rmul__(other = other)
 
         if other <= 0:
             raise ValueError('Cannot perform a multiplication by a negative number or by zero.')
 
         return TimeInterval(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Time', float, int]) -> Union['Time', float]:
+    def __truediv__(self, other: Time | float | int) -> Time | float:
         super().__truediv__(other = other)
 
         if isinstance(other, Time):
             return self.__value/other.to(self.__unit).value
         else:
             return TimeInterval(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Time interval numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be
         positive.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Time interval numerical value.
@@ -1532,15 +1532,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return super().unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'TimeInterval':
+    def to(self, target_unit: str, inplace: bool = False) -> TimeInterval:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1617,62 +1617,62 @@
     """
 
     __UNITS = {'m': 1,
                'dm': 1e-1,
                'cm': 1e-2,
                'mm': 1e-3}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         if value <= 0:
             raise ValueError("Parameter 'value' must be positive.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union['Length', float, int]) -> Union['Surface', 'Length']:
+    def __mul__(self, other: Length | float | int) -> Surface | Length:
         super().__mul__(other = other)
 
         if not isinstance(other, Length) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Length):
             return Surface(value = self.to('m').value*other.to('m').value, unit = 'm^2')
         else:
             return Length(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Length':
+    def __rmul__(self, other: float | int) -> Length:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return Length(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Length', float, int]) -> Union['Length', float]:
+    def __truediv__(self, other: Length | float | int) -> Length | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Length) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Length):
             return self.__value/other.to(self.__unit).value
         else:
             return Length(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Length numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Length numerical value.
 
@@ -1707,15 +1707,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Length':
+    def to(self, target_unit: str, inplace: bool = False) -> Length:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1801,59 +1801,59 @@
     """
 
     __UNITS = {'m^2': 1,
                'dm^2': 1e-2,
                'cm^2': 1e-4,
                'mm^2': 1e-6}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         if value <= 0:
             raise ValueError("Parameter 'value' must be positive.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'Surface':
+    def __mul__(self, other: float | int) -> Surface:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return Surface(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Surface':
+    def __rmul__(self, other: float | int) -> Surface:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return Surface(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Surface', float, int]) -> Union['Surface', float]:
+    def __truediv__(self, other: Surface | float | int) -> Surface | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Surface) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Surface):
             return self.__value/other.to(self.__unit).value
         else:
             return Surface(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Surface numerical value. The relative unit is expressed by the :py:attr:`unit` property. It must be positive.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Surface numerical value.
 
@@ -1888,15 +1888,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Surface':
+    def to(self, target_unit: str, inplace: bool = False) -> Surface:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -1984,43 +1984,43 @@
 
     __UNITS = {'N': 1,
                'mN': 1e-3,
                'kN': 1e3,
                'kgf': 9.80665,
                'gf': 9.80665e-3}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'Force':
+    def __mul__(self, other: float | int) -> Force:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return Force(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Force':
+    def __rmul__(self, other: float | int) -> Force:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return Force(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Force', 'Surface', float, int]) -> Union['Force', 'Stress', float]:
+    def __truediv__(self, other: Force | Surface | float | int) -> Force | Stress | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Force) and not isinstance(other, Surface) and not isinstance(other, float) \
                 and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
@@ -2028,15 +2028,15 @@
             return self.__value/other.to(self.__unit).value
         elif isinstance(other, Surface):
             return Stress(value = self.to('N').value/other.to('m^2').value, unit = 'Pa')
         else:
             return Force(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Force numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Force numerical value.
 
@@ -2070,15 +2070,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Force':
+    def to(self, target_unit: str, inplace: bool = False) -> Force:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -2164,56 +2164,56 @@
     """
 
     __UNITS = {'Pa': 1,
                'kPa': 1e3,
                'MPa': 1e6,
                'GPa': 1e9}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'Stress':
+    def __mul__(self, other: float | int) -> Stress:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return Stress(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Stress':
+    def __rmul__(self, other: float | int) -> Stress:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return Stress(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Stress', float, int]) -> Union['Stress', float]:
+    def __truediv__(self, other: Stress | float | int) -> Stress | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Stress) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Stress):
             return self.__value/other.to(self.__unit).value
         else:
             return Stress(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Stress numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Stress numerical value.
 
@@ -2246,15 +2246,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Stress':
+    def to(self, target_unit: str, inplace: bool = False) -> Stress:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
@@ -2339,56 +2339,56 @@
         measurement.
     """
 
     __UNITS = {'A': 1,
                'mA': 1e-3,
                'uA': 1e-6}
 
-    def __init__(self, value: Union[float, int], unit: str):
+    def __init__(self, value: float | int, unit: str):
         super().__init__(value = value, unit = unit)
 
         if unit not in self.__UNITS.keys():
             raise KeyError(f"{self.__class__.__name__} unit '{unit}' not available. "
                            f"Available units are: {list(self.__UNITS.keys())}.")
 
         self.__value = value
         self.__unit = unit
 
-    def __mul__(self, other: Union[float, int]) -> 'Current':
+    def __mul__(self, other: float | int) -> Current:
         super().__mul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         return Current(value = self.__value*other, unit = self.__unit)
 
-    def __rmul__(self, other: Union[float, int]) -> 'Current':
+    def __rmul__(self, other: float | int) -> Current:
         super().__rmul__(other = other)
 
         if not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to multiply a {other.__class__.__name__} by an '
                             f'{self.__class__.__name__}.')
 
         return Current(value = self.__value*other, unit = self.__unit)
 
-    def __truediv__(self, other: Union['Current', float, int]) -> Union['Current', float]:
+    def __truediv__(self, other: Current | float | int) -> Current | float:
         super().__truediv__(other = other)
 
         if not isinstance(other, Current) and not isinstance(other, float) and not isinstance(other, int):
             raise TypeError(f'It is not allowed to divide an {self.__class__.__name__} by a '
                             f'{other.__class__.__name__}.')
 
         if isinstance(other, Current):
             return self.__value/other.to(self.__unit).value
         else:
             return Current(value = self.__value/other, unit = self.__unit)
 
     @property
-    def value(self) -> Union[float, int]:
+    def value(self) -> float | int:
         """Electrical current numerical value. The relative unit is expressed by the :py:attr:`unit` property.
 
         Returns
         -------
         :py:class:`float` or :py:class:`int`
             Electrical current numerical value.
 
@@ -2420,15 +2420,15 @@
            ``TypeError``
                If :py:attr:`unit` is not a :py:class:`str`.
            ``KeyError``
                If the :py:attr:`unit` is not among available ones.
         """
         return self.__unit
 
-    def to(self, target_unit: str, inplace: bool = False) -> 'Current':
+    def to(self, target_unit: str, inplace: bool = False) -> Current:
         """It converts actual :py:attr:`value` to a new value computed using ``target_unit`` as the reference unit of
         measurement. \n
         If ``inplace`` is ``True``, it overrides actual :py:attr:`value` and :py:attr:`unit`, otherwise it returns a new
         instance with the converted :py:attr:`value` and the ``target_unit`` as :py:attr:`unit`.
 
         Parameters
         ----------
```

### Comparing `gearpy-0.7.0/gearpy/utils/animate.py` & `gearpy-0.7.1/gearpy/utils/animate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import DCMotor
 from gearpy.units import Time
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation
-from typing import List, Optional, Union
+from typing import Optional
 
 
 def dc_motor_characteristics_animation(motor: DCMotor,
-                                       time: List[Time],
-                                       interval: Optional[Union[float, int]] = 200,
+                                       time: list[Time],
+                                       interval: Optional[float | int] = 200,
                                        torque_speed_curve: Optional[bool] = True,
                                        torque_current_curve: Optional[bool] = True,
                                        angular_speed_unit: Optional[str] = 'rad/s',
                                        torque_unit: Optional[str] = 'Nm',
                                        current_unit: Optional[str] = 'A',
                                        figsize: Optional[tuple] = None,
                                        line_color: Optional[str] = None,
                                        marker_color: Optional[str] = None,
-                                       marker_size: Optional[Union[float, int]] = None,
-                                       padding: Optional[Union[float, int]] = 0.1,
+                                       marker_size: Optional[float | int] = None,
+                                       padding: Optional[float | int] = 0.1,
                                        show: Optional[bool] = True) -> FuncAnimation:
     """It generates an animation of a :py:class:`DCMotor <gearpy.mechanical_objects.dc_motor.DCMotor>` torque-speed and
     torque-current characteristic curves and relative working points during the simulation. \n
     Each simulated time step is a frame on the animation. \n
     It generates two subplots, one for each characteristic curve. It is possible to isolate a single characteristic to
     be plotted with optional parameters ``torque_speed_curve`` and ``torque_current_curve``. \n
     The characteristic curves can be modified by the motor pulse width modulation
```

### Comparing `gearpy-0.7.0/gearpy/utils/export.py` & `gearpy-0.7.1/gearpy/utils/export.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/utils/relations.py` & `gearpy-0.7.1/gearpy/utils/relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from __future__ import annotations
 from gearpy.mechanical_objects import RotatingObject, MotorBase, GearBase, MatingMaster, MatingSlave, WormGear, \
                                       WormWheel
-from typing import Union
 
 
 def add_gear_mating(master: GearBase,
                     slave: GearBase,
-                    efficiency: Union[float, int]) -> None:
+                    efficiency: float | int) -> None:
     """It creates a gear mating between two existing gears. This mating is used to compose the
     :py:class:`Powertrain <gearpy.powertrain.Powertrain>`. \n
     The ratio of the angular speed of the ``master`` gear over the angular speed of the ``slave`` gear is equal to the
     ratio of the ``slave`` gear number of teeth over the ``master`` gear number of teeth. \n
     The ``master`` gear is closest to the motor and transfers a fraction of the driving torque to the ``slave`` one,
     based on the ``efficiency`` value: the higher the ``efficiency``, the higher the fraction of transferred driving
     torque.
@@ -104,17 +104,17 @@
     master.mating_role = MatingMaster
     slave.driven_by = master
     slave.mating_role = MatingSlave
     slave.master_gear_ratio = slave.n_teeth/master.n_teeth
     slave.master_gear_efficiency = efficiency
 
 
-def add_worm_gear_mating(master: Union[WormGear, WormWheel],
-                         slave: Union[WormGear, WormWheel],
-                         friction_coefficient: Union[float, int]) -> None:
+def add_worm_gear_mating(master: WormGear | WormWheel,
+                         slave: WormGear | WormWheel,
+                         friction_coefficient: float | int) -> None:
     """It creates a gear mating between a worm gear and a worm wheel. This mating is used to compose the
     :py:class:`Powertrain <gearpy.powertrain.Powertrain>`. \n
     The ``master`` gear is closest to the motor and transfers a fraction of the driving torque to the ``slave`` one,
     based on the mating efficiency, which depends on the ``friction_coefficient``: the higher the
     ``friction_coefficient``, the lower the fraction of transferred driving torque.
 
     Parameters
```

### Comparing `gearpy-0.7.0/gearpy/utils/stop_condition/operator.py` & `gearpy-0.7.1/gearpy/utils/stop_condition/operator.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/utils/stop_condition/operator_base.py` & `gearpy-0.7.1/gearpy/utils/stop_condition/operator_base.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy/utils/stop_condition/stop_condition.py` & `gearpy-0.7.1/gearpy/utils/stop_condition/stop_condition.py`

 * *Files identical despite different names*

### Comparing `gearpy-0.7.0/gearpy.egg-info/SOURCES.txt` & `gearpy-0.7.1/gearpy.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.rst
+pyproject.toml
 setup.py
 gearpy/__init__.py
 gearpy/powertrain.py
 gearpy/solver.py
 gearpy.egg-info/PKG-INFO
 gearpy.egg-info/SOURCES.txt
 gearpy.egg-info/dependency_links.txt
@@ -14,14 +16,16 @@
 gearpy/mechanical_objects/helical_gear.py
 gearpy/mechanical_objects/mating_roles.py
 gearpy/mechanical_objects/mechanical_object_base.py
 gearpy/mechanical_objects/spur_gear.py
 gearpy/mechanical_objects/worm_gear.py
 gearpy/mechanical_objects/worm_wheel.py
 gearpy/mechanical_objects/gear_data/__init__.py
+gearpy/mechanical_objects/gear_data/lewis_factor_table.csv
+gearpy/mechanical_objects/gear_data/worm_gear_and_wheel_data.csv
 gearpy/motor_control/__init__.py
 gearpy/motor_control/motor_control_base.py
 gearpy/motor_control/pwm_control.py
 gearpy/motor_control/rules/__init__.py
 gearpy/motor_control/rules/constant_pwm.py
 gearpy/motor_control/rules/reach_angular_position.py
 gearpy/motor_control/rules/rules_base.py
```

