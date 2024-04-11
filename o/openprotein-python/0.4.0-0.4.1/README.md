# Comparing `tmp/openprotein_python-0.4.0.tar.gz` & `tmp/openprotein_python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.4.0.tar", max compression
+gzip compressed data, was "openprotein_python-0.4.1.tar", max compression
```

## Comparing `openprotein_python-0.4.0.tar` & `openprotein_python-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1543 2023-08-07 09:39:52.360055 openprotein_python-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     6547 2024-04-09 02:52:00.438597 openprotein_python-0.4.0/README.md
--rw-r--r--   0        0        0     2841 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/__init__.py
--rw-r--r--   0        0        0      215 2023-08-07 09:39:52.528056 openprotein_python-0.4.0/openprotein/_version.py
--rw-r--r--   0        0        0      148 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/__init__.py
--rw-r--r--   0        0        0    25646 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/align.py
--rw-r--r--   0        0        0    13759 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/data.py
--rw-r--r--   0        0        0    16169 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/design.py
--rw-r--r--   0        0        0    33640 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/embedding.py
--rw-r--r--   0        0        0    12214 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/fold.py
--rw-r--r--   0        0        0    10523 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/jobs.py
--rw-r--r--   0        0        0    18226 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/poet.py
--rw-r--r--   0        0        0    17476 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/predict.py
--rw-r--r--   0        0        0    18835 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/api/train.py
--rw-r--r--   0        0        0     4060 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/base.py
--rw-r--r--   0        0        0      232 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/config.py
--rw-r--r--   0        0        0     1479 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/errors.py
--rw-r--r--   0        0        0     1055 2023-08-04 09:17:01.541290 openprotein_python-0.4.0/openprotein/fasta.py
--rw-r--r--   0        0        0     1889 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/futures.py
--rw-r--r--   0        0        0     5775 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/jobs.py
--rw-r--r--   0        0        0     1504 2024-04-09 02:52:00.530598 openprotein_python-0.4.0/openprotein/schemas.py
--rw-r--r--   0        0        0      595 2024-04-09 03:30:11.136957 openprotein_python-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 openprotein_python-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-07 09:06:21.673361 openprotein_python-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0     6547 2024-04-11 01:35:45.720845 openprotein_python-0.4.1/README.md
+-rw-r--r--   0        0        0     2841 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/__init__.py
+-rw-r--r--   0        0        0      215 2023-08-07 10:10:58.702051 openprotein_python-0.4.1/openprotein/_version.py
+-rw-r--r--   0        0        0      148 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/__init__.py
+-rw-r--r--   0        0        0    25646 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/align.py
+-rw-r--r--   0        0        0    13759 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/data.py
+-rw-r--r--   0        0        0    16169 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/design.py
+-rw-r--r--   0        0        0    33640 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/embedding.py
+-rw-r--r--   0        0        0    12214 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/fold.py
+-rw-r--r--   0        0        0    10523 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/jobs.py
+-rw-r--r--   0        0        0    18226 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/poet.py
+-rw-r--r--   0        0        0    17476 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/predict.py
+-rw-r--r--   0        0        0    18835 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/api/train.py
+-rw-r--r--   0        0        0     4060 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/base.py
+-rw-r--r--   0        0        0      232 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/config.py
+-rw-r--r--   0        0        0     1479 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-07 09:06:21.713361 openprotein_python-0.4.1/openprotein/fasta.py
+-rw-r--r--   0        0        0     1889 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/futures.py
+-rw-r--r--   0        0        0     5775 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/jobs.py
+-rw-r--r--   0        0        0     1504 2024-04-11 01:35:45.628845 openprotein_python-0.4.1/openprotein/schemas.py
+-rw-r--r--   0        0        0      595 2024-04-11 01:37:08.216748 openprotein_python-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7325 1970-01-01 00:00:00.000000 openprotein_python-0.4.1/PKG-INFO
```

### Comparing `openprotein_python-0.4.0/LICENSE.txt` & `openprotein_python-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/README.md` & `openprotein_python-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/__init__.py` & `openprotein_python-0.4.1/openprotein/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/align.py` & `openprotein_python-0.4.1/openprotein/api/align.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/data.py` & `openprotein_python-0.4.1/openprotein/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/design.py` & `openprotein_python-0.4.1/openprotein/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/embedding.py` & `openprotein_python-0.4.1/openprotein/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/fold.py` & `openprotein_python-0.4.1/openprotein/api/fold.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/jobs.py` & `openprotein_python-0.4.1/openprotein/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/poet.py` & `openprotein_python-0.4.1/openprotein/api/poet.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/predict.py` & `openprotein_python-0.4.1/openprotein/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/api/train.py` & `openprotein_python-0.4.1/openprotein/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/base.py` & `openprotein_python-0.4.1/openprotein/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/errors.py` & `openprotein_python-0.4.1/openprotein/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/fasta.py` & `openprotein_python-0.4.1/openprotein/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/futures.py` & `openprotein_python-0.4.1/openprotein/futures.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/jobs.py` & `openprotein_python-0.4.1/openprotein/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/openprotein/schemas.py` & `openprotein_python-0.4.1/openprotein/schemas.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.4.0/pyproject.toml` & `openprotein_python-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openprotein_python"
 packages = [{include = "openprotein"}]
-version = "0.4.0"
+version = "0.4.1"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `openprotein_python-0.4.0/PKG-INFO` & `openprotein_python-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.4.0
+Version: 0.4.1
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

