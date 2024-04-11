# Comparing `tmp/pyrt_lib_rasmusklitgaard-0.2.5.tar.gz` & `tmp/pyrt_lib_rasmusklitgaard-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.2.5.tar", last modified: Wed Apr 10 12:43:26 2024, max compression
+gzip compressed data, was "pyrt_lib_rasmusklitgaard-0.2.6.tar", last modified: Wed Apr 10 13:04:28 2024, max compression
```

## Comparing `pyrt_lib_rasmusklitgaard-0.2.5.tar` & `pyrt_lib_rasmusklitgaard-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:43:26.704283 pyrt_lib_rasmusklitgaard-0.2.5/
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.5/LICENSE
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 12:43:26.704283 pyrt_lib_rasmusklitgaard-0.2.5/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.5/README.md
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-10 12:43:21.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyproject.toml
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:43:26.704283 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/
--rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      126 2024-04-09 08:44:27.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/__init__.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-10 12:43:24.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/cohort.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-10 12:43:24.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/helpers.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/image_looper.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    13107 2024-04-10 12:43:24.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-10 12:43:24.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/patient.py
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-10 12:43:24.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/select_structures.py
-drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 12:43:26.704283 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/
--rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 12:43:26.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-10 12:43:26.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-10 12:43:26.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-10 12:43:26.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-10 12:43:26.000000 pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
--rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-10 12:43:26.704283 pyrt_lib_rasmusklitgaard-0.2.5/setup.cfg
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 13:04:28.542864 pyrt_lib_rasmusklitgaard-0.2.6/
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    35076 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.6/LICENSE
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 13:04:28.542864 pyrt_lib_rasmusklitgaard-0.2.6/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      967 2024-02-06 14:03:05.000000 pyrt_lib_rasmusklitgaard-0.2.6/README.md
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      921 2024-04-10 13:04:22.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyproject.toml
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 13:04:28.542864 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/
+-rwxrwxr-x   0 rasmus    (1000) rasmus    (1000)      126 2024-04-09 08:44:27.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/__init__.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     4113 2024-04-10 13:04:26.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/cohort.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    10392 2024-04-10 13:04:26.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/helpers.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      793 2024-04-09 08:44:14.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/image_looper.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    13107 2024-04-10 13:04:26.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)    32581 2024-04-10 13:04:26.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/patient.py
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)     1242 2024-04-10 13:04:26.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/select_structures.py
+drwxrwxr-x   0 rasmus    (1000) rasmus    (1000)        0 2024-04-10 13:04:28.542864 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/
+-rw-r--r--   0 rasmus    (1000) rasmus    (1000)     1776 2024-04-10 13:04:28.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      539 2024-04-10 13:04:28.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)        1 2024-04-10 13:04:28.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/dependency_links.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)      140 2024-04-10 13:04:28.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/requires.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       25 2024-04-10 13:04:28.000000 pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/top_level.txt
+-rw-rw-r--   0 rasmus    (1000) rasmus    (1000)       38 2024-04-10 13:04:28.542864 pyrt_lib_rasmusklitgaard-0.2.6/setup.cfg
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/LICENSE` & `pyrt_lib_rasmusklitgaard-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.2.5
+Version: 0.2.6
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/README.md` & `pyrt_lib_rasmusklitgaard-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyproject.toml` & `pyrt_lib_rasmusklitgaard-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "pyrt_lib_rasmusklitgaard"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Rasmus Klitgaard", email="rasmusklitgaard97@gmail.com" },
 ]
 description = "PYthon RadioTherapy library"
 readme = "README.md"
 dependencies = [
 "numpy>=1.26.3",
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/cohort.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/cohort.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/helpers.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/helpers.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/image_looper.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/image_looper.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/lkb_ntcp.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/lkb_ntcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 
 	lwd_rbe = 1+0.055 * letd_array_in_structure
 	lwd_dose_in_structure = lwd_rbe / 1.1 * dose_array_in_structure
 
 	original_vXgy = len(dose_array_in_structure[dose_array_in_structure>=dose_threshold]) / len(dose_array_in_structure)
 	lwd_rbe_vXgy = len(lwd_dose_in_structure[lwd_dose_in_structure>=dose_threshold]) / len(lwd_dose_in_structure)
 
-	return lwd_rbe_vXgy / original_vXgy * 100
+	return (lwd_rbe_vXgy - original_vXgy)*100
 
 def calculate_let_percentage_over_threshold_rectum(patient : Patient, structure_of_interest, dose_threshold, percentage) -> float:
 	flk_dicom_paths = [s for s in patient.list_of_dicom_file_paths if s.split("/")[-1][:3] == "FLK"]
 	flk_biodose_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:12] == "FLK_Bio-dose"][0]
 	flk_letd_dicom_path = [s for s in flk_dicom_paths if s.split("/")[-1][:8] == "FLK_LETd"][0]
 
 	flk_biodose_dicom = pd.read_file(flk_biodose_dicom_path)
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/patient.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/patient.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard/select_structures.py` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard/select_structures.py`

 * *Files identical despite different names*

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrt_lib_rasmusklitgaard
-Version: 0.2.5
+Version: 0.2.6
 Summary: PYthon RadioTherapy library
 Author-email: Rasmus Klitgaard <rasmusklitgaard97@gmail.com>
 Project-URL: Homepage, https://gitlab.com/dcpt-research/pyrt-lib
 Project-URL: Issues, https://gitlab.com/dcpt-research/pyrt-lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrt_lib_rasmusklitgaard-0.2.5/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt` & `pyrt_lib_rasmusklitgaard-0.2.6/pyrt_lib_rasmusklitgaard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

