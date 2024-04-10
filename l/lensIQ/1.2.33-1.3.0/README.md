# Comparing `tmp/lensIQ-1.2.33.tar.gz` & `tmp/lensIQ-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensIQ-1.2.33.tar", last modified: Mon Feb 26 21:02:49 2024, max compression
+gzip compressed data, was "lensIQ-1.3.0.tar", last modified: Wed Apr 10 22:24:05 2024, max compression
```

## Comparing `lensIQ-1.2.33.tar` & `lensIQ-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 21:02:49.590499 lensIQ-1.2.33/
--rw-rw-rw-   0        0        0     3758 2024-01-12 23:13:24.000000 lensIQ-1.2.33/LICENSE
--rw-rw-rw-   0        0        0     6133 2024-02-26 21:02:49.590499 lensIQ-1.2.33/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2024-02-23 18:42:25.000000 lensIQ-1.2.33/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 21:02:49.540001 lensIQ-1.2.33/lensIQ/
--rw-rw-rw-   0        0        0      254 2024-01-09 19:31:09.000000 lensIQ-1.2.33/lensIQ/__init__.py
--rw-rw-rw-   0        0        0    22102 2024-01-25 19:50:47.000000 lensIQ-1.2.33/lensIQ/defaultCalData.py
--rw-rw-rw-   0        0        0    48419 2024-02-23 18:53:29.000000 lensIQ-1.2.33/lensIQ/lensIQ.py
-drwxrwxrwx   0        0        0        0 2024-02-26 21:02:49.590499 lensIQ-1.2.33/lensIQ.egg-info/
--rw-rw-rw-   0        0        0     6133 2024-02-26 21:02:49.000000 lensIQ-1.2.33/lensIQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-02-26 21:02:49.000000 lensIQ-1.2.33/lensIQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 21:02:49.000000 lensIQ-1.2.33/lensIQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-26 21:02:49.000000 lensIQ-1.2.33/lensIQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-26 21:02:49.000000 lensIQ-1.2.33/lensIQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      878 2024-02-23 18:42:18.000000 lensIQ-1.2.33/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-26 21:02:49.600832 lensIQ-1.2.33/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.377166 lensIQ-1.3.0/
+-rw-rw-rw-   0        0        0     3758 2024-01-12 23:13:24.000000 lensIQ-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6131 2024-04-10 22:24:05.373395 lensIQ-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5344 2024-04-10 22:16:28.000000 lensIQ-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.296223 lensIQ-1.3.0/lensIQ/
+-rw-rw-rw-   0        0        0      254 2024-01-09 19:31:09.000000 lensIQ-1.3.0/lensIQ/__init__.py
+-rw-rw-rw-   0        0        0    22102 2024-01-25 19:50:47.000000 lensIQ-1.3.0/lensIQ/defaultCalData.py
+-rw-rw-rw-   0        0        0    49490 2024-04-10 22:15:50.000000 lensIQ-1.3.0/lensIQ/lensIQ.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.371400 lensIQ-1.3.0/lensIQ.egg-info/
+-rw-rw-rw-   0        0        0     6131 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      877 2024-04-10 22:16:18.000000 lensIQ-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-10 22:24:05.378169 lensIQ-1.3.0/setup.cfg
```

### Comparing `lensIQ-1.2.33/LICENSE` & `lensIQ-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lensIQ-1.2.33/PKG-INFO` & `lensIQ-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensIQ
-Version: 1.2.33
+Version: 1.3.0
 Summary: Theia MCR motor control conversions and calculations
 Author-email: Mark Peterson <mpeterson@theiatech.com>
 Project-URL: Homepage, https://github.com/cliquot22/lensIQ
 Project-URL: Bug Tracker, https://github.com/cliquot22/lensIQ/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
@@ -90,8 +90,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.2.33
+v.1.3.0
```

### Comparing `lensIQ-1.2.33/README.md` & `lensIQ-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.2.33
+v.1.3.0
```

### Comparing `lensIQ-1.2.33/lensIQ/defaultCalData.py` & `lensIQ-1.3.0/lensIQ/defaultCalData.py`

 * *Files identical despite different names*

### Comparing `lensIQ-1.2.33/lensIQ/lensIQ.py` & `lensIQ-1.3.0/lensIQ/lensIQ.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,18 +391,37 @@
             err = lensIQ.ERR_RANGE_MAX
             zoomStep = zoomStepMax
 
         # save the results
         self.updateEngValues('zoomStep', zoomStep)
         return zoomStep, err
 
-    # calculate object distance from focus motor step
+    # calculate focus motor step from object distance and zoom step
+    def zoomStep2FocusStep(self, zoomStep:int, OD:float, BFL:int=0) -> Tuple[int, str]:
+        '''
+        Calculate focus motor step from object distance and zoom step. 
+        The focus motor step number will be limited to the available range.
+        Maximum object distance input can be 1000m (infinity).  Minimum object distance
+        can be 0 but focus motor step may not support this minimum.  Also, the focus/zoom
+        calculation can cause fitting errors outside the acceptable range.
+        ### input
+        - zoomStep: current zoom motor step position
+        - OD: object distance
+        - BFL (optional: 0): back focus step adjustment
+        ### return
+        [focusStep, note]
+        'note' string value can be: ['OK' | 'no cal data' | 'out of range-min' | 'out of range-max' | 'no OD set' | 'not a number']
+        '''
+        focusStep, err = self.OD2FocusStep(OD, zoomStep, BFL)
+        return focusStep, err
+    
+    # calculate focus motor step from object distance and zoom step (alternate)
     def OD2FocusStep(self, OD:float, zoomStep:int, BFL:int=0) -> Tuple[int, str]:
         '''
-        Calculate object distance from focus motor step. 
+        Calculate focus motor step from object distance and zoom step. 
         The focus motor step number will be limited to the available range.
         Maximum object distance input can be 1000m (infinity).  Minimum object distance
         can be 0 but focus motor step may not support this minimum.  Also, the focus/zoom
         calculation can cause fitting errors outside the acceptable range.
         ### input
         - OD: object distance
         - zoomStep: current zoom motor step position
@@ -873,15 +892,15 @@
         correctionValue = nppp.polyval(FL, self.BFLCorrectionCoeffs)
         return int(correctionValue)
 
     # store data points for BFL correction
     def addBFLCorrection(self, FL:float, focusStep:int, OD:float=1000000) -> list:
         '''
         Store data points for BFL correction. 
-        With the lens set to an object distance and focal length, the calculated focal step is compared
+        With the lens set to an object distance and focal length, the calculated focus step is compared
         to the set best focus position.  The difference is added to the BFL correction factor list.  
         Add a focus shift amount to the list and fit for focal length [[FL, focus shift], [...]]. 
         
         NOTE: all points are used for fitting regardless of the object distance.  Make sure the saved
         points all have the same object distance.  
         ### input
         - FL: current focal length
```

### Comparing `lensIQ-1.2.33/lensIQ.egg-info/PKG-INFO` & `lensIQ-1.3.0/lensIQ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensIQ
-Version: 1.2.33
+Version: 1.3.0
 Summary: Theia MCR motor control conversions and calculations
 Author-email: Mark Peterson <mpeterson@theiatech.com>
 Project-URL: Homepage, https://github.com/cliquot22/lensIQ
 Project-URL: Bug Tracker, https://github.com/cliquot22/lensIQ/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
@@ -90,8 +90,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.2.33
+v.1.3.0
```

### Comparing `lensIQ-1.2.33/pyproject.toml` & `lensIQ-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lensIQ"
-version = "1.2.33"
+version = "1.3.0"
 authors = [
   { name="Mark Peterson", email="mpeterson@theiatech.com" },
 ]
 description = "Theia MCR motor control conversions and calculations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

