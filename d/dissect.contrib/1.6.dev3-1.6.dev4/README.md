# Comparing `tmp/dissect.contrib-1.6.dev3.tar.gz` & `tmp/dissect.contrib-1.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.contrib-1.6.dev3.tar", last modified: Thu Mar 28 17:21:40 2024, max compression
+gzip compressed data, was "dissect.contrib-1.6.dev4.tar", last modified: Thu Apr 11 11:56:26 2024, max compression
```

## Comparing `dissect.contrib-1.6.dev3.tar` & `dissect.contrib-1.6.dev4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/dissect.contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-28 17:21:40.000000 dissect.contrib-1.6.dev3/dissect.contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-28 17:21:40.000000 dissect.contrib-1.6.dev3/dissect.contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:40.000000 dissect.contrib-1.6.dev3/dissect.contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:40.000000 dissect.contrib-1.6.dev3/dissect.contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-28 17:21:35.000000 dissect.contrib-1.6.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/template/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/template/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.968193 dissect.contrib-1.6.dev3/template/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.968193 dissect.contrib-1.6.dev3/template/dissect/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.972193 dissect.contrib-1.6.dev3/template/dissect/contrib/template/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/template/dissect/contrib/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-28 17:21:29.000000 dissect.contrib-1.6.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/dissect.contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-11 11:56:26.000000 dissect.contrib-1.6.dev4/dissect.contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 11:56:26.000000 dissect.contrib-1.6.dev4/dissect.contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:26.000000 dissect.contrib-1.6.dev4/dissect.contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:56:26.000000 dissect.contrib-1.6.dev4/dissect.contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-11 11:56:21.000000 dissect.contrib-1.6.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/template/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.289391 dissect.contrib-1.6.dev4/template/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.289391 dissect.contrib-1.6.dev4/template/dissect/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:56:26.293391 dissect.contrib-1.6.dev4/template/dissect/contrib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/template/dissect/contrib/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-11 11:56:17.000000 dissect.contrib-1.6.dev4/tox.ini
```

### Comparing `dissect.contrib-1.6.dev3/LICENSE` & `dissect.contrib-1.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.6.dev3/PKG-INFO` & `dissect.contrib-1.6.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.6.dev3
+Version: 1.6.dev4
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.6.dev3/README.md` & `dissect.contrib-1.6.dev4/README.md`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.6.dev3/dissect.contrib.egg-info/PKG-INFO` & `dissect.contrib-1.6.dev4/dissect.contrib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.contrib
-Version: 1.6.dev3
+Version: 1.6.dev4
 Summary: This project is a meta package: it reserves the namespace for Dissect packages made by external contributors
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: repository, https://github.com/fox-it/dissect.contrib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `dissect.contrib-1.6.dev3/pyproject.toml` & `dissect.contrib-1.6.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.6.dev3/template/pyproject.toml` & `dissect.contrib-1.6.dev4/template/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.contrib-1.6.dev3/tox.ini` & `dissect.contrib-1.6.dev4/tox.ini`

 * *Files identical despite different names*

