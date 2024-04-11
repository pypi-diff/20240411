# Comparing `tmp/bedboss-0.2.0.tar.gz` & `tmp/bedboss-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bedboss-0.2.0.tar", last modified: Mon Apr  8 17:58:14 2024, max compression
+gzip compressed data, was "bedboss-0.2.1.tar", last modified: Thu Apr 11 17:11:46 2024, max compression
```

## Comparing `bedboss-0.2.0.tar` & `bedboss-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-08 17:58:05.000000 bedboss-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 17:58:05.000000 bedboss-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 17:58:14.470189 bedboss-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-08 17:58:05.000000 bedboss-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.462189 bedboss-0.2.0/bedboss/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedboss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedbuncher/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/bedbuncher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedbuncher/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5113 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedbuncher/tools/bedsetStat.R
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedclassifier/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedclassifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedclassifier/bedclassifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedmaker/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14256 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/bedmaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedmaker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedqc/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3354 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/bedqc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedqc/est_line.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedstat/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6020 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/bedstat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/bedstat/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/bedstat/tools/regionstat.R
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/bedboss/qdrant_index/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/qdrant_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/qdrant_index/qdrant_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3999 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/requirements_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-08 17:58:05.000000 bedboss-0.2.0/bedboss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/bedboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 17:58:14.000000 bedboss-0.2.0/bedboss.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.466189 bedboss-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 17:58:05.000000 bedboss-0.2.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:58:14.470189 bedboss-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-08 17:58:05.000000 bedboss-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:14.470189 bedboss-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedbuncher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedclassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedmaker.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedqc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 17:58:05.000000 bedboss-0.2.0/test/test_bedstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 17:11:37.000000 bedboss-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 17:11:37.000000 bedboss-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-11 17:11:46.324185 bedboss-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-11 17:11:37.000000 bedboss-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.320185 bedboss-0.2.1/bedboss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedboss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.320185 bedboss-0.2.1/bedboss/bedbuncher/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedbuncher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedbuncher/bedbuncher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.320185 bedboss-0.2.1/bedboss/bedbuncher/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5113 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedbuncher/tools/bedsetStat.R
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.320185 bedboss-0.2.1/bedboss/bedclassifier/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedclassifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedclassifier/bedclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss/bedmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedmaker/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14483 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedmaker/bedmaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedmaker/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedmaker/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedmaker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss/bedqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedqc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3354 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedqc/bedqc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      376 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedqc/est_line.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss/bedstat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedstat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6020 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedstat/bedstat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss/bedstat/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/bedstat/tools/regionstat.R
+-rw-r--r--   0 runner    (1001) docker     (127)    14770 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss/qdrant_index/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/qdrant_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/qdrant_index/qdrant_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3999 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/requirements_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-11 17:11:37.000000 bedboss-0.2.1/bedboss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/bedboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 17:11:46.000000 bedboss-0.2.1/bedboss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 17:11:37.000000 bedboss-0.2.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 17:11:37.000000 bedboss-0.2.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 17:11:37.000000 bedboss-0.2.1/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 17:11:37.000000 bedboss-0.2.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:11:46.324185 bedboss-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-11 17:11:37.000000 bedboss-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:46.324185 bedboss-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:37.000000 bedboss-0.2.1/test/test_bedbuncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-11 17:11:37.000000 bedboss-0.2.1/test/test_bedclassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:37.000000 bedboss-0.2.1/test/test_bedmaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:37.000000 bedboss-0.2.1/test/test_bedqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:11:37.000000 bedboss-0.2.1/test/test_bedstat.py
```

### Comparing `bedboss-0.2.0/LICENSE` & `bedboss-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/PKG-INFO` & `bedboss-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedboss
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pipelines for genomic region file to produce bed files, and it's statistics
 Home-page: https://databio.org
 Author-email: khorosh@virginia.edu
 License: BSD2
 Keywords: project,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,15 @@
 License-File: LICENSE
 Requires-Dist: logmuse>=0.2.7
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: peppy>=0.40.1
 Requires-Dist: yacman>=0.8.4
 Requires-Dist: requests>=2.28.2
 Requires-Dist: piper>=v0.14.0
-Requires-Dist: bbconf>=0.5.0
+Requires-Dist: bbconf>=0.5.1
 Requires-Dist: refgenconf>=0.12.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: ubiquerg>=0.6.2
 Requires-Dist: pephubclient>=0.2.1
 Requires-Dist: geniml>=0.2.0
 
 <h1 align="center">bedboss</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bedboss Version: 0.2.0 Summary: Pipelines for
+Metadata-Version: 2.1 Name: bedboss Version: 0.2.1 Summary: Pipelines for
 genomic region file to produce bed files, and it's statistics Home-page: https:
 //databio.org Author-email: khorosh@virginia.edu License: BSD2 Keywords:
 project,bioinformatics,sequencing,ngs,workflow Classifier: Development Status
 :: 3 - Alpha Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: logmuse>=0.2.7 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: peppy>=0.40.1 Requires-Dist: yacman>=0.8.4 Requires-Dist:
-requests>=2.28.2 Requires-Dist: piper>=v0.14.0 Requires-Dist: bbconf>=0.5.0
+requests>=2.28.2 Requires-Dist: piper>=v0.14.0 Requires-Dist: bbconf>=0.5.1
 Requires-Dist: refgenconf>=0.12.2 Requires-Dist: pandas>=1.5.3 Requires-Dist:
 ubiquerg>=0.6.2 Requires-Dist: pephubclient>=0.2.1 Requires-Dist: geniml>=0.2.0
                              ************ bbeeddbboossss ************
   [![PEP compatible](https://pepkit.github.io/img/PEP-compatible-green.svg)]
  (https://pep.databio.org/) ![Run pytests](https://github.com/bedbase/bedboss/
      workflows/Run%20instalation%20test/badge.svg) [![pypi-badge](https://
    img.shields.io/pypi/v/bedboss?color=%2334D058)](https://pypi.org/project/
```

### Comparing `bedboss-0.2.0/README.md` & `bedboss-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/__init__.py` & `bedboss-0.2.1/bedboss/__init__.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedboss.py` & `bedboss-0.2.1/bedboss/bedboss.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import subprocess
 
 import pephubclient
 from pephubclient.helpers import is_registry_path, MessageHandler as m
 from bbconf.bbagent import BedBaseAgent
 from bbconf.models.base_models import FileModel
 
-
 from bedboss.bedstat.bedstat import bedstat
 from bedboss.bedmaker.bedmaker import make_all
 from bedboss.bedbuncher import run_bedbuncher
 from bedboss.const import (
     BEDBOSS_PEP_SCHEMA_PATH,
     PKG_NAME,
 )
@@ -227,14 +226,15 @@
     Run all bedboss pipelines for all samples in the pep file.
     bedmaker -> bedqc -> bedstat -> qdrant_indexing -> bedbuncher
 
     :param str bedbase_config: bedbase configuration file path
     :param str output_folder: output statistics folder
     :param Union[str, peppy.Project] pep: path to the pep file or pephub registry path
     :param str bedset_id: bedset identifier
+    :param str bedset_name: bedset name
     :param str rfg_config: path to the genome config file (refgenie)
     :param bool create_bedset: whether to create bedset
     :param bool upload_qdrant: whether to upload bedfiles to qdrant
     :param bool check_qc: whether to run quality control during badmaking
     :param str ensdb: a full path to the ensdb gtf file required for genomes not in GDdata
     :param bool just_db_commit: whether save only to the database (Without saving locally )
     :param bool force_overwrite: whether to overwrite the existing record
@@ -259,27 +259,29 @@
         raise BedBossException("Incorrect pep type. Exiting...")
 
     bbagent = BedBaseAgent(bedbase_config)
 
     validate_project(pep, BEDBOSS_PEP_SCHEMA_PATH)
 
     for i, pep_sample in enumerate(pep.samples):
+        m.print_success(f"Processing sample {i + 1}/{len(pep.samples)}")
         _LOGGER.info(f"Running bedboss pipeline for {pep_sample.sample_name}")
         if pep_sample.get("file_type"):
             if pep_sample.get("file_type").lower() == "narrowpeak":
                 is_narrow_peak = True
             else:
                 is_narrow_peak = False
         else:
             is_narrow_peak = False
         try:
             bed_id = run_all(
                 input_file=pep_sample.input_file,
                 input_type=pep_sample.input_type,
                 genome=pep_sample.genome,
+                name=pep_sample.sample_name,
                 bedbase_config=bbagent,
                 narrowpeak=is_narrow_peak,
                 chrom_sizes=pep_sample.get("chrom_sizes"),
                 open_signal_matrix=pep_sample.get("open_signal_matrix"),
                 other_metadata=pep_sample.to_dict(),
                 outfolder=output_folder,
                 rfg_config=rfg_config,
@@ -306,14 +308,15 @@
             name=bedset_name or pep.name,
             output_folder=output_folder,
             description=pep.description,
             heavy=True,
             upload_pephub=upload_pephub,
             upload_s3=upload_s3,
             no_fail=no_fail,
+            force_overwrite=force_overwrite,
         )
     else:
         _LOGGER.info(
             f"Skipping bedset creation. Create_bedset is set to {create_bedset}"
         )
     m.print_success(f"Processed samples: {processed_ids}")
     m.print_error(f"Failed samples: {failed_samples}")
```

### Comparing `bedboss-0.2.0/bedboss/bedbuncher/bedbuncher.py` & `bedboss-0.2.1/bedboss/bedbuncher/bedbuncher.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
         statistics=True,
         description=description,
         upload_pephub=upload_pephub,
         upload_s3=upload_s3,
         plots=plots.model_dump(exclude_none=True, exclude_unset=True),
         local_path=output_folder,
         no_fail=no_fail,
+        overwrite=force_overwrite,
     )
 
 
 def run_bedbuncher_form_pep(
     bedbase_config: str,
     bedset_pep: Union[str, peppy.Project],
     output_folder: str,
```

### Comparing `bedboss-0.2.0/bedboss/bedbuncher/tools/bedsetStat.R` & `bedboss-0.2.1/bedboss/bedbuncher/tools/bedsetStat.R`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedclassifier/bedclassifier.py` & `bedboss-0.2.1/bedboss/bedclassifier/bedclassifier.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedmaker/bedmaker.py` & `bedboss-0.2.1/bedboss/bedmaker/bedmaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,22 @@
             multi=True,
         )
         pm_clean = True
     else:
         pm_clean = False
     _LOGGER.info(f"Generating bigBed files for: {bed_path}")
 
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
+    bigbed_output_folder = os.path.join(output_path, BIGBED_FILE_NAME)
+    if not os.path.exists(bigbed_output_folder):
+        os.makedirs(bigbed_output_folder)
 
     bedfile_name = os.path.split(bed_path)[1]
     fileid = os.path.splitext(os.path.splitext(bedfile_name)[0])[0]
     # Produce bigBed (big_narrow_peak) file from peak file
-    big_bed_path = os.path.join(output_path, BIGBED_FILE_NAME, fileid + ".bigBed")
+    big_bed_path = os.path.join(bigbed_output_folder, fileid + ".bigBed")
     if not chrom_sizes:
         try:
             chrom_sizes = get_chrom_sizes(genome=genome, rfg_config=rfg_config)
         except MissingGenomeError:
             _LOGGER.error(f"Could not find Genome in refgenie. Skipping...")
             chrom_sizes = ""
 
@@ -187,18 +188,21 @@
     file_base_name = os.path.basename(input_file)
     input_extension = os.path.splitext(file_base_name)[1]
 
     width = "bdgbroadcall" if not narrowpeak else "bdgpeakcall"
 
     # creat cmd to run that convert non bed file to bed file
     if input_type == InputTypes.BED.value:
-        # If bed file was provided:
-        bbclient = BBClient()
-        bed_id = bbclient.add_bed_to_cache(input_file)
-        output_path = bbclient.seek(bed_id)
+        try:
+            # If bed file was provided:
+            bbclient = BBClient()
+            bed_id = bbclient.add_bed_to_cache(input_file)
+            output_path = bbclient.seek(bed_id)
+        except FileNotFoundError as e:
+            raise BedBossException(f"File not found: {input_file} Error: {e}")
 
     else:
         _LOGGER.info(f"Converting {input_file} to BED format")
 
         # Use the gzip and shutil modules to produce temporary unzipped files
         if input_extension == ".gz":
             temp_input_file = os.path.join(
```

### Comparing `bedboss-0.2.0/bedboss/bedmaker/const.py` & `bedboss-0.2.1/bedboss/bedmaker/const.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedmaker/models.py` & `bedboss-0.2.1/bedboss/bedmaker/models.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedmaker/utils.py` & `bedboss-0.2.1/bedboss/bedmaker/utils.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedqc/bedqc.py` & `bedboss-0.2.1/bedboss/bedqc/bedqc.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedstat/bedstat.py` & `bedboss-0.2.1/bedboss/bedstat/bedstat.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/bedstat/tools/regionstat.R` & `bedboss-0.2.1/bedboss/bedstat/tools/regionstat.R`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/cli.py` & `bedboss-0.2.1/bedboss/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,14 +410,22 @@
     from bbconf import BedBaseAgent
 
     bbagent = BedBaseAgent(config)
     bbagent.bedset.delete(identifier)
     print(f"BedSet {identifier} deleted from the bedbase database")
 
 
+@app.command(help="check installed R packages")
+def check_requirements():
+    from bedboss.bedboss import requirements_check
+
+    print("Checking piplines requirements...")
+    requirements_check()
+
+
 @app.callback()
 def common(
     ctx: typer.Context,
     version: bool = typer.Option(
         None, "--version", "-v", callback=version_callback, help="App version"
     ),
 ):
```

### Comparing `bedboss-0.2.0/bedboss/const.py` & `bedboss-0.2.1/bedboss/const.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/exceptions.py` & `bedboss-0.2.1/bedboss/exceptions.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/models.py` & `bedboss-0.2.1/bedboss/models.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/requirements_test.sh` & `bedboss-0.2.1/bedboss/requirements_test.sh`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss/utils.py` & `bedboss-0.2.1/bedboss/utils.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/bedboss.egg-info/PKG-INFO` & `bedboss-0.2.1/bedboss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bedboss
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pipelines for genomic region file to produce bed files, and it's statistics
 Home-page: https://databio.org
 Author-email: khorosh@virginia.edu
 License: BSD2
 Keywords: project,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -17,15 +17,15 @@
 License-File: LICENSE
 Requires-Dist: logmuse>=0.2.7
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: peppy>=0.40.1
 Requires-Dist: yacman>=0.8.4
 Requires-Dist: requests>=2.28.2
 Requires-Dist: piper>=v0.14.0
-Requires-Dist: bbconf>=0.5.0
+Requires-Dist: bbconf>=0.5.1
 Requires-Dist: refgenconf>=0.12.2
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: ubiquerg>=0.6.2
 Requires-Dist: pephubclient>=0.2.1
 Requires-Dist: geniml>=0.2.0
 
 <h1 align="center">bedboss</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: bedboss Version: 0.2.0 Summary: Pipelines for
+Metadata-Version: 2.1 Name: bedboss Version: 0.2.1 Summary: Pipelines for
 genomic region file to produce bed files, and it's statistics Home-page: https:
 //databio.org Author-email: khorosh@virginia.edu License: BSD2 Keywords:
 project,bioinformatics,sequencing,ngs,workflow Classifier: Development Status
 :: 3 - Alpha Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
 Engineering :: Bio-Informatics Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: logmuse>=0.2.7 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: peppy>=0.40.1 Requires-Dist: yacman>=0.8.4 Requires-Dist:
-requests>=2.28.2 Requires-Dist: piper>=v0.14.0 Requires-Dist: bbconf>=0.5.0
+requests>=2.28.2 Requires-Dist: piper>=v0.14.0 Requires-Dist: bbconf>=0.5.1
 Requires-Dist: refgenconf>=0.12.2 Requires-Dist: pandas>=1.5.3 Requires-Dist:
 ubiquerg>=0.6.2 Requires-Dist: pephubclient>=0.2.1 Requires-Dist: geniml>=0.2.0
                              ************ bbeeddbboossss ************
   [![PEP compatible](https://pepkit.github.io/img/PEP-compatible-green.svg)]
  (https://pep.databio.org/) ![Run pytests](https://github.com/bedbase/bedboss/
      workflows/Run%20instalation%20test/badge.svg) [![pypi-badge](https://
    img.shields.io/pypi/v/bedboss?color=%2334D058)](https://pypi.org/project/
```

### Comparing `bedboss-0.2.0/bedboss.egg-info/SOURCES.txt` & `bedboss-0.2.1/bedboss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/setup.py` & `bedboss-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `bedboss-0.2.0/test/test_bedclassifier.py` & `bedboss-0.2.1/test/test_bedclassifier.py`

 * *Files identical despite different names*

