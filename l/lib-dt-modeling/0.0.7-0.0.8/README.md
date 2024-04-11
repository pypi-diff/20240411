# Comparing `tmp/lib-dt-modeling-0.0.7.tar.gz` & `tmp/lib-dt-modeling-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-modeling-0.0.7.tar", last modified: Thu Apr 11 18:18:35 2024, max compression
+gzip compressed data, was "lib-dt-modeling-0.0.8.tar", last modified: Thu Apr 11 18:44:48 2024, max compression
```

## Comparing `lib-dt-modeling-0.0.7.tar` & `lib-dt-modeling-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1941 2023-12-17 21:31:25.000000 lib-dt-modeling-0.0.7/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.744574 lib-dt-modeling-0.0.7/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-11 18:18:26.000000 lib-dt-modeling-0.0.7/src/dt_modeling/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:14:45.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2708 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/dynamics_delay.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1527 2024-04-11 18:14:09.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/generic_kinematics.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1252 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/platform_dynamics.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7200 2024-04-11 18:17:35.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/pwm_dynamics.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      187 2023-06-15 23:02:47.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3058 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/PWM.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1821 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/forward.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2386 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/inverse.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      286 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      493 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/types.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3253 2023-12-05 17:28:48.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/velocity_odometer.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/
--rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      841 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       40 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1880 2024-04-11 18:44:25.000000 lib-dt-modeling-0.0.8/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.680656 lib-dt-modeling-0.0.8/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.680656 lib-dt-modeling-0.0.8/src/dt_modeling/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-11 18:44:44.000000 lib-dt-modeling-0.0.8/src/dt_modeling/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.680656 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:14:45.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2708 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/dynamics_delay.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1527 2024-04-11 18:14:09.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/generic_kinematics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1252 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/platform_dynamics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7200 2024-04-11 18:17:35.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/pwm_dynamics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      187 2023-06-15 23:02:47.000000 lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.680656 lib-dt-modeling-0.0.8/src/dt_modeling/electronics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3058 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/electronics/PWM.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/electronics/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1821 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/forward.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2386 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/inverse.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      286 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/src/dt_modeling/odometry/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/odometry/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      493 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.8/src/dt_modeling/odometry/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3253 2023-12-05 17:28:48.000000 lib-dt-modeling-0.0.8/src/dt_modeling/odometry/velocity_odometer.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:44:48.684656 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:44:48.000000 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      841 2024-04-11 18:44:48.000000 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-11 18:44:48.000000 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       40 2024-04-11 18:44:48.000000 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2024-04-11 18:44:48.000000 lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/top_level.txt
```

### Comparing `lib-dt-modeling-0.0.7/setup.py` & `lib-dt-modeling-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,15 @@
         raise ValueError(filename)
     return version
 
 
 version = get_version_from_source(f"src/{package_name.replace('-', '_')}/__init__.py")
 
 install_requires = [
-    # numpy (1.21.5 is the last numpy supporting Python 3.7)
-    "numpy<=1.21.5",
+    "numpy<=1.26.2",
     "transformations~=2021.6.6"
 ]
 tests_require = []
 
 # compile description
 underline = "=" * (len(package_name) + len(short_description) + 2)
 description = """
```

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/dynamics_delay.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/dynamics_delay.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/generic_kinematics.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/generic_kinematics.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/platform_dynamics.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/platform_dynamics.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/pwm_dynamics.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/dynamics/pwm_dynamics.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/electronics/PWM.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/electronics/PWM.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/forward.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/forward.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/inverse.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/kinematics/inverse.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/dt_modeling/odometry/velocity_odometer.py` & `lib-dt-modeling-0.0.8/src/dt_modeling/odometry/velocity_odometer.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/SOURCES.txt` & `lib-dt-modeling-0.0.8/src/lib_dt_modeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

