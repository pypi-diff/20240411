# Comparing `tmp/mocca2-0.0.8.tar.gz` & `tmp/mocca2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocca2-0.0.8.tar", last modified: Tue Apr  9 20:55:45 2024, max compression
+gzip compressed data, was "mocca2-0.1.0.tar", last modified: Wed Apr 10 19:29:36 2024, max compression
```

## Comparing `mocca2-0.0.8.tar` & `mocca2-0.1.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-09 20:55:37.000000 mocca2-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-09 20:55:45.338719 mocca2-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-09 20:55:37.000000 mocca2-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-09 20:55:37.000000 mocca2-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:55:45.338719 mocca2-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.330719 mocca2-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.330719 mocca2-0.0.8/src/mocca2/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/baseline/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/arpls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/asls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/flatfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/baseline/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17213 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/data2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/deconvolved_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/classes/peak.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/clustering/cluster_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.334719 mocca2-0.0.8/src/mocca2/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21627 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/dataset/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/alternating_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/deconvolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/fit_peak_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/guess_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/nonnegative_lstsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/deconvolution/peak_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/example_data/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-09 20:55:37.000000 mocca2-0.0.8/src/mocca2/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/example_data/loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/chemstation.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/empower.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/labsolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/parsers/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/find_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/merge_overlapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/peaks/split.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:41.000000 mocca2-0.0.8/src/mocca2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/src/mocca2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 20:55:45.000000 mocca2-0.0.8/src/mocca2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:55:45.338719 mocca2-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 20:55:41.000000 mocca2-0.0.8/tests/test_example_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-09 20:55:41.000000 mocca2-0.0.8/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.718620 mocca2-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-10 19:29:25.000000 mocca2-0.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 19:29:36.718620 mocca2-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-10 19:29:25.000000 mocca2-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-10 19:29:25.000000 mocca2-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:29:36.718620 mocca2-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.706620 mocca2-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.710620 mocca2-0.1.0/src/mocca2/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.710620 mocca2-0.1.0/src/mocca2/baseline/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/baseline/arpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/baseline/asls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/baseline/flatfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/baseline/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.714620 mocca2-0.1.0/src/mocca2/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/data2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/deconvolved_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/classes/peak.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.714620 mocca2-0.1.0/src/mocca2/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/clustering/cluster_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.714620 mocca2-0.1.0/src/mocca2/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24559 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/dataset/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.714620 mocca2-0.1.0/src/mocca2/deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/alternating_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/deconvolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/fit_peak_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/guess_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/nnls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/nonnegative_lstsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/deconvolution/peak_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.714620 mocca2-0.1.0/src/mocca2/example_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 19:29:25.000000 mocca2-0.1.0/src/mocca2/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/example_data/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.718620 mocca2-0.1.0/src/mocca2/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/parsers/chemstation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/parsers/empower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/parsers/labsolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/parsers/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.718620 mocca2-0.1.0/src/mocca2/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/peaks/find_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/peaks/merge_overlapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/peaks/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:29.000000 mocca2-0.1.0/src/mocca2/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.718620 mocca2-0.1.0/src/mocca2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-10 19:29:36.000000 mocca2-0.1.0/src/mocca2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-10 19:29:36.000000 mocca2-0.1.0/src/mocca2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:29:36.000000 mocca2-0.1.0/src/mocca2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 19:29:36.000000 mocca2-0.1.0/src/mocca2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 19:29:36.000000 mocca2-0.1.0/src/mocca2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:29:36.718620 mocca2-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-10 19:29:29.000000 mocca2-0.1.0/tests/test_example_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 19:29:29.000000 mocca2-0.1.0/tests/test_serialization.py
```

### Comparing `mocca2-0.0.8/LICENSE.txt` & `mocca2-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/PKG-INFO` & `mocca2-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.0.8
+Version: 0.1.0
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://oboril.github.io/mocca/
 Project-URL: Issues, https://github.com/oboril/mocca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mocca2-0.0.8/README.md` & `mocca2-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/pyproject.toml` & `mocca2-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mocca2"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Jan Oboril", email="jan.oboril@gmail.com" },
 ]
 description = "MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -24,8 +24,8 @@
   'pandas > 2.1',
   'matplotlib > 3.6',
   'pyarrow > 15.0'
 ]
 
 [project.urls]
 Homepage = "https://oboril.github.io/mocca/"
-Issues = "https://github.com/oboril/mocca/issues"
+Issues = "https://github.com/oboril/mocca/issues"
```

### Comparing `mocca2-0.0.8/src/mocca2/__init__.py` & `mocca2-0.1.0/src/mocca2/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/__main__.py` & `mocca2-0.1.0/src/mocca2/__main__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/baseline/arpls.py` & `mocca2-0.1.0/src/mocca2/baseline/arpls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/baseline/asls.py` & `mocca2-0.1.0/src/mocca2/baseline/asls.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/baseline/flatfit.py` & `mocca2-0.1.0/src/mocca2/baseline/flatfit.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/baseline/wrapper.py` & `mocca2-0.1.0/src/mocca2/baseline/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/classes/chromatogram.py` & `mocca2-0.1.0/src/mocca2/classes/chromatogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         self,
         method: Literal["asls", "arpls", "flatfit"] = "flatfit",
         smoothness: float = 1.0,
         p: float | None = None,
         tol: float = 1e-7,
         max_iter: int | None = None,
         smooth_wl: int | None = None,
-    ) -> None:
+    ) -> Chromatogram:
         """
         Corrects the baseline using AsLS, arPLS or FlatFit algorithm
 
         Parameters
         ----------
         data: NDArray | Data2D
             Data with shape [N] or [sample, N]
@@ -127,32 +127,38 @@
 
         max_iter: int | None
             maximum number of iterations. If not specified, guessed automatically
 
         smooth_wl: int | None
             if specified, applies Savitzky-Golay filter (order 2) accross wavelength axis with given window size
 
+        Returns
+        -------
+        Chromatogram
+            Returns self
         """
 
         self.data -= estimate_baseline(
             self, method, smoothness, p, tol, max_iter, smooth_wl
         ).data
 
+        return self
+
     def find_peaks(
         self,
         contraction: Literal["mean", "max", "weighted_mean"] = "mean",
         min_rel_height: float = 0.01,
         min_height: float = 10.0,
         width_at: float = 0.1,
         expand_borders: bool = True,
         merge_overlapping: bool = True,
         split_threshold: float | None = 0.05,
         min_elution_time: float | None = None,
         max_elution_time: float | None = None,
-    ) -> None:
+    ) -> Chromatogram:
         """
         Finds all peaks in contracted data. Assumes that baseline is flat and centered around 0.
 
         Parameters
         ----------
         contraction: Literal['mean', 'max', 'weighted_mean']
             Contraction method to project 2D data into 1D
@@ -177,14 +183,19 @@
 
         min_elution_time: int | None
             if specified, peaks with maximum before `min_elution_time` are omitted
 
         max_elution_time: int | None
             if specified, peaks with maximum after `max_elution_time` are omitted
 
+        Returns
+        -------
+        Chromatogram
+            Returns self
+
         Description
         -----------
 
         1. The peaks are picked using scipy.signal.find_peaks and filtered based on `min_rel_height`
         2. If `min_elution_time` or `max_elution_time` are specified, the peaks are filtered
         3. If `expand_borders`, the borders of the peaks are expanded down to baseline (up to estimated background noise)
         4. If `merge_overlapping`, any overlapping peaks are merged. See `merge_overlapping_peaks`
@@ -210,24 +221,26 @@
             (
                 self.closest_time(max_elution_time)[0]
                 if max_elution_time is not None
                 else None
             ),
         )
 
+        return self
+
     def deconvolve_peaks(
         self,
         model: (
             PeakModel
             | Literal["BiGaussian", "BiGaussianTailing", "FraserSuzuki", "Bemg"]
         ),
         min_r2: float,
         relaxe_concs: bool,
         max_comps: int,
-    ) -> None:
+    ) -> Chromatogram:
         """
         Deconvolves peaks with increasingly more components until MSE limit is reached. See `deconvolve_adaptive()` for details.
 
         Parameters
         ----------
         model: PeakModel | Literal['BiGaussian', 'BiGaussianTailing', 'FraserSuzuki']
             mathematical model used for fitting shapes of components of peaks
@@ -237,16 +250,23 @@
 
         relaxe_concs: bool
             If False, the fitted peak model functions are returned. Otherwise, the concentrations are refined with restricted least squares
 
         max_comps: int
             Maximum number of components that can be fitted
 
+        Returns
+        -------
+        Chromatogram
+            Returns self
         """
 
+        if len(self.peaks) == 0:
+            return self
+
         base_ms = np.mean([np.mean(peak.data(self.data) ** 2) for peak in self.peaks])
 
         for idx, peak in enumerate(self.peaks):
             # prepare input data
             peak_data = peak.data(self)
             peak_ms = np.mean(peak_data**2)
 
@@ -267,14 +287,16 @@
                 concentrations=concs,
                 spectra=spectra,
                 residual_mse=mse,
                 r2=r2,
                 resolved=max_mse > mse,
             )
 
+        return self
+
     def all_components(
         self, sort_by: Callable[[Component], Any] | None = None
     ) -> List[Component]:
         """Returns all peak components from this chromatogram"""
 
         components = []
         for peak in self.peaks:
@@ -380,15 +402,15 @@
         compounds: Dict[int, Compound],
         model: (
             PeakModel
             | Literal["BiGaussian", "BiGaussianTailing", "FraserSuzuki", "Bemg"]
         ),
         relaxe_concs: bool,
         min_rel_integral: float,
-    ) -> None:
+    ) -> Chromatogram:
         """
         Refines the concentration profiles using averaged spectra of the compounds.
 
         Removes components with insuffucient integrals.
         """
 
         if isinstance(model, str):
@@ -428,29 +450,31 @@
                 comp.concentration = conc
                 comp.integral = np.sum(conc)
                 comp.spectrum = spectrum
                 comp.peak_fraction = np.sum(conc) / total_conc
 
         # remove components with insufficient integrals
         min_integral = (
-            max([component.integral for component in self.all_components()])
+            max([0] + [component.integral for component in self.all_components()])
             * min_rel_integral
         )
 
         # remove small components
         for peak in self.peaks:
             peak.components = [
                 component
                 for component in peak.components
                 if component.integral > min_integral
             ]
 
         # remove peaks with no components
         self.peaks = [peak for peak in self.peaks if len(peak.components) > 0]
 
+        return self
+
     # serialization and deserialization
     def to_dict(self) -> Dict[str, Any]:
         """Converts the data to a dictionary for serialization"""
         data = super().to_dict().copy()
         data["peaks"] = [peak.to_dict().copy() for peak in self.peaks]
         data["sample_path"] = self.sample_path
         data["blank_path"] = self.blank_path
@@ -507,26 +531,48 @@
             "#e377c2",
             "#7f7f7f",
             "#bcbd22",
             "#17becf",
         ]
 
         idx = 0
+        contracted = self.contract()
+
         for peak in self.peaks:
-            for component in peak.components:
-                time = peak.time(self.time)
-                intensity = component.concentration
-                ax.plot(
-                    time,
-                    intensity,
-                    color=colors[idx % len(colors)],
-                    linestyle="-",
-                )
-                ax.fill_between(
-                    time,
-                    intensity,
+            if isinstance(peak, DeconvolvedPeak):
+                for component in peak.components:
+                    time = peak.time(self.time)
+                    intensity = component.concentration
+                    ax.plot(
+                        time,
+                        intensity,
+                        color=colors[idx % len(colors)],
+                        linestyle="-",
+                    )
+                    ax.fill_between(
+                        time,
+                        intensity,
+                        color=colors[idx % len(colors)],
+                        alpha=0.3,
+                    )
+                    idx += 1
+            else:
+                mid = (self.time[peak.left] + self.time[peak.right]) / 2
+                stretch = (-self.time[peak.left] + self.time[peak.right]) / 2
+                ax.errorbar(
+                    [mid],
+                    [0],
+                    xerr=[stretch],
                     color=colors[idx % len(colors)],
-                    alpha=0.3,
+                    capsize=3,
                 )
+                for max in peak.all_maxima:
+                    ax.vlines(
+                        self.time[max],
+                        0,
+                        contracted[max],
+                        colors=colors[idx % len(colors)],
+                        lw=1.0,
+                    )
                 idx += 1
 
         return ax
```

### Comparing `mocca2-0.0.8/src/mocca2/classes/component.py` & `mocca2-0.1.0/src/mocca2/classes/component.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/classes/compound.py` & `mocca2-0.1.0/src/mocca2/classes/compound.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/classes/data2d.py` & `mocca2-0.1.0/src/mocca2/classes/data2d.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -263,21 +263,21 @@
         ax: matplotlib.axes.Axes = None,
         color: str = "k",
         label: str | None = None,
         zero_line: bool = False,
     ) -> matplotlib.axes.Axes:
         """Plots the data using matplotlib.pyplot.imshow"""
 
+        if ax is None:
+            fig, ax = plt.subplots()
+
         # draw line at 0
         if zero_line:
             ax.axhline(0, color="k", lw=0.5, alpha=0.5)
 
-        if ax is None:
-            fig, ax = plt.subplots()
-
         ax.plot(self.time, self.contract(), "-", color=color, label=label)
         ax.set_xlabel("Time [min]")
         ax.set_ylabel("Absorbance [mAU]")
 
         # set x limit to the time range
         ax.set_xlim(self.time[0], self.time[-1])
```

### Comparing `mocca2-0.0.8/src/mocca2/classes/deconvolved_peak.py` & `mocca2-0.1.0/src/mocca2/classes/deconvolved_peak.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/classes/peak.py` & `mocca2-0.1.0/src/mocca2/classes/peak.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/clustering/cluster_components.py` & `mocca2-0.1.0/src/mocca2/clustering/cluster_components.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/dataset/dataset.py` & `mocca2-0.1.0/src/mocca2/dataset/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The class Dataset provides very high-level interface for processing sets of chromatograms"""
 
 from __future__ import annotations
 from typing import Dict, Tuple, Any, List
 from numpy.typing import NDArray
-from copy import deepcopy
 
+from multiprocessing import Pool
 import pandas as pd  # type: ignore
 import numpy as np
 
 from mocca2.classes.chromatogram import Chromatogram
 from mocca2.classes.data2d import Data2D
 from mocca2.classes import Compound, Component
 from mocca2.dataset.settings import ProcessingSettings
@@ -30,30 +30,30 @@
 
     compound_references: Dict[int, Tuple[str, float | None]]
     """If some chromatogram is reference for a compound, this we be stored here as [chromatogram id -> (compound name, concentration?)]"""
 
     istd_concentrations: Dict[int, float]
     """Concentrations of internal standard [chromatogram id -> concentration]"""
 
-    istd_chromatogram: int | None
+    _istd_chromatogram: int | None
     """ID of reference chromatogram for internal standard"""
 
     istd_compound: int | None
     """ID of compound that is internal standard"""
 
     settings: ProcessingSettings | None
     """Settings for automatic chromatogram processing"""
 
     def __init__(self):
         self.chromatograms = {}
         self._raw_2d_data = {}
         self.compounds = {}
         self.compound_references = {}
         self.istd_concentrations = {}
-        self.istd_chromatogram = None
+        self._istd_chromatogram = None
         self.istd_compound = None
         self.settings = ProcessingSettings()
 
     def add_chromatogram(
         self,
         chromatogram: Chromatogram,
         istd_concentration: float | None = None,
@@ -221,53 +221,61 @@
                             print(
                                 f"Compound {compound.name} has conc factor vs ISTD {compound.concentration_factor_vs_istd:0.3f}"
                             )
 
                 return component.compound_id
             return None
 
-        def name_impurities_in_chromatogram(chromatogram: Chromatogram, name: str):
-            components = chromatogram.all_components(sort_by=lambda c: c.integral)
-            count = 1
-            for component in components:
-                if component.compound_id is None:
-                    continue
-                if self.compounds[component.compound_id].name is not None:
-                    continue
-                self.compounds[component.compound_id].name = name + f" impurity {count}"
-                count += 1
+        # def name_impurities_in_chromatogram(chromatogram: Chromatogram, name: str):
+        #     components = chromatogram.all_components(sort_by=lambda c: c.integral)
+        #     count = 1
+        #     for component in components:
+        #         if component.compound_id is None:
+        #             continue
+        #         if self.compounds[component.compound_id].name is not None:
+        #             continue
+        #         self.compounds[component.compound_id].name = name + f" impurity {count}"
+        #         count += 1
 
         # name ISTD
-        if self.istd_chromatogram is not None:
-            name, conc = self.compound_references[self.istd_chromatogram]
+        if self._istd_chromatogram is not None:
+            name, conc = self.compound_references[self._istd_chromatogram]
             istd_id = name_main_compound_in_chromatogram(
-                self.istd_chromatogram, name, conc
+                self._istd_chromatogram, name, conc
             )
             self.istd_compound = istd_id
 
         # Set names and conversion factors for known compounds
         for idx, (name, conc) in self.compound_references.items():
             # make sure to skip ISTD
-            if idx == self.istd_chromatogram:
+            if idx == self._istd_chromatogram:
                 continue
             name_main_compound_in_chromatogram(idx, name, conc)
 
         # Set names for impurities in reference chromatograms
         # for idx, (name, _) in self.compound_references.items():
         #     name_impurities_in_chromatogram(self.chromatograms[idx], name)
 
         # Set default names for other compounds
         for compound in self.compounds.values():
             if compound.name is None:
                 compound.name = f"@ {self.time()[compound.elution_time]:0.3f}"
 
-    def process_all(self, settings: ProcessingSettings, verbose: bool = True):
+    def process_all(
+        self, settings: ProcessingSettings, verbose: bool = True, cores: int = 1
+    ):
         """Processes all chromatograms: finds and deconvolves peaks, creates averaged compounds, and refines peaks"""
         self.settings = settings
 
+        def check_nans(self):
+            if any([c is None for c in self.chromatograms.values()]):
+                raise Exception("Some chromatograms are missing")
+
+        check_nans(self)
+
         # Reset some values
         self.compounds = {}
         for chromatogram in self.chromatograms.values():
             chromatogram.peaks = []
 
         if verbose:
             print("Cropping wavelengths")
@@ -276,53 +284,107 @@
             cropped = raw.extract_wavelength(
                 settings.min_wavelength, settings.max_wavelength
             )
             self.chromatograms[idx].data = cropped.data
             self.chromatograms[idx].time = cropped.time
             self.chromatograms[idx].wavelength = cropped.wavelength
 
+        # Baseline correction
         if verbose:
             print("Correcting baseline")
-        # Baseline correction
-        for chromatogram in self.chromatograms.values():
-            chromatogram.correct_baseline(
-                method=settings.baseline_model,
-                smoothness=settings.baseline_smoothness,
-                smooth_wl=max(len(self.wavelength()) // 20, 4),  # type: ignore
-            )
+        kwargs = {
+            "method": settings.baseline_model,
+            "smoothness": settings.baseline_smoothness,
+            "smooth_wl": max(len(self.wavelength()) // 20, 4),
+        }
+        if cores == 1:
+            for chromatogram in self.chromatograms.values():
+                chromatogram.correct_baseline(**kwargs)
+        else:
+            with Pool(cores) as p:
+                keys = list(self.chromatograms.keys())
+                results = p.starmap(
+                    _double_star_args,
+                    [
+                        (
+                            Chromatogram.correct_baseline,
+                            {"self": self.chromatograms[k], **kwargs},
+                        )
+                        for k in keys
+                    ],
+                )
+                for id, chromatogram in zip(keys, results):
+                    self.chromatograms[id] = chromatogram
+        check_nans(self)
 
+        # Peak picking
         if verbose:
             print("Picking peaks")
-        # Peak picking
-        for chromatogram in self.chromatograms.values():
-            chromatogram.find_peaks(
-                min_rel_height=settings.min_rel_prominence,
-                min_height=settings.min_prominence,
-                width_at=settings.border_max_peak_cutoff,
-                split_threshold=settings.split_threshold,
-                min_elution_time=settings.min_elution_time,
-                max_elution_time=settings.max_elution_time,
-            )
+        kwargs = {
+            "min_rel_height": settings.min_rel_prominence,
+            "min_height": settings.min_prominence,
+            "width_at": settings.border_max_peak_cutoff,
+            "split_threshold": settings.split_threshold,
+            "min_elution_time": settings.min_elution_time,
+            "max_elution_time": settings.max_elution_time,
+        }
+        if cores == 1:
+            for chromatogram in self.chromatograms.values():
+                chromatogram.find_peaks(**kwargs)
+        else:
+            with Pool(cores) as p:
+                keys = list(self.chromatograms.keys())
+                results = p.starmap(
+                    _double_star_args,
+                    [
+                        (
+                            Chromatogram.find_peaks,
+                            {"self": self.chromatograms[k], **kwargs},
+                        )
+                        for k in keys
+                    ],
+                )
+                for id, chromatogram in zip(keys, results):
+                    self.chromatograms[id] = chromatogram
+        check_nans(self)
 
+        # Initial deconvolution
         if verbose:
             print("Deconvolution")
-        # Initial deconvolution
-        for idx, chromatogram in enumerate(self.chromatograms.values()):
-            if verbose:
-                print(f"Chromatogram {idx+1}/{len(self.chromatograms)}")
-            chromatogram.deconvolve_peaks(
-                model=settings.peak_model,
-                min_r2=settings.explained_threshold,
-                relaxe_concs=settings.relaxe_concs,
-                max_comps=settings.max_peak_comps,
-            )
+        kwargs = {
+            "model": settings.peak_model,
+            "min_r2": settings.explained_threshold,
+            "relaxe_concs": settings.relaxe_concs,
+            "max_comps": settings.max_peak_comps,
+        }
+        if cores == 1:
+            for idx, chromatogram in enumerate(self.chromatograms.values()):
+                if verbose:
+                    print(f"Chromatogram {idx+1}/{len(self.chromatograms)}")
+                chromatogram.deconvolve_peaks(**kwargs)
+        else:
+            with Pool(cores) as p:
+                keys = list(self.chromatograms.keys())
+                results = p.starmap(
+                    _double_star_args,
+                    [
+                        (
+                            Chromatogram.deconvolve_peaks,
+                            {"self": self.chromatograms[k], **kwargs},
+                        )
+                        for k in keys
+                    ],
+                )
+                for id, chromatogram in zip(keys, results):
+                    self.chromatograms[id] = chromatogram
+        check_nans(self)
 
+        # Cluster individual peaks to build averaged compounds
         if verbose:
             print("Clustering compounds")
-        # Cluster individual peaks to build averaged compounds
         components = [
             component
             for chromatogram in self.chromatograms.values()
             for component in chromatogram.all_components()
         ]
 
         dt = self.time_step()
@@ -366,29 +428,46 @@
         def importance(comp: Component) -> float:
             return comp.integral * comp.peak_fraction**4
 
         self.compounds = cluster_components(
             components, are_same=are_same_compound, weights=importance
         )
 
+        # Refine peaks
         if verbose:
             print("Refining peaks")
-        # Refine peaks
-        for chromatogram in self.chromatograms.values():
-            chromatogram.refine_peaks(
-                self.compounds,
-                settings.peak_model,
-                settings.relaxe_concs,
-                settings.explained_threshold,
-                settings.min_rel_integral,
-            )
+        kwargs = {
+            "compounds": self.compounds,
+            "model": settings.peak_model,
+            "relaxe_concs": settings.relaxe_concs,
+            "min_rel_integral": settings.min_rel_integral,
+        }
+        if cores == 1:
+            for chromatogram in self.chromatograms.values():
+                chromatogram.refine_peaks(**kwargs)
+        else:
+            with Pool(cores) as p:
+                keys = list(self.chromatograms.keys())
+                results = p.starmap(
+                    _double_star_args,
+                    [
+                        (
+                            Chromatogram.refine_peaks,
+                            {"self": self.chromatograms[k], **kwargs},
+                        )
+                        for k in keys
+                    ],
+                )
+                for id, chromatogram in zip(keys, results):
+                    self.chromatograms[id] = chromatogram
+        check_nans(self)
 
+        # Remove compounds that are not present
         if verbose:
             print("Naming compounds")
-        # Remove compounds that are not present
         present = set()
         for chromatogram in self.chromatograms.values():
             for component in chromatogram.all_components():
                 present.add(component.compound_id)
         self.compounds = {
             id: compound for id, compound in self.compounds.items() if id in present
         }
@@ -562,15 +641,15 @@
         """Converts the data to a dictionary for serialization"""
         dic = {
             "chromatograms": {k: v.to_dict() for k, v in self.chromatograms.items()},
             "_raw_2d_data": {k: v.to_dict() for k, v in self._raw_2d_data.items()},
             "compounds": {k: v.to_dict() for k, v in self.compounds.items()},
             "compound_references": self.compound_references,
             "istd_concentrations": self.istd_concentrations,
-            "istd_chromatogram": self.istd_chromatogram,
+            "istd_chromatogram": self._istd_chromatogram,
             "istd_compound": self.istd_compound,
             "settings": self.settings.to_dict(),
         }
         return dic | {"__classname__": "MoccaDataset"}
 
     @staticmethod
     def from_dict(data: Dict[str, Any]) -> MoccaDataset:
@@ -585,11 +664,15 @@
             int(k): Data2D.from_dict(v) for k, v in data["_raw_2d_data"].items()
         }
         dataset.compounds = {
             int(k): Compound.from_dict(v) for k, v in data["compounds"].items()
         }
         dataset.compound_references = data["compound_references"]
         dataset.istd_concentrations = data["istd_concentrations"]
-        dataset.istd_chromatogram = data["istd_chromatogram"]
+        dataset._istd_chromatogram = data["istd_chromatogram"]
         dataset.istd_compound = data["istd_compound"]
         dataset.settings = ProcessingSettings.from_dict(data["settings"])
         return dataset
+
+
+def _double_star_args(func, kwargs):
+    return func(**kwargs)
```

### Comparing `mocca2-0.0.8/src/mocca2/dataset/settings.py` & `mocca2-0.1.0/src/mocca2/dataset/settings.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/__init__.py` & `mocca2-0.1.0/src/mocca2/deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/alternating_lstsq.py` & `mocca2-0.1.0/src/mocca2/deconvolution/alternating_lstsq.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/deconvolve.py` & `mocca2-0.1.0/src/mocca2/deconvolution/deconvolve.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/fit_peak_model.py` & `mocca2-0.1.0/src/mocca2/deconvolution/fit_peak_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """Routines for fitting peak models to peak data"""
 
 from typing import Tuple
 from numpy.typing import NDArray
 import warnings
 
 import numpy as np
-from scipy.optimize import minimize # type: ignore
-from scipy.signal import find_peaks # type: ignore
-from scipy.signal import savgol_filter # type: ignore
+from scipy.optimize import minimize  # type: ignore
+from scipy.signal import find_peaks  # type: ignore
+from scipy.signal import savgol_filter  # type: ignore
 
 from mocca2.deconvolution.peak_models import PeakModel
-from mocca2.deconvolution.nonnegative_lstsq import concentrations_from_spectra, spectra_from_concentrations
+from mocca2.deconvolution.nonnegative_lstsq import (
+    concentrations_from_spectra,
+    spectra_from_concentrations,
+)
 from mocca2.deconvolution.guess_spectra import guess_spectra
 
+
 def fit_peak_model(
-        data: NDArray,
-        model: PeakModel,
-        spectra: NDArray | None = None,
-        n_compounds: int | None = None,
-        adjust_spectra: bool = True,
-        initial_params: None | NDArray = None,
-        initial_concs: None | NDArray = None
-    ) -> Tuple[NDArray, float, NDArray]:
+    data: NDArray,
+    model: PeakModel,
+    spectra: NDArray | None = None,
+    n_compounds: int | None = None,
+    adjust_spectra: bool = True,
+    initial_params: None | NDArray = None,
+    initial_concs: None | NDArray = None,
+) -> Tuple[NDArray, float, NDArray]:
     """
     Fits peak shapes to data. Spectra can be fixed or fitted too.
 
     Parameters
     ----------
     data: NDArray
         2D chromatogram data, [wavelength, time]
@@ -34,38 +38,40 @@
         mathematical model of the peak shape
 
     spectra: NDArray | None
         absorption spectra of individual components, [components, wavelength]. If not provided, guess_spectra() is used.
 
     n_compounds: int | None = None
         number of peaks to deconvolve, must be provided if spectra is None. Ignored if spectra are provided
-    
+
     adjust_spectra: bool
         whether the spectra should be also fitted. When False, the spectra are kept constant
-    
+
     initial_params: None | NDArray
         initial parameters for the models, flattened
-    
+
     initial_concs: None | NDArray
         initial guess of the concentrations
 
     Returns
     -------
     NDArray:
         Concentrations [component, time]
-    
-    float 
+
+    float
         Mean Squared Error
 
     NDArray:
         The optimized parameters, flattened
-    
+
     """
     if spectra is not None:
-        assert data.shape[0] == spectra.shape[1], "The shapes of data and spectra don't match in fit_peak_model()"
+        assert (
+            data.shape[0] == spectra.shape[1]
+        ), "The shapes of data and spectra don't match in fit_peak_model()"
     else:
         spectra = guess_spectra(data, n_compounds)
 
     # Some generally useful variables
     t = np.arange(data.shape[1], dtype=float)
     n_comps = spectra.shape[0]
     n_params = model.n_params()
@@ -79,114 +85,146 @@
         if initial_concs is None:
             # adjust spectra guess to mean=1
             spectra = (spectra.T / np.mean(spectra, axis=1)).T
             # add peaks and remove their contribution one by one
             residual_data = data.copy()
             for peak_index in range(spectra.shape[0]):
                 # get concentrations guess
-                concentrations, _ = concentrations_from_spectra(residual_data, spectra[peak_index:])
+                concentrations, _ = concentrations_from_spectra(
+                    residual_data, spectra[peak_index:]
+                )
                 # smooth out the concentrations
                 for idx in range(concentrations.shape[0]):
-                    concentrations[idx] = savgol_filter(concentrations[idx], max(data.shape[1]//20,5), 2)
+                    concentrations[idx] = savgol_filter(
+                        concentrations[idx], max(data.shape[1] // 20, 5), 2
+                    )
+
                 # find highest peak
-                component, _ = np.unravel_index(np.argmax(concentrations), concentrations.shape)
+                component, _ = np.unravel_index(
+                    np.argmax(concentrations), concentrations.shape
+                )
 
                 conc = concentrations[component]
-                peaks, info = find_peaks(conc, width=0., height=0.)
+                peaks, info = find_peaks(conc, width=2, height=0, rel_height=0.3)
                 if len(peaks) > 0:
-                    idx = np.argmax(info['peak_heights'])
-                    height = info['peak_heights'][idx]
+                    idx = np.argmax(info["peak_heights"])
+                    height = info["peak_heights"][idx]
                     mu = peaks[idx]
-                    s1 = peaks[idx] - info['left_ips'][idx]
-                    s2 = info['right_ips'][idx] - peaks[idx]
+                    s1 = peaks[idx] - info["left_ips"][idx]
+                    s2 = info["right_ips"][idx] - peaks[idx]
                 # otherwise use moments
                 else:
                     height = np.max(conc)
-                    mu = np.sum(conc*t)/(np.sum(conc) + 1e-7)
-                    s1 = np.sqrt(np.sum(conc*(t - mu)**2 * (t < mu))/(np.sum(conc * (t < mu)) + 1e-7))
-                    s2 = np.sqrt(np.sum(conc*(t - mu)**2 * (t < mu))/(np.sum(conc * (t < mu)) + 1e-7))
+                    mu = np.sum(conc * t) / (np.sum(conc) + 1e-7)
+                    s1 = np.sqrt(
+                        np.sum(conc * (t - mu) ** 2 * (t < mu))
+                        / (np.sum(conc * (t < mu)) + 1e-7)
+                    )
+                    s2 = np.sqrt(
+                        np.sum(conc * (t - mu) ** 2 * (t < mu))
+                        / (np.sum(conc * (t < mu)) + 1e-7)
+                    )
                 # get the peak parameters
-                params = model.init_guess(height, mu, s1, s2)
+                params = model.init_guess(height, mu, s1 * 1.2, s2 * 1.2)
                 p0.append(params)
 
                 # substract data accounted for by the peak
-                residual_data -= np.outer(spectra[component+peak_index], model.val(t, *params))
+                residual_data -= np.outer(
+                    spectra[component + peak_index], model.val(t, *params)
+                )
 
                 # swap remove the spectrum guess
-                spectra[[peak_index, component+peak_index]] = spectra[[component+peak_index, peak_index]]
+                spectra[[peak_index, component + peak_index]] = spectra[
+                    [component + peak_index, peak_index]
+                ]
         else:
             concentrations = initial_concs
-        
+
             for conc in concentrations:
                 # if peak is present use it to get initial parameters
-                peaks, info = find_peaks(conc, width=0., height=0.)
+                peaks, info = find_peaks(conc, width=2, height=0.0, rel_height=0.3)
                 if len(peaks) > 0:
-                    idx = np.argmax(info['peak_heights'])
-                    height = info['peak_heights'][idx]
+                    idx = np.argmax(info["peak_heights"])
+                    height = info["peak_heights"][idx]
                     mu = peaks[idx]
-                    s1 = peaks[idx] - info['left_ips'][idx]
-                    s2 = info['right_ips'][idx] - peaks[idx]
+                    s1 = peaks[idx] - info["left_ips"][idx]
+                    s2 = info["right_ips"][idx] - peaks[idx]
                 # otherwise use moments
                 else:
                     height = np.max(conc)
-                    mu = np.sum(conc*t)/(np.sum(conc) + 1e-7)
-                    s1 = np.sqrt(np.sum(conc*(t - mu)**2 * (t < mu))/(np.sum(conc * (t < mu)) + 1e-7))
-                    s2 = np.sqrt(np.sum(conc*(t - mu)**2 * (t < mu))/(np.sum(conc * (t < mu)) + 1e-7))
+                    mu = np.sum(conc * t) / (np.sum(conc) + 1e-7)
+                    s1 = np.sqrt(
+                        np.sum(conc * (t - mu) ** 2 * (t < mu))
+                        / (np.sum(conc * (t < mu)) + 1e-7)
+                    )
+                    s2 = np.sqrt(
+                        np.sum(conc * (t - mu) ** 2 * (t < mu))
+                        / (np.sum(conc * (t < mu)) + 1e-7)
+                    )
 
                 # get initial guess
-                params = model.init_guess(height, mu, s1, s2)
+                params = model.init_guess(height, mu, s1 * 1.2, s2 * 1.2)
 
                 # make sure the initial guess is within bounds
                 for i, (low, high) in enumerate(bounds):
                     params[i] = np.clip(params[i], low, high)
-                    
+
                 p0.append(params)
-        
+
         initial_params = np.array(p0).flatten()
 
-    def loss_and_grad(params: NDArray, data: NDArray, spectra: NDArray, t: NDArray) -> Tuple[float, NDArray]:
+    def loss_and_grad(
+        params: NDArray, data: NDArray, spectra: NDArray, t: NDArray
+    ) -> Tuple[float, NDArray]:
         """Returns MSE and gradient. Would be good to test that this is correct."""
         # Reshape params to [component, param]
         if not adjust_spectra:
             params = params.reshape([n_comps, n_params])
         else:
-            params = params.reshape([n_comps, n_params-1])
-            params = np.concatenate([np.ones([n_comps,1], dtype=float), params], axis=1)
+            params = params.reshape([n_comps, n_params - 1])
+            params = np.concatenate(
+                [np.ones([n_comps, 1], dtype=float), params], axis=1
+            )
 
         # Get concentrations [component, time]
         concs = np.array([model.val(t, *p) for p in params])
 
         # Get spectra
         if adjust_spectra:
             spectra = spectra_from_concentrations(data, concs)[0]
 
         # Get residues and mse
         residues = spectra.T @ concs - data
         mse = np.mean(residues**2)
 
         # Get gradients of reconstructed data [param, wl, time]
         if not adjust_spectra:
-            sTc_grad = np.zeros([n_comps*n_params, data.shape[0], data.shape[1]])
+            sTc_grad = np.zeros([n_comps * n_params, data.shape[0], data.shape[1]])
             for comp_idx, param in enumerate(params):
-                sTc_grad[comp_idx*n_params : (comp_idx+1)*n_params] = np.einsum('w,pt->pwt', spectra[comp_idx],  model.grad(t, *param))
+                sTc_grad[comp_idx * n_params : (comp_idx + 1) * n_params] = np.einsum(
+                    "w,pt->pwt", spectra[comp_idx], model.grad(t, *param)
+                )
         else:
-            sTc_grad = np.zeros([n_comps*(n_params-1), data.shape[0], data.shape[1]])
+            sTc_grad = np.zeros(
+                [n_comps * (n_params - 1), data.shape[0], data.shape[1]]
+            )
             for comp_idx, param in enumerate(params):
-                sTc_grad[comp_idx*(n_params-1) : (comp_idx+1)*(n_params-1)] = np.einsum('w,pt->pwt', spectra[comp_idx],  model.grad(t, *param)[1:])
+                sTc_grad[
+                    comp_idx * (n_params - 1) : (comp_idx + 1) * (n_params - 1)
+                ] = np.einsum("w,pt->pwt", spectra[comp_idx], model.grad(t, *param)[1:])
 
         # Get gradients fo square residues [param, wavele, time]
         res_grad = 2 * sTc_grad * residues
 
         # Average over wavelength and time axis
-        grad = np.mean(res_grad, axis=(1,2))
+        grad = np.mean(res_grad, axis=(1, 2))
 
         # Return MSE
         return mse, grad
 
-
     # Prepare for the optimization
     if not adjust_spectra:
         bounds = bounds * n_comps
     else:
         bounds = bounds[1:] * n_comps
 
     # remove height from params if spectra can be adjusted
@@ -198,27 +236,29 @@
     # These methods seem to work well: L-BFGS-B (with increased maxls), TNC, SLSQP
     result = minimize(
         lambda params: loss_and_grad(params, data, spectra, t),
         x0=initial_params,
         jac=True,
         bounds=bounds,
         method="L-BFGS-B",
-        options={'maxls':100},
-        tol=1e-10
+        options={"maxls": 100},
+        tol=1e-10,
     )
 
     # it is not a big issue if the optimization does not converged, if this function is called iteratively
     if not result.success:
-        warnings.warn("fit_peak_model(): Optimization failed to converge: " + result.message)
+        warnings.warn(
+            "fit_peak_model(): Optimization failed to converge: " + result.message
+        )
 
     params = result.x
     # Reshape params to [component, param]
     if not adjust_spectra:
-        params = params.reshape([len(params)//n_params, n_params])
+        params = params.reshape([len(params) // n_params, n_params])
     else:
-        n_peaks = len(params)//(n_params-1)
-        params = params.reshape([n_peaks, n_params-1])
-        params = np.concatenate([np.ones([n_peaks,1], dtype=float), params], axis=1)
+        n_peaks = len(params) // (n_params - 1)
+        params = params.reshape([n_peaks, n_params - 1])
+        params = np.concatenate([np.ones([n_peaks, 1], dtype=float), params], axis=1)
     # Get concentrations [component, time]
     concs = np.array([model.val(t, *p) for p in params])
 
-    return concs, result.fun, params.flatten()
+    return concs, result.fun, params.flatten()
```

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/guess_spectra.py` & `mocca2-0.1.0/src/mocca2/deconvolution/guess_spectra.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/nonnegative_lstsq.py` & `mocca2-0.1.0/src/mocca2/deconvolution/nonnegative_lstsq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,83 @@
 from typing import Tuple
 from numpy.typing import NDArray
 
 import numpy as np
-from scipy.optimize import nnls # type: ignore
 
-def concentrations_from_spectra(data: NDArray, spectra: NDArray) -> Tuple[NDArray, float]:
+# from scipy.linalg import solve, LinAlgWarning
+from mocca2.deconvolution.nnls import nnls
+import warnings
+
+
+def concentrations_from_spectra(
+    data: NDArray, spectra: NDArray
+) -> Tuple[NDArray, float]:
     """
     Calculates positive concentrations such that the mean squared error is minimized. Returns concentrations and MSE
 
     Parameters
     ----------
     data: NDArray
         Absorbance data [wavelength, time]
-    
+
     spectra: NDArray
         Spectra of the individual compounds [compound, wavelength]
 
     Returns
     -------
     NDArray
         Positive concentrations that minimize the MSE [compound, time]
     float
         MSE
-        
+
     """
 
-    assert data.shape[0] == spectra.shape[1], "The shapes do not match in concentrations_from_spectra()"
+    assert (
+        data.shape[0] == spectra.shape[1]
+    ), "The shapes do not match in concentrations_from_spectra()"
 
     concs = []
     error = 0
     for t in range(data.shape[1]):
-        conc, loss = nnls(spectra.T, data[:,t])
+        try:
+            conc, loss = nnls(spectra.T, data[:, t])
+        except:
+            # if failed to converge, solve with l2 norm
+            conc, loss = nnls(spectra.T, data[:, t], l2=1e-3)
+
         concs.append(conc)
         error += loss**2
 
     concentrations = np.array(concs).T
     mse = error / data.shape[0] / data.shape[1]
 
     return concentrations, mse
 
 
-def spectra_from_concentrations(data: NDArray, concentrations: NDArray) -> Tuple[NDArray, float]:
+def spectra_from_concentrations(
+    data: NDArray, concentrations: NDArray
+) -> Tuple[NDArray, float]:
     """
     Calculates positive spectra such that the mean squared error is minimized. Returns spectra and MSE
 
     Parameters
     ----------
     data: NDArray
         Absorbance data [wavelength, time]
-    
+
     concentrations: NDArray
         Concentrations of the individual compounds [compound, time]
 
     Returns
     -------
     NDArray
         Positive spectra that minimize the MSE [compound, wavelength]
     float
         MSE
     """
 
-    assert data.shape[1] == concentrations.shape[1], "The shapes do not match in spectra_from_concentrations()"
-
+    assert (
+        data.shape[1] == concentrations.shape[1]
+    ), "The shapes do not match in spectra_from_concentrations()"
 
     # Mathematically, this is identical problem, so reuse the other function
     return concentrations_from_spectra(data.T, concentrations)
-
```

### Comparing `mocca2-0.0.8/src/mocca2/deconvolution/peak_models.py` & `mocca2-0.1.0/src/mocca2/deconvolution/peak_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 
 from typing import List, Tuple
 from numpy.typing import NDArray
 
 import numpy as np
 
+
 class PeakModel:
     """Abstract class for functions that model peak shape"""
 
     def __call__(self, t: float | NDArray, *params: float) -> float | NDArray:
         """
         Returns height of peak specified by params at given time `t`.
         """
@@ -27,15 +28,17 @@
 
     def grad(self, t: float | NDArray, *params: float) -> NDArray:
         """
         Returns gradient w.r.t params. If t is array, the return shape is [parameter, t]
         """
         raise NotImplemented
 
-    def init_guess(self, height: float, maximum: float, width_left: float, width_right: float) -> NDArray:
+    def init_guess(
+        self, height: float, maximum: float, width_left: float, width_right: float
+    ) -> NDArray:
         """
         Creates initial guess of the model parameters from peak descriptors (height, location of maximum, left and right widths of peak)
         """
         raise NotImplemented
 
     def get_bounds(self, max_t: float) -> List[Tuple[float, float]]:
         """
@@ -45,290 +48,282 @@
         """
         raise NotImplemented
 
     def n_params(self) -> int:
         """Returns number of parameters of the model"""
         raise NotImplemented
 
+
 def test_gradients(model: PeakModel, t: NDArray, params: List[float]) -> bool:
     """
     Compares gradient from the model with numerical gradients. Returns True is all gradients are close.
-    
+
     This is useful when making sure that gradients in new peak model are all correct.
     """
     eps = 1e-5
     grad = model.grad(t, *params)
 
     for pidx, pgrad in enumerate(grad):
         pl = params.copy()
         pr = params.copy()
         pl[pidx] -= eps
         pr[pidx] += eps
-        num_grad = (model.val(t, *pr) - model.val(t, *pl)) / (2*eps)
+        num_grad = (model.val(t, *pr) - model.val(t, *pl)) / (2 * eps)
 
         if not np.allclose(pgrad, num_grad, rtol=1e-5):
-            print("Gradient does not match for parameter", pidx+1)
+            print("Gradient does not match for parameter", pidx + 1)
             print(pgrad)
             print(num_grad)
             return False
     return True
 
+
 class BiGaussian(PeakModel):
     """BiGaussian peak model"""
 
     def n_params(self) -> int:
         return 4
 
     def val(self, t: float | NDArray, *params: float) -> float | NDArray:
         h, mu, s1, s2 = params
-        v = (t < mu) * np.exp(- (t - mu)**2 / (2 * s1**2))
-        v += (t > mu) * np.exp(- (t - mu)**2 / (2 * s2**2))
+        v = (t < mu) * np.exp(-((t - mu) ** 2) / (2 * s1**2))
+        v += (t > mu) * np.exp(-((t - mu) ** 2) / (2 * s2**2))
         return v * h
 
     def grad(self, t: float | NDArray, *params: float) -> NDArray:
         h, mu, s1, s2 = params
 
-        left_gauss = (t < mu) * np.exp(- (t - mu)**2 / (2 * s1**2))
-        right_gauss = (t > mu) * np.exp(- (t - mu)**2 / (2 * s2**2))
+        left_gauss = (t < mu) * np.exp(-((t - mu) ** 2) / (2 * s1**2))
+        right_gauss = (t > mu) * np.exp(-((t - mu) ** 2) / (2 * s2**2))
 
         grad_h = left_gauss + right_gauss
-        grad_mu = h * (t-mu) * (left_gauss/s1**2 + right_gauss/s2**2)
-        grad_s1 = h * (t-mu)**2 / s1**3 * left_gauss
-        grad_s2 = h * (t-mu)**2 / s2**3 * right_gauss
+        grad_mu = h * (t - mu) * (left_gauss / s1**2 + right_gauss / s2**2)
+        grad_s1 = h * (t - mu) ** 2 / s1**3 * left_gauss
+        grad_s2 = h * (t - mu) ** 2 / s2**3 * right_gauss
 
         return np.array([grad_h, grad_mu, grad_s1, grad_s2])
-    
-    def init_guess(self, height: float, maximum: float, width_left: float, width_right: float) -> NDArray:
-        x0 = [
-            height,
-            maximum,
-            width_left,
-            width_right
-        ]
+
+    def init_guess(
+        self, height: float, maximum: float, width_left: float, width_right: float
+    ) -> NDArray:
+        x0 = [height, maximum, width_left, width_right]
 
         return np.array(x0)
-    
+
     def get_bounds(self, max_t: float) -> List[Tuple[float, float]]:
-        const = [
-            (0., np.inf),
-            (0., max_t),
-            (1., max_t/4.),
-            (1., max_t/4.)
-        ]
+        const = [(0.0, np.inf), (0.0, max_t), (1.0, max_t / 4.0), (1.0, max_t / 4.0)]
 
         return const
 
 
 class BiGaussianTailing(PeakModel):
     """BiGaussian with exponential tailing peak model"""
 
     def n_params(self) -> int:
         return 6
 
     def val(self, t: float | NDArray, *params: float) -> float | NDArray:
         h, mu, s1, s2, tail_h, tail_w = params
-        v = (t < mu) * np.exp(- (t - mu)**2 / (2 * s1**2))
-        v += (t > mu) * np.exp(- (t - mu)**2 / (2 * s2**2)) * (1. - tail_h)
-        v += (t > mu) * np.exp(- np.clip(t-mu,0,None)/tail_w) * tail_h
+        v = (t < mu) * np.exp(-((t - mu) ** 2) / (2 * s1**2))
+        v += (t > mu) * np.exp(-((t - mu) ** 2) / (2 * s2**2)) * (1.0 - tail_h)
+        v += (t > mu) * np.exp(-np.clip(t - mu, 0, None) / tail_w) * tail_h
         return v * h
 
     def grad(self, t: float | NDArray, *params: float) -> NDArray:
         h, mu, s1, s2, tail_h, tail_w = params
 
-        left_gauss = (t < mu) * np.exp(- (t - mu)**2 / (2 * s1**2))
-        right_gauss = (t > mu) * np.exp(- (t - mu)**2 / (2 * s2**2)) 
-        tail = (t > mu) * np.exp(- np.clip(t-mu,0,None)/tail_w) 
-
-        grad_h = left_gauss + right_gauss * (1. - tail_h) + tail * tail_h
-        grad_mu = h * (t-mu) * (left_gauss/s1**2 + right_gauss*(1. - tail_h)/s2**2)
+        left_gauss = (t < mu) * np.exp(-((t - mu) ** 2) / (2 * s1**2))
+        right_gauss = (t > mu) * np.exp(-((t - mu) ** 2) / (2 * s2**2))
+        tail = (t > mu) * np.exp(-np.clip(t - mu, 0, None) / tail_w)
+
+        grad_h = left_gauss + right_gauss * (1.0 - tail_h) + tail * tail_h
+        grad_mu = (
+            h * (t - mu) * (left_gauss / s1**2 + right_gauss * (1.0 - tail_h) / s2**2)
+        )
         grad_mu += h * tail * tail_h / tail_w
-        grad_s1 = h * (t-mu)**2 / s1**3 * left_gauss
-        grad_s2 = h * (t-mu)**2 / s2**3 * right_gauss * (1. - tail_h)
-        grad_tail_h = - h * right_gauss + h * tail
-        grad_tail_w = h * tail * tail_h * (t-mu)/tail_w**2
+        grad_s1 = h * (t - mu) ** 2 / s1**3 * left_gauss
+        grad_s2 = h * (t - mu) ** 2 / s2**3 * right_gauss * (1.0 - tail_h)
+        grad_tail_h = -h * right_gauss + h * tail
+        grad_tail_w = h * tail * tail_h * (t - mu) / tail_w**2
 
         return np.array([grad_h, grad_mu, grad_s1, grad_s2, grad_tail_h, grad_tail_w])
-    
-    def init_guess(self, height: float, maximum: float, width_left: float, width_right: float) -> NDArray:
-        x0 = [
-            height,
-            maximum,
-            width_left,
-            width_right,
-            0.,
-            10.
-        ]
+
+    def init_guess(
+        self, height: float, maximum: float, width_left: float, width_right: float
+    ) -> NDArray:
+        x0 = [height, maximum, width_left, width_right, 0.0, 10.0]
 
         return np.array(x0)
-    
+
     def get_bounds(self, max_t: float) -> List[Tuple[float, float]]:
         const = [
-            (0., np.inf),
-            (0., max_t),
-            (1., max_t/4.),
-            (1., max_t/4.),
-            (0., 0.2),
-            (1., max_t)
+            (0.0, np.inf),
+            (0.0, max_t),
+            (1.0, max_t / 4.0),
+            (1.0, max_t / 4.0),
+            (0.0, 0.2),
+            (1.0, max_t),
         ]
 
         return const
 
 
 class FraserSuzuki(PeakModel):
     """Fraser-Suzuki peak model"""
 
     def n_params(self) -> int:
         return 4
 
     def val(self, t: float | NDArray, *params: float) -> float | NDArray:
         h, mu, sigma, a = params
 
-        z = 1+a*(t-mu)/sigma
+        z = 1 + a * (t - mu) / sigma
         defined = z > 0
         z = np.clip(z, 1e-100, None)
 
         ln_z = np.log(z)
 
-        f = defined * np.exp(- 1/2/a**2 * ln_z**2)
+        f = defined * np.exp(-1 / 2 / a**2 * ln_z**2)
 
         return f * h
 
     def grad(self, t: float | NDArray, *params: float) -> NDArray:
         h, mu, sigma, a = params
 
-        z = 1+a*(t-mu)/sigma
+        z = 1 + a * (t - mu) / sigma
         defined = z > 0
         z = np.clip(z, 1e-100, None)
 
         ln_z = np.log(z)
 
-        f = defined * np.exp(- 1/2/a**2 * ln_z**2)
+        f = defined * np.exp(-1 / 2 / a**2 * ln_z**2)
 
         grad_h = f
 
         grad_mu = h * f * ln_z / (z * sigma * a)
 
         grad_sigma = grad_mu * (t - mu) / sigma
 
-        grad_a = grad_mu / a**2 * (- a * (t-mu) + z * sigma * ln_z)
+        grad_a = grad_mu / a**2 * (-a * (t - mu) + z * sigma * ln_z)
 
         return np.array([grad_h, grad_mu, grad_sigma, grad_a])
-    
-    def init_guess(self, height: float, maximum: float, width_left: float, width_right: float) -> NDArray:
+
+    def init_guess(
+        self, height: float, maximum: float, width_left: float, width_right: float
+    ) -> NDArray:
         x0 = [
             height,
             maximum,
-            (width_left+width_right)/2,
-            0.1
+            max((width_left + width_right) / 2, 1),
+            0.1,
         ]
 
         return np.array(x0)
-    
+
     def get_bounds(self, max_t: float) -> List[Tuple[float, float]]:
         const = [
-            (0., np.inf),
-            (0., max_t),
-            (1., max_t/4.),
-            (1e-10, 10.),
+            (0.0, np.inf),
+            (0.0, max_t),
+            (1.0, max_t / 4.0),
+            (1e-10, 10.0),
         ]
 
         return const
 
+
 from scipy.special import log_ndtr
+
+
 def log_erfc(x):
-    return log_ndtr(- x * np.sqrt(2)) + np.log(2)
+    return log_ndtr(-x * np.sqrt(2)) + np.log(2)
+
 
 class Bemg(PeakModel):
     """Bi-Exponentially Modified Gaussian peak model"""
 
     def n_params(self) -> int:
         return 5
 
     def val(self, t: float | NDArray, *params: float) -> float | NDArray:
         h, m, s, a, b = params
-        tm = t-m
-        as2 = a*s**2
-        bs2 = b*s**2
-        sq2s2 = np.sqrt(2*s**2)
+        tm = t - m
+        as2 = a * s**2
+        bs2 = b * s**2
+        sq2s2 = np.sqrt(2 * s**2)
 
-        erfc_a_arg = (as2 + tm)/sq2s2
-        exp_a_arg = a*as2/2 + a*tm
+        erfc_a_arg = (as2 + tm) / sq2s2
+        exp_a_arg = a * as2 / 2 + a * tm
 
-        erfc_b_arg = (bs2 - tm)/sq2s2
-        exp_b_arg = b*bs2/2 - b*tm
+        erfc_b_arg = (bs2 - tm) / sq2s2
+        exp_b_arg = b * bs2 / 2 - b * tm
 
         part_a = np.exp(log_erfc(erfc_a_arg) + exp_a_arg)
         part_b = np.exp(log_erfc(erfc_b_arg) + exp_b_arg)
 
-        scale = 0.5*(s+1)
+        scale = 0.5 * (s + 1)
 
         val = scale * (part_a + part_b)
 
         return val * h
 
     def grad(self, t: float | NDArray, *params: float) -> NDArray:
         h, m, s, a, b = params
-        tm = t-m
+        tm = t - m
         ai = a
         bi = b
-        as2 = ai*s**2
-        bs2 = bi*s**2
-        sq2s2 = np.sqrt(2*s**2)
+        as2 = ai * s**2
+        bs2 = bi * s**2
+        sq2s2 = np.sqrt(2 * s**2)
         r2 = np.sqrt(2)
         rpi = np.sqrt(np.pi)
 
-        erfc_a_arg = (as2 + tm)/sq2s2
-        exp_a_arg = ai*as2/2 + ai*tm
+        erfc_a_arg = (as2 + tm) / sq2s2
+        exp_a_arg = ai * as2 / 2 + ai * tm
 
-        erfc_b_arg = (bs2 - tm)/sq2s2
-        exp_b_arg = bi*bs2/2 - bi*tm
+        erfc_b_arg = (bs2 - tm) / sq2s2
+        exp_b_arg = bi * bs2 / 2 - bi * tm
 
         part_a = np.exp(log_erfc(erfc_a_arg) + exp_a_arg)
         part_b = np.exp(log_erfc(erfc_b_arg) + exp_b_arg)
 
-        scale = 0.5*(s+1)
+        scale = 0.5 * (s + 1)
 
         val = scale * (part_a + part_b)
 
-        d_erfc_a = -2/rpi*np.exp(-erfc_a_arg**2 + exp_a_arg)
-        d_erfc_b = -2/rpi*np.exp(-erfc_b_arg**2 + exp_b_arg)
+        d_erfc_a = -2 / rpi * np.exp(-(erfc_a_arg**2) + exp_a_arg)
+        d_erfc_b = -2 / rpi * np.exp(-(erfc_b_arg**2) + exp_b_arg)
 
-        d_m = -d_erfc_a/sq2s2 - a * part_a
-        d_m += d_erfc_b/sq2s2 + b * part_b
+        d_m = -d_erfc_a / sq2s2 - a * part_a
+        d_m += d_erfc_b / sq2s2 + b * part_b
         d_m *= scale
 
-        d_s = d_erfc_a * (ai - tm/s**2)/r2 + s*ai**2 * part_a
-        d_s += d_erfc_b * (bi + tm/s**2)/r2 + s*bi**2 * part_b
+        d_s = d_erfc_a * (ai - tm / s**2) / r2 + s * ai**2 * part_a
+        d_s += d_erfc_b * (bi + tm / s**2) / r2 + s * bi**2 * part_b
         d_s *= scale
         d_s += 0.5 * (part_a + part_b)
 
-        d_a = s/r2 * d_erfc_a + (as2 + tm)*part_a
+        d_a = s / r2 * d_erfc_a + (as2 + tm) * part_a
         d_a *= scale
 
-        d_b = s/r2 * d_erfc_b + (bs2 - tm)*part_b
+        d_b = s / r2 * d_erfc_b + (bs2 - tm) * part_b
         d_b *= scale
 
-        return np.array([val, d_m*h, d_s*h, d_a*h, d_b*h])
+        return np.array([val, d_m * h, d_s * h, d_a * h, d_b * h])
 
-    
-    def init_guess(self, height: float, maximum: float, width_left: float, width_right: float) -> NDArray:
-        width = (width_left + width_right) / 2.
-        x0 = [
-            height,
-            maximum,
-            width,
-            1.,
-            1.
-        ]
+    def init_guess(
+        self, height: float, maximum: float, width_left: float, width_right: float
+    ) -> NDArray:
+        width = (width_left + width_right) / 2.0
+        x0 = [height, maximum, width, 1.0, 1.0]
 
         return np.array(x0)
-    
+
     def get_bounds(self, max_t: float) -> List[Tuple[float, float]]:
         const = [
-            (0., np.inf),
-            (0., max_t),
-            (1., max_t),
+            (0.0, np.inf),
+            (0.0, max_t),
+            (1.0, max_t),
             (0.01, max_t),
             (0.01, max_t),
         ]
 
-        return const
+        return const
```

### Comparing `mocca2-0.0.8/src/mocca2/example_data/loaders.py` & `mocca2-0.1.0/src/mocca2/example_data/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,26 +293,38 @@
     chromatograms = {}
 
     if substract_blank:
         blank = Chromatogram(filename("gradient_97"))
     else:
         blank = None
 
-    chromatograms["istd"] = Chromatogram(filename("istd_96"), blank)
-    chromatograms["educt_1"] = Chromatogram(filename("educt_88"), blank)
-    chromatograms["educt_2"] = Chromatogram(filename("educt_89"), blank)
-    chromatograms["product_1"] = Chromatogram(filename("product_92"), blank)
-    chromatograms["product_2"] = Chromatogram(filename("product_93"), blank)
-    chromatograms["cn_source_a"] = Chromatogram(filename("cnsource_a_98"), blank)
-    chromatograms["cn_source_d"] = Chromatogram(filename("cnsource_d_99"), blank)
+    chromatograms["istd"] = Chromatogram(filename("istd_96"), blank, name="istd")
+    chromatograms["educt_1"] = Chromatogram(filename("educt_88"), blank, name="educt_1")
+    chromatograms["educt_2"] = Chromatogram(filename("educt_89"), blank, name="educt_2")
+    chromatograms["product_1"] = Chromatogram(
+        filename("product_92"), blank, name="product_1"
+    )
+    chromatograms["product_2"] = Chromatogram(
+        filename("product_93"), blank, name="product_2"
+    )
+    chromatograms["cn_source_a"] = Chromatogram(
+        filename("cnsource_a_98"), blank, name="cn_source_a"
+    )
+    chromatograms["cn_source_d"] = Chromatogram(
+        filename("cnsource_d_99"), blank, name="cn_source_d"
+    )
 
     chromatograms["reactions"] = []
     for i in range(84):
         chromatograms["reactions"].append(
-            Chromatogram(filename(f"sample_{i+4:d}"), blank)
+            Chromatogram(
+                filename(f"sample_{i+4:d}"),
+                blank,
+                name=f"reaction_{i+1:d}",
+            )
         )
 
     return chromatograms
 
 
 def benzaldehyde(substract_blank: bool = True) -> Tuple[Chromatogram, Chromatogram]:
     """Loads tutorial data published with the original MOCCA package, these contain 1mM and 0.5mM benzaldehyde respectively."""
```

### Comparing `mocca2-0.0.8/src/mocca2/math.py` & `mocca2-0.1.0/src/mocca2/math.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/parsers/empower.py` & `mocca2-0.1.0/src/mocca2/parsers/empower.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/parsers/labsolutions.py` & `mocca2-0.1.0/src/mocca2/parsers/labsolutions.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/parsers/wrapper.py` & `mocca2-0.1.0/src/mocca2/parsers/wrapper.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/peaks/find_peaks.py` & `mocca2-0.1.0/src/mocca2/peaks/find_peaks.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/peaks/merge_overlapping.py` & `mocca2-0.1.0/src/mocca2/peaks/merge_overlapping.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2/peaks/split.py` & `mocca2-0.1.0/src/mocca2/peaks/split.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/src/mocca2.egg-info/PKG-INFO` & `mocca2-0.1.0/src/mocca2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocca2
-Version: 0.0.8
+Version: 0.1.0
 Summary: MOCCA2 is an open-source Python project to analyze HPLC-DAD raw data
 Author-email: Jan Oboril <jan.oboril@gmail.com>
 Project-URL: Homepage, https://oboril.github.io/mocca/
 Project-URL: Issues, https://github.com/oboril/mocca/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mocca2-0.0.8/src/mocca2.egg-info/SOURCES.txt` & `mocca2-0.1.0/src/mocca2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 src/mocca2/dataset/dataset.py
 src/mocca2/dataset/settings.py
 src/mocca2/deconvolution/__init__.py
 src/mocca2/deconvolution/alternating_lstsq.py
 src/mocca2/deconvolution/deconvolve.py
 src/mocca2/deconvolution/fit_peak_model.py
 src/mocca2/deconvolution/guess_spectra.py
+src/mocca2/deconvolution/nnls.py
 src/mocca2/deconvolution/nonnegative_lstsq.py
 src/mocca2/deconvolution/peak_models.py
 src/mocca2/example_data/__init__.py
 src/mocca2/example_data/loaders.py
 src/mocca2/parsers/__init__.py
 src/mocca2/parsers/chemstation.py
 src/mocca2/parsers/empower.py
```

### Comparing `mocca2-0.0.8/tests/test_example_data.py` & `mocca2-0.1.0/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `mocca2-0.0.8/tests/test_serialization.py` & `mocca2-0.1.0/tests/test_serialization.py`

 * *Files identical despite different names*

