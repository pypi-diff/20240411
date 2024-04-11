# Comparing `tmp/polytrend-1.0.1.tar.gz` & `tmp/polytrend-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytrend-1.0.1.tar", last modified: Thu Apr 11 19:42:15 2024, max compression
+gzip compressed data, was "polytrend-1.0.2.tar", last modified: Thu Apr 11 19:55:49 2024, max compression
```

## Comparing `polytrend-1.0.1.tar` & `polytrend-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:42:15.475819 polytrend-1.0.1/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.1/LICENSE
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:42:15.475819 polytrend-1.0.1/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.1/README.md
-drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:42:15.475819 polytrend-1.0.1/polytrend.egg-info/
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/PKG-INFO
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      173 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/SOURCES.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/dependency_links.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:42:15.000000 polytrend-1.0.1/polytrend.egg-info/top_level.txt
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 19:36:12.000000 polytrend-1.0.1/pyproject.toml
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 19:42:15.475819 polytrend-1.0.1/setup.cfg
--rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      273 2024-04-11 19:37:41.000000 polytrend-1.0.1/setup.py
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:55:49.815840 polytrend-1.0.2/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)    35149 2024-04-11 19:01:45.000000 polytrend-1.0.2/LICENSE
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:55:49.815840 polytrend-1.0.2/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     2591 2024-04-11 19:01:45.000000 polytrend-1.0.2/README.md
+drwxr-xr-x   0 magawkgawks  (1000) magawkgawks  (1000)        0 2024-04-11 19:55:49.815840 polytrend-1.0.2/polytrend.egg-info/
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)     3197 2024-04-11 19:55:49.000000 polytrend-1.0.2/polytrend.egg-info/PKG-INFO
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      173 2024-04-11 19:55:49.000000 polytrend-1.0.2/polytrend.egg-info/SOURCES.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:55:49.000000 polytrend-1.0.2/polytrend.egg-info/dependency_links.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)        1 2024-04-11 19:55:49.000000 polytrend-1.0.2/polytrend.egg-info/top_level.txt
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      800 2024-04-11 19:55:28.000000 polytrend-1.0.2/pyproject.toml
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)       38 2024-04-11 19:55:49.815840 polytrend-1.0.2/setup.cfg
+-rw-r--r--   0 magawkgawks  (1000) magawkgawks  (1000)      386 2024-04-11 19:55:32.000000 polytrend-1.0.2/setup.py
```

### Comparing `polytrend-1.0.1/LICENSE` & `polytrend-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.1/PKG-INFO` & `polytrend-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.1
+Version: 1.0.2
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `polytrend-1.0.1/README.md` & `polytrend-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `polytrend-1.0.1/polytrend.egg-info/PKG-INFO` & `polytrend-1.0.2/polytrend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polytrend
-Version: 1.0.1
+Version: 1.0.2
 Summary: PolyTrend is a regression tool that fits polynomial curves to noisy data.
 Author-email: Emmanuel Asiimwe <asiimwemmanuel47@gmail.com>
 Project-URL: Homepage, https://github.com/asiimwemmanuel/polytrend
 Project-URL: Issues, https://github.com/asiimwemmanuel/polytrend/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

