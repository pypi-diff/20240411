# Comparing `tmp/pyPhasesML-0.8.6.tar.gz` & `tmp/pyPhasesML-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.8.6.tar", last modified: Fri Jan 26 16:46:08 2024, max compression
+gzip compressed data, was "pyPhasesML-0.9.0.tar", last modified: Thu Apr 11 11:39:17 2024, max compression
```

## Comparing `pyPhasesML-0.8.6.tar` & `pyPhasesML-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.491036 pyPhasesML-0.8.6/
--rw-rw-rw-   0 root         (0) root         (0)     1086 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3704 2024-01-26 16:46:08.490036 pyPhasesML-0.8.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3317 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.485036 pyPhasesML-0.8.6/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2695 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1638 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     4177 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/ModelAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.486036 pyPhasesML-0.8.6/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10753 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7391 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    10632 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.487036 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/
--rw-rw-rw-   0 root         (0) root         (0)      734 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CSVLogger.py
--rw-rw-rw-   0 root         (0) root         (0)     1875 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/Callback.py
--rw-rw-rw-   0 root         (0) root         (0)     5206 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CyclicLearningrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1748 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/FindLearningRate.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/LoadOptimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/SystemCheckPoint.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/adapter/torch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.489036 pyPhasesML-0.8.6/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      493 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/BatchMap.py
--rw-rw-rw-   0 root         (0) root         (0)      874 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/DataLoader.py
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/DataPipe.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/PreloadPipe.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/ShuffleMap.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/TorchMap.py
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.489036 pyPhasesML-0.8.6/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5542 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.490036 pyPhasesML-0.8.6/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19833 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 16:46:08.485036 pyPhasesML-0.8.6/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3704 2024-01-26 16:46:08.000000 pyPhasesML-0.8.6/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1603 2024-01-26 16:46:08.000000 pyPhasesML-0.8.6/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 16:46:08.000000 pyPhasesML-0.8.6/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-01-26 16:46:08.000000 pyPhasesML-0.8.6/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-01-26 16:46:08.000000 pyPhasesML-0.8.6/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-01-26 16:45:47.000000 pyPhasesML-0.8.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-26 16:46:08.491036 pyPhasesML-0.8.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-26 16:45:49.000000 pyPhasesML-0.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.088355 pyPhasesML-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-11 11:39:17.088355 pyPhasesML-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.082355 pyPhasesML-0.9.0/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4177 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/ModelAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.083355 pyPhasesML-0.9.0/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10753 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7391 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    10683 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:38:58.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.085355 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/
+-rw-rw-rw-   0 root         (0) root         (0)      734 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CSVLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1875 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/Callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     5206 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CyclicLearningrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/FindLearningRate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/LoadOptimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/SystemCheckPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/adapter/torch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.087355 pyPhasesML-0.9.0/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      493 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/BatchMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/DataLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/DataPipe.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/PreloadPipe.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/ShuffleMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/TorchMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.087355 pyPhasesML-0.9.0/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:38:58.000000 pyPhasesML-0.9.0/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.088355 pyPhasesML-0.9.0/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19833 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:39:17.082355 pyPhasesML-0.9.0/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-11 11:39:17.000000 pyPhasesML-0.9.0/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1569 2024-04-11 11:39:17.000000 pyPhasesML-0.9.0/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:39:17.000000 pyPhasesML-0.9.0/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-11 11:39:17.000000 pyPhasesML-0.9.0/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-11 11:39:17.000000 pyPhasesML-0.9.0/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-04-11 11:38:57.000000 pyPhasesML-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 11:39:17.088355 pyPhasesML-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-04-11 11:38:59.000000 pyPhasesML-0.9.0/setup.py
```

### Comparing `pyPhasesML-0.8.6/LICENSE` & `pyPhasesML-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/PKG-INFO` & `pyPhasesML-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.8.6
+Version: 0.9.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.8.6/README.md` & `pyPhasesML-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.9.0/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/DataSet.py` & `pyPhasesML-0.9.0/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.9.0/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.9.0/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/Model.py` & `pyPhasesML-0.9.0/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/ModelManager.py` & `pyPhasesML-0.9.0/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/Plugin.py` & `pyPhasesML-0.9.0/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,16 +239,17 @@
             if self.finish:
                 break
 
         self.trigger("trainingEnd", self)
 
         self.fullEpochs = self.epoch
         self.trigger("trainEnd", self)
-        self.log("load best Model: %s" % self.bestModelPath)
-        self.loadState(self.load(self.bestModelPath))
+        if self.bestModelPath is not None:
+            self.log("load best Model: %s" % self.bestModelPath)
+            self.loadState(self.load(self.bestModelPath))
         return self.model
 
     def getModelPath(self):
         return self.logPath
 
     def build(self):
         torchSeed = 2
```

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CSVLogger.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CSVLogger.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/Callback.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/Callback.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CheckPoint.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/CyclicLearningrate.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/CyclicLearningrate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/FindLearningRate.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/FindLearningRate.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/LoadOptimizer.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/LoadOptimizer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/adapter/torch/SystemCheckPoint.py` & `pyPhasesML-0.9.0/pyPhasesML/adapter/torch/SystemCheckPoint.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/config.yaml` & `pyPhasesML-0.9.0/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/datapipes/BatchMap.py` & `pyPhasesML-0.9.0/pyPhasesML/datapipes/BatchMap.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/datapipes/DataLoader.py` & `pyPhasesML-0.9.0/pyPhasesML/datapipes/DataLoader.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.9.0/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/datapipes/PreloadPipe.py` & `pyPhasesML-0.9.0/pyPhasesML/datapipes/PreloadPipe.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.9.0/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.9.0/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.9.0/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.9.0/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.8.6
+Version: 0.9.0
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.8.6/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.9.0/pyPhasesML.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 pyPhasesML/DataSet.py
 pyPhasesML/DataversionManager.py
 pyPhasesML/FeatureExtraction.py
 pyPhasesML/Model.py
 pyPhasesML/ModelAdapter.py
 pyPhasesML/ModelManager.py
 pyPhasesML/Plugin.py
-pyPhasesML/SignalPreprocessing.py
 pyPhasesML/__init__.py
 pyPhasesML/config.yaml
 pyPhasesML.egg-info/PKG-INFO
 pyPhasesML.egg-info/SOURCES.txt
 pyPhasesML.egg-info/dependency_links.txt
 pyPhasesML.egg-info/requires.txt
 pyPhasesML.egg-info/top_level.txt
```

### Comparing `pyPhasesML-0.8.6/pyproject.toml` & `pyPhasesML-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.8.6/setup.py` & `pyPhasesML-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.8.6"[1:],
+    version="v0.9.0"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

