# Comparing `tmp/rrcgeoviz-0.1.3.tar.gz` & `tmp/rrcgeoviz-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrcgeoviz-0.1.3.tar", last modified: Tue Apr  9 06:29:23 2024, max compression
+gzip compressed data, was "rrcgeoviz-0.1.4.tar", last modified: Thu Apr 11 16:44:00 2024, max compression
```

## Comparing `rrcgeoviz-0.1.3.tar` & `rrcgeoviz-0.1.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/rrcgeoviz/
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/GeneratedData.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/GeoVizPanelDashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.758123 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorExample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorPOI.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.762124 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/
--rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/ports.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/src/rrcgeoviz/features/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/Downloadables.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeartureDataFrameEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureAllMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertMap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertopic.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYearMonths.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeaturePOI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureThreeD.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureWordCloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureYearlyRange.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/HelpfulFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/features/ParentGeovizFeature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/src/rrcgeoviz/geoviz_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 06:29:23.000000 rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 06:29:23.766124 rrcgeoviz-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-09 06:29:16.000000 rrcgeoviz-0.1.3/tests/test_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.843062 rrcgeoviz-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-11 16:44:00.843062 rrcgeoviz-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:44:00.843062 rrcgeoviz-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.831061 rrcgeoviz-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.831061 rrcgeoviz-0.1.4/src/rrcgeoviz/
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/GeneratedData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/GeoVizPanelDashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.831061 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.835062 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/BaseBlock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.835062 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.839062 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/GeneratorBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/GeneratorExample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/GeneratorPOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/ParentDataGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.839062 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    44894 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/data/ports.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.839062 rrcgeoviz-0.1.4/src/rrcgeoviz/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/Downloadables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeartureDataFrameEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureAllMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureBertMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureBertopic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureOneYear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureOneYearMonths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeaturePOI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureThreeD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureWordCloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureYearlyRange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/HelpfulFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/features/ParentGeovizFeature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/src/rrcgeoviz/geoviz_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.839062 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 16:44:00.000000 rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:44:00.839062 rrcgeoviz-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-11 16:43:55.000000 rrcgeoviz-0.1.4/tests/test_arguments.py
```

### Comparing `rrcgeoviz-0.1.3/PKG-INFO` & `rrcgeoviz-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
@@ -35,15 +35,21 @@
 
 First, install GeoViz:
 
 ```bash
 pip install rrcgeoviz
 ```
 
-Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
+Once done, run the following command to create an config file through a GUI:
+
+```bash
+rrcgeoviz --init
+```
+
+The config file is JSON that specifies the data to be looked at and visualized. Here's a sample one:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
         "time_column": "date",
@@ -79,21 +85,23 @@
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
 
 ## Brief overview of how it works (for contributers)
 
+![image](Geoviz_overview_diagram.png)
+
 When running from the command line, the main() function in src/rrcgeoviz/geoviz_cli.py runs. The options and dataset are stored in an [Arguments object](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/arguments.py). 
 
-The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it for it to store. The data is then passed back to the Arguments object as the .generateddata attribute.
+The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it available. The data is then passed back to the Arguments object as the generateddata attribute.
 
 The Arguments object with the data, options, and generated data is passed to the [GeoVizPanelDashboard class](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeoVizPanelDashboard.py). Here, the data is checked (i.e. it is not null, it's in the correct range, etc.) and then the relevant classes in the ALL_FEATURE_CLASSES  array are called to create the features for GeoViz. These don't make any data, just render what's there into pretty visualizations.
 
 Here's a general flow of how to add new components:
-1. If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference.
-2. If a new data generator was made, add it to the DATA_GENERATORS array at the top of the GeneratedData file.
-3. Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like.
-4. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
+
+- Data Generator: If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference. Once it's made, add it to the DATA_GENERATORS array at the top of the src/rrcgeoviz/GeneratedData file.
+
+- Visualizer: Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
 
 That's pretty much it!
```

### Comparing `rrcgeoviz-0.1.3/README.md` & `rrcgeoviz-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,21 @@
 
 First, install GeoViz:
 
 ```bash
 pip install rrcgeoviz
 ```
 
-Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
+Once done, run the following command to create an config file through a GUI:
+
+```bash
+rrcgeoviz --init
+```
+
+The config file is JSON that specifies the data to be looked at and visualized. Here's a sample one:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
         "time_column": "date",
@@ -52,21 +58,23 @@
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
 
 ## Brief overview of how it works (for contributers)
 
+![image](Geoviz_overview_diagram.png)
+
 When running from the command line, the main() function in src/rrcgeoviz/geoviz_cli.py runs. The options and dataset are stored in an [Arguments object](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/arguments.py). 
 
-The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it for it to store. The data is then passed back to the Arguments object as the .generateddata attribute.
+The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it available. The data is then passed back to the Arguments object as the generateddata attribute.
 
 The Arguments object with the data, options, and generated data is passed to the [GeoVizPanelDashboard class](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeoVizPanelDashboard.py). Here, the data is checked (i.e. it is not null, it's in the correct range, etc.) and then the relevant classes in the ALL_FEATURE_CLASSES  array are called to create the features for GeoViz. These don't make any data, just render what's there into pretty visualizations.
 
 Here's a general flow of how to add new components:
-1. If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference.
-2. If a new data generator was made, add it to the DATA_GENERATORS array at the top of the GeneratedData file.
-3. Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like.
-4. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
+
+- Data Generator: If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference. Once it's made, add it to the DATA_GENERATORS array at the top of the src/rrcgeoviz/GeneratedData file.
+
+- Visualizer: Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
 
 That's pretty much it!
```

### Comparing `rrcgeoviz-0.1.3/pyproject.toml` & `rrcgeoviz-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/GeneratedData.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/GeneratedData.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/GeoVizPanelDashboard.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/GeoVizPanelDashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
     def create_template(self, args: Arguments):
         template = pn.template.BootstrapTemplate(
             title="GeoViz - " + str(args.getDataFileName()),
             collapsed_sidebar=True,
             logo=LOGO_PATH,
             favicon=FAVICON_PATH,
         )
+        pn.config.theme = "dark"
         mainColumn = pn.Column()
         nlpColumn = pn.Column()
         mainColumn = self.addCorrectElements(args, mainColumn, FEATURE_CLASSES)
         nlpColumn = self.addCorrectElements(args, nlpColumn, NLP_FEATURE_CLASSES)
 
         template.main.append(
             pn.Tabs(
@@ -197,13 +198,10 @@
                         raise TypeError(
                             "Column "
                             + required_column
                             + " is required for "
                             + feature.getOptionName()
                         )
 
-                mainColumn.append(
-                    pn.pane.HTML("<h2>" + feature.getHeaderText() + "</h2>")
-                )
                 mainColumn.append(feature.generateFeature())
 
         return mainColumn
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreator.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreator.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
 from rrcgeoviz.JsonCreatorClasses.Sections.CacheSetter import CacheSetter
 
 from rrcgeoviz.JsonCreatorClasses.Sections.FeatureCustomizationsSetter import (
     FeatureCustomizationsSetter,
 )
 
+from rrcgeoviz.JsonCreatorClasses.Sections.BaseSection import BaseSection
+
 
 def main_javacreator():
     json_page = pn.Column()
-    sections = [
-        ColumnSetter(),
-        FeatureSetter(),
-        FeatureCustomizationsSetter(),
-        CacheSetter(),
-    ]
-    for section in sections:
-        json_page.append(section.generate_section())
-    json_page.append(DownloadSection(sections).generate_section())
+    columnSetter = ColumnSetter()
+    featureSetter = FeatureSetter()
+    cacheSetter = CacheSetter()
+    json_page.append(columnSetter.generate_section())
+    json_page.append(featureSetter.generate_section(setGrid=True))
+    json_page.append(cacheSetter.generate_section())
+    json_page.append(
+        DownloadSection([columnSetter, featureSetter, cacheSetter]).generate_section()
+    )
 
     json_page.servable()
     pn.serve(json_page)
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/ArrayTextBox.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/DownloadButton.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/ImageCheckbox.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,10 +16,10 @@
     def generate_block(self):
         def update_value(boxTicked):
             if boxTicked:
                 self.stored_value = True
 
         checkbox = pn.widgets.Checkbox(name=self.name)
         binded_checkbox = pn.bind(update_value, boxTicked=checkbox)
-        image = pn.pane.Image(self.image_url, width=500, caption=self.image_description)
+        image = pn.pane.Image(self.image_url, sizing_mode="stretch_width")
         column = pn.Column(checkbox, binded_checkbox, image)
         return column
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/TextBox.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Blocks/Toggle.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/BaseSection.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,42 @@
         raise NotImplementedError("return either string 'dict' or 'array")
 
     def get_block_values(self):
         out = []
         for block in self.blocks:
             out.append(block.get_value())
 
-    def generate_section(self):
+    def generate_section(self, setGrid=False):
         self.blocks = self.generate_blocks()
 
         output = pn.Column()
         output.append(
             pn.Row(
                 pn.layout.HSpacer(),
                 pn.widgets.StaticText(
                     value=self.header_text(),
                 ),
                 pn.layout.HSpacer(),
             )
         )
-        for block in self.blocks:
-            row = pn.Row(
-                pn.layout.HSpacer(), block.generate_block(), pn.layout.HSpacer()
-            )
-            output.append(row)
+
+        if not setGrid:
+            for block in self.blocks:
+                row = pn.Row(
+                    pn.layout.HSpacer(), block.generate_block(), pn.layout.HSpacer()
+                ).servable()
+                output.append(row)
+        else:
+            useable_feature_blocks = []
+            for block in self.blocks:
+                useable_feature_blocks.append(
+                    pn.Column(block.generate_block(), sizing_mode="stretch_width")
+                )
+            output.append(pn.GridBox(*useable_feature_blocks, ncols=5))
+
         return output
 
     def __init__(self) -> None:
         self.blocks = None
 
     def get_blocks(self):
         if self.blocks is None:
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/CacheSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/ColumnSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/DownloadSection.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureCustomizationsSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/JsonCreatorClasses/Sections/FeatureSetter.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/arguments.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/arguments.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorBertopic.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/GeneratorBertopic.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/GeneratorPOI.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/GeneratorPOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/ParentDataGenerator.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/ParentDataGenerator.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/datagenerators/data/ports.csv` & `rrcgeoviz-0.1.4/src/rrcgeoviz/datagenerators/data/ports.csv`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/Downloadables.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/Downloadables.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureAllMonths.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureAllMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertMap.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureBertMap.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureBertopic.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureBertopic.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureHeatmap.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureHeatmap.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYear.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureOneYear.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureOneYearMonths.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureOneYearMonths.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeaturePOI.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeaturePOI.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureSearch.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureSearch.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureThreeD.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureThreeD.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureWordCloud.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureWordCloud.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/FeatureYearlyRange.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/FeatureYearlyRange.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/HelpfulFunctions.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/HelpfulFunctions.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/features/ParentGeovizFeature.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/features/ParentGeovizFeature.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,22 +29,25 @@
 
     def getHeaderText(self):
         raise NotImplementedError(
             "Feature subclasses need to return text to be put in the header above the feature."
         )
 
     def generateFeature(self):
-        component_checkbox = pn.widgets.Checkbox(name="Toggle Visibility", value=False)
-
+        header_text = pn.widgets.StaticText(
+            name="Static Text", value=self.getHeaderText(), height=12
+        )
         feature = pn.Column(
-            component_checkbox,
-            pn.Column(
+            pn.Card(
                 self._generateComponent().servable(),
-                visible=component_checkbox.param.value,
+                header=pn.panel(header_text, height=12),
+                sizing_mode="stretch_width",
+                collapsed=False,
             ),
+            sizing_mode="stretch_width",
         ).servable()
 
         return feature
 
     def _generateComponent(self):
         raise NotImplementedError(
             "Add the code to create the actual feature here. Wrap it in a Panel.Column"
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz/geoviz_cli.py` & `rrcgeoviz-0.1.4/src/rrcgeoviz/geoviz_cli.py`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/PKG-INFO` & `rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrcgeoviz
-Version: 0.1.3
+Version: 0.1.4
 Summary: EDA tool for spatio-temporal data
 Author-email: Jonas Nielsen <bobthebuilder.chfi@gmail.com>, Daniel Millward <dfmillward02@gmail.com>, Stephen Tveten  <stveten@student.byu.edu>
 Project-URL: Documentation, https://rincon-geoviz.readthedocs.io/en/latest/index.html
 Project-URL: Homepage, https://github.com/rrc-byu/ds-capstone-2023-2024
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ydata-profiling==4.6.2
@@ -35,15 +35,21 @@
 
 First, install GeoViz:
 
 ```bash
 pip install rrcgeoviz
 ```
 
-Once done, create an options.json file for your spatio-temporal CSV dataset. Here's a basic example:
+Once done, run the following command to create an config file through a GUI:
+
+```bash
+rrcgeoviz --init
+```
+
+The config file is JSON that specifies the data to be looked at and visualized. Here's a sample one:
 
 ```json
 {
     "columns": {
         "latitude_column": "latitude",
         "longitude_column": "longitude",
         "time_column": "date",
@@ -79,21 +85,23 @@
 rrcgeoviz path/to/dataset.csv path/to/options.json
 ```
 
 A tab should open in your browser with all of the enabled features!
 
 ## Brief overview of how it works (for contributers)
 
+![image](Geoviz_overview_diagram.png)
+
 When running from the command line, the main() function in src/rrcgeoviz/geoviz_cli.py runs. The options and dataset are stored in an [Arguments object](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/arguments.py). 
 
-The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it for it to store. The data is then passed back to the Arguments object as the .generateddata attribute.
+The Arguments object is first passed to the [GeneratedData](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeneratedData.py) class. The GeneratedData class checks whether to pull data from the cache or not. If it needs new data, then it calls any relevant classes in the DATA_GENERATORS array to make it available. The data is then passed back to the Arguments object as the generateddata attribute.
 
 The Arguments object with the data, options, and generated data is passed to the [GeoVizPanelDashboard class](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/GeoVizPanelDashboard.py). Here, the data is checked (i.e. it is not null, it's in the correct range, etc.) and then the relevant classes in the ALL_FEATURE_CLASSES  array are called to create the features for GeoViz. These don't make any data, just render what's there into pretty visualizations.
 
 Here's a general flow of how to add new components:
-1. If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference.
-2. If a new data generator was made, add it to the DATA_GENERATORS array at the top of the GeneratedData file.
-3. Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like.
-4. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
+
+- Data Generator: If new data is required (e.g. distance to nearest POI) create a new subclass of the [ParentGeneratorClass](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/ParentDataGenerator.py) in src/rrcgeoviz/datagenerators. Look at [GeneratorExample](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/datagenerators/GeneratorExample.py) for reference. Once it's made, add it to the DATA_GENERATORS array at the top of the src/rrcgeoviz/GeneratedData file.
+
+- Visualizer: Create the panel component as a subclass of [ParentGeovizFeatures](https://github.com/rrc-byu/ds-capstone-2023-2024/blob/main/src/rrcgeoviz/features/ParentGeovizFeature.py) in src/rrcgeoviz/features. Look at other features in the directory for a sense of what they look like. Add the new feature to the ALL_FEATURE_CLASSES array at the top of the GeoVizPanelDashboard file.
 
 That's pretty much it!
```

### Comparing `rrcgeoviz-0.1.3/src/rrcgeoviz.egg-info/SOURCES.txt` & `rrcgeoviz-0.1.4/src/rrcgeoviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rrcgeoviz-0.1.3/tests/test_arguments.py` & `rrcgeoviz-0.1.4/tests/test_arguments.py`

 * *Files identical despite different names*

