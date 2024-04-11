# Comparing `tmp/internetnl_domain_analyse-1.9.3.tar.gz` & `tmp/internetnl_domain_analyse-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.9.3.tar", last modified: Thu Apr 11 18:52:44 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-1.9.4.tar", last modified: Thu Apr 11 19:26:41 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.9.3.tar` & `internetnl_domain_analyse-1.9.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.3/.pre-commit-config.yaml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.3/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      920 2024-04-11 18:50:41.000000 internetnl_domain_analyse-1.9.3/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.3/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.3/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.3/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.3/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.3/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.259559 internetnl_domain_analyse-1.9.3/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.267559 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    71935 2024-04-11 18:06:06.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.271560 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.271560 internetnl_domain_analyse-1.9.3/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.3/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.4/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.4/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      960 2024-04-11 19:25:17.000000 internetnl_domain_analyse-1.9.4/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.4/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.4/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.4/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.4/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.933969 internetnl_domain_analyse-1.9.4/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.4/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.925969 internetnl_domain_analyse-1.9.4/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.937969 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    72001 2024-04-11 19:24:42.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 19:26:41.000000 internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 19:26:41.941969 internetnl_domain_analyse-1.9.4/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.4/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.4/tox.ini
```

### Comparing `internetnl_domain_analyse-1.9.3/.coveragerc` & `internetnl_domain_analyse-1.9.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/.gitignore` & `internetnl_domain_analyse-1.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/.readthedocs.yml` & `internetnl_domain_analyse-1.9.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/CHANGELOG.rst` & `internetnl_domain_analyse-1.9.4/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 =========
 Changelog
 =========
 
-Version 1.9.3
+Version 1.9.4
 =============
 - Nu statistieken op basis van weighted_sample_statistics
 - Force calculate included
+- Histograms can now be plotted as well
 
 Version 1.8.7
 =============
 - Nu kan je breakdowns ook als combinaties geven. Nodig voor publicatie 2023
 - legend default aan plaatjes toegevoegd nu we meerdere jaren hebben
 - eval statement kan gebruikt worden om afgeleide kolommen te maken
 - dump cache as sqlite optie. Duplicated kolommen worden verwijderd
```

### Comparing `internetnl_domain_analyse-1.9.3/CONTRIBUTING.rst` & `internetnl_domain_analyse-1.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/LICENSE.txt` & `internetnl_domain_analyse-1.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/PKG-INFO` & `internetnl_domain_analyse-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.3
+Version: 1.9.4
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.3/docs/Makefile` & `internetnl_domain_analyse-1.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/docs/conf.py` & `internetnl_domain_analyse-1.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/docs/index.rst` & `internetnl_domain_analyse-1.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-1.9.4/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/setup.cfg` & `internetnl_domain_analyse-1.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/setup.py` & `internetnl_domain_analyse-1.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 import yaml
 
-from weighted_sample_statistics import (WeightedSampleStatistics, VariableProperties)
+from weighted_sample_statistics import WeightedSampleStatistics, VariableProperties
 from weighted_sample_statistics import (
     get_records_select,
     rename_all_variables,
-    prepare_df_for_statistics
+    prepare_df_for_statistics,
 )
 from internetnl_domain_analyse.domain_plots import (
     make_cdf_plot,
     make_bar_plot,
     make_bar_plot_stacked,
 )
 from internetnl_domain_analyse.latex_output import make_latex_overview
@@ -50,35 +50,35 @@
 
 def make_plot_cache_file_name(cache_directory, file_base, prefix):
     return cache_directory / Path("_".join([prefix, file_base, "cache_for_plot.pkl"]))
 
 
 class ImageFileInfo:
     def __init__(
-            self, scan_data_key, cache_file_name_base="image_info", cache_directory="cache"
+        self, scan_data_key, cache_file_name_base="image_info", cache_directory="cache"
     ):
         self.scan_data_key = scan_data_key
         self.cache_directory = Path(cache_directory)
         self.cache_directory.mkdir(exist_ok=True)
         cache_file_name = Path(
             "_".join([cache_file_name_base, scan_data_key])
         ).with_suffix(".yml")
         self.cache_file_name = self.cache_directory / cache_file_name
 
         self.data = None
 
     def add_entry(
-            self,
-            plot_key,
-            plot_info,
-            image_key,
-            sub_image_label,
-            file_name,
-            tex_right_shift=None,
-            section=None,
+        self,
+        plot_key,
+        plot_info,
+        image_key,
+        sub_image_label,
+        file_name,
+        tex_right_shift=None,
+        section=None,
     ):
         """add a new entry"""
 
         if image_key not in self.data.keys():
             self.data[image_key] = dict()
         self.data[image_key][plot_key] = dict(
             file_name=file_name,
@@ -112,24 +112,24 @@
             else:
                 self.data[var_name] = var_entry
 
     def read_cache(self):
         """Lees de cache"""
         if self.cache_file_name.exists():
             with codecs.open(
-                    self.cache_file_name.as_posix(), "r", encoding="UTF-8"
+                self.cache_file_name.as_posix(), "r", encoding="UTF-8"
             ) as stream:
                 self.data = yaml.load(stream=stream, Loader=yaml.Loader)
         else:
             self.data = dict()
 
     def write_cache(self):
         """Schrijf de cache"""
         with codecs.open(
-                self.cache_file_name.as_posix(), "w", encoding="UTF-8"
+            self.cache_file_name.as_posix(), "w", encoding="UTF-8"
         ) as stream:
             yaml.dump(data=self.data, stream=stream, Dumper=yaml.Dumper)
 
 
 class RecordsCacheInfo:
     def __init__(self, records_cache_data: dict, year: str, stat_directory: str = None):
         """
@@ -183,43 +183,43 @@
                 f"records_df_{self.year_digits}_2",
                 f"info_records_df_{self.year_digits}",
             ]
 
 
 class DomainAnalyser:
     def __init__(
-            self,
-            scan_data_key=None,
-            cache_file_base="tables_df",
-            cache_directory_base_name=None,
-            tld_extract_cache_directory=None,
-            output_file=None,
-            reset=None,
-            records_cache_info: RecordsCacheInfo = None,
-            internet_nl_filename=None,
-            breakdown_labels=None,
-            statistics: dict = None,
-            default_scan=None,
-            variables: dict = None,
-            module_info: dict = None,
-            weights=None,
-            url_key="website_url",
-            suffix_key="suffix",
-            translations=None,
-            module_key="module",
-            variable_key="variable",
-            sheet_renames=None,
-            n_digits=None,
-            write_dataframe_to_sqlite=False,
-            statistics_to_xls=False,
-            n_bins=100,
-            mode=None,
-            correlations=None,
-            categories=None,
-            dump_cache_as_sqlite=False,
+        self,
+        scan_data_key=None,
+        cache_file_base="tables_df",
+        cache_directory_base_name=None,
+        tld_extract_cache_directory=None,
+        output_file=None,
+        reset=None,
+        records_cache_info: RecordsCacheInfo = None,
+        internet_nl_filename=None,
+        breakdown_labels=None,
+        statistics: dict = None,
+        default_scan=None,
+        variables: dict = None,
+        module_info: dict = None,
+        weights=None,
+        url_key="website_url",
+        suffix_key="suffix",
+        translations=None,
+        module_key="module",
+        variable_key="variable",
+        sheet_renames=None,
+        n_digits=None,
+        write_dataframe_to_sqlite=False,
+        statistics_to_xls=False,
+        n_bins=100,
+        mode=None,
+        correlations=None,
+        categories=None,
+        dump_cache_as_sqlite=False,
     ):
 
         _logger.info(f"Running here {os.getcwd()}")
 
         self.records_cache_info = records_cache_info
 
         if output_file is None:
@@ -510,16 +510,16 @@
                 units_scaling_factor_key=units_schaal_factor_key,
                 report_numbers=var_prop_klass.report_number,
             )
 
             stats.calculate()
 
             if (
-                    not np.isnan(var_prop_klass.report_number)
-                    and var_prop_klass.report_number
+                not np.isnan(var_prop_klass.report_number)
+                and var_prop_klass.report_number
             ):
                 all_stats[column] = stats.records_sum
             else:
                 all_stats[column] = stats.records_weighted_mean_agg
 
             # voeg hier het histogram van de data toe
             all_hist[var_key] = calculate_histogram_per_breakdown(
@@ -614,17 +614,17 @@
         )
         _logger.info(f"Writing to {sum_file}")
         sum_per_number_of_cat_df.to_pickle(sum_file)
 
     def calculate_correlations_and_scores(self):
 
         if (
-                self.corr_pkl_file.exists()
-                and self.score_pkl_file.exists()
-                and self.reset is None
+            self.corr_pkl_file.exists()
+            and self.score_pkl_file.exists()
+            and self.reset is None
         ):
             _logger.info(
                 f"Cache {self.corr_pkl_file} and {self.score_pkl_file} already exist. "
                 f"Skip calculation and go to plot"
             )
             return
 
@@ -705,15 +705,15 @@
 
             file_name = Path("_".join([file_base, self.scan_data_key]) + ".pkl")
             cache_file = self.cache_directory / file_name
 
             group_by = list(props["groupby"].values())
             group_by_original = None
             if (
-                    group_by_if_not_exist := props.get("groupby_if_not_exist")
+                group_by_if_not_exist := props.get("groupby_if_not_exist")
             ) and self.dataframe is not None:
                 have_missing_groups = False
                 for group in group_by:
                     if group not in self.dataframe.columns:
                         have_missing_groups = True
                 if have_missing_groups:
                     group_by_original = group_by
@@ -981,47 +981,47 @@
         if self.dump_cache_as_sqlite:
             sqlite_cache = self.cache_file.with_suffix(".sqlite")
             dump_data_frame_as_sqlite(dataframe=self.dataframe, file_name=sqlite_cache)
 
 
 class DomainPlotter:
     def __init__(
-            self,
-            scan_data,
-            scan_data_key=None,
-            default_scan=None,
-            plot_info=None,
-            show_plots=False,
-            barh=False,
-            image_directory=None,
-            cache_directory=None,
-            image_type="pdf",
-            max_plots=None,
-            tex_prepend_path=None,
-            statistics=None,
-            variables=None,
-            cdf_plot=False,
-            bar_plot=False,
-            cor_plot=False,
-            cumulative=False,
-            show_title=False,
-            breakdown_labels=None,
-            translations: dict = None,
-            export_highcharts=False,
-            highcharts_directory=None,
-            correlations=None,
-            tex_horizontal_shift=None,
-            bovenschrift=True,
-            variables_to_plot=None,
-            exclude_variables=None,
-            force_plots=False,
-            latex_files=False,
-            years_to_add_to_plot_legend=None,
-            module_info=None,
-            english=False,
+        self,
+        scan_data,
+        scan_data_key=None,
+        default_scan=None,
+        plot_info=None,
+        show_plots=False,
+        barh=False,
+        image_directory=None,
+        cache_directory=None,
+        image_type="pdf",
+        max_plots=None,
+        tex_prepend_path=None,
+        statistics=None,
+        variables=None,
+        cdf_plot=False,
+        bar_plot=False,
+        cor_plot=False,
+        cumulative=False,
+        show_title=False,
+        breakdown_labels=None,
+        translations: dict = None,
+        export_highcharts=False,
+        highcharts_directory=None,
+        correlations=None,
+        tex_horizontal_shift=None,
+        bovenschrift=True,
+        variables_to_plot=None,
+        exclude_variables=None,
+        force_plots=False,
+        latex_files=False,
+        years_to_add_to_plot_legend=None,
+        module_info=None,
+        english=False,
     ):
 
         self.english = english
         self.scan_data = scan_data
         self.scan_data_key = scan_data_key
         self.default_scan = default_scan
         self.plot_info = plot_info
@@ -1219,30 +1219,30 @@
             _logger.info(f"Plotting {plot_key}")
 
             plot_count = 0
             stop_plotting = False
             if stats_df is not None:
 
                 for module_name, module_df in stats_df.groupby(
-                        level=module_level_name, sort=False
+                    level=module_level_name, sort=False
                 ):
                     do_this_module = True
                     for mod_key, mod_prop in module_info.items():
                         if mod_prop.get("label") == module_name and not mod_prop.get(
-                                "include", True
+                            "include", True
                         ):
                             do_this_module = False
                     if not do_this_module:
                         continue
 
                     _logger.info(f"Module {module_name}")
                     if stop_plotting:
                         break
                     for question_name, question_df in module_df.groupby(
-                            level=question_level_name, sort=False
+                        level=question_level_name, sort=False
                     ):
                         _logger.debug(f"Question {question_name}")
 
                         # voorlaatste kolom bevat de variabele namen
                         variable_name_key = question_df.index.names[-2]
                         plot_variable = question_df.index.get_level_values(
                             variable_name_key
@@ -1286,19 +1286,19 @@
                             var_name=original_name,
                             breakdown_name=plot_key,
                         )
                         export_highcharts = export_highcharts_bar
                         if cdf_prop := cdf_variables.get(original_name):
                             highcharts_directory_cdf = self.highcharts_directory
                             if highcharts_info_per_year := cdf_prop.get(
-                                    "highcharts_info_per_year"
+                                "highcharts_info_per_year"
                             ):
                                 for (
-                                        hc_year_key,
-                                        hc_year_prop,
+                                    hc_year_key,
+                                    hc_year_prop,
                                 ) in highcharts_info_per_year.items():
                                     hc_dir = highcharts_directory_cdf / Path(
                                         hc_year_prop["highcharts_directory"]
                                     )
                                     hc_lab = hc_year_prop.get("highcharts_label")
                                     highcharts_info_per_year[hc_year_key] = dict(
                                         highcharts_directory=hc_dir,
@@ -1311,15 +1311,15 @@
                                 export_highcharts_cdf = export_hc_cdf
                         else:
                             plot_cdf = False
                             highcharts_info_per_year = None
                         if plot_info.directory is not None:
                             # we overschrijven hier de subdir die onder de statistiek opgegeven is
                             highcharts_directory = (
-                                    self.highcharts_directory / plot_info.directory
+                                self.highcharts_directory / plot_info.directory
                             )
                         else:
                             if plot_bar:
                                 highcharts_directory = highcharts_directory_bar
                             else:
                                 highcharts_directory = highcharts_directory_cdf
                         if plot_info.label is not None:
@@ -1392,15 +1392,15 @@
                         yoff = 0
 
                         if reference_lines is not None:
                             for ref_key, ref_prop in reference_lines.items():
                                 ref_stat_df = reference_lines[ref_key]["data"]
                                 ref_quest_df = None
                                 for ref_quest_name, ref_quest_df in ref_stat_df.groupby(
-                                        level=question_level_name
+                                    level=question_level_name
                                 ):
                                     if ref_quest_name == question_name:
                                         break
                                 if ref_quest_df is not None:
                                     mask2 = get_option_mask(
                                         question_df=ref_quest_df,
                                         variables=variables,
@@ -1524,16 +1524,23 @@
                                     )
                                     continue
                                 hist_info = scan_data_analyses_year.all_hist_per_format[
                                     plot_key
                                 ][original_name]
                                 highcharts_info = highcharts_info_per_year[year]
 
-                                if hist_info is not None:
+                                if hist_info is not None and isinstance(
+                                    hist_info, dict
+                                ):
                                     for grp_key, hist in hist_info.items():
+                                        if hist is None:
+                                            _logger.debug(
+                                                f"Hist {grp_key} does not have a histogram. Skipping"
+                                            )
+                                            continue
                                         im_file_2 = make_cdf_plot(
                                             hist=hist,
                                             plot_key=plot_key,
                                             scan_data_key=scan_data_key,
                                             grp_key=grp_key,
                                             module_name=module_name,
                                             question_name=question_name,
@@ -1650,15 +1657,15 @@
             df[column_name] = df[column_name].pad()
         plot_df = df.reset_index().set_index(index_names, drop=True)
 
     return plot_df
 
 
 def calculate_histogram_per_breakdown(
-        data: DataFrame, var_key: str, df_weights: Series, n_bins: int = 100
+    data: DataFrame, var_key: str, df_weights: Series, n_bins: int = 100
 ) -> dict:
     """
     Bereken per breakdown van de data het histogram die hoort bij var_key
 
     Parameters
     ----------
     data: DataFrame
```

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.9.3
+Version: 1.9.4
 Summary: A tool to create image belong to internetnl time series
 Home-page: https://github.com/eelcovv/internetnl_domain_analyse
 Author: Eelco van Vliet
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
```

### Comparing `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-1.9.4/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.9.3/tox.ini` & `internetnl_domain_analyse-1.9.4/tox.ini`

 * *Files identical despite different names*

