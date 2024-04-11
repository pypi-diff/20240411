# Comparing `tmp/dagster-pandera-0.23.0.tar.gz` & `tmp/dagster-pandera-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pandera-0.23.0.tar", last modified: Thu Apr  4 19:53:57 2024, max compression
+gzip compressed data, was "dagster-pandera-0.23.1.tar", last modified: Thu Apr 11 18:17:11 2024, max compression
```

## Comparing `dagster-pandera-0.23.0.tar` & `dagster-pandera-0.23.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:57.427427 dagster-pandera-0.23.0/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-04 19:53:57.427427 dagster-pandera-0.23.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:57.427427 dagster-pandera-0.23.0/dagster_pandera/
--rw-r--r--   0 root         (0) root         (0)     9259 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/dagster_pandera/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/dagster_pandera/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/dagster_pandera/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:57.427427 dagster-pandera-0.23.0/dagster_pandera.egg-info/
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-04 19:53:57.000000 dagster-pandera-0.23.0/dagster_pandera.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      322 2024-04-04 19:53:57.000000 dagster-pandera-0.23.0/dagster_pandera.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:53:57.000000 dagster-pandera-0.23.0/dagster_pandera.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-04 19:53:57.000000 dagster-pandera-0.23.0/dagster_pandera.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 19:53:57.000000 dagster-pandera-0.23.0/dagster_pandera.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      150 2024-04-04 19:53:57.431427 dagster-pandera-0.23.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1359 2024-04-04 19:44:08.000000 dagster-pandera-0.23.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:17:11.335217 dagster-pandera-0.23.1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-11 18:17:11.335217 dagster-pandera-0.23.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:17:11.335217 dagster-pandera-0.23.1/dagster_pandera/
+-rw-r--r--   0 root         (0) root         (0)     9259 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/dagster_pandera/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/dagster_pandera/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/dagster_pandera/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:17:11.335217 dagster-pandera-0.23.1/dagster_pandera.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-11 18:17:11.000000 dagster-pandera-0.23.1/dagster_pandera.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      322 2024-04-11 18:17:11.000000 dagster-pandera-0.23.1/dagster_pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:17:11.000000 dagster-pandera-0.23.1/dagster_pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-11 18:17:11.000000 dagster-pandera-0.23.1/dagster_pandera.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 18:17:11.000000 dagster-pandera-0.23.1/dagster_pandera.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2024-04-11 18:17:11.335217 dagster-pandera-0.23.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-11 18:04:20.000000 dagster-pandera-0.23.1/setup.py
```

### Comparing `dagster-pandera-0.23.0/LICENSE` & `dagster-pandera-0.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.23.0/PKG-INFO` & `dagster-pandera-0.23.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.23.0
+Version: 0.23.1
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pandera-0.23.0/dagster_pandera/__init__.py` & `dagster-pandera-0.23.1/dagster_pandera/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-pandera-0.23.0/dagster_pandera.egg-info/PKG-INFO` & `dagster-pandera-0.23.1/dagster_pandera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-pandera
-Version: 0.23.0
+Version: 0.23.1
 Summary: Integration layer for dagster and pandera.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-pandera-0.23.0/setup.py` & `dagster-pandera-0.23.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_pandera_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.0", "pandas", "pandera>=0.14.2"],
+    install_requires=["dagster==1.7.1", "pandas", "pandera>=0.14.2"],
     extras_require={
         "test": [
             "pytest",
         ],
     },
 )
```

