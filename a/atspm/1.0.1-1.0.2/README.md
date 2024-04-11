# Comparing `tmp/atspm-1.0.1.tar.gz` & `tmp/atspm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atspm-1.0.1.tar", last modified: Thu Apr 11 18:12:52 2024, max compression
+gzip compressed data, was "atspm-1.0.2.tar", last modified: Thu Apr 11 18:22:30 2024, max compression
```

## Comparing `atspm-1.0.1.tar` & `atspm-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 18:12:52.030192 atspm-1.0.1/
--rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       76 2024-04-11 18:05:43.000000 atspm-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2452 2024-04-11 18:12:52.029192 atspm-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1979 2024-04-11 00:14:17.000000 atspm-1.0.1/README.md
--rw-rw-rw-   0        0        0      579 2024-04-11 18:12:43.000000 atspm-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 18:12:52.030192 atspm-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 18:12:52.008192 atspm-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 18:12:52.016192 atspm-1.0.1/src/atspm/
--rw-rw-rw-   0        0        0    16337 2024-04-11 16:55:36.000000 atspm-1.0.1/src/atspm/Aggregations.py
--rw-rw-rw-   0        0        0       78 2024-04-11 16:51:21.000000 atspm-1.0.1/src/atspm/__init__.py
--rw-rw-rw-   0        0        0      505 2024-04-11 16:48:33.000000 atspm-1.0.1/src/atspm/sample_data.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:12:52.028192 atspm-1.0.1/src/atspm.egg-info/
--rw-rw-rw-   0        0        0     2452 2024-04-11 18:12:51.000000 atspm-1.0.1/src/atspm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-11 18:12:52.000000 atspm-1.0.1/src/atspm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 18:12:51.000000 atspm-1.0.1/src/atspm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-11 18:12:51.000000 atspm-1.0.1/src/atspm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 18:22:30.131035 atspm-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-04-11 00:30:22.000000 atspm-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-04-11 18:18:08.000000 atspm-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2452 2024-04-11 18:22:30.130035 atspm-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1979 2024-04-11 00:14:17.000000 atspm-1.0.2/README.md
+-rw-rw-rw-   0        0        0      579 2024-04-11 18:22:19.000000 atspm-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 18:22:30.132035 atspm-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 18:22:30.108660 atspm-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 18:22:30.119089 atspm-1.0.2/src/atspm/
+-rw-rw-rw-   0        0        0    16337 2024-04-11 16:55:36.000000 atspm-1.0.2/src/atspm/Aggregations.py
+-rw-rw-rw-   0        0        0       78 2024-04-11 16:51:21.000000 atspm-1.0.2/src/atspm/__init__.py
+-rw-rw-rw-   0        0        0    13989 2024-04-11 00:14:17.000000 atspm-1.0.2/src/atspm/queries.sql
+-rw-rw-rw-   0        0        0      505 2024-04-11 16:48:33.000000 atspm-1.0.2/src/atspm/sample_data.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:22:30.130035 atspm-1.0.2/src/atspm.egg-info/
+-rw-rw-rw-   0        0        0     2452 2024-04-11 18:22:30.000000 atspm-1.0.2/src/atspm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-11 18:22:30.000000 atspm-1.0.2/src/atspm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 18:22:30.000000 atspm-1.0.2/src/atspm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 18:22:30.000000 atspm-1.0.2/src/atspm.egg-info/top_level.txt
```

### Comparing `atspm-1.0.1/LICENSE` & `atspm-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atspm-1.0.1/PKG-INFO` & `atspm-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `atspm-1.0.1/README.md` & `atspm-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atspm-1.0.1/pyproject.toml` & `atspm-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atspm"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Shawn Strasser", email="shawn.strasser@odot.oregon.gov" },
 ]
 description = "Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atspm-1.0.1/src/atspm/Aggregations.py` & `atspm-1.0.2/src/atspm/Aggregations.py`

 * *Files identical despite different names*

### Comparing `atspm-1.0.1/src/atspm.egg-info/PKG-INFO` & `atspm-1.0.2/src/atspm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atspm
-Version: 1.0.1
+Version: 1.0.2
 Summary: Aggregates hi-res data from ATC traffic signal controllers into 15-minute binned ATSPM/performance measures.
 Author-email: Shawn Strasser <shawn.strasser@odot.oregon.gov>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

