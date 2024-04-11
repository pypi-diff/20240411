# Comparing `tmp/brainglobe-utils-0.4.2.tar.gz` & `tmp/brainglobe-utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-utils-0.4.2.tar", last modified: Mon Mar 25 11:21:42 2024, max compression
+gzip compressed data, was "brainglobe-utils-0.4.3.tar", last modified: Thu Apr 11 15:26:48 2024, max compression
```

## Comparing `brainglobe-utils-0.4.2.tar` & `brainglobe-utils-0.4.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.418584 brainglobe-utils-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.402583 brainglobe-utils-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.406584 brainglobe-utils-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-25 11:21:42.414584 brainglobe-utils-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.406584 brainglobe-utils-0.4.2/brainglobe_utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.406584 brainglobe-utils-0.4.2/brainglobe_utils/IO/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/IO/cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/IO/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/IO/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.406584 brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.406584 brainglobe-utils-0.4.2/brainglobe_utils/brainreg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/brainreg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/brainreg/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.410584 brainglobe-utils-0.4.2/brainglobe_utils/cells/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/cells/cells.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.410584 brainglobe-utils-0.4.2/brainglobe_utils/citation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/bibtex_fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/citation/text_fmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.410584 brainglobe-utils-0.4.2/brainglobe_utils/general/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/string.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/general/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.410584 brainglobe-utils-0.4.2/brainglobe_utils/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.414584 brainglobe-utils-0.4.2/brainglobe_utils/image_io/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image_io/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image_io/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/image_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.414584 brainglobe-utils-0.4.2/brainglobe_utils/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/pandas/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.414584 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/brainglobe.png
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/collapsible_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/brainglobe_utils/qtpy/logo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:21:42.414584 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-25 11:21:42.000000 brainglobe-utils-0.4.2/brainglobe_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-03-25 11:21:38.000000 brainglobe-utils-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:21:42.418584 brainglobe-utils-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.120339 brainglobe-utils-0.4.3/brainglobe_utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/IO/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12867 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/IO/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/brainreg/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/cells/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/cells/cells.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.124339 brainglobe-utils-0.4.3/brainglobe_utils/citation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/bibtex_fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/cite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10639 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/citation/text_fmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/general/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/image_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20135 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/image_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/pandas/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/brainglobe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/collapsible_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/brainglobe_utils/qtpy/logo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:26:48.128339 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:26:48.000000 brainglobe-utils-0.4.3/brainglobe_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-11 15:26:43.000000 brainglobe-utils-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:26:48.132340 brainglobe-utils-0.4.3/setup.cfg
```

### Comparing `brainglobe-utils-0.4.2/.github/workflows/test_and_deploy.yml` & `brainglobe-utils-0.4.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/.gitignore` & `brainglobe-utils-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/LICENSE` & `brainglobe-utils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/PKG-INFO` & `brainglobe-utils-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Tyson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `brainglobe-utils-0.4.2/README.md` & `brainglobe-utils-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/analysis.py` & `brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/analysis.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/brainmapper/export.py` & `brainglobe-utils-0.4.3/brainglobe_utils/brainmapper/export.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/brainreg/transform.py` & `brainglobe-utils-0.4.3/brainglobe_utils/brainreg/transform.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/bibtex_fmt.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/bibtex_fmt.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/cite.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/cite.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/fetch.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/fetch.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/format.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/format.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/repositories.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/repositories.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/citation/text_fmt.py` & `brainglobe-utils-0.4.3/brainglobe_utils/citation/text_fmt.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/general/list.py` & `brainglobe-utils-0.4.3/brainglobe_utils/general/list.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/general/numerical.py` & `brainglobe-utils-0.4.3/brainglobe_utils/general/numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/general/system.py` & `brainglobe-utils-0.4.3/brainglobe_utils/general/system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/image/heatmap.py` & `brainglobe-utils-0.4.3/brainglobe_utils/image/heatmap.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/image/scale.py` & `brainglobe-utils-0.4.3/brainglobe_utils/image/scale.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,38 @@
 import numpy as np
 
 
 def scale_to_16_bits(img):
     """
     Normalise the input image to the full 0-2^16 bit depth.
 
-    :param np.array img: The input image
-    :return: The normalised image
-    :rtype: np.array
+    Parameters
+    ----------
+    img : np.ndarray
+        The input image
+
+    Returns
+    -------
+    np.ndarray
+        The normalised image
     """
     normalised = img / img.max()
     return normalised * (2**16 - 1)
 
 
 def scale_and_convert_to_16_bits(img):
     """
     Normalise the input image to the full 0-2^16 bit depth, and return as
     type: "np.uint16".
 
-    :param np.array img: The input image
-    :return: The normalised, 16 bit image
-    :rtype: np.array
+    Parameters
+    ----------
+    img : np.ndarray
+        The input image
+
+    Returns
+    -------
+    np.ndarray
+        The normalised, 16 bit image
     """
     img = scale_to_16_bits(img)
     return img.astype(np.uint16, copy=False)
```

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/image_io/load.py` & `brainglobe-utils-0.4.3/brainglobe_utils/image_io/load.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/image_io/save.py` & `brainglobe-utils-0.4.3/brainglobe_utils/image_io/save.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/image_io/utils.py` & `brainglobe-utils-0.4.3/brainglobe_utils/image_io/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/pandas/misc.py` & `brainglobe-utils-0.4.3/brainglobe_utils/pandas/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,69 @@
 import numpy as np
 import pandas as pd
 
 
 def initialise_df(*column_names):
     """
-    Initialise a pandasdataframe with n column names
-    :param str column_names: N column names
-    :return: Empty pandas dataframe with specified column names
+    Initialise a pandas dataframe with n column names.
+
+    Parameters
+    ----------
+    *column_names : str
+        N column names
+
+    Returns
+    -------
+    pd.DataFrame
+        Empty pandas dataframe with specified column names
     """
     return pd.DataFrame(columns=column_names)
 
 
 def sanitise_df(df):
     """
-    Replaces infinite values in a dataframe with NaN
-    :param df: Any dataframe
-    :return: Dataframe with Inf replaced with NaN
+    Replaces infinite values in a dataframe with NaN.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Any dataframe
+
+    Returns
+    -------
+    pd.DataFrame
+        Dataframe with Inf replaced with NaN.
     """
     df = df.replace(np.inf, np.nan)
     return df
 
 
 def safe_pandas_concat(df1: pd.DataFrame, df2: pd.DataFrame) -> pd.DataFrame:
     """
     Concatenate two DataFrames without relying on deprecated functionality
     when one of the DataFrames is empty.
-    If df1 and df2 are non-empty, return the concatenation.
+
+    If df1 and df2 are non-empty, return the concatenation. df2 will extend df1
+    in the resulting DataFrame.
     If df1 is empty and df2 is not, return a copy of df2.
     If df1 is non-empty and df2 is, return a copy of df1.
     If df1 and df2 are empty, return an empty DataFrame with the same column
     names as df1.
-    :param df1: DataFrame to concatenate.
-    :param df2: DataFrame to concatenate.
-    :returns: DataFrame formed from concatenation of df1 and df2.
+
+    Parameters
+    ----------
+    df1 : pd.DataFrame
+        DataFrame to concatenate.
+    df2 : pd.DataFrame
+        DataFrame to concatenate.
+
+    Returns
+    -------
+    pd.DataFrame
+        DataFrame formed from concatenation of df1 and df2.
     """
     if df1.empty and df2.empty:
         return pd.DataFrame(columns=df1.columns)
     elif df1.empty:
         return df2.copy()
     elif df2.empty:
         return df1.copy()
```

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/qtpy/brainglobe.png` & `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/brainglobe.png`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/qtpy/collapsible_widget.py` & `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/qtpy/dialog.py` & `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     )
     if message_reply == QMessageBox.Yes:
         return True
     else:
         return False
 
 
-def display_info(widget, title, message):
+def display_info(widget: QWidget, title: str, message: str):
     """
     Display information in a pop-up that can only be accepted
     """
     QMessageBox.information(
         widget,
         title,
         message,
```

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils/qtpy/interaction.py` & `brainglobe-utils-0.4.3/brainglobe_utils/qtpy/interaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,58 +42,72 @@
 
     layout.addWidget(button, row, column)
     button.clicked.connect(connected_function)
     return button
 
 
 def add_checkbox(
-    layout, default, label, row: int = 0, column: int = 0, tooltip=None
-):
+    layout: QLayout,
+    default: bool,
+    label: str,
+    row: int = 0,
+    column: int = 0,
+    tooltip: Optional[str] = None,
+) -> QCheckBox:
+    """
+    Add a checkbox to *layout*.
+    """
     box = QCheckBox()
     box.setChecked(default)
     if tooltip:
         box.setToolTip(tooltip)
     layout.addWidget(QLabel(label), row, column)
     layout.addWidget(box, row, column + 1)
     return box
 
 
 def add_float_box(
-    layout,
-    default,
-    minimum,
-    maximum,
-    label,
-    step,
+    layout: QLayout,
+    default: float,
+    minimum: float,
+    maximum: float,
+    label: str,
+    step: float,
     row: int = 0,
     column: int = 0,
-    tooltip=None,
-):
+    tooltip: Optional[str] = None,
+) -> QDoubleSpinBox:
+    """
+    Add a spin box for float values to *layout*.
+    """
     box = QDoubleSpinBox()
     box.setMinimum(minimum)
     box.setMaximum(maximum)
     box.setValue(default)
     box.setSingleStep(step)
     if tooltip:
         box.setToolTip(tooltip)
     layout.addWidget(QLabel(label), row, column)
     layout.addWidget(box, row, column + 1)
     return box
 
 
 def add_int_box(
-    layout,
-    default,
-    minimum,
-    maximum,
-    label,
+    layout: QLayout,
+    default: int,
+    minimum: int,
+    maximum: int,
+    label: str,
     row: int = 0,
     column: int = 0,
-    tooltip=None,
-):
+    tooltip: Optional[str] = None,
+) -> QSpinBox:
+    """
+    Add a spin box for integer values to *layout*.
+    """
     box = QSpinBox()
     box.setMinimum(minimum)
     box.setMaximum(maximum)
     # Not always set if not after min & max
     box.setValue(default)
     if tooltip:
         box.setToolTip(tooltip)
@@ -105,15 +119,15 @@
 def add_combobox(
     layout: QLayout,
     label: str,
     items: List[str],
     row: int = 0,
     column: int = 0,
     label_stack: bool = False,
-    callback=None,
+    callback: Optional[Callable] = None,
     width: int = 150,
 ) -> Tuple[QComboBox, Optional[QLabel]]:
     """
     Add a selection box to *layout*.
     """
     if label_stack:
         combobox_row = row + 1
```

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils.egg-info/PKG-INFO` & `brainglobe-utils-0.4.3/brainglobe_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Tyson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `brainglobe-utils-0.4.2/brainglobe_utils.egg-info/SOURCES.txt` & `brainglobe-utils-0.4.3/brainglobe_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.4.2/pyproject.toml` & `brainglobe-utils-0.4.3/pyproject.toml`

 * *Files identical despite different names*

