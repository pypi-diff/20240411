# Comparing `tmp/GRSdriver-1.0.2.1.tar.gz` & `tmp/GRSdriver-1.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GRSdriver-1.0.2.1.tar", last modified: Wed Apr 10 17:58:41 2024, max compression
+gzip compressed data, was "GRSdriver-1.0.2a0.tar", last modified: Wed Apr 10 17:54:17 2024, max compression
```

## Comparing `GRSdriver-1.0.2.1.tar` & `GRSdriver-1.0.2a0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:58:41.521125 GRSdriver-1.0.2.1/
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:58:41.513125 GRSdriver-1.0.2.1/GRSdriver/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      195 2024-04-10 17:21:57.000000 GRSdriver-1.0.2.1/GRSdriver/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    21581 2024-04-08 16:59:28.000000 GRSdriver-1.0.2.1/GRSdriver/driver_S2_SAFE.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     7659 2024-04-08 16:59:28.000000 GRSdriver-1.0.2.1/GRSdriver/driver_landsat_col2.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:58:41.513125 GRSdriver-1.0.2.1/GRSdriver/rsr/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/__init__.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:58:41.517125 GRSdriver-1.0.2.1/GRSdriver/rsr/data/
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   174535 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    81844 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/L4_TM_RSR.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    80969 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/L5_TM_RSR.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)    87561 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/L7_RSR.xlsx
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   655775 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx
--rwxrwxr-x   0 harmel    (1001) harmel    (1001)   882434 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/__init__.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/rsr_landsat_8_oli.nc
--rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/data/rsr_landsat_9_oli.nc
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     2754 2024-02-12 15:04:09.000000 GRSdriver-1.0.2.1/GRSdriver/rsr/landsat_formatting.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1889 2024-04-10 17:05:28.000000 GRSdriver-1.0.2.1/GRSdriver/run.py
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     8096 2024-04-10 11:19:05.000000 GRSdriver-1.0.2.1/GRSdriver/visual.py
-drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:58:41.517125 GRSdriver-1.0.2.1/GRSdriver.egg-info/
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15500 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)      773 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       50 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/entry_points.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       44 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/requires.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       29 2024-04-10 17:58:41.000000 GRSdriver-1.0.2.1/GRSdriver.egg-info/top_level.txt
--rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 GRSdriver-1.0.2.1/LICENSE
--rw-r--r--   0 harmel    (1001) harmel    (1001)    15500 2024-04-10 17:58:41.517125 GRSdriver-1.0.2.1/PKG-INFO
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1777 2024-04-10 11:19:39.000000 GRSdriver-1.0.2.1/README.md
--rw-rw-r--   0 harmel    (1001) harmel    (1001)     1240 2024-04-10 17:58:34.000000 GRSdriver-1.0.2.1/pyproject.toml
--rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-10 17:58:41.521125 GRSdriver-1.0.2.1/setup.cfg
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:54:17.352055 GRSdriver-1.0.2a0/
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:54:17.348055 GRSdriver-1.0.2a0/GRSdriver/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)      195 2024-04-10 17:21:57.000000 GRSdriver-1.0.2a0/GRSdriver/__init__.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    21581 2024-04-08 16:59:28.000000 GRSdriver-1.0.2a0/GRSdriver/driver_S2_SAFE.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     7659 2024-04-08 16:59:28.000000 GRSdriver-1.0.2a0/GRSdriver/driver_landsat_col2.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:54:17.348055 GRSdriver-1.0.2a0/GRSdriver/rsr/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/__init__.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:54:17.352055 GRSdriver-1.0.2a0/GRSdriver/rsr/data/
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   174535 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    81844 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/L4_TM_RSR.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    80969 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/L5_TM_RSR.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)    87561 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/L7_RSR.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   655775 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx
+-rwxrwxr-x   0 harmel    (1001) harmel    (1001)   882434 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        0 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/__init__.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/rsr_landsat_8_oli.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)   165342 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/data/rsr_landsat_9_oli.nc
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     2754 2024-02-12 15:04:09.000000 GRSdriver-1.0.2a0/GRSdriver/rsr/landsat_formatting.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1889 2024-04-10 17:05:28.000000 GRSdriver-1.0.2a0/GRSdriver/run.py
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     8096 2024-04-10 11:19:05.000000 GRSdriver-1.0.2a0/GRSdriver/visual.py
+drwxrwxr-x   0 harmel    (1001) harmel    (1001)        0 2024-04-10 17:54:17.352055 GRSdriver-1.0.2a0/GRSdriver.egg-info/
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15500 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)      773 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)        1 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       50 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/entry_points.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       44 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/requires.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       29 2024-04-10 17:54:17.000000 GRSdriver-1.0.2a0/GRSdriver.egg-info/top_level.txt
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)    11349 2024-04-09 09:36:02.000000 GRSdriver-1.0.2a0/LICENSE
+-rw-r--r--   0 harmel    (1001) harmel    (1001)    15500 2024-04-10 17:54:17.352055 GRSdriver-1.0.2a0/PKG-INFO
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1777 2024-04-10 11:19:39.000000 GRSdriver-1.0.2a0/README.md
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)     1240 2024-04-10 17:54:04.000000 GRSdriver-1.0.2a0/pyproject.toml
+-rw-rw-r--   0 harmel    (1001) harmel    (1001)       38 2024-04-10 17:54:17.352055 GRSdriver-1.0.2a0/setup.cfg
```

### Comparing `GRSdriver-1.0.2.1/GRSdriver/driver_S2_SAFE.py` & `GRSdriver-1.0.2a0/GRSdriver/driver_S2_SAFE.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/driver_landsat_col2.py` & `GRSdriver-1.0.2a0/GRSdriver/driver_landsat_col2.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/Ball_BA_RSR.v1.2.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/L4_TM_RSR.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/L4_TM_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/L5_TM_RSR.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/L5_TM_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/L7_RSR.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/L7_RSR.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/L9_OLI2_Ball_FPM_RSR.v1.0.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/Sentinel-2_MSI_Spectral_Responses.xlsx`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/rsr_landsat_8_oli.nc` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/rsr_landsat_8_oli.nc`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/data/rsr_landsat_9_oli.nc` & `GRSdriver-1.0.2a0/GRSdriver/rsr/data/rsr_landsat_9_oli.nc`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/rsr/landsat_formatting.py` & `GRSdriver-1.0.2a0/GRSdriver/rsr/landsat_formatting.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/run.py` & `GRSdriver-1.0.2a0/GRSdriver/run.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver/visual.py` & `GRSdriver-1.0.2a0/GRSdriver/visual.py`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/GRSdriver.egg-info/PKG-INFO` & `GRSdriver-1.0.2a0/GRSdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.2.1
+Version: 1.0.2a0
 Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `GRSdriver-1.0.2.1/GRSdriver.egg-info/SOURCES.txt` & `GRSdriver-1.0.2a0/GRSdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/LICENSE` & `GRSdriver-1.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/PKG-INFO` & `GRSdriver-1.0.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GRSdriver
-Version: 1.0.2.1
+Version: 1.0.2a0
 Summary: Driver for L1C satellite images dedicated to GRS processor
 Author-email: Tristan Harmel <tristan.harmel@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `GRSdriver-1.0.2.1/README.md` & `GRSdriver-1.0.2a0/README.md`

 * *Files identical despite different names*

### Comparing `GRSdriver-1.0.2.1/pyproject.toml` & `GRSdriver-1.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GRSdriver"
-version = "1.0.2.1"
+version = "1.0.2.a"
 description = "Driver for L1C satellite images dedicated to GRS processor"
 readme = "README.md"
 authors = [{ name = "Tristan Harmel", email = "tristan.harmel@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

