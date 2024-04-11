# Comparing `tmp/geo_parameters-0.2.2.tar.gz` & `tmp/geo_parameters-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_parameters-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_parameters-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_parameters-0.2.2.tar` & `geo_parameters-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1776 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/.gitignore
--rw-r--r--   0        0        0     1079 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/LICENSE
--rw-r--r--   0        0        0     3386 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/README.md
--rw-r--r--   0        0        0       91 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/environment.yml
--rw-r--r--   0        0        0       90 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/geo_parameters/__init__.py
--rw-r--r--   0        0        0      376 2024-04-11 12:10:04.065410 geo_parameters-0.2.2/geo_parameters/grid.py
--rw-r--r--   0        0        0     1967 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/geo_parameters/metaparameter.py
--rw-r--r--   0        0        0     1298 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/geo_parameters/ocean.py
--rw-r--r--   0        0        0     1124 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/geo_parameters/parameter_funcs.py
--rw-r--r--   0        0        0    10723 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/geo_parameters/wave.py
--rw-r--r--   0        0        0     1388 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/geo_parameters/wind.py
--rw-r--r--   0        0        0      450 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1810 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/tests/test_doc.py
--rw-r--r--   0        0        0     1020 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/tests/test_funcs.py
--rw-r--r--   0        0        0      808 2024-04-11 12:10:04.069410 geo_parameters-0.2.2/tests/test_names.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1776 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3386 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/README.md
+-rw-r--r--   0        0        0       91 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/environment.yml
+-rw-r--r--   0        0        0       90 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/grid.py
+-rw-r--r--   0        0        0     1967 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/metaparameter.py
+-rw-r--r--   0        0        0     1298 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/ocean.py
+-rw-r--r--   0        0        0     1124 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/parameter_funcs.py
+-rw-r--r--   0        0        0    10727 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/wave.py
+-rw-r--r--   0        0        0     1388 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/wind.py
+-rw-r--r--   0        0        0      450 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1810 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_doc.py
+-rw-r--r--   0        0        0     1020 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_funcs.py
+-rw-r--r--   0        0        0      808 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_names.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.3/PKG-INFO
```

### Comparing `geo_parameters-0.2.2/.github/workflows/tests.yml` & `geo_parameters-0.2.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/.gitignore` & `geo_parameters-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/LICENSE` & `geo_parameters-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/README.md` & `geo_parameters-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/geo_parameters/metaparameter.py` & `geo_parameters-0.2.3/geo_parameters/metaparameter.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/geo_parameters/ocean.py` & `geo_parameters-0.2.3/geo_parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/geo_parameters/parameter_funcs.py` & `geo_parameters-0.2.3/geo_parameters/parameter_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/geo_parameters/wave.py` & `geo_parameters-0.2.3/geo_parameters/wave.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,23 +331,23 @@
 class Freq(MetaParameter):
     name = "freq"
     _long_name = "frequency"
     _standard_name = ["wave_frequency", "sea_surface_wave_frequency"]
     _unit = ureg.s**-1
 
 
-class DirFrom(MetaParameter):
-    name = "dir"
+class DirsFrom(MetaParameter):
+    name = "dirs"
     _long_name = "wave_direction"
     _standard_name = "sea_surface_wave_from_direction"
     _unit = ureg.deg
 
 
-class DirTo(MetaParameter):
-    name = "dir"
+class DirsTo(MetaParameter):
+    name = "dirs"
     _long_name = "wave_direction"
     _standard_name = "sea_surface_wave_to_direction"
     _unit = ureg.deg
 
 
 ## Moments (non-standard)
 class M0(MetaParameter):
```

### Comparing `geo_parameters-0.2.2/geo_parameters/wind.py` & `geo_parameters-0.2.3/geo_parameters/wind.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/tests/test_doc.py` & `geo_parameters-0.2.3/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/tests/test_funcs.py` & `geo_parameters-0.2.3/tests/test_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.2/tests/test_names.py` & `geo_parameters-0.2.3/tests/test_names.py`

 * *Files identical despite different names*

