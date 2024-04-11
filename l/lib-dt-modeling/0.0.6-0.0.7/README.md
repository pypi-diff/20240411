# Comparing `tmp/lib-dt-modeling-0.0.6.tar.gz` & `tmp/lib-dt-modeling-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dt-modeling-0.0.6.tar", last modified: Tue Dec  5 17:10:37 2023, max compression
+gzip compressed data, was "lib-dt-modeling-0.0.7.tar", last modified: Thu Apr 11 18:18:35 2024, max compression
```

## Comparing `lib-dt-modeling-0.0.6.tar` & `lib-dt-modeling-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      461 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1941 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/dt_modeling/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-12-05 17:09:05.000000 lib-dt-modeling-0.0.6/src/dt_modeling/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/dt_modeling/electronics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3058 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/electronics/PWM.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/electronics/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1821 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/forward.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2386 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/inverse.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      286 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/dt_modeling/odometry/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/odometry/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      493 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.6/src/dt_modeling/odometry/types.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3269 2023-12-05 17:08:34.000000 lib-dt-modeling-0.0.6/src/dt_modeling/odometry/velocity_odometer.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-12-05 17:10:37.864693 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      461 2023-12-05 17:10:37.000000 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      593 2023-12-05 17:10:37.000000 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-12-05 17:10:37.000000 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       40 2023-12-05 17:10:37.000000 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2023-12-05 17:10:37.000000 lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1941 2023-12-17 21:31:25.000000 lib-dt-modeling-0.0.7/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.744574 lib-dt-modeling-0.0.7/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2024-04-11 18:18:26.000000 lib-dt-modeling-0.0.7/src/dt_modeling/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:14:45.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2708 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/dynamics_delay.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1527 2024-04-11 18:14:09.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/generic_kinematics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1252 2024-04-11 18:10:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/platform_dynamics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7200 2024-04-11 18:17:35.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/pwm_dynamics.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      187 2023-06-15 23:02:47.000000 lib-dt-modeling-0.0.7/src/dt_modeling/dynamics/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3058 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/PWM.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/electronics/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1821 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/forward.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2386 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/inverse.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      286 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      493 2023-04-19 19:49:21.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/types.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3253 2023-12-05 17:28:48.000000 lib-dt-modeling-0.0.7/src/dt_modeling/odometry/velocity_odometer.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-11 18:18:35.748574 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      477 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      841 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       40 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2024-04-11 18:18:35.000000 lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/top_level.txt
```

### Comparing `lib-dt-modeling-0.0.6/setup.py` & `lib-dt-modeling-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # :==> Fill in your project data here
 # The package name is the name on PyPI
 # it is not the python module names.
 package_name = "dt-modeling"
 library_webpage = f"http://github.com/duckietown/lib-{package_name}"
 maintainer = "Andrea F. Daniele"
-maintainer_email = "afdaniele@duckietown.org"
+maintainer_email = "afdaniele@duckietown.com"
 short_description = "Modeling components of Duckietown's autonomy behavior."
 full_description = """
 Modeling components of the autonomous behavior pipeline running on Duckietown robots.
 """
 
 # Read version from the __init__ file
 def get_version_from_source(filename):
```

### Comparing `lib-dt-modeling-0.0.6/src/dt_modeling/electronics/PWM.py` & `lib-dt-modeling-0.0.7/src/dt_modeling/electronics/PWM.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/forward.py` & `lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/forward.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.6/src/dt_modeling/kinematics/inverse.py` & `lib-dt-modeling-0.0.7/src/dt_modeling/kinematics/inverse.py`

 * *Files identical despite different names*

### Comparing `lib-dt-modeling-0.0.6/src/dt_modeling/odometry/velocity_odometer.py` & `lib-dt-modeling-0.0.7/src/dt_modeling/odometry/velocity_odometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         self._pose: Pose2DEstimate = Pose2DEstimate(0, 0, 0, 0)
 
     def update(self, v: float, omega: float, timestamp: float = None):
         """
         Performs the calclulation from velocity to pose and publishes a messsage with the result.
 
         Args:
-            v (:obj:`float`):           desired linear velocity of the chassis in meters/second
-            omega (:obj:`float`):       desired angular velocity of the chassis in radians/second
+            v (:obj:`float`):           linear velocity of the chassis in meters/second
+            omega (:obj:`float`):       angular velocity of the chassis in radians/second
             timestamp (:obj:`float`):   timestamp in seconds when the reading was performed, if
                                         None is given, the current time is used
 
         """
         timestamp = timestamp if timestamp is not None else time.time()
 
         with self._lock:
```

### Comparing `lib-dt-modeling-0.0.6/src/lib_dt_modeling.egg-info/SOURCES.txt` & `lib-dt-modeling-0.0.7/src/lib_dt_modeling.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 setup.py
 src/dt_modeling/__init__.py
+src/dt_modeling/dynamics/__init__.py
+src/dt_modeling/dynamics/dynamics_delay.py
+src/dt_modeling/dynamics/generic_kinematics.py
+src/dt_modeling/dynamics/platform_dynamics.py
+src/dt_modeling/dynamics/pwm_dynamics.py
+src/dt_modeling/dynamics/types.py
 src/dt_modeling/electronics/PWM.py
 src/dt_modeling/electronics/__init__.py
 src/dt_modeling/kinematics/__init__.py
 src/dt_modeling/kinematics/forward.py
 src/dt_modeling/kinematics/inverse.py
 src/dt_modeling/kinematics/utils.py
 src/dt_modeling/odometry/__init__.py
```

