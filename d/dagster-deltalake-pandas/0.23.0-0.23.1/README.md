# Comparing `tmp/dagster-deltalake-pandas-0.23.0.tar.gz` & `tmp/dagster-deltalake-pandas-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-pandas-0.23.0.tar", last modified: Thu Apr  4 19:51:32 2024, max compression
+gzip compressed data, was "dagster-deltalake-pandas-0.23.1.tar", last modified: Thu Apr 11 18:16:12 2024, max compression
```

## Comparing `dagster-deltalake-pandas-0.23.0.tar` & `dagster-deltalake-pandas-0.23.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:32.490469 dagster-deltalake-pandas-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      778 2024-04-04 19:51:32.490469 dagster-deltalake-pandas-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:32.490469 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/deltalake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:32.490469 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      778 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-04 19:51:32.000000 dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      135 2024-04-04 19:51:32.490469 dagster-deltalake-pandas-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1484 2024-04-04 19:44:08.000000 dagster-deltalake-pandas-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:12.798822 dagster-deltalake-pandas-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-11 18:16:12.798822 dagster-deltalake-pandas-0.23.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:12.794822 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/deltalake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:12.798822 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-11 18:16:12.000000 dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-11 18:16:12.802822 dagster-deltalake-pandas-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-04-11 18:04:20.000000 dagster-deltalake-pandas-0.23.1/setup.py
```

### Comparing `dagster-deltalake-pandas-0.23.0/LICENSE` & `dagster-deltalake-pandas-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-pandas-0.23.0/PKG-INFO` & `dagster-deltalake-pandas-0.23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-pandas
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for storing Pandas DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas/deltalake_pandas_type_handler.py` & `dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas/deltalake_pandas_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-pandas-0.23.0/dagster_deltalake_pandas.egg-info/PKG-INFO` & `dagster-deltalake-pandas-0.23.1/dagster_deltalake_pandas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake-pandas
-Version: 0.23.0
+Version: 0.23.1
 Summary: Package for storing Pandas DataFrames in Delta tables.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake-pandas
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-pandas-0.23.0/setup.py` & `dagster-deltalake-pandas-0.23.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.0",
-        "dagster-deltalake==0.23.0",
+        "dagster==1.7.1",
+        "dagster-deltalake==0.23.1",
         "pandas",
     ],
     zip_safe=False,
 )
```

