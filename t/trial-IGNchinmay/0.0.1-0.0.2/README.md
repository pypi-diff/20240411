# Comparing `tmp/trial_IGNchinmay-0.0.1.tar.gz` & `tmp/trial_IGNchinmay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trial_IGNchinmay-0.0.1.tar", last modified: Thu Apr 11 07:37:11 2024, max compression
+gzip compressed data, was "trial_IGNchinmay-0.0.2.tar", last modified: Thu Apr 11 10:05:46 2024, max compression
```

## Comparing `trial_IGNchinmay-0.0.1.tar` & `trial_IGNchinmay-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 07:37:11.008347 trial_IGNchinmay-0.0.1/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.1/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 07:37:11.008347 trial_IGNchinmay-0.0.1/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      212 2024-04-11 07:36:58.000000 trial_IGNchinmay-0.0.1/README.md
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-11 07:07:12.000000 trial_IGNchinmay-0.0.1/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-11 07:37:11.008347 trial_IGNchinmay-0.0.1/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 07:37:11.008347 trial_IGNchinmay-0.0.1/trial_IGNchinmay/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3078 2024-04-11 07:16:32.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 07:37:11.008347 trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 07:37:11.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-11 07:37:11.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-11 07:37:11.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-11 07:37:11.000000 trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:05:46.797520 trial_IGNchinmay-0.0.2/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.2/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 10:05:46.797520 trial_IGNchinmay-0.0.2/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      212 2024-04-11 07:36:58.000000 trial_IGNchinmay-0.0.2/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-11 10:05:17.000000 trial_IGNchinmay-0.0.2/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-11 10:05:46.797520 trial_IGNchinmay-0.0.2/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:05:46.793521 trial_IGNchinmay-0.0.2/trial_IGNchinmay/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3078 2024-04-11 07:16:32.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay/json_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-11 10:05:46.797520 trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      830 2024-04-11 10:05:46.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-11 10:05:46.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-11 10:05:46.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-11 10:05:46.000000 trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/top_level.txt
```

### Comparing `trial_IGNchinmay-0.0.1/LICENSE` & `trial_IGNchinmay-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trial_IGNchinmay-0.0.1/PKG-INFO` & `trial_IGNchinmay-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trial_IGNchinmay-0.0.1/pyproject.toml` & `trial_IGNchinmay-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trial_IGNchinmay"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `trial_IGNchinmay-0.0.1/trial_IGNchinmay/json_utils.py` & `trial_IGNchinmay-0.0.2/trial_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `trial_IGNchinmay-0.0.1/trial_IGNchinmay.egg-info/PKG-INFO` & `trial_IGNchinmay-0.0.2/trial_IGNchinmay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

