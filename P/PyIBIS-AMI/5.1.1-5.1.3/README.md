# Comparing `tmp/PyIBIS-AMI-5.1.1.tar.gz` & `tmp/PyIBIS-AMI-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIBIS-AMI-5.1.1.tar", last modified: Mon Feb 12 21:45:49 2024, max compression
+gzip compressed data, was "PyIBIS-AMI-5.1.3.tar", last modified: Thu Apr 11 14:09:37 2024, max compression
```

## Comparing `PyIBIS-AMI-5.1.1.tar` & `PyIBIS-AMI-5.1.3.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.746342 PyIBIS-AMI-5.1.1/
--rw-rw-rw-   0        0        0     1301 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/LICENSE
--rw-rw-rw-   0        0        0      229 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4033 2024-02-12 21:45:49.746342 PyIBIS-AMI-5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2782 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.683965 PyIBIS-AMI-5.1.1/docs/
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.694059 PyIBIS-AMI-5.1.1/docs/source/
--rw-rw-rw-   0        0        0     9612 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      692 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/docs/source/index.rst
--rw-rw-rw-   0        0        0      119 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/docs/source/intro.rst
--rw-rw-rw-   0        0        0     1292 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/docs/source/modules.rst
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.707133 PyIBIS-AMI-5.1.1/examples/
--rw-rw-rw-   0        0        0      990 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/all_taps.run
--rw-rw-rw-   0        0        0      398 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/bandwidth.run
--rw-rw-rw-   0        0        0      729 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/dummy.em
--rw-rw-rw-   0        0        0      362 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/examples.md
--rw-rw-rw-   0        0        0     3717 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/freq_resp.em
--rw-rw-rw-   0        0        0     1949 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/impulse.em
--rw-rw-rw-   0        0        0    27454 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/impulse_response_8ma.txt
--rw-rw-rw-   0        0        0      557 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/mode.run
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.707133 PyIBIS-AMI-5.1.1/examples/stratix4_ami_tx_runs/
--rw-rw-rw-   0        0        0     1693 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/stratix4_ami_tx_runs/all_taps.run
--rw-rw-rw-   0        0        0     4012 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/examples/stratix4_ami_tx_runs/test_results.xml
--rw-rw-rw-   0        0        0     2000 2024-02-12 21:33:01.000000 PyIBIS-AMI-5.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-12 21:45:49.746342 PyIBIS-AMI-5.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.686029 PyIBIS-AMI-5.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.746342 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/
--rw-rw-rw-   0        0        0     4033 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1133 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-12 21:45:49.000000 PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.714151 PyIBIS-AMI-5.1.1/src/pyibisami/
--rw-rw-rw-   0        0        0      622 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/__init__.py
--rw-rw-rw-   0        0        0      322 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/__main__.py
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.734293 PyIBIS-AMI-5.1.1/src/pyibisami/ami/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/__init__.py
--rw-rw-rw-   0        0        0     6584 2024-02-12 21:25:10.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/config.py
--rw-rw-rw-   0        0        0      519 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/generic.ami.em
--rw-rw-rw-   0        0        0     5930 2024-02-12 21:25:10.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/generic.ibs.em
--rw-rw-rw-   0        0        0    15661 2023-11-21 20:22:24.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/model.py
--rw-rw-rw-   0        0        0    12833 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/parameter.py
--rw-rw-rw-   0        0        0    19784 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ami/parser.py
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.734293 PyIBIS-AMI-5.1.1/src/pyibisami/ibis/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ibis/__init__.py
--rw-rw-rw-   0        0        0    11820 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ibis/file.py
--rw-rw-rw-   0        0        0    16189 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ibis/model.py
--rw-rw-rw-   0        0        0    13710 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/src/pyibisami/ibis/parser.py
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.744327 PyIBIS-AMI-5.1.1/src/pyibisami/tools/
--rw-rw-rw-   0        0        0        0 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/src/pyibisami/tools/__init__.py
--rw-rw-rw-   0        0        0     9166 2023-11-22 10:41:46.000000 PyIBIS-AMI-5.1.1/src/pyibisami/tools/run_tests.py
--rw-rw-rw-   0        0        0     1704 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/src/pyibisami/tools/test_results.xsl
-drwxrwxrwx   0        0        0        0 2024-02-12 21:45:49.746342 PyIBIS-AMI-5.1.1/tests/
--rw-rw-rw-   0        0        0     4621 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.1/tests/test_run_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/
+-rw-rw-rw-   0        0        0     1301 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/LICENSE
+-rw-rw-rw-   0        0        0      229 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3971 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2720 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.078482 PyIBIS-AMI-5.1.3/docs/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.088521 PyIBIS-AMI-5.1.3/docs/source/
+-rw-rw-rw-   0        0        0      323 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/ami.rst
+-rw-rw-rw-   0        0        0    10396 2024-04-11 14:06:38.000000 PyIBIS-AMI-5.1.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      256 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/ibis.rst
+-rw-rw-rw-   0        0        0      581 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1371 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/install.rst
+-rw-rw-rw-   0        0        0      158 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      152 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/docs/source/tools.rst
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.108653 PyIBIS-AMI-5.1.3/examples/
+-rw-rw-rw-   0        0        0      990 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/all_taps.run
+-rw-rw-rw-   0        0        0      398 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/bandwidth.run
+-rw-rw-rw-   0        0        0      729 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/dummy.em
+-rw-rw-rw-   0        0        0      362 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/examples.md
+-rw-rw-rw-   0        0        0     3717 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/freq_resp.em
+-rw-rw-rw-   0        0        0     1949 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/impulse.em
+-rw-rw-rw-   0        0        0    27454 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/impulse_response_8ma.txt
+-rw-rw-rw-   0        0        0      557 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/mode.run
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.108653 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/
+-rw-rw-rw-   0        0        0     1693 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/all_taps.run
+-rw-rw-rw-   0        0        0     4012 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/test_results.xml
+-rw-rw-rw-   0        0        0     2000 2024-04-11 14:05:06.000000 PyIBIS-AMI-5.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.078482 PyIBIS-AMI-5.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.146839 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/
+-rw-rw-rw-   0        0        0     3971 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1198 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      100 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      118 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 14:09:37.000000 PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.118700 PyIBIS-AMI-5.1.3/src/pyibisami/
+-rw-rw-rw-   0        0        0      624 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.128736 PyIBIS-AMI-5.1.3/src/pyibisami/ami/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/__init__.py
+-rw-rw-rw-   0        0        0     9835 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/config.py
+-rw-rw-rw-   0        0        0      519 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ami.em
+-rw-rw-rw-   0        0        0     5930 2024-02-12 22:17:02.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ibs.em
+-rw-rw-rw-   0        0        0    15750 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/model.py
+-rw-rw-rw-   0        0        0    12833 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/parameter.py
+-rw-rw-rw-   0        0        0    19786 2024-02-16 17:03:29.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ami/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:08.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/__init__.py
+-rw-rw-rw-   0        0        0    11873 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/file.py
+-rw-rw-rw-   0        0        0    16188 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/model.py
+-rw-rw-rw-   0        0        0    13712 2024-04-11 14:01:12.000000 PyIBIS-AMI-5.1.3/src/pyibisami/ibis/parser.py
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/src/pyibisami/tools/
+-rw-rw-rw-   0        0        0        0 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/__init__.py
+-rw-rw-rw-   0        0        0     9166 2024-02-14 15:27:28.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/run_tests.py
+-rw-rw-rw-   0        0        0     1704 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/src/pyibisami/tools/test_results.xsl
+drwxrwxrwx   0        0        0        0 2024-04-11 14:09:37.138776 PyIBIS-AMI-5.1.3/tests/
+-rw-rw-rw-   0        0        0     4621 2023-11-15 18:18:09.000000 PyIBIS-AMI-5.1.3/tests/test_run_tests.py
```

### Comparing `PyIBIS-AMI-5.1.1/LICENSE` & `PyIBIS-AMI-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/PKG-INFO` & `PyIBIS-AMI-5.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIBIS-AMI
-Version: 5.1.1
+Version: 5.1.3
 Summary: Facilitates working directly with IBIS-AMI DLLs from the Python command prompt.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
 Project-URL: documentation, https://github.com/capn-freako/PyAMI/wiki
 Keywords: ibis-ami
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 PyIBIS-AMI is a Python package of tools useful in the development and testing of IBIS-AMI models.
 This library is used in [PyBERT](https://github.com/capn-freako/PyBERT) and also provides two
 command line applications.
 
 It can be installed via `conda`.  PyPi support is experimental but can be installed with
  `pip install PyIBIS-AMI`.
 
-[View API/Developer's Documentation.](https://htmlpreview.github.io/?https://github.com/capn-freako/PyAMI/blob/master/docs/build/html/index.html)
+[View API/Developer's Documentation.](https://pyibis-ami.readthedocs.io/en/latest/)
 
 ## Command Line Tools
 
 ### AMI Config
 
 ```shell
 ami_config -h
```

### Comparing `PyIBIS-AMI-5.1.1/README.md` & `PyIBIS-AMI-5.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PyIBIS-AMI is a Python package of tools useful in the development and testing of IBIS-AMI models.
 This library is used in [PyBERT](https://github.com/capn-freako/PyBERT) and also provides two
 command line applications.
 
 It can be installed via `conda`.  PyPi support is experimental but can be installed with
  `pip install PyIBIS-AMI`.
 
-[View API/Developer's Documentation.](https://htmlpreview.github.io/?https://github.com/capn-freako/PyAMI/blob/master/docs/build/html/index.html)
+[View API/Developer's Documentation.](https://pyibis-ami.readthedocs.io/en/latest/)
 
 ## Command Line Tools
 
 ### AMI Config
 
 ```shell
 ami_config -h
```

### Comparing `PyIBIS-AMI-5.1.1/docs/source/conf.py` & `PyIBIS-AMI-5.1.3/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# PyBERT Developer Guide documentation build configuration file, created by
+# PyIBIS-AMI Developer Guide documentation build configuration file, created by
 # sphinx-quickstart on Tue Feb 10 10:04:12 2015.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
@@ -14,53 +14,80 @@
 
 import os
 import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-# sys.path.insert(0, os.path.abspath('.'))
+sys.path.insert(0, os.path.abspath("../../src"))
 
 # -- General configuration ------------------------------------------------
 
-# dbanas-2015_02_14
-autoclass_content = "both"
-
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "sphinx.ext.napoleon", "m2r2"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.coverage",
+    "sphinx.ext.todo",
+    # "sphinx.ext.autosummary",
+    "m2r2",
+]
+autodoc_default_options = {
+    "undoc-members": True,
+    "inherited-members": False,
+    "show-inheritance": True,
+    "members": True,
+    "exclude-members": "default_traits_view",
+}
+autodoc_mock_imports = [
+    "chaco",
+    "click",
+    "em",
+    "enable",
+    "matplotlib",
+    "numpy",
+    "traits",
+    "traitsui",
+]
+autoclass_content = "both"
+autodata_content = "both"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
-# General information about the project.
-project = "PyIBIS-AMI Developer Guide"
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+project = "PyIBIS-AMI User's Guide"
 copyright = "2015, David Banas"
+author = "David Banas"
+release = "v5.1.3"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "4.0"
+version = "5.1"
 # The full version, including alpha/beta/rc tags.
-release = "4.0.0"
+release = "5.1.3"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
@@ -69,15 +96,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = []
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -97,18 +124,20 @@
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
 
 # -- Options for HTML output ----------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "default"
+html_theme = "sphinx_rtd_theme"
+todo_include_todos = True
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -192,35 +221,35 @@
 # html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
 # html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "PyIBIS-AMIDeveloperGuidedoc"
+htmlhelp_basename = "PyIBIS-AMIUserGuidedoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #'preamble': '',
-    # Latex figure (float) alignment
-    #'figure_align': 'htbp',
-}
+# latex_elements = {
+# The paper size ('letterpaper' or 'a4paper').
+#'papersize': 'letterpaper',
+# The font size ('10pt', '11pt' or '12pt').
+#'pointsize': '10pt',
+# Additional stuff for the LaTeX preamble.
+#'preamble': '',
+# Latex figure (float) alignment
+#'figure_align': 'htbp',
+# }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    ("index", "PyIBIS-AMIDeveloperGuide.tex", "PyIBIS-AMI Developer Guide Documentation", "David Banas", "manual"),
-]
+# latex_documents = [
+#     ("index", "PyIBIS-AMIDeveloperGuide.tex", "PyIBIS-AMI Developer Guide Documentation", "David Banas", "manual"),
+# ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
@@ -239,36 +268,36 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [("index", "pyibis-amideveloperguide", "PyIBIS-AMI Developer Guide Documentation", ["David Banas"], 1)]
+# man_pages = [("index", "pyibis-amideveloperguide", "PyIBIS-AMI Developer Guide Documentation", ["David Banas"], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        "index",
-        "PyIBIS-AMIDeveloperGuide",
-        "PyIBIS-AMI Developer Guide Documentation",
-        "David Banas",
-        "PyIBIS-AMIDeveloperGuide",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
+# texinfo_documents = [
+#     (
+#         "index",
+#         "PyIBIS-AMIDeveloperGuide",
+#         "PyIBIS-AMI Developer Guide Documentation",
+#         "David Banas",
+#         "PyIBIS-AMIDeveloperGuide",
+#         "One line description of project.",
+#         "Miscellaneous",
+#     ),
+# ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
 
 # If false, no module index is generated.
 # texinfo_domain_indices = True
```

### Comparing `PyIBIS-AMI-5.1.1/docs/source/index.rst` & `PyIBIS-AMI-5.1.3/docs/source/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 .. PyIBIS-AMI Developer Guide documentation master file, created by
    copying PyIBIS-AMI Sphinx files on Tue Jan 24 2017.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-===========================================
- *PyIBIS-AMI* Source Code Developer's Guide
-===========================================
+*PyIBIS-AMI* API User's Guide
+==============================
 
-Welcome to the *PyIBIS-AMI Developer's Guide*!
-==============================================
+Welcome to the *PyIBIS-AMI* API user's documentation!
 
 Contents
 --------
 
 .. toctree::
    :maxdepth: 2
 
-   intro
+   install
    modules
 
 Indices and tables
-==================
+------------------
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 .. mdinclude:: ../../README.md
```

### Comparing `PyIBIS-AMI-5.1.1/examples/all_taps.run` & `PyIBIS-AMI-5.1.3/examples/all_taps.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/dummy.em` & `PyIBIS-AMI-5.1.3/examples/dummy.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/freq_resp.em` & `PyIBIS-AMI-5.1.3/examples/freq_resp.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/impulse.em` & `PyIBIS-AMI-5.1.3/examples/impulse.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/impulse_response_8ma.txt` & `PyIBIS-AMI-5.1.3/examples/impulse_response_8ma.txt`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/mode.run` & `PyIBIS-AMI-5.1.3/examples/mode.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/stratix4_ami_tx_runs/all_taps.run` & `PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/all_taps.run`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/examples/stratix4_ami_tx_runs/test_results.xml` & `PyIBIS-AMI-5.1.3/examples/stratix4_ami_tx_runs/test_results.xml`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/pyproject.toml` & `PyIBIS-AMI-5.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 4249 532d 414d 4922 0d0a 6465 7363 7269  BIS-AMI"..descri
 00000080: 7074 696f 6e20 3d20 2246 6163 696c 6974  ption = "Facilit
 00000090: 6174 6573 2077 6f72 6b69 6e67 2064 6972  ates working dir
 000000a0: 6563 746c 7920 7769 7468 2049 4249 532d  ectly with IBIS-
 000000b0: 414d 4920 444c 4c73 2066 726f 6d20 7468  AMI DLLs from th
 000000c0: 6520 5079 7468 6f6e 2063 6f6d 6d61 6e64  e Python command
 000000d0: 2070 726f 6d70 742e 220d 0a76 6572 7369   prompt."..versi
-000000e0: 6f6e 203d 2022 352e 312e 3122 0d0a 6175  on = "5.1.1"..au
+000000e0: 6f6e 203d 2022 352e 312e 3322 0d0a 6175  on = "5.1.3"..au
 000000f0: 7468 6f72 7320 3d20 5b20 7b6e 616d 6520  thors = [ {name 
 00000100: 3d20 2244 6176 6964 2042 616e 6173 222c  = "David Banas",
 00000110: 2020 2020 2065 6d61 696c 203d 2022 6361       email = "ca
 00000120: 706e 2e66 7265 616b 6f40 676d 6169 6c2e  pn.freako@gmail.
 00000130: 636f 6d22 7d0d 0a20 2020 2020 2020 2020  com"}..         
 00000140: 202c 207b 6e61 6d65 203d 2022 4461 7669   , {name = "Davi
 00000150: 6420 5061 7474 6572 736f 6e22 7d0d 0a20  d Patterson"}..
```

### Comparing `PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/PKG-INFO` & `PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyIBIS-AMI
-Version: 5.1.1
+Version: 5.1.3
 Summary: Facilitates working directly with IBIS-AMI DLLs from the Python command prompt.
 Author: David Patterson
 Author-email: David Banas <capn.freako@gmail.com>
 License: BSD
 Project-URL: documentation, https://github.com/capn-freako/PyAMI/wiki
 Keywords: ibis-ami
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 PyIBIS-AMI is a Python package of tools useful in the development and testing of IBIS-AMI models.
 This library is used in [PyBERT](https://github.com/capn-freako/PyBERT) and also provides two
 command line applications.
 
 It can be installed via `conda`.  PyPi support is experimental but can be installed with
  `pip install PyIBIS-AMI`.
 
-[View API/Developer's Documentation.](https://htmlpreview.github.io/?https://github.com/capn-freako/PyAMI/blob/master/docs/build/html/index.html)
+[View API/Developer's Documentation.](https://pyibis-ami.readthedocs.io/en/latest/)
 
 ## Command Line Tools
 
 ### AMI Config
 
 ```shell
 ami_config -h
```

### Comparing `PyIBIS-AMI-5.1.1/src/PyIBIS_AMI.egg-info/SOURCES.txt` & `PyIBIS-AMI-5.1.3/src/PyIBIS_AMI.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+docs/source/ami.rst
 docs/source/conf.py
+docs/source/ibis.rst
 docs/source/index.rst
-docs/source/intro.rst
+docs/source/install.rst
 docs/source/modules.rst
+docs/source/tools.rst
 examples/all_taps.run
 examples/bandwidth.run
 examples/dummy.em
 examples/examples.md
 examples/freq_resp.em
 examples/impulse.em
 examples/impulse_response_8ma.txt
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/__init__.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 Original Author: David Banas <capn.freako@gmail.com>
 
 Original Date:   3 July 2012
 
 Copyright (c) 2012 by David Banas; All rights reserved World wide.
 """
+
 from importlib.metadata import version as _get_version
 
 # Set PEP396 version attribute
 try:
     __version__ = _get_version("PyIBIS-AMI")
 except:
     __version__ = "(dev)"
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ami/generic.ami.em` & `PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ami.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ami/generic.ibs.em` & `PyIBIS-AMI-5.1.3/src/pyibisami/ami/generic.ibs.em`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ami/model.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ami/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Original Author: David Banas
 
 Original Date:   July 3, 2012
 
 Copyright (c) 2019 David Banas; All rights reserved World wide.
 """
+
 import copy as cp
 from ctypes import CDLL, byref, c_char_p, c_double
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 
@@ -211,15 +212,20 @@
 
     Notes:
         * Makes the calling of ``AMI_Close()`` automagic,
           by calling it from the destructor.
     """
 
     def __init__(self, filename):
-        """Load the dll and bind the 3 AMI functions."""
+        """
+        Load the dll and bind the 3 AMI functions.
+
+        Args:
+            filename(str): The DLL/SO file name.
+        """
 
         self._ami_mem_handle = None
         my_dll = CDLL(filename)
         self._amiInit = my_dll.AMI_Init
         try:
             self._amiGetWave = my_dll.AMI_GetWave
         except:
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ami/parameter.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ami/parameter.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ami/parser.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ami/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 Original author: David Banas <capn.freako@gmail.com>
 
 Original date:   December 17, 2016
 
 Copyright (c) 2019 David Banas; all rights reserved World wide.
 """
+
 import re
 
 from parsec import ParseError, generate, many, many1, regex, string
 from traits.api import Bool, Enum, HasTraits, Range, Trait
 from traitsui.api import Group, Item, View
 from traitsui.menu import ModalButtons
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ibis/file.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Original Author: David Banas <capn.freako@gmail.com>
 
 Original Date:   November 1, 2019
 
 For information regarding the IBIS modeling standard, visit:
 https://ibis.org/
 
-*Note:* The ``IBISModel`` class, defined here, needs to be kept separate from the
-other IBIS-related classes, defined in the ``ibis_model`` module, in order to
+**Note:** The ``IBISModel`` class, defined here, needs to be kept separate from the
+other IBIS-related classes, defined in the ``model`` module, in order to
 avoid circular imports.
 
 Copyright (c) 2019 by David Banas; All rights reserved World wide.
 """
 
 import platform
 from datetime import datetime
@@ -99,15 +99,15 @@
 
     def __init__(self, ibis_file_name, is_tx, debug=False, gui=True):
         """
         Args:
             ibis_file_name (str): The name of the IBIS file.
             is_tx (bool): True if this is a Tx model.
 
-        KeywordArgs:
+        Keyword Args:
             debug (bool): Output debugging info to console when true.
                 Default = False
             gui (bool): Set to `False` for command line and/or script usage.
                 Default = True.
         """
 
         # Super-class initialization is ABSOLUTELY NECESSARY, in order
@@ -160,14 +160,15 @@
 
         self.log("Done.")
 
     def __str__(self):
         return f"IBIS Model '{self._model_dict['file_name']}'"
 
     def info(self):
+        """Basic information about the IBIS model."""
         res = ""
         try:
             for k in ["ibis_ver", "file_name", "file_rev"]:
                 res += k + ":\t" + str(self._model_dict[k]) + "\n"
         except:
             print(self._model_dict)
             raise
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ibis/model.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class Component(HasTraits):
     """Encapsulation of a particular component from an IBIS model file."""
 
     def __init__(self, subDict):
         """
         Args:
-            subDict (dict): Dictionary of [Component] sub-keywords/params.
+            subDict(dict): Dictionary of [Component] sub-keywords/params.
         """
 
         # Super-class initialization is ABSOLUTELY NECESSARY, in order
         # to get all the Traits/UI machinery setup correctly.
         super().__init__()
 
         # Stash the sub-keywords/parameters.
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/ibis/parser.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/ibis/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 def logf(p, preStr=""):
     """Logs failure at point of occurence.
 
     Args:
         p (Parser): The original parser.
 
-    KeywordArgs:
+    Keyword Args:
         preStr (str): A prefix string to use in failure message.
                       (Default = <empty string>)
     """
 
     @Parser
     def fn(txt, ix):
         res = p(txt, ix)
@@ -468,15 +468,15 @@
 
 def parse_ibis_file(ibis_file_contents_str, debug=False):
     """Parse the contents of an IBIS file.
 
     Args:
         ibis_file_contents_str (str): The contents of the IBIS file, as a single string.
 
-    KeywordArgs:
+    Keyword Args:
         debug (bool): Output debugging info to console when true.
             Default = False
 
     Example:
         ::
 
             with open(<ibis_file_name>) as ibis_file:
```

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/tools/run_tests.py` & `PyIBIS-AMI-5.1.3/src/pyibisami/tools/run_tests.py`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/src/pyibisami/tools/test_results.xsl` & `PyIBIS-AMI-5.1.3/src/pyibisami/tools/test_results.xsl`

 * *Files identical despite different names*

### Comparing `PyIBIS-AMI-5.1.1/tests/test_run_tests.py` & `PyIBIS-AMI-5.1.3/tests/test_run_tests.py`

 * *Files identical despite different names*

