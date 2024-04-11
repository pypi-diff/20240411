# Comparing `tmp/stabilizer_timelime-0.0.5.tar.gz` & `tmp/stabilizer_timelime-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.0.5.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.0.6.tar", max compression
```

## Comparing `stabilizer_timelime-0.0.5.tar` & `stabilizer_timelime-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.0.5/LICENSE
--rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.0.5/README.md
--rw-r--r--   0        0        0      630 2024-04-11 19:45:47.883512 stabilizer_timelime-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 18:41:51.440222 stabilizer_timelime-0.0.5/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0     7274 2024-04-11 19:45:19.104475 stabilizer_timelime-0.0.5/stabilizer_timelime/src/slurpdata.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 stabilizer_timelime-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 18:45:02.113558 stabilizer_timelime-0.0.6/LICENSE
+-rw-r--r--   0        0        0       23 2024-04-02 18:45:48.645909 stabilizer_timelime-0.0.6/README.md
+-rw-r--r--   0        0        0      630 2024-04-11 19:47:08.616929 stabilizer_timelime-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 18:41:51.440222 stabilizer_timelime-0.0.6/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0     7274 2024-04-11 19:45:19.104475 stabilizer_timelime-0.0.6/stabilizer_timelime/src/slurpdata.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 stabilizer_timelime-0.0.6/PKG-INFO
```

### Comparing `stabilizer_timelime-0.0.5/LICENSE` & `stabilizer_timelime-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.0.5/pyproject.toml` & `stabilizer_timelime-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.0.5"
+version = "0.0.6"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `stabilizer_timelime-0.0.5/stabilizer_timelime/src/slurpdata.py` & `stabilizer_timelime-0.0.6/stabilizer_timelime/src/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.0.5/PKG-INFO` & `stabilizer_timelime-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.0.5
+Version: 0.0.6
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

