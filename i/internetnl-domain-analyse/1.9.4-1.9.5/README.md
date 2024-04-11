# Comparing `tmp/internetnl_domain_analyse-1.9.4.tar.gz` & `tmp/internetnl_domain_analyse-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.9.4.tar", last modified: Thu Apr 11 19:26:41 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-1.9.5.tar", last modified: Thu Apr 11 20:23:36 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.9.4.tar` & `internetnl_domain_analyse-1.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.4/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.4/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      960 2024-04-11 19:25:17.000000 internetnl_domain_analyse-1.9.4/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.4/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.4/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.4/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.4/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.4/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.925969 internetnl_domain_analyse-1.9.4/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.937969 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    72001 2024-04-11 19:24:42.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.4/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.647242 internetnl_domain_analyse-1.9.5/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.5/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.5/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      960 2024-04-11 20:22:03.000000 internetnl_domain_analyse-1.9.5/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.5/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 20:23:36.647242 internetnl_domain_analyse-1.9.5/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.639242 internetnl_domain_analyse-1.9.5/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.639242 internetnl_domain_analyse-1.9.5/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.5/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.5/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.5/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.639242 internetnl_domain_analyse-1.9.5/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.5/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 20:23:36.647242 internetnl_domain_analyse-1.9.5/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.631241 internetnl_domain_analyse-1.9.5/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.643242 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    72179 2024-04-11 20:20:38.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.647242 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 20:23:36.000000 internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 20:23:36.647242 internetnl_domain_analyse-1.9.5/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.5/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.5/tox.ini
```

### Comparing `internetnl_domain_analyse-1.9.4/.coveragerc` & `internetnl_domain_analyse-1.9.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/.gitignore` & `internetnl_domain_analyse-1.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/.readthedocs.yml` & `internetnl_domain_analyse-1.9.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/CHANGELOG.rst` & `internetnl_domain_analyse-1.9.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =========
 Changelog
 =========
 
-Version 1.9.4
+Version 1.9.5
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
 - Histograms can now be plotted as well
 
 Version 1.8.7
 =============
```

### Comparing `internetnl_domain_analyse-1.9.4/CONTRIBUTING.rst` & `internetnl_domain_analyse-1.9.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/LICENSE.txt` & `internetnl_domain_analyse-1.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/PKG-INFO` & `internetnl_domain_analyse-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.4
+Version: 1.9.5
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.4/docs/Makefile` & `internetnl_domain_analyse-1.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/docs/conf.py` & `internetnl_domain_analyse-1.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/docs/index.rst` & `internetnl_domain_analyse-1.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-1.9.5/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/setup.cfg` & `internetnl_domain_analyse-1.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/setup.py` & `internetnl_domain_analyse-1.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,17 +492,21 @@
                     var_filter=var_filter,
                 )
             except KeyError:
                 _logger.info(f"Failed to get selection of {column}. Skipping")
                 continue
 
             if data is None:
-                _logger.warning(f"Could not get data selection for {var_key}. Skipping")
+                _logger.info(f"Could not get data selection for {var_key}. Skipping")
                 continue
 
+            if data.index.size < df_weights.index.size:
+                _logger.debug("we filtered data. Also filter the weights")
+                df_weights.reindex(data.index)
+
             stats = WeightedSampleStatistics(
                 group_keys=group_by,
                 records_df_selection=data,
                 weights_df=df_weights,
                 column_list=column_list,
                 var_type=var_type,
                 var_weight_key=var_weight_key,
@@ -1529,15 +1533,15 @@
                                 highcharts_info = highcharts_info_per_year[year]
 
                                 if hist_info is not None and isinstance(
                                     hist_info, dict
                                 ):
                                     for grp_key, hist in hist_info.items():
                                         if hist is None:
-                                            _logger.debug(
+                                            _logger.warning(
                                                 f"Hist {grp_key} does not have a histogram. Skipping"
                                             )
                                             continue
                                         im_file_2 = make_cdf_plot(
                                             hist=hist,
                                             plot_key=plot_key,
                                             scan_data_key=scan_data_key,
```

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.4
+Version: 1.9.5
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-1.9.5/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.4/tox.ini` & `internetnl_domain_analyse-1.9.5/tox.ini`

 * *Files identical despite different names*

