# Comparing `tmp/qualipy-1.0.2.tar.gz` & `tmp/qualipy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualipy-1.0.2.tar", last modified: Wed Aug 30 03:27:58 2023, max compression
+gzip compressed data, was "qualipy-1.1.0.tar", last modified: Thu Apr 11 00:23:58 2024, max compression
```

## Comparing `qualipy-1.0.2.tar` & `qualipy-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/
--rw-r--r--   0 kali      (1000) kali      (1000)     1070 2023-08-19 19:48:12.000000 qualipy-1.0.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     2882 2023-08-30 03:27:58.893682 qualipy-1.0.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      861 2023-08-30 03:24:31.000000 qualipy-1.0.2/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)     2238 2023-08-30 03:13:09.000000 qualipy-1.0.2/readme.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-08-30 03:27:58.893682 qualipy-1.0.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      344 2023-08-20 01:08:08.000000 qualipy-1.0.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.889682 qualipy-1.0.2/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.889682 qualipy-1.0.2/src/qualipy/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3372 2023-08-30 02:48:34.000000 qualipy-1.0.2/src/qualipy/__main__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/src/qualipy/authentication/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/authentication/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      451 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/authentication/authenticator.py
--rw-r--r--   0 kali      (1000) kali      (1000)      555 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/authentication/keyring_authenticator.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/src/qualipy/config/
--rw-r--r--   0 kali      (1000) kali      (1000)     1250 2023-08-29 00:50:53.000000 qualipy-1.0.2/src/qualipy/config/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2306 2023-08-30 02:48:34.000000 qualipy-1.0.2/src/qualipy/config/app_config.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/src/qualipy/exceptions/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/exceptions/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      794 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/exceptions/app_exceptions.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/src/qualipy/proj_mgmt_plugins/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/proj_mgmt_plugins/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     9125 2023-08-29 00:11:47.000000 qualipy-1.0.2/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py
--rw-r--r--   0 kali      (1000) kali      (1000)      736 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.893682 qualipy-1.0.2/src/qualipy/test_plugins/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/test_plugins/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)      588 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/test_plugins/behave_plugin.py
--rw-r--r--   0 kali      (1000) kali      (1000)      339 2023-08-19 19:48:12.000000 qualipy-1.0.2/src/qualipy/test_plugins/test_plugin.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-08-30 03:27:58.889682 qualipy-1.0.2/src/qualipy.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     2882 2023-08-30 03:27:58.000000 qualipy-1.0.2/src/qualipy.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      804 2023-08-30 03:27:58.000000 qualipy-1.0.2/src/qualipy.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-08-30 03:27:58.000000 qualipy-1.0.2/src/qualipy.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       31 2023-08-30 03:27:58.000000 qualipy-1.0.2/src/qualipy.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        8 2023-08-30 03:27:58.000000 qualipy-1.0.2/src/qualipy.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1070 2024-01-13 00:11:01.000000 qualipy-1.1.0/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     2867 2024-04-11 00:23:58.994543 qualipy-1.1.0/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      792 2024-04-10 04:14:30.000000 qualipy-1.1.0/pyproject.toml
+-rw-r--r--   0 kali      (1000) kali      (1000)     2209 2024-04-11 00:23:52.000000 qualipy-1.1.0/readme.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-11 00:23:58.994543 qualipy-1.1.0/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      344 2024-01-13 00:11:01.000000 qualipy-1.1.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.990543 qualipy-1.1.0/src/
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.990543 qualipy-1.1.0/src/qualipy/
+-rw-r--r--   0 kali      (1000) kali      (1000)       44 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3552 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/__main__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/authentication/
+-rw-r--r--   0 kali      (1000) kali      (1000)       62 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      942 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/authenticator.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1809 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/authentication/keyring_authenticator.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/config/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2172 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/config/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5509 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/config/app_config.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/data_management/
+-rw-r--r--   0 kali      (1000) kali      (1000)      159 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5444 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/csv_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1506 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6811 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/data_manager.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3026 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/excel_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1980 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/json_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2604 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/xml_data_loader.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1812 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/data_management/yaml_data_loader.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/exceptions/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1537 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/exceptions/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/
+-rw-r--r--   0 kali      (1000) kali      (1000)       86 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    12900 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1874 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/proj_mgmt_plugin.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy/test_plugins/
+-rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      752 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/behave_plugin.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      783 2024-04-10 03:56:13.000000 qualipy-1.1.0/src/qualipy/test_plugins/test_plugin.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/src/qualipy.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     2867 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1148 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       31 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        8 2024-04-11 00:23:58.000000 qualipy-1.1.0/src/qualipy.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-11 00:23:58.994543 qualipy-1.1.0/tests/
+-rw-r--r--   0 kali      (1000) kali      (1000)      121 2024-04-10 03:56:13.000000 qualipy-1.1.0/tests/test_main.py
```

### Comparing `qualipy-1.0.2/LICENSE` & `qualipy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualipy-1.0.2/PKG-INFO` & `qualipy-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: qualipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Automated test process framework
 Author-email: Charles Morris <cmorris616@gmail.com>
 Project-URL: Homepage, https://github.com/cmorris616/qualipy
 Project-URL: Bug Tracker, https://github.com/cmorris616/qualipy/issues
-Project-URL: Documentation, https://cmorris-qualipy.readthedocs.io/en/v1.0.2
 Keywords: test,testing,project management,jira,framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: behave
+Requires-Dist: keyring
+Requires-Dist: requests
+Requires-Dist: PyYAML
 
 # QualiPy
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
-
-Coming Soon:
 - Moving user stories based on the outcome of the tests
+- Moving user stories based on test results]
 - Loading test data to be used during the testing process
-- Cleaning up the test data after the testing has completed
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
 Like the testing plugins, QualiPy can also use multiple project management software suites (such as JIRA) via plugins.
```

### Comparing `qualipy-1.0.2/pyproject.toml` & `qualipy-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qualipy"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="Charles Morris", email="cmorris616@gmail.com" },
 ]
 description = "Automated test process framework"
 readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,11 +23,10 @@
   "requests",
   "PyYAML"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/cmorris616/qualipy"
 "Bug Tracker" = "https://github.com/cmorris616/qualipy/issues"
-"Documentation" = "https://cmorris-qualipy.readthedocs.io/en/v1.0.2"
 
 # [tool.setuptools.packages.find]
 # exclude = ["docs*", "tests*"]
```

### Comparing `qualipy-1.0.2/readme.md` & `qualipy-1.1.0/readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # QualiPy
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
-
-Coming Soon:
 - Moving user stories based on the outcome of the tests
+- Moving user stories based on test results]
 - Loading test data to be used during the testing process
-- Cleaning up the test data after the testing has completed
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
 Like the testing plugins, QualiPy can also use multiple project management software suites (such as JIRA) via plugins.
```

### Comparing `qualipy-1.0.2/src/qualipy/__main__.py` & `qualipy-1.1.0/src/qualipy/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import logging
 import os
 import shutil
 import importlib
 
 from qualipy.config import get_config, load_config
+from qualipy.data_management.data_manager import DataManager
 from qualipy.test_plugins.behave_plugin import BehavePlugin
 
 OUTPUT_DIRECTORY = 'qualipy_output'
 
 parser = argparse.ArgumentParser(
     prog='QualiPy - Python Testing Framework',
     description='Adds automation to the testing process'
@@ -98,13 +99,17 @@
 
 module = importlib.import_module(test_module)
 class_ = getattr(module, test_class)
 
 test_plugin = class_(config)
 test_plugin.execute()
 
+# Move user stories
+if config.move_user_stories:
+    proj_mgmt_plugin.move_user_stories(test_plugin.test_results_file)
+
 # Upload results
-if config._upload_test_results:
+if config.upload_test_results:
     proj_mgmt_plugin.upload_test_results(test_plugin.test_results_file)
 
 if __name__ == '__main__':
     pass
```

### Comparing `qualipy-1.0.2/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py` & `qualipy-1.1.0/src/qualipy/proj_mgmt_plugins/jira_proj_mgmt_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""
+This module contains the project management plugin for JIRA.
+"""
 import json
 import logging
 import os
 import tempfile
 from zipfile import ZipFile
 import requests
 import base64
-from qualipy.exceptions.app_exceptions import HttpException, InvalidTestingTypeError, MissingUrlError
+from qualipy.exceptions import HttpException, InvalidTestingTypeError, MissingUrlError
 from .proj_mgmt_plugin import TESTING_TYPE_PROGRESSION, TESTING_TYPE_REGRESSION, ProjMgmtPlugin
 
 # JSON keys/field names
 DESCRIPTION_KEY = 'description'
 FIELDS_KEY = 'fields'
 ID_FIELD = 'id'
 INWARD_ISSUE_KEY = 'inwardIssue'
@@ -21,22 +24,40 @@
 PROJECT_FIELD = 'project'
 TESTED_BY_VALUE = 'tested by'
 TOTAL_ISSUES_KEY = 'total'
 TYPE_KEY = 'type'
 
 # API Paths
 ISSUE_SEARCH_PATH = '/rest/api/2/search'
+ISSUE_PATH = '/rest/api/2/issue'
 PROJECT_SEARCH_PATH = '/rest/api/2/project'
 TEST_EXPORT_PATH = '/rest/raven/1.0/export/test'
 TEST_RESULTS_IMPORT_PATH = '/rest/raven/1.0/import/execution/behave/multipart'
 
 
 class JiraProjMgmtPlugin(ProjMgmtPlugin):
+    """
+    The plugin for interacting with JIRA for testing purposes.
+    """
 
     def __init__(self, **kwargs):
+        """
+        Initializes this plugin based on the provided kwargs.
+
+        :param kwargs: Keyword arguments for initialization
+            * authenticator: The authenticator to be used when interacting with
+                             the project management system.
+
+            * config: The application configuration dict.  This provides the
+                      project management plugin with the ability to use custom
+                      configuration settings.
+            
+            * features_directory: the directory to which the feature files should
+                                  be downloaded.
+        """
         super().__init__(**kwargs)
         self._regression_test_query = self._config.get(
             'jira.regression.test.query', 'type=Test')
         self._progression_test_query = self._config.get(
             'jira.progression.test.query', 'type=Story and status=Test')
         self._jira_url = self._config.get('jira.url', '')
         self._max_results = self._config.get('jira.max.results', 1000)
@@ -58,14 +79,17 @@
             self._export_regression_tests()
         elif self._testing_type == TESTING_TYPE_PROGRESSION:
             self._export_progression_tests()
         else:
             raise InvalidTestingTypeError(self._testing_type)
 
     def _export_progression_tests(self):
+        """
+        Exports the progression tests based on the progression test query.
+        """
         logging.info('Exporting progression tests from JIRA')
         logging.info('Querying for user stories')
         stories = self._query_issues(self._progression_test_query)
 
         issue_keys = []
 
         for story in stories:
@@ -103,14 +127,17 @@
             temp_file.write(response.content)
             temp_file.seek(0)
 
             with ZipFile(temp_file.name, 'r') as zip_file:
                 zip_file.extractall(path=self._features_directory)
 
     def _export_regression_tests(self):
+        """
+        Exports the regression tests based on the regression test query.
+        """
         logging.info('Exporting regression tests from JIRA')
         issues = self._query_issues(self._regression_test_query)
 
         if issues is None or len(issues) == 0:
             logging.info('No regression tests found')
             return
 
@@ -129,14 +156,17 @@
             temp_file.write(response.content)
             temp_file.seek(0)
 
             with ZipFile(temp_file.name, 'r') as zip_file:
                 zip_file.extractall(path=self._features_directory)
 
     def _get_jira_project(self):
+        """
+        Queries JIRA for the project information.
+        """
         if self._jira_project is not None:
             return self._jira_project
 
         if self._project_key == '':
             logging.warning('No JIRA project key set.  Unable to retrieve project info.')
             return None
 
@@ -154,14 +184,17 @@
             ISSUE_KEY_FIELD: response_dict[ISSUE_KEY_FIELD],
             DESCRIPTION_KEY: response_dict[DESCRIPTION_KEY]
         }
 
         return self._jira_project
 
     def _get_request_headers(self):
+        """
+        Returns the headers for requests to JIRA.
+        """
         if self._use_access_token:
             logging.debug('Using access token to connect to JIRA')
             auth_header_value = f'Bearer {self._authenticator.get_api_key()}'
         else:
             logging.debug('Using username and password to connect to to JIRA')
             auth_header_value = 'Basic ' + base64.b64encode(
                 f'{self._authenticator.get_username()}:{self._authenticator.get_password()}'
@@ -169,14 +202,19 @@
 
         return {
             'Authorization': auth_header_value,
             'Content-Type': 'application/json'
         }
 
     def _query_issues(self, jql):
+        """
+        Queries JIRA using the provided JQL query.
+
+        :param jql:  The JIRA Query Language (JQL) query to be used for querying issues.
+        """
         # Get credentials and set the authorization header
         headers = self._get_request_headers()
 
         start_item = 0
         expected_issue_count = self._max_results
         issues = []
 
@@ -205,14 +243,80 @@
             expected_issue_count = response_dict[TOTAL_ISSUES_KEY]
             start_item += 1
 
             if self._project_key == '' and len(issues) > 0:
                 self._project_key = issues[0][FIELDS_KEY][PROJECT_FIELD][ISSUE_KEY_FIELD]
 
         return issues
+    
+    def move_user_stories(self, test_results_file):
+        if self._testing_type != TESTING_TYPE_PROGRESSION:
+            logging.debug('Not moving user stories as testing type is not progression')
+            return
+        
+        if not os.path.exists(test_results_file):
+            logging.error(f"The test results file was not found - '{test_results_file}'")
+            return
+        
+        test_results = []
+
+        with open(test_results_file, 'r') as results_file:
+            test_results = json.load(results_file)
+
+        if len(test_results) == 0 or 'elements' not in test_results[0].keys():
+            logging.info('No test results found')
+            return
+        
+        headers = self._get_request_headers()
+
+        from qualipy.config import get_config
+        app_config = get_config()
+
+        for test in test_results[0]['elements']:
+            if 'tags' not in test.keys():
+                continue
+
+            tags = test['tags']
+
+            if test['status'] == 'passed':
+                target_transition = app_config.success_story_status
+            else:
+                target_transition = app_config.failed_story_status
+
+            for tag in tags:
+                response = requests.get(
+                    url=f'{self._jira_url}{ISSUE_PATH}/{tag}/transitions',
+                    headers=headers
+                )
+
+                if response.status_code == 404:
+                    continue
+
+                transitions = json.loads(response.content.decode('utf-8'))['transitions']
+                transition_id = -1
+
+                for transition in transitions:
+                    if transition['name'].lower() == target_transition.lower():
+                        transition_id = transition['id']
+                        response = requests.post(
+                            url=f'{self._jira_url}/rest/api/2/issue/{tag}/transitions',
+                            json={'transition': {'id': transition_id}},
+                            headers=headers
+                        )
+
+                        if response.status_code != 204:
+                            logging.error(
+                                f'An error occurred while moving user story {tag}' \
+                                f'\nStatus Code: {response.status_code}' \
+                                f'\nResponse: {response.content.decode("utf-8")}'
+                            )
+                        break
+
+
+        # do transition
 
     def upload_test_results(self, test_results_file):
 
         if self._get_jira_project() is None:
             logging.error('JIRA project info not available.  Unable to upload results.')
             return
```

### Comparing `qualipy-1.0.2/src/qualipy.egg-info/PKG-INFO` & `qualipy-1.1.0/src/qualipy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: qualipy
-Version: 1.0.2
+Version: 1.1.0
 Summary: Automated test process framework
 Author-email: Charles Morris <cmorris616@gmail.com>
 Project-URL: Homepage, https://github.com/cmorris616/qualipy
 Project-URL: Bug Tracker, https://github.com/cmorris616/qualipy/issues
-Project-URL: Documentation, https://cmorris-qualipy.readthedocs.io/en/v1.0.2
 Keywords: test,testing,project management,jira,framework
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: behave
+Requires-Dist: keyring
+Requires-Dist: requests
+Requires-Dist: PyYAML
 
 # QualiPy
 QualiPy is a framework for assisting with the automated testing process.  Qualipy is not meant to replace pytest, behave, or other testing frameworks.  Instead, it is meant to augment the process to provider further automation.  It can be configured based on the needs of the project and the availablility of other technologies.
 
 QualiPy features include:
 - Exporting feature files from JIRA for progression and regression testing
 - Uploading test results to JIRA
 - Support for custom project management, authentication, and testing plugins
-
-Coming Soon:
 - Moving user stories based on the outcome of the tests
+- Moving user stories based on test results]
 - Loading test data to be used during the testing process
-- Cleaning up the test data after the testing has completed
 - Data management across steps and scenarios
 
 ## Test Plugins
 QualiPy is built to use multiple testing frameworks via plugins.  Currently, QualiPy supports the behave framework out of the box for business-driven development.
 
 ## Project Management Plugins
 Like the testing plugins, QualiPy can also use multiple project management software suites (such as JIRA) via plugins.
```

