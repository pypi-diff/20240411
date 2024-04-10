# Comparing `tmp/dkist-processing-test-1.9.8.tar.gz` & `tmp/dkist-processing-test-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-test-1.9.8.tar", last modified: Tue Mar  5 19:12:30 2024, max compression
+gzip compressed data, was "dkist-processing-test-1.9.9.tar", last modified: Tue Mar 26 22:59:08 2024, max compression
```

## Comparing `dkist-processing-test-1.9.8.tar` & `dkist-processing-test-1.9.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.373908 dkist-processing-test-1.9.8/
--rw-rw-rw-   0 root         (0) root         (0)     2417 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2024 2024-03-05 19:12:30.373908 dkist-processing-test-1.9.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3662 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.369908 dkist-processing-test-1.9.8/dkist_processing_test/
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.369908 dkist-processing-test-1.9.8/dkist_processing_test/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/models/parameters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.369908 dkist-processing-test-1.9.8/dkist_processing_test/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1429 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/fail.py
--rw-rw-rw-   0 root         (0) root         (0)     3983 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/fake_science.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/high_memory.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/movie.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/noop.py
--rw-rw-rw-   0 root         (0) root         (0)     2329 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1397 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.373908 dkist-processing-test-1.9.8/dkist_processing_test/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    18758 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/tests/test_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.373908 dkist-processing-test-1.9.8/dkist_processing_test/workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5727 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/common_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2174 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/end_to_end.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/exercise_numba.py
--rw-rw-rw-   0 root         (0) root         (0)      326 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/fail.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/noop.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/resource_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1647 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/dkist_processing_test/workflows/trial_end_to_end.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-05 19:12:30.369908 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2024 2024-03-05 19:12:30.000000 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-05 19:12:30.000000 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-05 19:12:30.000000 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      534 2024-03-05 19:12:30.000000 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-05 19:12:30.000000 dkist-processing-test-1.9.8/dkist_processing_test.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1357 2024-03-05 19:12:30.373908 dkist-processing-test-1.9.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-05 19:12:21.000000 dkist-processing-test-1.9.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.426622 dkist-processing-test-1.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2024-03-26 22:59:08.426622 dkist-processing-test-1.9.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3662 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.422622 dkist-processing-test-1.9.9/dkist_processing_test/
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.422622 dkist-processing-test-1.9.9/dkist_processing_test/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1217 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/models/parameters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.422622 dkist-processing-test-1.9.9/dkist_processing_test/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/fake_science.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/high_memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/movie.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)     2329 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1397 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.422622 dkist-processing-test-1.9.9/dkist_processing_test/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    18758 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/tests/test_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.426622 dkist-processing-test-1.9.9/dkist_processing_test/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5727 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/common_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/end_to_end.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/exercise_numba.py
+-rw-rw-rw-   0 root         (0) root         (0)      326 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/fail.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/noop.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/resource_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1647 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/dkist_processing_test/workflows/trial_end_to_end.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 22:59:08.422622 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2024-03-26 22:59:08.000000 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-26 22:59:08.000000 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-26 22:59:08.000000 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-03-26 22:59:08.000000 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-26 22:59:08.000000 dkist-processing-test-1.9.9/dkist_processing_test.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2024-03-26 22:59:08.426622 dkist-processing-test-1.9.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-26 22:59:01.000000 dkist-processing-test-1.9.9/setup.py
```

### Comparing `dkist-processing-test-1.9.8/.gitignore` & `dkist-processing-test-1.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/.pre-commit-config.yaml` & `dkist-processing-test-1.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/PKG-INFO` & `dkist-processing-test-1.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.9.8
+Version: 1.9.9
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.9.8/README.rst` & `dkist-processing-test-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/bitbucket-pipelines.yml` & `dkist-processing-test-1.9.9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/models/parameters.py` & `dkist-processing-test-1.9.9/dkist_processing_test/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/__init__.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/exercise_numba.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/exercise_numba.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/fake_science.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/fake_science.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/high_memory.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/high_memory.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/movie.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/parse.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/quality.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/trial_output_data.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tasks/write_l1.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tests/conftest.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tests/test_parameters.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/tests/test_tasks.py` & `dkist-processing-test-1.9.9/dkist_processing_test/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/workflows/common_tasks.py` & `dkist-processing-test-1.9.9/dkist_processing_test/workflows/common_tasks.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/workflows/end_to_end.py` & `dkist-processing-test-1.9.9/dkist_processing_test/workflows/end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/workflows/noop.py` & `dkist-processing-test-1.9.9/dkist_processing_test/workflows/noop.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test/workflows/trial_end_to_end.py` & `dkist-processing-test-1.9.9/dkist_processing_test/workflows/trial_end_to_end.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test.egg-info/PKG-INFO` & `dkist-processing-test-1.9.9/dkist_processing_test.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-test
-Version: 1.9.8
+Version: 1.9.9
 Summary: Example Instrument code that is used by the DKIST Science Data Processing pipelines to test processing infrastructure.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-test/src/main/
 Author: NSO / AURA
 Author-email: dkistdc@nso.edu
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test.egg-info/SOURCES.txt` & `dkist-processing-test-1.9.9/dkist_processing_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-test-1.9.8/dkist_processing_test.egg-info/requires.txt` & `dkist-processing-test-1.9.9/dkist_processing_test.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==6.0.3
+dkist-processing-common==6.0.4
 dkist-header-validator==5.1.0
 dkist-service-configuration==1.1.0
 dkist-fits-specifications==4.1.1
 numba==0.57.1
 astropy==5.3.0
 numpy==1.24.3
 dkist-spectral-lines==2.0.0
```

### Comparing `dkist-processing-test-1.9.8/setup.cfg` & `dkist-processing-test-1.9.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 6.0.3
+	dkist-processing-common == 6.0.4
 	dkist-header-validator == 5.1.0
 	dkist-service-configuration == 1.1.0
 	dkist-fits-specifications == 4.1.1
 	numba == 0.57.1
 	astropy == 5.3.0
 	numpy == 1.24.3
 	dkist-spectral-lines == 2.0.0
```

