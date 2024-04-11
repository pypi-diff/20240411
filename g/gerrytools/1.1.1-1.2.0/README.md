# Comparing `tmp/gerrytools-1.1.1.tar.gz` & `tmp/gerrytools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gerrytools-1.1.1.tar", last modified: Fri Apr 28 15:28:10 2023, max compression
+gzip compressed data, was "gerrytools-1.2.0.tar", last modified: Thu Apr 11 18:52:54 2024, max compression
```

## Comparing `gerrytools-1.1.1.tar` & `gerrytools-1.2.0.tar`

### file list

```diff
@@ -1,70 +1,79 @@
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.624028 gerrytools-1.1.1/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1469 2023-01-23 15:04:17.000000 gerrytools-1.1.1/LICENSE
--rw-rw----   0 cricha10 (31944) cricha10  (6417)       44 2023-01-23 15:04:17.000000 gerrytools-1.1.1/MANIFEST.in
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     6176 2023-04-28 15:28:10.622264 gerrytools-1.1.1/PKG-INFO
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     5862 2023-04-28 15:26:34.000000 gerrytools-1.1.1/README.md
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.288438 gerrytools-1.1.1/gerrytools/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)       46 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/__init__.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.363536 gerrytools-1.1.1/gerrytools/data/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    12360 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/AssignmentCompressor.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1629 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/URLs.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      760 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/__init__.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    11786 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/acs.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    10384 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/census.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    17386 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/estimatecvap.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     7726 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/fetch.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1563 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/geometries.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     3602 2023-04-28 15:26:34.000000 gerrytools-1.1.1/gerrytools/data/remap.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.407685 gerrytools-1.1.1/gerrytools/geometry/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      781 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/__init__.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     4923 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/compactness.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1117 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dataframe.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     9249 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dissolve.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1862 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/dualgraph.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    20337 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/optimize.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2330 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/unitmap.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1302 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/geometry/updater.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.513960 gerrytools-1.1.1/gerrytools/plotting/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      961 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/__init__.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     3774 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/annotation.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1732 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/bins.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     4237 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/boxplot.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     4978 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/choropleth.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     3780 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/colors.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1701 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/districtnumbers.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2721 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/drawgraph.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2352 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/drawplan.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2696 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/gifs.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     3666 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/histogram.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    20106 2023-01-23 15:04:17.000000 gerrytools-1.1.1/gerrytools/plotting/latexcolors.json
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2291 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/multidimensional.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2171 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/scatterplot.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     2430 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/sealevel.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      396 2023-01-23 15:04:17.000000 gerrytools-1.1.1/gerrytools/plotting/utils.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     4677 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/plotting/violin.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.566645 gerrytools-1.1.1/gerrytools/scoring/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1589 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/__init__.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1547 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/contiguity.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1399 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/demographics.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     5406 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/partisan.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1037 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/population.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    28615 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/scores.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     7151 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/splits.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1012 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/scoring/types.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.584368 gerrytools-1.1.1/gerrytools/utilities/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     3026 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/JSON.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      177 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/__init__.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1238 2023-04-28 15:26:35.000000 gerrytools-1.1.1/gerrytools/utilities/rename.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.314274 gerrytools-1.1.1/gerrytools.egg-info/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     6176 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/PKG-INFO
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1728 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/SOURCES.txt
--rw-rw----   0 cricha10 (31944) cricha10  (6417)        1 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/dependency_links.txt
--rw-rw----   0 cricha10 (31944) cricha10  (6417)      215 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/requires.txt
--rw-rw----   0 cricha10 (31944) cricha10  (6417)       11 2023-04-28 15:28:10.000000 gerrytools-1.1.1/gerrytools.egg-info/top_level.txt
--rw-rw----   0 cricha10 (31944) cricha10  (6417)       38 2023-04-28 15:28:10.626540 gerrytools-1.1.1/setup.cfg
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1105 2023-04-28 15:27:54.000000 gerrytools-1.1.1/setup.py
-drwxrwx---   0 cricha10 (31944) cricha10  (6417)        0 2023-04-28 15:28:10.615783 gerrytools-1.1.1/tests/
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    19311 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_data.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     4968 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_geometry.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)     1883 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_plotting.py
--rw-rw----   0 cricha10 (31944) cricha10  (6417)    10529 2023-04-28 15:26:35.000000 gerrytools-1.1.1/tests/test_scoring.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1469 2024-04-11 18:51:40.000000 gerrytools-1.2.0/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)       44 2024-04-11 18:51:40.000000 gerrytools-1.2.0/MANIFEST.in
+-rw-r--r--   0 peter     (1000) peter     (1000)     7581 2024-04-11 18:52:54.057885 gerrytools-1.2.0/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     7246 2024-04-11 18:51:40.000000 gerrytools-1.2.0/README.md
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.054551 gerrytools-1.2.0/gerrytools/
+-rw-r--r--   0 peter     (1000) peter     (1000)      528 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/__init__.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.054551 gerrytools-1.2.0/gerrytools/ben/
+-rw-r--r--   0 peter     (1000) peter     (1000)      952 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/ben/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8750 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/ben/binary_ensemble.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      988 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/ben/docker_manager.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    12240 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/ben/parse.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    22007 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/ben/reben.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.054551 gerrytools-1.2.0/gerrytools/data/
+-rw-r--r--   0 peter     (1000) peter     (1000)    12345 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/AssignmentCompressor.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1629 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/URLs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      761 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11786 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/acs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    10384 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/census.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    17620 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/estimatecvap.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7726 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/fetch.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1563 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/geometries.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3602 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/data/remap.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/geometry/
+-rw-r--r--   0 peter     (1000) peter     (1000)      781 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4923 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/compactness.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1117 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/dataframe.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     9249 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/dissolve.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1862 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/dualgraph.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    20437 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/optimize.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2330 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/unitmap.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1302 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/geometry/updater.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/mgrp/
+-rw-r--r--   0 peter     (1000) peter     (1000)      624 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    13522 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/run_container.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/mgrp/runners/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/runners/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     6682 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/runners/forest.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8742 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/runners/recom.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8207 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/mgrp/runners/smc.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/plotting/
+-rw-r--r--   0 peter     (1000) peter     (1000)      961 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3774 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/annotation.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1732 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/bins.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4237 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/boxplot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5559 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/choropleth.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3781 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/colors.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1701 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/districtnumbers.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2721 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/drawgraph.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2366 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/drawplan.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2696 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/gifs.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5871 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/histogram.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    20106 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/latexcolors.json
+-rw-r--r--   0 peter     (1000) peter     (1000)     2291 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/multidimensional.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4765 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/scatterplot.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2430 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/sealevel.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      396 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/utils.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4803 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/plotting/violin.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/scoring/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1589 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1547 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/contiguity.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1399 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/demographics.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5406 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/partisan.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1037 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/population.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    28601 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/scores.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7151 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/splits.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1012 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/scoring/types.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.057885 gerrytools-1.2.0/gerrytools/utilities/
+-rw-r--r--   0 peter     (1000) peter     (1000)     3038 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/utilities/JSON.py
+-rw-r--r--   0 peter     (1000) peter     (1000)      177 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/utilities/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1238 2024-04-11 18:51:40.000000 gerrytools-1.2.0/gerrytools/utilities/rename.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2024-04-11 18:52:54.054551 gerrytools-1.2.0/gerrytools.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)     7581 2024-04-11 18:52:54.000000 gerrytools-1.2.0/gerrytools.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)     1978 2024-04-11 18:52:54.000000 gerrytools-1.2.0/gerrytools.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2024-04-11 18:52:54.000000 gerrytools-1.2.0/gerrytools.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      265 2024-04-11 18:52:54.000000 gerrytools-1.2.0/gerrytools.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       11 2024-04-11 18:52:54.000000 gerrytools-1.2.0/gerrytools.egg-info/top_level.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       38 2024-04-11 18:52:54.057885 gerrytools-1.2.0/setup.cfg
+-rw-r--r--   0 peter     (1000) peter     (1000)     1278 2024-04-11 18:51:40.000000 gerrytools-1.2.0/setup.py
```

### Comparing `gerrytools-1.1.1/LICENSE` & `gerrytools-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/PKG-INFO` & `gerrytools-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,95 @@
-Metadata-Version: 2.1
-Name: gerrytools
-Version: 1.1.1
-Summary: Tools for processing and visualizing districting plans.
-Home-page: https://github.com/mggg/gerrytools
-Author: MGGG Redistricting Lab
-Author-email: engineering@mggg.org
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) 
+[![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) 
+[![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) 
+[![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) 
+[![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
 
 
 ## Installation
+
 ### Using `pip` (recommended)
+
 To install GerryTools from [PyPi](https://pypi.org/project/gerrytools/), run
 
+```console
+pip install gerrytools
 ```
-$ pip install gerrytools
+
+from the command line. if you would like to use the `mgrp` and `ben` modules as well,
+you can invoke 
+
+```console
+pip install gerrytools[mgrp]
 ```
 
-from the command line.
+you will need to make sure that [Docker Desktop](https://www.docker.com/get-started/)
+is installed on your machine an updated to version >= 4.28.0. For more information on
+getting this set up, please see 
+[our documentation page](https://gerrytools.readthedocs.io/en/latest/topics/docker/)
 
 ## Usage
-### Contents
+
 GerryTools is split up into multiple sub-packages, each designed to simplify and
 standardize redistricting workflows.
 
-* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you
-can find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20),
-ACS CVAP Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric
-data. You can also find tools for moving CVAP data to other levels of geometry (e.g. prorating 2019 CVAP on 2019 Census tracts to 2020 blocks).
-* **`gerrytools.geometry`** provides facilities for dealing with geometric and
-related data. There are tools for translating and evaluating GerryChain
-[`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to 2020 VTDs), creating
-[dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs), and optimization algorithms for renaming districts.
-* **`gerrytools.plotting`** contains methods for generating extremely high-quality 
-Lab-standard data visualizations.
-* **`gerrytools.scoring`** provides a vast array of redistricting plan scores. These
-can be used standalone _or_ as GerryChain
-[updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
-* **`gerrychain.utilities`** has ease-of-use methods for renaming directories
-containing shapefiles (which comes in handy more often than you'd think) and making
-JSON objects out of Python objects (useful when trying to organize information
-for many districting plans in a standard format).
+* **`gerrytools.ben`** BEN (binary-ensemble) is our general purpose compression
+    algorithm for working with ensembles of plans. In general, the ben algorithm can
+    improve the storage of an ensemble of plans by an order of magnitude. When combined
+    with the special XBEN (eXtreme BEN) portion of the algorithm, many ensembles of
+    plans can be compressed small enough to fit into an email (~25Mb).
+
+* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you can
+    find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20), ACS CVAP
+    Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric data. You
+    can also find tools for moving CVAP data to other levels of geometry (e.g. prorating
+    2019 CVAP on 2019 Census tracts to 2020 blocks).
+
+* **`gerrytools.geometry`** provides facilities for dealing with geometric and related
+    data. There are tools for translating and evaluating GerryChain
+    [`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, 
+    performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to
+    2020 VTDs), creating 
+    [dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs),
+    and optimization algorithms for renaming districts.
+
+* **`gerrytools.mgrp`** this module uses a Docker container to allow users to access several
+    ensemble methods for generating districting plans on a state. In particular our Rust
+    implementation of our `gerrychain` library, `frcw`, the Julia implementation of 
+    [Forest Recom](https://arxiv.org/pdf/2008.08054.pdf), and the R/C++ implementation of
+    [Sequential Monte Carlo (SMC)](https://github.com/alarm-redist/redist) are available
+    through this module. 
+
+* **`gerrytools.plotting`** contains methods for generating extremely
+    high-quality Lab-standard data visualizations.
+
+* **`gerrytools.scoring`** provides a vast array of redistricting plan scores.
+    These can be used standalone _or_ as GerryChain 
+    [updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
+
+* **`gerrychain.utilities`** has ease-of-use methods for renaming
+    directories containing shapefiles (which comes in handy more often than you'd
+    think) and making JSON objects out of Python objects (useful when trying to
+    organize information for many districting plans in a standard format).
+
+<!-- ### Example
 
-### Example
 GerryTools is easy to use and is designed to simplify data- and redistricting-related
 workflows. For example, let's say we want to analyze Alabama's citizen voting-age
 population data on 2020 Census tracts. First, we can download the geometric data
 for the state using `gerrytools.data.geometry20()`:
 
 ```python
 from gerrytools.data import geometry20
@@ -93,26 +123,31 @@
 
 # Merge. Note that the DataFrames have different unique identifier columns --- this
 # is intentional, and serves to differentiate datasets of varying geometric levels.
 merged = geometric.merge(demographic, left_on="GEOID20", right_on="TRACT20")
 ```
 
 And there we are — what once took hours of setup and parsing now takes less than a
-minute.
+minute. -->
 
 ## Contributing
+
 GerryTools is an active project, and has multiple contributors. If you'd like to
 contribute, here are a few house rules:
 
 1. After cloning this repository, run `sh setup.sh` to download and install
 necessary git hooks and linting configurations.
+
 2. **Follow the [PEP8 style guide](https://peps.python.org/pep-0008/)**. After
 installing the above git hooks, linting is performed before every push. PEP8 errors can be automatically corrected by running `autopep8 --in-place --aggressive -r gerrytools` on the command line from the root directory.
+
 3. **Write tests.** All changes, major or minor, **must** be accompanied by testing
 code. Code and tests will be immediately reviewed by Lab maintainers.
+
 4. Test coverage must stay **at least** the same; this can be checked by running
 `pytest --cov=evaltools` after the tests are added to `tests/`.
+
 5. **Write documentation.** All changes should be documented via docstrings,
 and code should be repletely commented. It's much easier to decipher commented
 code! Docstring documentation is compiled on every commit via git hooks.
 
 We look forward to your contributions!
```

### Comparing `gerrytools-1.1.1/README.md` & `gerrytools-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,107 @@
+Metadata-Version: 2.1
+Name: gerrytools
+Version: 1.2.0
+Summary: Tools for processing and visualizing districting plans.
+Home-page: https://github.com/mggg/gerrytools
+Author: MGGG Redistricting Lab
+Author-email: engineering@mggg.org
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: mgrp
+License-File: LICENSE
+
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) 
+[![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) 
+[![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) 
+[![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) 
+[![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
 
 
 ## Installation
+
 ### Using `pip` (recommended)
+
 To install GerryTools from [PyPi](https://pypi.org/project/gerrytools/), run
 
+```console
+pip install gerrytools
 ```
-$ pip install gerrytools
+
+from the command line. if you would like to use the `mgrp` and `ben` modules as well,
+you can invoke 
+
+```console
+pip install gerrytools[mgrp]
 ```
 
-from the command line.
+you will need to make sure that [Docker Desktop](https://www.docker.com/get-started/)
+is installed on your machine an updated to version >= 4.28.0. For more information on
+getting this set up, please see 
+[our documentation page](https://gerrytools.readthedocs.io/en/latest/topics/docker/)
 
 ## Usage
-### Contents
+
 GerryTools is split up into multiple sub-packages, each designed to simplify and
 standardize redistricting workflows.
 
-* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you
-can find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20),
-ACS CVAP Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric
-data. You can also find tools for moving CVAP data to other levels of geometry (e.g. prorating 2019 CVAP on 2019 Census tracts to 2020 blocks).
-* **`gerrytools.geometry`** provides facilities for dealing with geometric and
-related data. There are tools for translating and evaluating GerryChain
-[`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to 2020 VTDs), creating
-[dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs), and optimization algorithms for renaming districts.
-* **`gerrytools.plotting`** contains methods for generating extremely high-quality 
-Lab-standard data visualizations.
-* **`gerrytools.scoring`** provides a vast array of redistricting plan scores. These
-can be used standalone _or_ as GerryChain
-[updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
-* **`gerrychain.utilities`** has ease-of-use methods for renaming directories
-containing shapefiles (which comes in handy more often than you'd think) and making
-JSON objects out of Python objects (useful when trying to organize information
-for many districting plans in a standard format).
+* **`gerrytools.ben`** BEN (binary-ensemble) is our general purpose compression
+    algorithm for working with ensembles of plans. In general, the ben algorithm can
+    improve the storage of an ensemble of plans by an order of magnitude. When combined
+    with the special XBEN (eXtreme BEN) portion of the algorithm, many ensembles of
+    plans can be compressed small enough to fit into an email (~25Mb).
+
+* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you can
+    find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20), ACS CVAP
+    Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric data. You
+    can also find tools for moving CVAP data to other levels of geometry (e.g. prorating
+    2019 CVAP on 2019 Census tracts to 2020 blocks).
+
+* **`gerrytools.geometry`** provides facilities for dealing with geometric and related
+    data. There are tools for translating and evaluating GerryChain
+    [`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, 
+    performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to
+    2020 VTDs), creating 
+    [dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs),
+    and optimization algorithms for renaming districts.
+
+* **`gerrytools.mgrp`** this module uses a Docker container to allow users to access several
+    ensemble methods for generating districting plans on a state. In particular our Rust
+    implementation of our `gerrychain` library, `frcw`, the Julia implementation of 
+    [Forest Recom](https://arxiv.org/pdf/2008.08054.pdf), and the R/C++ implementation of
+    [Sequential Monte Carlo (SMC)](https://github.com/alarm-redist/redist) are available
+    through this module. 
+
+* **`gerrytools.plotting`** contains methods for generating extremely
+    high-quality Lab-standard data visualizations.
+
+* **`gerrytools.scoring`** provides a vast array of redistricting plan scores.
+    These can be used standalone _or_ as GerryChain 
+    [updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
+
+* **`gerrychain.utilities`** has ease-of-use methods for renaming
+    directories containing shapefiles (which comes in handy more often than you'd
+    think) and making JSON objects out of Python objects (useful when trying to
+    organize information for many districting plans in a standard format).
+
+<!-- ### Example
 
-### Example
 GerryTools is easy to use and is designed to simplify data- and redistricting-related
 workflows. For example, let's say we want to analyze Alabama's citizen voting-age
 population data on 2020 Census tracts. First, we can download the geometric data
 for the state using `gerrytools.data.geometry20()`:
 
 ```python
 from gerrytools.data import geometry20
@@ -82,26 +135,31 @@
 
 # Merge. Note that the DataFrames have different unique identifier columns --- this
 # is intentional, and serves to differentiate datasets of varying geometric levels.
 merged = geometric.merge(demographic, left_on="GEOID20", right_on="TRACT20")
 ```
 
 And there we are — what once took hours of setup and parsing now takes less than a
-minute.
+minute. -->
 
 ## Contributing
+
 GerryTools is an active project, and has multiple contributors. If you'd like to
 contribute, here are a few house rules:
 
 1. After cloning this repository, run `sh setup.sh` to download and install
 necessary git hooks and linting configurations.
+
 2. **Follow the [PEP8 style guide](https://peps.python.org/pep-0008/)**. After
 installing the above git hooks, linting is performed before every push. PEP8 errors can be automatically corrected by running `autopep8 --in-place --aggressive -r gerrytools` on the command line from the root directory.
+
 3. **Write tests.** All changes, major or minor, **must** be accompanied by testing
 code. Code and tests will be immediately reviewed by Lab maintainers.
+
 4. Test coverage must stay **at least** the same; this can be checked by running
 `pytest --cov=evaltools` after the tests are added to `tests/`.
+
 5. **Write documentation.** All changes should be documented via docstrings,
 and code should be repletely commented. It's much easier to decipher commented
 code! Docstring documentation is compiled on every commit via git hooks.
 
 We look forward to your contributions!
```

### Comparing `gerrytools-1.1.1/gerrytools/data/AssignmentCompressor.py` & `gerrytools-1.2.0/gerrytools/data/AssignmentCompressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 
 
 class AssignmentCompressor:
     """
     A class for compressing and decompressing lots of assignments very, very
     quickly. Intended for use with ``jsonlines``-like libraries (where
     assignments are read in line-by-line) or for network requests (where
-    assignments are retrieved one-by-one). When decompressing, yields ``dict``s
+    assignments are retrieved one-by-one). When decompressing, yields ``dict`` s
     where keys are in sorted order.
 
     The compression schema considers the set of unique identifiers, imposes an
     ordering (lexicographic order) on the identifiers, and matches the
     assignment to that ordering. We assign all unassigned units to ``"-1"``
     and, once the default cache size is hit (or assignments are no longer being
     read in), compress all assignments in the cache. Assignments are read in
     and out in the same order, and the keys for each assignment are in the
     same order.
 
     Example:
+
         To compress assignments, we need a set of unique identifiers such that
         each identifier maps one geometric unit to one district.
 
+
             ...
 
             geoids = blocks["GEOID20"].astype(str)
-            ac = AssignmentCompressor(
-                 geoids, location="compressed-assignments.ac")
+            ac = AssignmentCompressor(geoids, location="compressed-assignments.ac")
 
             with ac as compressor:
                 for assignment in assignments:
                     # Here, ensure that all assignments have string keys and
                     # string values; also ensure that an assignment's keys are
                     # a subset of geoids (or whatever IDs you're passing).
                     compressor.compress(assignment)
@@ -48,15 +49,14 @@
             geoids = blocks["GEOID20"].astype(str)
             ac = AssignmentCompressor(geoids, location="compressed-assignments.ac")
 
             for assignment in ac.decompress():
                 <do whatever!>
 
             ...
-
     Attributes:
         DISTRICT_DELIMITER (bytes): A bytestring which separates district
             identifiers in an assignment.
         ASSIGNMENT_DELIMITER (bytes): A bytestring which separates assignments from
             each other.
         CHUNK_DELIMITER (bytes): A bytestring which separates assignment chunks
             from each other.
@@ -225,15 +225,15 @@
                     writer.write(self.CHUNK_DELIMITER)
 
             # Reset the cache.
             self.cache = []
 
     def decompress(self):
         """
-        Decompresses the data at ``location``. A generator which ``yield``s
+        Decompresses the data at ``location``. A generator which ``yield`` s
         assignments.
 
         Yields:
             Decompressed assignment dictionaries.
         """
         # Open the compressed file. Then we read it in chunks, loading until
         # we hit our separator or until the end of the file.
```

### Comparing `gerrytools-1.1.1/gerrytools/data/URLs.py` & `gerrytools-1.2.0/gerrytools/data/URLs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/data/__init__.py` & `gerrytools-1.2.0/gerrytools/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Facilities for processing data and districting plans in a standardized fashion.
 """
+
 from .acs import acs5, cvap
 from .AssignmentCompressor import AssignmentCompressor
 from .census import census10, census20, variables
 from .estimatecvap import estimatecvap2010, estimatecvap2020, fetchgeometries
 from .fetch import Submission, submissions, tabularized
 from .geometries import geometries20
 from .remap import remap
```

### Comparing `gerrytools-1.1.1/gerrytools/data/acs.py` & `gerrytools-1.2.0/gerrytools/data/acs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/data/census.py` & `gerrytools-1.2.0/gerrytools/data/census.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/data/estimatecvap.py` & `gerrytools-1.2.0/gerrytools/data/estimatecvap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
+import warnings
 
 from ..geometry import unitmap
 from .acs import acs5, cvap
 from .census import census20
 
 
 def estimatecvap2020(state) -> pd.DataFrame:
     """
     Estimates 2020 CVAP on 2020 blocks using 2020 PL94 data. **This method
     serves a different purpose than `gerrytools.data.estimatecvap.
     estimatecvap2010()`:** rather than using geometric procedures to
     put CVAP data on old geometries, this method takes advantage of the
     Census's geographic hierarchy, and associates finer-grained 2020 CVAP
-    data with 2020 blocks. _No geometric data or procedures are used here_.
+    data with 2020 blocks. *No geometric data or procedures are used here*.
     The resulting data can then be adjoined to 2020 block geometries (or
     assigned to VTDs, assigned to districts, etc.) and be used to build
     other units of varying size.
 
     Args:
         state (State): The `us.State` for which CVAP will be estimated.
 
@@ -195,16 +196,16 @@
     group, users specify a triple \((X, Y, Z)\) where \(X\) is the old CVAP
     column for that group, \(Y\) is the old VAP column for that group, and
     \(Z\) is the new VAP column for that group, which must be an existing
     column on `base`. Then, the estimated new CVAP for that group will be
     constructed by multiplying \((X / Y) \cdot Z\) for each new geometry.
 
     <div style="text-align: center;">
-        </br>
-        <img width="75%" src="../images/cvap-estimation.png"/>
+    </br>
+    <img width="75%" src="../images/cvap-estimation.png"/>
     </div>
 
     Args:
         base (GeoDataFrame): A `GeoDataFrame` with the appropriate columns for
             estimating CVAP.
         state (State): The `us.State` object for which CVAP data is retrieved.
         groups (list): `(X, Y, Z)` triples for each desired CVAP group to be
@@ -309,17 +310,16 @@
     #   1.  if there are 0 *CVAP reported and 0 *VAP reported, we set the
     #        weight to the average *CVAP/*VAP ratio within the county;
     #   2.  if there are 0 *CVAP reported and *VAP > 0, we set the weight to
     #        zero_fill;
     #   3.  if *CVAP > 0 but *VAP = 0 or *CVAP/*VAP > percentage_cap, we set
     #       the weight to 1.
     statewide = {
-        cvap + "%": source[cvap].sum() / source[vap].sum()
-        if source[vap].sum() != 0
-        else 0
+        cvap
+        + "%": source[cvap].sum() / source[vap].sum() if source[vap].sum() != 0 else 0
         for (cvap, vap, _) in groups
     }
 
     # Rename colunms with percentages.
     cvappcts = [cvap + "%" for (cvap, _, _) in groups]
 
     # Get the county names and compute population-weighted CVAP averages. This
@@ -386,28 +386,35 @@
     assert all(np.all(source[p + "%"] > 0) for (p, _, __) in groups)
 
     # Set indices and create a mapping from IDs to weights.
     source = source.set_index(cvap_geoid)
     source = source[cvappcts]
     weights = source.to_dict(orient="index")
 
+    # If the first character of the first key is "0", then we need to pad
+    # the keys since ix gets interpreted as a float later.
+    if [*weights.keys()][0][0] == "0":
+        pad = "0"
+    else:
+        pad = ""
+
     # Group by the CVAP GEOID.
     groupedtogeometry = list(pared.groupby(cvap_geoid))
 
     # Get the year suffix so we can replace columns.
     yearsuffix = str(year)[2:]
 
     # For each of the geometry groups (e.g. a set of rows of blocks
     # corresponding to a single tract), and for each of the CVAP groups,
     # apply the appropriate weight to the blocks' 2020 VAP populations.
     for ix, group in groupedtogeometry:
         for cvap10, vap10, vap20 in groups:
             weight = cvap10 + "%"
             cvap20 = cvap10.replace(yearsuffix, "20_EST")
-            group[weight] = weights[ix][weight]
+            group[weight] = weights[pad + str(int(ix))][weight]
             group[cvap20] = group[weight] * group[vap20]
 
     # Re-create a dataframe and strip out % columns, leaving only the estimate
     # columns.
     weightedbase = pd.concat(frame for _, frame in groupedtogeometry)
     weightedbase = weightedbase.drop(columns=[p + "%" for (p, _, _) in groups])
     return weightedbase
```

### Comparing `gerrytools-1.1.1/gerrytools/data/fetch.py` & `gerrytools-1.2.0/gerrytools/data/fetch.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/data/geometries.py` & `gerrytools-1.2.0/gerrytools/data/geometries.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/data/remap.py` & `gerrytools-1.2.0/gerrytools/data/remap.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/__init__.py` & `gerrytools-1.2.0/gerrytools/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/compactness.py` & `gerrytools-1.2.0/gerrytools/geometry/compactness.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/dataframe.py` & `gerrytools-1.2.0/gerrytools/geometry/dataframe.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/dissolve.py` & `gerrytools-1.2.0/gerrytools/geometry/dissolve.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/dualgraph.py` & `gerrytools-1.2.0/gerrytools/geometry/dualgraph.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/optimize.py` & `gerrytools-1.2.0/gerrytools/geometry/optimize.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     crs=None,
 ) -> pd.DataFrame:
     r"""
     Given two GeoDataFrames, each encoding districting plans, computes the areal
     overlap between each pair of districts. `left` is the districting plan to be
     relabeled (e.g. a proposed districting plan) and `right` is the districting
     plan with district labels we're trying to match (e.g. an enacted districting
-    plan). If `left` (denoted \(L\)) has \(n\) districts and `right` (denoted \(R\)) has
-    \(m\) districts, an \(n \times m\) matrix \(C\) is computed, where the entry
-    \(M_{ij}\) represents the area of the intersection of the districts \(L_i\) and
-    \(R_j\). \(C\) is represented as a pandas DataFrame, where the row indices are
+    plan). If `left` (denoted :math:`L`) has :math:`n` districts and `right` (denoted :math:`R`) has
+    :math:`m` districts, an :math:`n \times m` matrix :math:`C` is computed, where the entry
+    :math:`M_{ij}` represents the area of the intersection of the districts :math:`L_i` and
+    :math:`R_j`. :math:`C` is represented as a pandas DataFrame, where the row indices are
     the labels in `left`, and are the preimage of the label mapping; column indices
     are the labels in `right`, and are the image of the label mapping.
 
     Args:
         left (pd.DataFrame): GeoDataFrame whose labels are the preimage of the
             relabeling.
         right (pd.DataFrame): GeoDataFrame whose labels are the image of the
             relabeling.
         assignment (str): Column on `left` and `right` which contains the district
             identifier.
 
     Returns:
-        Cost matrix \(C\), represented as a DataFrame.
+        Cost matrix :math:`C`, represented as a DataFrame.
     """
     # Force the two things to be the same CRS (or the provided CRS)
     if crs:
         left = left.to_crs(crs)
         right = right.to_crs(crs)
     else:
         right = right.to_crs(left.crs)
@@ -72,24 +72,24 @@
 def populationoverlap(
     left: pd.DataFrame,
     right: pd.DataFrame,
     identifier: str = "GEOID20",
     population: str = "TOTPOP20",
     assignment: str = "DISTRICT",
 ) -> pd.DataFrame:
-    r"""
+    """
     Given two unit-level DataFrames — i.e. two dataframes where each row represents
     an atomic unit like Census blocks or VTDs, and each row contains a district
     assignment — computes the amount of population shared by each pair of districts.
     `left` is the districting plan to be relabeled (e.g. a proposed districting
     plan) and `right` is the districting plan with district labels we're trying
-    to match (e.g. an enacted districting plan). If `left` (denoted \(L\)) has
-    \(n\) districts and `right` (denoted \(R\)) has \(m\) districts, an
-    \(n \times m\) matrix \(C\) is computed, where the entry \(M_{ij}\) represents
-    the population shared by the districts \(L_i\) and \(R_j\). \(C\) is
+    to match (e.g. an enacted districting plan). If `left` (denoted :math:`L`) has
+    :math:`n` districts and `right` (denoted :math:`R`) has :math:`m` districts, an
+    :math:`n \times m` matrix :math:`C` is computed, where the entry :math:`M_{ij}` represents
+    the population shared by the districts :math:`L_i` and :math:`R_j`. :math:`C` is
     represented as a pandas DataFrame, where the row indices are the labels in
     `left`, and are the preimage of the label mapping; column indices are the labels
     in `right`, and are the image of the label mapping.
 
     Args:
         left (pd.DataFrame): DataFrame whose labels are the preimage of the relabeling.
         right (pd.DataFrame): DataFrame whose labels are the image of the relabeling.
@@ -141,15 +141,15 @@
 
 def optimalrelabeling(
     left: Any,
     right: Any,
     maximize: bool = True,
     costmatrix: Callable = populationoverlap,
 ) -> dict:
-    r"""
+    """
     Finds the optimal relabeling for two districting plans.
 
     Args:
         left (Any): Data structure which can be passed to `costmatrix` to construct
             a cost matrix. District labels will be the preimage of the relabeling.
             If the default `costmatrix` function is used, these must be pandas
             DataFrames where one row corresponds to one atomic unit (e.g. Census
@@ -178,48 +178,41 @@
             `gerrytools.geometry.optimize.populationoverlap()` and
             `gerrytools.geometry.optimize.arealoverlap()`.
 
     Returns:
         A dictionary which maps district labels in `left` to district labels in
         `right`, according to the weighting scheme applied in `costmatrix`.
 
-    </br>
-
-    This is an [assignment problem](https://bit.ly/3wnyS4F)
-    and is equivalently a [(min/max)imal bipartite matching problem](http://bit.ly/2OfwUeh).
-    Consider two districting plans \(L\) and \(R\), with \(n\) and \(m\) districts
-    respectively. Set \(V_L\) and \(V_R\) to be sets of vertices such that
-    a vertex \(l_i\) in \(V_L\) corresponds to the district \(L_i\) in \(L\), and
-    similarly for vertices \(r_j\) in \(V_R\); draw edges \((l_i, r_j)\) for each
-    \(i\) from \(1\) to \(n,\) and each \(j\) from \(1\) to \(m.\) In doing so,
-    we construct the [bipartite graph](https://bit.ly/39rDldy) \(K_{n,m}\):
-
-    <div style="text-align: center;">
-        </br>
-        <img width="40%" src="../images/bipartite-matching.png"/>
-    </div>
+    This is an `assignment problem <https://bit.ly/3wnyS4F>`_
+    and is equivalently a `(min/max)imal bipartite matching problem <http://bit.ly/2OfwUeh>`_.
+    Consider two districting plans :math:`L` and :math:`R`, with :math:`n` and :math:`m` districts
+    respectively. Set :math:`V_L` and :math:`V_R` to be sets of vertices such that
+    a vertex :math:`l_i` in :math:`V_L` corresponds to the district :math:`L_i` in :math:`L`, and
+    similarly for vertices :math:`r_j` in :math:`V_R`; draw edges :math:`(l_i, r_j)` for each
+    :math:`i` from :math:`1` to :math:`n,` and each :math:`j` from :math:`1` to :math:`m.`
+    In doing so, we construct the `bipartite graph <https://bit.ly/39rDldy>` :math:`K_{n,m}`:
 
     We then assign each edge a weight according to some function
-    \(f: L\times R\ \to \mathbb{R}\), which consumes a pair of districts and returns
+    :math:`f: L\times R \to \\mathbb{R}`, which consumes a pair of districts and returns
     a number. For example, this function could be the amount of area shared by
-    the districts \(L_i\) and \(R_j\), like in `gerrytools.geometry.optimize.arealoverlap()`,
+    the districts :math:`L_i` and :math:`R_j`, like in
+    :func:`gerrytools.geometry.optimize.arealoverlap()`,
     or the amount of population the districts share, like in
-    `gerrytools.geometry.optimize.populationoverlap()`.
+    :func:`gerrytools.geometry.optimize.populationoverlap()`.
 
-    We then seek to find the set of weighted edges \(M\) such that all vertices
-    \(l_i\) and \(r_j\) appear at most once in \(M\), and that the sum of \(M\)'s
+    We then seek to find the set of weighted edges :math:`M` such that all vertices
+    :math:`l_i` and :math:`r_j` appear at most once in :math:`M`, and that the sum of :math:`M`'s
     weights is as small (or as large) as possible. To do so, we take the adjacency
-    matrix \(A\) of our graph \(K_{n,m}\), where the \(i, j\)th entry records
-    the weight of the edge \((l_i, r_j\)). Then, we want to select at most one entry
+    matrix :math:`A` of our graph :math:`K_{n,m}`, where the :math:`i, j`th entry records
+    the weight of the edge :math:`(l_i, r_j`). Then, we want to select at most one entry
     in each row and column, and ensure those entries have the smallest (or greatest)
-    possible sum. Using the [Jonker-Volgenant algorithm](DOI:10.1109/TAES.2016.140952) (as
+    possible sum. Using the `Jonker-Volgenant algorithm <DOI:10.1109/TAES.2016.140952>`_ (as
     implemented by scipy), we can find the row and column indices of these entries,
     and retrieve the district label pairs corresponding to each. The algorithm
-    achieves \(\textbf{O}(N^3)\) worst-case running time, where \(N = \max(n, m)\).
-
+    achieves :math:`\textbf{O}(N^3)` worst-case running time, where :math:`N = \\max(n, m)`.
     """
     # Our cost function should compute the weights between left and right. First,
     # we want to identify the indices of the preimage (row index) and column
     C = costmatrix(left, right)
     preimage, image = list(C.index), list(C)
 
     # Now we do our linear sum assignment, getting back the indices which maximize
```

### Comparing `gerrytools-1.1.1/gerrytools/geometry/unitmap.py` & `gerrytools-1.2.0/gerrytools/geometry/unitmap.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/geometry/updater.py` & `gerrytools-1.2.0/gerrytools/geometry/updater.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/__init__.py` & `gerrytools-1.2.0/gerrytools/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/annotation.py` & `gerrytools-1.2.0/gerrytools/plotting/annotation.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/bins.py` & `gerrytools-1.2.0/gerrytools/plotting/bins.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/boxplot.py` & `gerrytools-1.2.0/gerrytools/plotting/boxplot.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/choropleth.py` & `gerrytools-1.2.0/gerrytools/plotting/choropleth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.axes import Axes
+import geopandas as gpd
 
 from .colors import overlays as overlaycolors
 from .districtnumbers import districtnumbers
 
 
+# TODO: Update the docstring to include the new parameters.
 def choropleth(
     geometries,
     districts=None,
     assignment=None,
-    demographic="BVAP",
+    demographic_share_col=None,
     overlays=[],
     cmap="Purples",
     cbartitle=None,
-    numbers=True,
-    lw=1 / 8,
+    numbers=False,
+    base_lw=1 / 8,
+    base_linecolor="lightgray",
+    district_linecolor="black",
+    overlay_lw=1 / 4,
+    district_lw=3 / 2,
     fontsize=15,
     min=0,
     max=1,
     interval=1 / 10,
     colorbar=True,
+    figsize=(10, 10),
 ) -> Axes:
     r"""
     Visualization of population shares or totals in a state's map.
 
     Args:
         geometries (GeoDataFrame): Base geometries for the state. Population
             shares or totals will be drawn at this level (i.e. statistics are
             reported at this base geometric level).
         districts (GeoDataFrame, optional): Geometries for the districting plan.
             Assumes one geometry per district.
         assignment (str, optional): Required argument when `districts` are
             provided. Column of `districts` which defines the districing plan.
-        demographic (str, optional): The string representing the demographic to
+        demographic_share_col (str, optional): The string representing the demographic to
             be shown on the map. The string should specify a column in `geometries`.
             *This column must contain values in \\([0,1]\\).*
         overlays (list, optional): A list of GeoDataFrames desired to be overlaid on
             the map. Some options would include overlaying district assignments,
             blocks, VTDs, or counties. The first set of geometries in the list
             will be overlaid in the lightest color, and last will be overlaid in
             the darkest color.
@@ -58,19 +65,19 @@
         colorbar (bool, optional): Do we include the color bar?
 
     Returns:
         A matplotlib `Axes` object visualizing a choropleth map with the provided
         overlays.
     """
     # Get the figure and base axis sizes.
-    fig, base = plt.subplots(1, 1, figsize=(10, 10))
+    fig, base = plt.subplots(1, 1, figsize=figsize)
 
     # Get the title for the colorbar.
     if cbartitle is None:
-        cbartitle = demographic
+        cbartitle = demographic_share_col
 
     # Set minimum and maximum values.
     boundaries = np.arange(min, max + interval, interval)
     ticks = np.arange(min, max + interval, interval / 2)[:-1]
     labels = [
         f"{int(ticks[i-1]*100)} — {int(ticks[i+1]*100)}%" if i % 2 else ""
         for i in range(len(ticks))
@@ -82,19 +89,24 @@
         colorbarmap = plt.cm.get_cmap(cmap, len(boundaries))
     else:
         colorbarmap = cmap
 
     norm = mpl.colors.BoundaryNorm(boundaries, colorbarmap.N)
 
     # Plot geometries!
+    if assignment is not None:
+        geometries = geometries.dissolve(
+            by=assignment, aggfunc={demographic_share_col: "sum"}
+        )
+
     geometries.plot(
-        column=demographic,
+        column=demographic_share_col,
         cmap=cmap,
-        edgecolor="lightgray",
-        linewidth=lw,
+        edgecolor=base_linecolor,
+        linewidth=base_lw,
         vmin=min,
         vmax=max,
         ax=base,
     )
 
     # Create and plot the colorbar on the right side of the figure.
     if colorbar:
@@ -115,18 +127,22 @@
         geom = geom.to_crs(geometries.crs)
         geom.boundary.plot(
             edgecolor=overlaycolors[-(idx + 1)], linewidth=1 / 4, ax=base
         )
 
     # If district geometries are provided, plot them as well.
     if districts is not None:
-        districts.plot(edgecolor="black", linewidth=3 / 2, ax=base, color="None")
+        # if assignment is not None:
+        #     districts = districts.dissolve(by=assignment).reset_index()
+        districts.plot(
+            edgecolor=district_linecolor, linewidth=district_lw, ax=base, color="None"
+        )
 
     # If district numbers are to be plotted, plot those too!
-    if numbers:
+    if numbers and assignment:
         base = districtnumbers(
             base, districts, assignment=assignment, fontsize=fontsize
         )
 
     # Turn plot vertical/horizontal axes off and return base Axes.
     base.set_axis_off()
```

### Comparing `gerrytools-1.1.1/gerrytools/plotting/colors.py` & `gerrytools-1.2.0/gerrytools/plotting/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     tail = [hexshift(c) for c in colors * (repeats - 1)]
     return (colors + (tail if tail else []))[:N]
 
 
 def redbluecmap(n) -> List[Tuple]:
     """
     Generates a red/white/blue color palette in `n` colors with white at the
-    `mid`th index.
+    `mid` th index.
 
     Args:
         n (int): The number of colors to generate.
 
     Returns:
         List of RGB tuples.
     """
```

### Comparing `gerrytools-1.1.1/gerrytools/plotting/districtnumbers.py` & `gerrytools-1.2.0/gerrytools/plotting/districtnumbers.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/drawgraph.py` & `gerrytools-1.2.0/gerrytools/plotting/drawgraph.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/drawplan.py` & `gerrytools-1.2.0/gerrytools/plotting/drawplan.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,21 +32,20 @@
             `districtnumbers`.
 
     Returns:
         A `matplotlib` `Axes` object for the geometries attached to `districts`.
     """
     # Sort districts by their assignment and add a column specifying the color
     # index.
+    districts = districts.dissolve(by=assignment).reset_index()
     N = len(districts)
     districts = districts.to_crs("epsg:3857")
     districts[assignment] = districts[assignment].astype(int)
     districts = districts.sort_values(by=assignment)
     if colors is None:
-        districts["colorindex"] = list(range(N))
-
         # Assign colors.
         districts["color"] = districtr(N)
 
     # Plot the districts.
     base = districts.plot(
         color=districts[colors if colors else "color"],
         edgecolor="black",
```

### Comparing `gerrytools-1.1.1/gerrytools/plotting/gifs.py` & `gerrytools-1.2.0/gerrytools/plotting/gifs.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/histogram.py` & `gerrytools-1.2.0/gerrytools/plotting/histogram.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import random
 
 from matplotlib.axes import Axes
+import numpy as np
 
 from .bins import bins
 from .colors import citizenBlue, defaultGray, districtr
 
 
 def histogram(
     ax,
@@ -96,7 +97,62 @@
         ax.legend()
     if label:
         ax.set_xlabel(label, fontsize=fontsize)
     ax.get_yaxis().set_visible(False)
     if limits:
         ax.set_xlim(limits)
     return ax
+
+
+# def histogram(
+#     ax,
+#     scores,
+#     label=None,
+#     limits=(),
+# 	proposed_info={},
+# 	ticksize=12,
+# 	fontsize=24,
+# 	jitter=False,
+#     bin_width=None
+# ):
+#     """Refactored histogram plotting function."""
+
+#     def calculate_bins(scores, bin_width=None):
+#         """Calculate histogram bins, tick positions, and labels."""
+#         score_values = np.array(list(scores))
+#         if bin_width is None:
+#             bin_width = np.ptp(score_values) / 30  # Default heuristic
+#         bins = np.arange(score_values.min(), score_values.max() + bin_width, bin_width)
+#         tick_bins = bins[:-1] + bin_width / 2
+#         tick_labels = [f"{tick:.2f}" for tick in tick_bins]
+#         return bins, tick_bins, tick_labels, bin_width
+
+#     all_scores = np.concatenate([scores[k] for k in ['ensemble', 'citizen', 'proposed']])
+#     hist_bins, tick_bins, tick_labels, bin_width = calculate_bins(all_scores, bin_width)
+
+#     # Set ticks
+#     ax.set_xticks(tick_bins)
+#     ax.set_xticklabels(tick_labels, fontsize=ticksize)
+
+#     # Visual adjustments
+#     unique_scores = len(set(all_scores))
+#     rwidth = 0.8 if unique_scores < 20 else 1
+#     edgecolor = "black" if unique_scores < 20 else "white"
+#     alpha = 0.7 if scores.get("ensemble") and scores.get("citizen") else 1
+
+#     # Plot histograms for ensemble and citizen
+#     for kind, color in [("ensemble", "gray"), ("citizen", "#377eb8")]:
+#         if scores.get(kind):
+#             ax.hist(scores[kind], bins=hist_bins, color=color, rwidth=rwidth, edgecolor=edgecolor, alpha=alpha, density=True)
+
+#     # Plot proposed scores
+#     if scores.get("proposed"):
+#         for i, s in enumerate(scores["proposed"]):
+#             jitter_val = random.uniform(-bin_width / 4, bin_width / 4) if jitter and scores["proposed"].count(s) > 1 else 0
+#             ax.axvline(s + jitter_val, color=proposed_info['colors'][i], lw=2, label=f"{proposed_info['names'][i]}: {round(s, 2)}")
+
+#     ax.legend() if scores.get("proposed") else None
+#     ax.set_xlabel(label, fontsize=fontsize) if label else None
+#     ax.get_yaxis().set_visible(False)
+#     ax.set_xlim(limits) if limits else None
+
+#     return ax
```

### Comparing `gerrytools-1.1.1/gerrytools/plotting/latexcolors.json` & `gerrytools-1.2.0/gerrytools/plotting/latexcolors.json`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/multidimensional.py` & `gerrytools-1.2.0/gerrytools/plotting/multidimensional.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/sealevel.py` & `gerrytools-1.2.0/gerrytools/plotting/sealevel.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/plotting/violin.py` & `gerrytools-1.2.0/gerrytools/plotting/violin.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     (ensemble or citizen), and trim each sublist to only the values between the percentiles.
 
     Args:
         ax (Axes): `Axes` object on which the violins are plotted.
         scores (dict): Dictionary with keys of `ensemble`, `citizen`, `proposed`
             which map to lists of numerical scores.
         proposed_info (dict, optional): Dictionary with keys of `colors`, `names`;
-            the \(i\)th color in `color` corresponds to the \(i\)th name in `names.
+            the \(i\)th color in `color` corresponds to the \(i\)th name in `names`.
         percentiles (tuple, optional): Observations outside this range of
             percentiles are ignored. Defaults to `(1, 99)`, such that observations
             between the 1st and 99th percentiles (inclusive) are included, and
             all others are ignored.
         rotation (float, optional): Tick labels are rotated `rotation` degrees
             _counterclockwise_.
         ticksize (float, optional): Font size for tick labels.
@@ -91,17 +91,20 @@
                     random.uniform(-jitter, jitter)
                     if scores["proposed"][violin].count(score) > 1
                     else 0
                 )
                 ax.scatter(
                     violin + 1 + jitter_val,
                     score,
-                    color=scores["proposed"]["colors"][violin]
-                    if scores["proposed"]["colors"]
-                    else districtr(plan + 1).pop(),
+                    color=(
+                        scores["proposed"]["colors"][violin]
+                        if not isinstance(scores["proposed"], list)
+                        and scores["proposed"]["colors"]
+                        else districtr(plan + 1).pop()
+                    ),
                     edgecolor="black",
                     s=100,
                     alpha=0.9,
                     label=proposed_info["names"][plan] if violin == 0 else None,
                 )
         ax.legend()
         ax.grid(axis="x")
```

### Comparing `gerrytools-1.1.1/gerrytools/scoring/__init__.py` & `gerrytools-1.2.0/gerrytools/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/contiguity.py` & `gerrytools-1.2.0/gerrytools/scoring/contiguity.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/demographics.py` & `gerrytools-1.2.0/gerrytools/scoring/demographics.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/partisan.py` & `gerrytools-1.2.0/gerrytools/scoring/partisan.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/population.py` & `gerrytools-1.2.0/gerrytools/scoring/population.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/scores.py` & `gerrytools-1.2.0/gerrytools/scoring/scores.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,16 @@
         if verbose:
             result = []
             for part in tqdm(parts):
                 result.append(summarize(part, scores=scores, gdf=gdf, join_on=join_on))
             return result
         return [summarize(part, scores=scores) for part in parts]
     else:
-        with gzip.open(f"{output_file}.gz", "wt") if compress else open(
-            output_file, "w"
+        with (
+            gzip.open(f"{output_file}.gz", "wt") if compress else open(output_file, "w")
         ) as fout:
             iterator = tqdm(enumerate(parts)) if verbose else enumerate(parts)
             for i, part in iterator:
                 plan_details = summarize(part, scores=scores, gdf=gdf, join_on=join_on)
                 try:
                     plan_details["id"] = plan_names[i]
                 except BaseException:
@@ -208,16 +208,16 @@
 ) -> Score:
     """
     Score representing the number of "unit pieces" produced by the plan. For example,
     consider a state with 100 counties. Suppose that one county is split twice,
     and another once. Then, there are 3 + 2 = 5 "pieces," disregarding the
     counties kept whole.
 
-    Bear in mind that this calculates the number of _unit splits_, not the number
-    of _units split_: for example, if a district divides a county into three
+    Bear in mind that this calculates the number of *unit splits*, not the number
+    of *units split*: for example, if a district divides a county into three
     pieces, the former reports two splits (as a unit divided into three pieces is
     cut twice), while the latter would report one split (as there is one county
     being split).
 
     Args:
         unit (str): Data column; each assigns a vertex to a unit.
             Generally, these units are counties, VTDs, precincts, etc.
@@ -448,15 +448,15 @@
     """
     Score representing the efficiency gap metric of a plan with respect to a set of elections.
 
     Args:
         election_cols (Iterable[str]): The names of the election updaters over which to compute
             results for.
         mean (bool): Whether to return the mean of the score over all elections, or a dictionary
-                     of the score for each election.
+            of the score for each election.
 
     Returns:
         A score object with name `"efficiency_gap"`  and associated function that takes a partition
         and returns a PlanWideScoreValue for efficiency gap metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
@@ -469,20 +469,22 @@
     election_cols: Iterable[str], party: str, mean: bool = False
 ) -> Score:
     """
     Score representing the simplified efficiency gap metric of a plan with respect to a set of elections.
     The original formulation of efficiency gap quantifies the difference in "wasted" votes for the two
     parties across the state, as a share of votes cast. This is sensitive to turnout effects. The
     simplified score is equal to standard efficiency gap when the districts have equal turnout.
+
     Args:
         election_cols (Iterable[str]): The names of the election updaters over which to compute
             results for.
         party (str): The "point of view" political party.
         mean (bool): Whether to return the mean of the score over all elections, or a dictionary
-                     of the score for each election.
+            of the score for each election.
+
     Returns:
         A score object with name `"efficiency_gap"`  and associated function that takes a partition
         and returns a PlanWideScoreValue for efficiency gap metric.
     """
     prefix = "mean_" if mean else ""
     return Score(
         f"{prefix}simplified_efficiency_gap",
```

### Comparing `gerrytools-1.1.1/gerrytools/scoring/splits.py` & `gerrytools-1.2.0/gerrytools/scoring/splits.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/scoring/types.py` & `gerrytools-1.2.0/gerrytools/scoring/types.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools/utilities/JSON.py` & `gerrytools-1.2.0/gerrytools/utilities/JSON.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from typing import Any
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 
 class JSONtoObject(BaseModel):
     """
     Plan specification models. To better work with multiple plans at once, this
     plan specification allows users to specify information which should remain
     consistent across all operations; for example, the `column` field should be
@@ -31,15 +31,15 @@
     """
 
     type: str = None
     """
     The "type" of plan; could denote a party affiliation, a chamber, whatever.
     """
 
-    @validator("column")
+    @field_validator("column")
     def _validate_column(cls, column):
         """
         Validates the specified column name. For most of our purposes, we cannot
         include spaces, hyphens, percent signs, and other commonly-used special
         characters. Furthermore, because these plans are often saved in
         shapefiles, which have a 10-character column name limit, we force column
         names to be 10 or fewer characters.
```

### Comparing `gerrytools-1.1.1/gerrytools/utilities/rename.py` & `gerrytools-1.2.0/gerrytools/utilities/rename.py`

 * *Files identical despite different names*

### Comparing `gerrytools-1.1.1/gerrytools.egg-info/PKG-INFO` & `gerrytools-1.2.0/gerrytools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,107 @@
 Metadata-Version: 2.1
 Name: gerrytools
-Version: 1.1.1
+Version: 1.2.0
 Summary: Tools for processing and visualizing districting plans.
 Home-page: https://github.com/mggg/gerrytools
 Author: MGGG Redistricting Lab
 Author-email: engineering@mggg.org
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: mgrp
 License-File: LICENSE
 
 
 # gerrytools
-[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) [![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) [![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) [![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) [![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+
+[![CircleCI](https://dl.circleci.com/status-badge/img/gh/mggg/gerrytools/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/mggg/gerrytools/tree/main) 
+[![codecov](https://codecov.io/gh/mggg/gerrytools/branch/main/graph/badge.svg?token=O09GYF7C9X)](https://codecov.io/gh/mggg/gerrytools) 
+[![PyPI version](https://badge.fury.io/py/gerrytools.svg)](https://badge.fury.io/py/gerrytools) 
+[![docs](https://img.shields.io/badge/%E2%93%98-Documentation-%230099cd)](https://mggg.github.io/gerrytools/) 
+[![website](https://img.shields.io/badge/%F0%9F%8C%90%20-MGGG%20Redistricting%20Lab-%230099cd)](https://mggg.org) 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) 
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 
 A companion to [GerryChain](https://github.com/mggg/GerryChain), GerryTools is
 a robust suite of geometric and algorithmic tools to analyze districting plans
 and related data. GerryTools is actively developed and used by the
 [MGGG Redistricting Lab](https://mggg.org) and our collaborators to prepare
 accurate, precise, and clean information for our projects. It is distributed
 under a [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause).
 
 
 ## Installation
+
 ### Using `pip` (recommended)
+
 To install GerryTools from [PyPi](https://pypi.org/project/gerrytools/), run
 
+```console
+pip install gerrytools
 ```
-$ pip install gerrytools
+
+from the command line. if you would like to use the `mgrp` and `ben` modules as well,
+you can invoke 
+
+```console
+pip install gerrytools[mgrp]
 ```
 
-from the command line.
+you will need to make sure that [Docker Desktop](https://www.docker.com/get-started/)
+is installed on your machine an updated to version >= 4.28.0. For more information on
+getting this set up, please see 
+[our documentation page](https://gerrytools.readthedocs.io/en/latest/topics/docker/)
 
 ## Usage
-### Contents
+
 GerryTools is split up into multiple sub-packages, each designed to simplify and
 standardize redistricting workflows.
 
-* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you
-can find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20),
-ACS CVAP Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric
-data. You can also find tools for moving CVAP data to other levels of geometry (e.g. prorating 2019 CVAP on 2019 Census tracts to 2020 blocks).
-* **`gerrytools.geometry`** provides facilities for dealing with geometric and
-related data. There are tools for translating and evaluating GerryChain
-[`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to 2020 VTDs), creating
-[dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs), and optimization algorithms for renaming districts.
-* **`gerrytools.plotting`** contains methods for generating extremely high-quality 
-Lab-standard data visualizations.
-* **`gerrytools.scoring`** provides a vast array of redistricting plan scores. These
-can be used standalone _or_ as GerryChain
-[updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
-* **`gerrychain.utilities`** has ease-of-use methods for renaming directories
-containing shapefiles (which comes in handy more often than you'd think) and making
-JSON objects out of Python objects (useful when trying to organize information
-for many districting plans in a standard format).
+* **`gerrytools.ben`** BEN (binary-ensemble) is our general purpose compression
+    algorithm for working with ensembles of plans. In general, the ben algorithm can
+    improve the storage of an ensemble of plans by an order of magnitude. When combined
+    with the special XBEN (eXtreme BEN) portion of the algorithm, many ensembles of
+    plans can be compressed small enough to fit into an email (~25Mb).
+
+* **`gerrytools.data`** deals with the retrieval and processing of data. Here, you can
+    find tools for grabbing decennial Census ('10 and '20), ACS 5-year ('12-'20), ACS CVAP
+    Special Tab ('12-'20), districtr portal, and 2020 decennial Census geometric data. You
+    can also find tools for moving CVAP data to other levels of geometry (e.g. prorating
+    2019 CVAP on 2019 Census tracts to 2020 blocks).
+
+* **`gerrytools.geometry`** provides facilities for dealing with geometric and related
+    data. There are tools for translating and evaluating GerryChain
+    [`Partition`](https://mggg.github.io/GerryChain/api.html#module-gerrychain.partition)s, 
+    performing fast geometric dissolutions, creating unit maps (e.g. 2020 blocks to
+    2020 VTDs), creating 
+    [dual graphs for GerryChain](https://mggg.github.io/GerryChain/api.html#adjacency-graphs),
+    and optimization algorithms for renaming districts.
+
+* **`gerrytools.mgrp`** this module uses a Docker container to allow users to access several
+    ensemble methods for generating districting plans on a state. In particular our Rust
+    implementation of our `gerrychain` library, `frcw`, the Julia implementation of 
+    [Forest Recom](https://arxiv.org/pdf/2008.08054.pdf), and the R/C++ implementation of
+    [Sequential Monte Carlo (SMC)](https://github.com/alarm-redist/redist) are available
+    through this module. 
+
+* **`gerrytools.plotting`** contains methods for generating extremely
+    high-quality Lab-standard data visualizations.
+
+* **`gerrytools.scoring`** provides a vast array of redistricting plan scores.
+    These can be used standalone _or_ as GerryChain 
+    [updaters](https://mggg.github.io/GerryChain/api.html#module-gerrychain.updaters).
+
+* **`gerrychain.utilities`** has ease-of-use methods for renaming
+    directories containing shapefiles (which comes in handy more often than you'd
+    think) and making JSON objects out of Python objects (useful when trying to
+    organize information for many districting plans in a standard format).
+
+<!-- ### Example
 
-### Example
 GerryTools is easy to use and is designed to simplify data- and redistricting-related
 workflows. For example, let's say we want to analyze Alabama's citizen voting-age
 population data on 2020 Census tracts. First, we can download the geometric data
 for the state using `gerrytools.data.geometry20()`:
 
 ```python
 from gerrytools.data import geometry20
@@ -93,26 +135,31 @@
 
 # Merge. Note that the DataFrames have different unique identifier columns --- this
 # is intentional, and serves to differentiate datasets of varying geometric levels.
 merged = geometric.merge(demographic, left_on="GEOID20", right_on="TRACT20")
 ```
 
 And there we are — what once took hours of setup and parsing now takes less than a
-minute.
+minute. -->
 
 ## Contributing
+
 GerryTools is an active project, and has multiple contributors. If you'd like to
 contribute, here are a few house rules:
 
 1. After cloning this repository, run `sh setup.sh` to download and install
 necessary git hooks and linting configurations.
+
 2. **Follow the [PEP8 style guide](https://peps.python.org/pep-0008/)**. After
 installing the above git hooks, linting is performed before every push. PEP8 errors can be automatically corrected by running `autopep8 --in-place --aggressive -r gerrytools` on the command line from the root directory.
+
 3. **Write tests.** All changes, major or minor, **must** be accompanied by testing
 code. Code and tests will be immediately reviewed by Lab maintainers.
+
 4. Test coverage must stay **at least** the same; this can be checked by running
 `pytest --cov=evaltools` after the tests are added to `tests/`.
+
 5. **Write documentation.** All changes should be documented via docstrings,
 and code should be repletely commented. It's much easier to decipher commented
 code! Docstring documentation is compiled on every commit via git hooks.
 
 We look forward to your contributions!
```

### Comparing `gerrytools-1.1.1/gerrytools.egg-info/SOURCES.txt` & `gerrytools-1.2.0/gerrytools.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 setup.py
 gerrytools/__init__.py
 gerrytools.egg-info/PKG-INFO
 gerrytools.egg-info/SOURCES.txt
 gerrytools.egg-info/dependency_links.txt
 gerrytools.egg-info/requires.txt
 gerrytools.egg-info/top_level.txt
+gerrytools/ben/__init__.py
+gerrytools/ben/binary_ensemble.py
+gerrytools/ben/docker_manager.py
+gerrytools/ben/parse.py
+gerrytools/ben/reben.py
 gerrytools/data/AssignmentCompressor.py
 gerrytools/data/URLs.py
 gerrytools/data/__init__.py
 gerrytools/data/acs.py
 gerrytools/data/census.py
 gerrytools/data/estimatecvap.py
 gerrytools/data/fetch.py
@@ -21,14 +26,20 @@
 gerrytools/geometry/compactness.py
 gerrytools/geometry/dataframe.py
 gerrytools/geometry/dissolve.py
 gerrytools/geometry/dualgraph.py
 gerrytools/geometry/optimize.py
 gerrytools/geometry/unitmap.py
 gerrytools/geometry/updater.py
+gerrytools/mgrp/__init__.py
+gerrytools/mgrp/run_container.py
+gerrytools/mgrp/runners/__init__.py
+gerrytools/mgrp/runners/forest.py
+gerrytools/mgrp/runners/recom.py
+gerrytools/mgrp/runners/smc.py
 gerrytools/plotting/__init__.py
 gerrytools/plotting/annotation.py
 gerrytools/plotting/bins.py
 gerrytools/plotting/boxplot.py
 gerrytools/plotting/choropleth.py
 gerrytools/plotting/colors.py
 gerrytools/plotting/districtnumbers.py
@@ -48,12 +59,8 @@
 gerrytools/scoring/partisan.py
 gerrytools/scoring/population.py
 gerrytools/scoring/scores.py
 gerrytools/scoring/splits.py
 gerrytools/scoring/types.py
 gerrytools/utilities/JSON.py
 gerrytools/utilities/__init__.py
-gerrytools/utilities/rename.py
-tests/test_data.py
-tests/test_geometry.py
-tests/test_plotting.py
-tests/test_scoring.py
+gerrytools/utilities/rename.py
```

### Comparing `gerrytools-1.1.1/setup.py` & `gerrytools-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 requirements = [
-    "pandas",
+    "pandas<2.0.0,>=1.5.0",
     "scipy",
     "networkx",
     "geopandas",
-    "shapely",
+    "Shapely>=2.0.0",
     "matplotlib",
     "gerrychain",
     "sortedcontainers",
     "jsonlines",
     "opencv-python-headless",
     "imageio",
     "us",
     "pydantic",
     "censusdata",
     "seaborn",
-    "maup",
+    "maup<=1.1.0",
 ]
 
 # Set the version --- ensure that the latest tag matches this value.
-VERSION = "1.1.1"
+VERSION = "1.2.0"
 
 # Description.
 here = Path(__file__).parent
 DESCRIPTION = (here / "README.md").read_text()
 
 setup(
     name="gerrytools",
@@ -36,9 +36,20 @@
     description="Tools for processing and visualizing districting plans.",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mggg/gerrytools",
     packages=find_packages(exclude=["tests", "tutorials"]),
     install_requires=requirements,
     include_package_data=True,
-    extras_require={"dev": ["pdoc3", "flake8", "pytest", "autopep8", "pytest-cov", "black", "isort"]},
+    extras_require={
+        "dev": [
+            "pdoc3",
+            "flake8",
+            "pytest",
+            "autopep8",
+            "pytest-cov",
+            "black",
+            "isort",
+        ],
+        "mgrp": ["docker>=7.0.0"],
+    },
 )
```

