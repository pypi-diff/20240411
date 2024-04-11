# Comparing `tmp/roktools-6.0.3.tar.gz` & `tmp/roktools-6.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roktools-6.0.3.tar", max compression
+gzip compressed data, was "roktools-6.0.4.tar", max compression
```

## Comparing `roktools-6.0.3.tar` & `roktools-6.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-11 10:08:34.355899 roktools-6.0.3/LICENSE
--rw-r--r--   0        0        0     1480 2024-04-11 10:08:34.355899 roktools-6.0.3/README.md
--rw-r--r--   0        0        0     1162 2024-04-11 10:08:34.355899 roktools-6.0.3/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-11 10:08:34.355899 roktools-6.0.3/roktools/__init__.py
--rw-r--r--   0        0        0     4509 2024-04-11 10:08:34.355899 roktools-6.0.3/roktools/cl.py
--rw-r--r--   0        0        0      133 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/constants.py
--rw-r--r--   0        0        0      491 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/decorator.py
--rw-r--r--   0        0        0      927 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/file.py
--rw-r--r--   0        0        0    33609 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/geodetic.py
--rw-r--r--   0        0        0        0 2024-04-11 10:08:34.399898 roktools-6.0.3/roktools/gnss/__init__.py
--rw-r--r--   0        0        0     1878 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/gnss/edit.py
--rw-r--r--   0        0        0     1644 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/gnss/observables.py
--rw-r--r--   0        0        0     1244 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/gnss/residuals.py
--rw-r--r--   0        0        0     9505 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/gnss/types.py
--rw-r--r--   0        0        0     1479 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/logger.py
--rw-r--r--   0        0        0        0 2024-04-11 10:08:34.399898 roktools-6.0.3/roktools/orbit/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/orbit/kepler.py
--rw-r--r--   0        0        0     5898 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/orbit/tle.py
--rw-r--r--   0        0        0        0 2024-04-11 10:08:34.399898 roktools-6.0.3/roktools/parsers/rtklib/__init__,py
--rw-r--r--   0        0        0     5459 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/parsers/rtklib/stats.py
--rw-r--r--   0        0        0    29707 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/rinex.py
--rwxr-xr-x   0        0        0     1083 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/stats.py
--rwxr-xr-x   0        0        0     1598 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/tensorial.py
--rw-r--r--   0        0        0    11293 2024-04-11 10:08:34.359899 roktools-6.0.3/roktools/time.py
--rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 roktools-6.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-11 10:15:22.770942 roktools-6.0.4/LICENSE
+-rw-r--r--   0        0        0     1480 2024-04-11 10:15:22.770942 roktools-6.0.4/README.md
+-rw-r--r--   0        0        0     1162 2024-04-11 10:15:22.770942 roktools-6.0.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-11 10:15:22.770942 roktools-6.0.4/roktools/__init__.py
+-rw-r--r--   0        0        0     4509 2024-04-11 10:15:22.770942 roktools-6.0.4/roktools/cl.py
+-rw-r--r--   0        0        0      133 2024-04-11 10:15:22.770942 roktools-6.0.4/roktools/constants.py
+-rw-r--r--   0        0        0      491 2024-04-11 10:15:22.770942 roktools-6.0.4/roktools/decorator.py
+-rw-r--r--   0        0        0      927 2024-04-11 10:15:22.770942 roktools-6.0.4/roktools/file.py
+-rw-r--r--   0        0        0    33609 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/geodetic.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:15:22.818941 roktools-6.0.4/roktools/gnss/__init__.py
+-rw-r--r--   0        0        0     1878 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/gnss/edit.py
+-rw-r--r--   0        0        0     1644 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/gnss/observables.py
+-rw-r--r--   0        0        0     1244 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/gnss/residuals.py
+-rw-r--r--   0        0        0     9505 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/gnss/types.py
+-rw-r--r--   0        0        0     1479 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/logger.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:15:22.818941 roktools-6.0.4/roktools/orbit/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/orbit/kepler.py
+-rw-r--r--   0        0        0     5898 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/orbit/tle.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:15:22.818941 roktools-6.0.4/roktools/parsers/rtklib/__init__,py
+-rw-r--r--   0        0        0     5459 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/parsers/rtklib/stats.py
+-rw-r--r--   0        0        0    29707 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/rinex.py
+-rwxr-xr-x   0        0        0     1083 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/stats.py
+-rwxr-xr-x   0        0        0     1598 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/tensorial.py
+-rw-r--r--   0        0        0    11293 2024-04-11 10:15:22.774942 roktools-6.0.4/roktools/time.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 roktools-6.0.4/PKG-INFO
```

### Comparing `roktools-6.0.3/LICENSE` & `roktools-6.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/README.md` & `roktools-6.0.4/README.md`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/pyproject.toml` & `roktools-6.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "roktools"
-version = "6.0.3"
+version = "6.0.4"
 description = "Package with utilities and tools for GNSS data processing"
 authors = ["Rokubun <info@rokubun.cat>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.26.4"
```

### Comparing `roktools-6.0.3/roktools/cl.py` & `roktools-6.0.4/roktools/cl.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/file.py` & `roktools-6.0.4/roktools/file.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/geodetic.py` & `roktools-6.0.4/roktools/geodetic.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/gnss/edit.py` & `roktools-6.0.4/roktools/gnss/edit.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/gnss/observables.py` & `roktools-6.0.4/roktools/gnss/observables.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/gnss/residuals.py` & `roktools-6.0.4/roktools/gnss/residuals.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/gnss/types.py` & `roktools-6.0.4/roktools/gnss/types.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/logger.py` & `roktools-6.0.4/roktools/logger.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/orbit/kepler.py` & `roktools-6.0.4/roktools/orbit/kepler.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/orbit/tle.py` & `roktools-6.0.4/roktools/orbit/tle.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/parsers/rtklib/stats.py` & `roktools-6.0.4/roktools/parsers/rtklib/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/rinex.py` & `roktools-6.0.4/roktools/rinex.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/stats.py` & `roktools-6.0.4/roktools/stats.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/tensorial.py` & `roktools-6.0.4/roktools/tensorial.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/roktools/time.py` & `roktools-6.0.4/roktools/time.py`

 * *Files identical despite different names*

### Comparing `roktools-6.0.3/PKG-INFO` & `roktools-6.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 6.0.3
+Version: 6.0.4
 Summary: Package with utilities and tools for GNSS data processing
 Author: Rokubun
 Author-email: info@rokubun.cat
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

