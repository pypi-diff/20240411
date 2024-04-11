# Comparing `tmp/weighted_sample_statistics-0.1.0.tar.gz` & `tmp/weighted_sample_statistics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_sample_statistics-0.1.0.tar", last modified: Wed Apr 10 19:54:37 2024, max compression
+gzip compressed data, was "weighted_sample_statistics-0.1.1.tar", last modified: Wed Apr 10 20:17:35 2024, max compression
```

## Comparing `weighted_sample_statistics-0.1.0.tar` & `weighted_sample_statistics-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.0/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.0/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 19:52:50.000000 weighted_sample_statistics-0.1.0/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.1.0/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.1.0/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.753780 weighted_sample_statistics-0.1.0/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.753780 weighted_sample_statistics-0.1.0/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.1.0/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.1.0/docs/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.0/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1367 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.749779 weighted_sample_statistics-0.1.0/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.757779 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1045 2024-04-10 19:52:20.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    20106 2024-04-10 19:19:59.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/core.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/main.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15146 2024-04-10 19:52:33.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/utils.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/variable_properties.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1640 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      161 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 19:54:37.000000 weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 19:54:37.761780 weighted_sample_statistics-0.1.0/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.0/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      515 2024-04-10 19:33:28.000000 weighted_sample_statistics-0.1.0/tests/test_weighted_sample_statistics.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.0/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.317023 weighted_sample_statistics-0.1.1/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      609 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.1/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      566 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-10 17:21:44.000000 weighted_sample_statistics-0.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1032 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.1/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       78 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      166 2024-04-10 20:14:06.000000 weighted_sample_statistics-0.1.1/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12154 2024-04-10 19:11:28.000000 weighted_sample_statistics-0.1.1/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1082 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1677 2024-04-10 20:17:35.317023 weighted_sample_statistics-0.1.1/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      582 2024-04-10 19:13:54.000000 weighted_sample_statistics-0.1.1/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.313023 weighted_sample_statistics-0.1.1/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.313023 weighted_sample_statistics-0.1.1/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9881 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.1/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1473 2024-04-10 19:14:36.000000 weighted_sample_statistics-0.1.1/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      244 2024-04-10 17:19:07.000000 weighted_sample_statistics-0.1.1/docs/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      346 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       13 2024-04-10 17:23:13.000000 weighted_sample_statistics-0.1.1/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1374 2024-04-10 20:17:35.317023 weighted_sample_statistics-0.1.1/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      721 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.1/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.305023 weighted_sample_statistics-0.1.1/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.313023 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1045 2024-04-10 19:52:20.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    20106 2024-04-10 19:19:59.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/core.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     3356 2024-04-10 18:53:00.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/main.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    18074 2024-04-10 20:12:39.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/utils.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2886 2024-04-10 17:23:34.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/variable_properties.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.317023 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1677 2024-04-10 20:17:35.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      963 2024-04-10 20:17:35.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 20:17:35.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 20:15:49.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      167 2024-04-10 20:17:35.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       27 2024-04-10 20:17:35.000000 weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:17:35.317023 weighted_sample_statistics-0.1.1/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      294 2024-04-10 17:59:56.000000 weighted_sample_statistics-0.1.1/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      515 2024-04-10 19:33:28.000000 weighted_sample_statistics-0.1.1/tests/test_weighted_sample_statistics.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2851 2024-04-10 14:53:25.000000 weighted_sample_statistics-0.1.1/tox.ini
```

### Comparing `weighted_sample_statistics-0.1.0/.coveragerc` & `weighted_sample_statistics-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/.gitignore` & `weighted_sample_statistics-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/.readthedocs.yml` & `weighted_sample_statistics-0.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/CONTRIBUTING.rst` & `weighted_sample_statistics-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/LICENSE.txt` & `weighted_sample_statistics-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/PKG-INFO` & `weighted_sample_statistics-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
@@ -15,14 +15,15 @@
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pyscaffold; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: black; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `weighted_sample_statistics-0.1.0/README.rst` & `weighted_sample_statistics-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/docs/Makefile` & `weighted_sample_statistics-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/docs/conf.py` & `weighted_sample_statistics-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/docs/index.rst` & `weighted_sample_statistics-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/setup.cfg` & `weighted_sample_statistics-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 exclude = 
 	tests
 
 [options.extras_require]
 dev = tox
 	pyscaffold
 	pre-commit
+	black
 	setuptools
 	pytest
 	pytest-cov
 testing = 
 	setuptools
 	pytest
 	pytest-cov
```

### Comparing `weighted_sample_statistics-0.1.0/setup.py` & `weighted_sample_statistics-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/__init__.py` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/core.py` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/core.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/main.py` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/main.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/utils.py` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 Some utility functions.
 """
+
 import logging
 import re
-from pandas import DataFrame, Series
+
+import numpy as np
+import pandas as pd
+from pandas import DataFrame
 
 logger = logging.getLogger(__name__)
 
 
 def make_negation_name(column_name, suffix="_x") -> str:
     """Make a new column name based for the negative value
 
@@ -415,7 +419,84 @@
         stat_df = stat_df.round(decimals=n_digits)
 
     index_variables = [module_key, vraag_key, optie_key]
     if sort_index:
         stat_df.sort_values([module_key, vraag_key, variable_key], axis=0, inplace=True)
     stat_df.set_index(index_variables, inplace=True, drop=True)
     return stat_df
+
+
+def get_filtered_data_column(dataframe, column, var_filter=None, output_format=None):
+    """
+    Verkrijg de (gefilterde) kolom uit de dataframe.
+
+    Parameters
+    ----------
+    dataframe: pd.DataFrame
+        Alle data
+    column: str
+        Naam van de kolom die we willen selecteren
+    var_filter: str of dict or None
+        Eventueel een filter als we op een andere kolom uit data frame willen filteren.
+        Als een dict gegeven is ziet het er zou uit::
+
+            filter:
+                statline: kolomnaam_voor_filter_voor_statline_output
+                eurostat: kolomnaam_voor_filter_voor_euro_output
+
+        Als statline of eurostat niet gegeven is aan nemen voor die output alle data (ongefilterd)
+
+    output_format: str
+        Naam van de huidige output format
+
+    Returns
+    -------
+    pd.DataFrame:
+        Datakolom die we willen gebruiken voor de statistiek
+
+    """
+    # hier wordt de colom data geselecteerd, eventueel gefiltered als een filter variable
+    # gegeven is.
+    if var_filter is None:
+        # zonder filter nemen we alle data
+        records_selection = dataframe.loc[:, [column]]
+    else:
+
+        if isinstance(var_filter, dict):
+            # er is een filter in de vorm van een dict, dus een verschillende entry voor
+            # eurostat en statline (keys zijn eurostat of statline). Probeer de filter variable
+            # te krijgen
+            logger.debug(
+                f"Trying to get filter variabele for {column} with {var_filter}"
+            )
+            try:
+                var_filt = var_filter[output_format]
+            except KeyError as err:
+                # Als de variable niet gegevens is in de dict nemen we alsnog alle data
+                var_filt = None
+        else:
+            # het filter is als een key: value gegeven, dus zet het filter voor alle ouputs
+            var_filt = var_filter
+
+        if var_filt is None:
+            # als var_filt hier None was hadden we een dict zonder entry voor deze output.
+            # Dan nemen we dus ale data
+            logger.debug(
+                f"No valid entry for {var_filter} in {column} for {output_format}. "
+                f"Take all data"
+            )
+            records_selection = dataframe.loc[:, [column]]
+        else:
+            try:
+                mask = dataframe[var_filt] == 1
+            except KeyError:
+                # Er is een var_filt gegeven, maar deze kolom bestaat niet. Waarschuw en sla over
+                logger.warning(
+                    f"KeyError for {column}: {var_filt}. Opgeven filter column bestaat "
+                    f"niet!"
+                )
+                records_selection = None
+            else:
+                # We hebben een mask bepaald op basis van het filter. Verkrijg nu de gefilterde data
+                records_selection = dataframe.loc[mask, [column]]
+
+    return records_selection
```

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics/variable_properties.py` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics/variable_properties.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/PKG-INFO` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted_sample_statistics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculate statistics in dataframes using weighting functions
 Home-page: https://github.com/eelcovv/WeightedSampleStatistics
 Author: Eelco van Vliet
 Author-email: eelcovv@gmail.com
 License: MIT
 Project-URL: Documentation, https://weightedsamplestatistics.readthedocs.io/en/latest/
 Platform: any
@@ -15,14 +15,15 @@
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: numpy
 Requires-Dist: pandas
 Provides-Extra: dev
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: pyscaffold; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: black; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `weighted_sample_statistics-0.1.0/src/weighted_sample_statistics.egg-info/SOURCES.txt` & `weighted_sample_statistics-0.1.1/src/weighted_sample_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/tests/test_weighted_sample_statistics.py` & `weighted_sample_statistics-0.1.1/tests/test_weighted_sample_statistics.py`

 * *Files identical despite different names*

### Comparing `weighted_sample_statistics-0.1.0/tox.ini` & `weighted_sample_statistics-0.1.1/tox.ini`

 * *Files identical despite different names*

