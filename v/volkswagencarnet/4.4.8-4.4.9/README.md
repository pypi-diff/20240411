# Comparing `tmp/volkswagencarnet-4.4.8.tar.gz` & `tmp/volkswagencarnet-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/volkswagencarnet-4.4.8.tar", last modified: Mon Jun 22 13:08:32 2020, max compression
+gzip compressed data, was "dist/volkswagencarnet-4.4.9.tar", last modified: Tue Jun 23 13:37:00 2020, max compression
```

## Comparing `volkswagencarnet-4.4.8.tar` & `volkswagencarnet-4.4.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/.github/
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1272 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1007 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)    11356 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4599 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    17802 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (116)       42 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      439 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      896 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/tests/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2559 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-22 13:08:32.797497 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-22 13:08:32.000000 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      427 2020-06-22 13:08:32.000000 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-22 13:08:32.000000 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-06-22 13:08:32.000000 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-06-22 13:08:32.000000 volkswagencarnet-4.4.8/volkswagencarnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    50553 2020-06-22 13:08:20.000000 volkswagencarnet-4.4.8/volkswagencarnet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)       23 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (116)      532 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)      407 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1014 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      774 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     1379 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/.github/workflows/validate.yml
+-rw-r--r--   0 runner    (1001) docker     (116)    11356 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4599 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17802 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (116)       42 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      439 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      896 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.695001 volkswagencarnet-4.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      644 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/tests/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2559 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-23 13:37:00.699001 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     6091 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      511 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       46 2020-06-23 13:37:00.000000 volkswagencarnet-4.4.9/volkswagencarnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    50553 2020-06-23 13:36:50.000000 volkswagencarnet-4.4.9/volkswagencarnet.py
```

### Comparing `volkswagencarnet-4.4.8/.github/workflows/python-package.yml` & `volkswagencarnet-4.4.9/.github/workflows/validate.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
-name: Test Python Package
+name: Validate
 
 #on: [push]
-on: [push, pull_request]
+#on: [push, pull_request]
+on:
+  pull_request:
+    branches:
+      - master
+  push:
+    branches:
+      - master
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
     steps:
-      - uses: actions/checkout@v2
+      - name: Checkout code
+        uses: actions/checkout@v2
+
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
+
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install flake8 pytest
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+
       - name: Lint with flake8
         run: |
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
       - name: Test with pytest
```

### Comparing `volkswagencarnet-4.4.8/.github/workflows/python-publish.yml` & `volkswagencarnet-4.4.9/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 # push:
 #   tags:
 #     - "v*"
 
 on:
   push:
     tags:
-      - "v*.*.*"
+      - "vvvvvvv*.*.*"
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
+
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.x"
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
```

### Comparing `volkswagencarnet-4.4.8/LICENSE.txt` & `volkswagencarnet-4.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/PKG-INFO` & `volkswagencarnet-4.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 4.4.8
+Version: 4.4.9
 Summary: Communicate with Volkswagen WeConnect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
 License: UNKNOWN
 Description: # Volkswagen Carnet
```

### Comparing `volkswagencarnet-4.4.8/README.md` & `volkswagencarnet-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/dashboard.py` & `volkswagencarnet-4.4.9/dashboard.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/setup.py` & `volkswagencarnet-4.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/tests/dummy_test.py` & `volkswagencarnet-4.4.9/tests/dummy_test.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/utilities.py` & `volkswagencarnet-4.4.9/utilities.py`

 * *Files identical despite different names*

### Comparing `volkswagencarnet-4.4.8/volkswagencarnet.egg-info/PKG-INFO` & `volkswagencarnet-4.4.9/volkswagencarnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volkswagencarnet
-Version: 4.4.8
+Version: 4.4.9
 Summary: Communicate with Volkswagen WeConnect
 Home-page: https://github.com/robinostlund/volkswagencarnet
 Author: Robin Ostlund
 Author-email: me@robinostlund.name
 License: UNKNOWN
 Description: # Volkswagen Carnet
```

### Comparing `volkswagencarnet-4.4.8/volkswagencarnet.py` & `volkswagencarnet-4.4.9/volkswagencarnet.py`

 * *Files identical despite different names*

