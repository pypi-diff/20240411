# Comparing `tmp/AIPyS-0.0.3.tar.gz` & `tmp/AIPyS-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPyS-0.0.3.tar", last modified: Tue Apr  9 19:19:28 2024, max compression
+gzip compressed data, was "AIPyS-0.0.4.tar", last modified: Thu Apr 11 17:14:49 2024, max compression
```

## Comparing `AIPyS-0.0.3.tar` & `AIPyS-0.0.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:28.013363 AIPyS-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.322214 AIPyS-0.0.3/AIPyS/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.627395 AIPyS-0.0.3/AIPyS/CLI/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/CLI/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-09 18:32:27.000000 AIPyS-0.0.3/AIPyS/CLI/aipys.py
--rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.3/AIPyS/CLI/loadParameters.py
--rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.3/AIPyS/CLI/promptParameters.py
--rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.3/AIPyS/CLI/set_parameters.py
--rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.3/AIPyS/CLI/test.py
--rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.3/AIPyS/DataLoad.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.273189 AIPyS-0.0.3/AIPyS/classification/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.663304 AIPyS-0.0.3/AIPyS/classification/CNN/
--rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.3/AIPyS/classification/CNN/CNN_deploy.py
--rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/CNN/Taining_data_orgenizer.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/classification/CNN/__init__.py
--rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/CNN/mapSgRNA.py
--rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/CNN/model_builder.py
--rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/CNN/model_evaluation_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.716161 AIPyS-0.0.3/AIPyS/classification/bayes/
--rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/bayes/BayesianModels.py
--rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.3/AIPyS/classification/bayes/Baysian_deploy.py
--rw-rw-rw-   0        0        0     7624 2024-03-02 12:25:35.000000 AIPyS-0.0.3/AIPyS/classification/bayes/Baysian_training.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/bayes/DisplayImageFrame.py
--rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.3/AIPyS/classification/bayes/GranulaityMesure.py
--rw-rw-rw-   0        0        0    17734 2024-03-02 12:05:52.000000 AIPyS-0.0.3/AIPyS/classification/bayes/GranularityDataGen.py
--rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/bayes/GranularityDeploy.py
--rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/bayes/RunningWindow.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.3/AIPyS/classification/bayes/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.3/AIPyS/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.277178 AIPyS-0.0.3/AIPyS/segmentation/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.742092 AIPyS-0.0.3/AIPyS/segmentation/cellpose/
--rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.3/AIPyS/segmentation/cellpose/AIPS_cellpose.py
--rw-rw-rw-   0        0        0     1666 2024-02-29 21:42:22.000000 AIPyS-0.0.3/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
--rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.3/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/segmentation/cellpose/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.774007 AIPyS-0.0.3/AIPyS/segmentation/parametric/
--rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/segmentation/parametric/GlobalSeg.py
--rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.3/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/segmentation/parametric/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.858778 AIPyS-0.0.3/AIPyS/supportFunctions/
--rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_file_display.py
--rw-rw-rw-   0        0        0    11778 2024-03-02 20:08:24.000000 AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_functions.py
--rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_granularity.py
--rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_module.py
--rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_simulate.py
--rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/Display_composit.py
--rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/GranularityFunc.py
--rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/Granularity_cellprofiler.py
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.3/AIPyS/supportFunctions/display_and_xml.py
--rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.3/AIPyS/supportFunctions/unpack_h5.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.963497 AIPyS-0.0.3/AIPyS.egg-info/
--rw-rw-rw-   0        0        0     3821 2024-04-09 19:19:26.000000 AIPyS-0.0.3/AIPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2082 2024-04-09 19:19:27.000000 AIPyS-0.0.3/AIPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:19:26.000000 AIPyS-0.0.3/AIPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-04-09 19:19:26.000000 AIPyS-0.0.3/AIPyS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      337 2024-04-09 19:19:26.000000 AIPyS-0.0.3/AIPyS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 19:19:26.000000 AIPyS-0.0.3/AIPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3821 2024-04-09 19:19:28.009375 AIPyS-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-09 19:19:28.014361 AIPyS-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1386 2024-04-09 18:39:56.000000 AIPyS-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.284160 AIPyS-0.0.3/web_app/
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.881715 AIPyS-0.0.3/web_app/Image_labeling/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/web_app/Image_labeling/__init__.py
--rw-rw-rw-   0        0        0     6115 2024-03-01 12:33:36.000000 AIPyS-0.0.3/web_app/Image_labeling/app.py
--rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.3/web_app/Image_labeling/draft.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.923604 AIPyS-0.0.3/web_app/TableViz/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/web_app/TableViz/__init__.py
--rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.3/web_app/TableViz/app.py
--rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.3/web_app/TableViz/distplot.py
-drwxrwxrwx   0        0        0        0 2024-04-09 19:19:27.959508 AIPyS-0.0.3/web_app/measure_length/
--rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.3/web_app/measure_length/__init__.py
--rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.3/web_app/measure_length/app.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.822272 AIPyS-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.077514 AIPyS-0.0.4/AIPyS/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.364745 AIPyS-0.0.4/AIPyS/CLI/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/CLI/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-09 18:32:27.000000 AIPyS-0.0.4/AIPyS/CLI/aipys.py
+-rw-rw-rw-   0        0        0     3666 2024-03-02 14:46:53.000000 AIPyS-0.0.4/AIPyS/CLI/loadParameters.py
+-rw-rw-rw-   0        0        0     2761 2024-03-01 16:45:08.000000 AIPyS-0.0.4/AIPyS/CLI/promptParameters.py
+-rw-rw-rw-   0        0        0     9375 2024-04-09 18:42:35.000000 AIPyS-0.0.4/AIPyS/CLI/set_parameters.py
+-rw-rw-rw-   0        0        0      854 2024-02-29 17:57:58.000000 AIPyS-0.0.4/AIPyS/CLI/test.py
+-rw-rw-rw-   0        0        0     1500 2024-03-02 13:49:57.000000 AIPyS-0.0.4/AIPyS/DataLoad.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.019666 AIPyS-0.0.4/AIPyS/classification/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.405752 AIPyS-0.0.4/AIPyS/classification/CNN/
+-rw-rw-rw-   0        0        0     2501 2024-03-02 20:04:55.000000 AIPyS-0.0.4/AIPyS/classification/CNN/CNN_deploy.py
+-rw-rw-rw-   0        0        0     5086 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/Taining_data_orgenizer.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/classification/CNN/__init__.py
+-rw-rw-rw-   0        0        0     1908 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/mapSgRNA.py
+-rw-rw-rw-   0        0        0    18474 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/model_builder.py
+-rw-rw-rw-   0        0        0     8897 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/CNN/model_evaluation_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.460605 AIPyS-0.0.4/AIPyS/classification/bayes/
+-rw-rw-rw-   0        0        0     2596 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/BayesianModels.py
+-rw-rw-rw-   0        0        0     6221 2024-03-02 14:10:27.000000 AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_deploy.py
+-rw-rw-rw-   0        0        0     7817 2024-04-11 17:07:53.000000 AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_training.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/DisplayImageFrame.py
+-rw-rw-rw-   0        0        0     6145 2024-02-29 21:52:44.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranulaityMesure.py
+-rw-rw-rw-   0        0        0    17734 2024-03-02 12:05:52.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDataGen.py
+-rw-rw-rw-   0        0        0     5065 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDeploy.py
+-rw-rw-rw-   0        0        0     2024 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/RunningWindow.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:26.000000 AIPyS-0.0.4/AIPyS/classification/bayes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:37:34.000000 AIPyS-0.0.4/AIPyS/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.024653 AIPyS-0.0.4/AIPyS/segmentation/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.501496 AIPyS-0.0.4/AIPyS/segmentation/cellpose/
+-rw-rw-rw-   0        0        0     2283 2024-02-28 23:19:56.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpose.py
+-rw-rw-rw-   0        0        0     1666 2024-02-29 21:42:22.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py
+-rw-rw-rw-   0        0        0     2450 2024-03-02 12:03:05.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/StackObjects_cellpose.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/cellpose/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.527426 AIPyS-0.0.4/AIPyS/segmentation/parametric/
+-rw-rw-rw-   0        0        0     3564 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/GlobalSeg.py
+-rw-rw-rw-   0        0        0     2426 2024-02-28 23:19:56.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/segmentation/parametric/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.614628 AIPyS-0.0.4/AIPyS/supportFunctions/
+-rw-rw-rw-   0        0        0     6856 2024-03-02 13:11:22.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_file_display.py
+-rw-rw-rw-   0        0        0    11778 2024-03-02 20:08:24.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_functions.py
+-rw-rw-rw-   0        0        0    10310 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_granularity.py
+-rw-rw-rw-   0        0        0    14491 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_module.py
+-rw-rw-rw-   0        0        0     4250 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_simulate.py
+-rw-rw-rw-   0        0        0     7362 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/Display_composit.py
+-rw-rw-rw-   0        0        0     1252 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/GranularityFunc.py
+-rw-rw-rw-   0        0        0    16340 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/Granularity_cellprofiler.py
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/__init__.py
+-rw-rw-rw-   0        0        0     8046 2024-02-28 23:19:27.000000 AIPyS-0.0.4/AIPyS/supportFunctions/display_and_xml.py
+-rw-rw-rw-   0        0        0      421 2024-02-29 19:41:05.000000 AIPyS-0.0.4/AIPyS/supportFunctions/unpack_h5.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.731318 AIPyS-0.0.4/AIPyS.egg-info/
+-rw-rw-rw-   0        0        0     3821 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2082 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      337 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 17:14:48.000000 AIPyS-0.0.4/AIPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-04-04 15:36:53.000000 AIPyS-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3821 2024-04-11 17:14:49.817284 AIPyS-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:14:49.822272 AIPyS-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1386 2024-04-11 17:09:54.000000 AIPyS-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.031636 AIPyS-0.0.4/web_app/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.638564 AIPyS-0.0.4/web_app/Image_labeling/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/Image_labeling/__init__.py
+-rw-rw-rw-   0        0        0     6115 2024-03-01 12:33:36.000000 AIPyS-0.0.4/web_app/Image_labeling/app.py
+-rw-rw-rw-   0        0        0     1786 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/Image_labeling/draft.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.690430 AIPyS-0.0.4/web_app/TableViz/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/TableViz/__init__.py
+-rw-rw-rw-   0        0        0     4054 2024-03-01 12:56:00.000000 AIPyS-0.0.4/web_app/TableViz/app.py
+-rw-rw-rw-   0        0        0     2320 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/TableViz/distplot.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:14:49.728326 AIPyS-0.0.4/web_app/measure_length/
+-rw-rw-rw-   0        0        0        0 2024-02-28 23:19:27.000000 AIPyS-0.0.4/web_app/measure_length/__init__.py
+-rw-rw-rw-   0        0        0     4549 2024-02-29 19:09:36.000000 AIPyS-0.0.4/web_app/measure_length/app.py
```

### Comparing `AIPyS-0.0.3/AIPyS/CLI/aipys.py` & `AIPyS-0.0.4/AIPyS/CLI/aipys.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/CLI/loadParameters.py` & `AIPyS-0.0.4/AIPyS/CLI/loadParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/CLI/promptParameters.py` & `AIPyS-0.0.4/AIPyS/CLI/promptParameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/CLI/set_parameters.py` & `AIPyS-0.0.4/AIPyS/CLI/set_parameters.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/CLI/test.py` & `AIPyS-0.0.4/AIPyS/CLI/test.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/DataLoad.py` & `AIPyS-0.0.4/AIPyS/DataLoad.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/CNN/CNN_deploy.py` & `AIPyS-0.0.4/AIPyS/classification/CNN/CNN_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/CNN/Taining_data_orgenizer.py` & `AIPyS-0.0.4/AIPyS/classification/CNN/Taining_data_orgenizer.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/CNN/mapSgRNA.py` & `AIPyS-0.0.4/AIPyS/classification/CNN/mapSgRNA.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/CNN/model_builder.py` & `AIPyS-0.0.4/AIPyS/classification/CNN/model_builder.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/CNN/model_evaluation_utils.py` & `AIPyS-0.0.4/AIPyS/classification/CNN/model_evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/BayesianModels.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/BayesianModels.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/Baysian_deploy.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_deploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/Baysian_training.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/Baysian_training.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,17 +61,20 @@
         fractionData: int
             work on fraction of the data for training
         areaSel: int
             cutoff for area
         '''
         df_label = self.df
         if self.areaSel > 0:
-            df_label = df_label.loc[df_label['maskArea'] > self.areaSel,:].reset_index()
+            df_label = df_label.loc[df_label['maskArea'] > self.areaSel,:].reset_index(drop=True)
         if self.fractionData > 0:
-            df_label = df_label.sample(n=self.fractionData, replace=False).reset_index()
+            if self.fractionData > len(df_label):
+                df_label = df_label.sample(n=len(df_label)-1, replace=False).reset_index(drop=True)
+            else:
+                df_label = df_label.sample(n=self.fractionData, replace=False).reset_index(drop=True)
         if self.areaSel < 0 and self.fractionData < 0:
             OneNum = len(df_label.loc[df_label["label"]==1])
             ind_pheno_list = df_label.loc[df_label["label"]==1,:].index.to_list()
             ind_WT_list = df_label.loc[df_label["label"]==0,:].index.to_list()
             random.shuffle(ind_WT_list)
             ind_WT_list_sel= [ind_WT_list[i] for i in range(OneNum)]
             df_label = df_label.iloc[ind_WT_list_sel+ind_pheno_list,:]
```

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/GranulaityMesure.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/GranulaityMesure.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/GranularityDataGen.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDataGen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/GranularityDeploy.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/GranularityDeploy.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/classification/bayes/RunningWindow.py` & `AIPyS-0.0.4/AIPyS/classification/bayes/RunningWindow.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/segmentation/cellpose/AIPS_cellpose.py` & `AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py` & `AIPyS-0.0.4/AIPyS/segmentation/cellpose/AIPS_cellpse_video_gen.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/segmentation/cellpose/StackObjects_cellpose.py` & `AIPyS-0.0.4/AIPyS/segmentation/cellpose/StackObjects_cellpose.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/segmentation/parametric/GlobalSeg.py` & `AIPyS-0.0.4/AIPyS/segmentation/parametric/GlobalSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py` & `AIPyS-0.0.4/AIPyS/segmentation/parametric/ImageSeqGlobSeg.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_file_display.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_file_display.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_functions.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_functions.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_granularity.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_granularity.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_module.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_module.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/AIPS_simulate.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/AIPS_simulate.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/Display_composit.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/Display_composit.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/GranularityFunc.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/GranularityFunc.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/Granularity_cellprofiler.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/Granularity_cellprofiler.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS/supportFunctions/display_and_xml.py` & `AIPyS-0.0.4/AIPyS/supportFunctions/display_and_xml.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/AIPyS.egg-info/PKG-INFO` & `AIPyS-0.0.4/AIPyS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.3/AIPyS.egg-info/SOURCES.txt` & `AIPyS-0.0.4/AIPyS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/LICENSE` & `AIPyS-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/PKG-INFO` & `AIPyS-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPyS
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI Powered Photoswitchable Screen
 Home-page: 
 Author: Gil Kanfer
 Author-email: gil.kanfer.il@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AIPyS-0.0.3/setup.py` & `AIPyS-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="AIPyS",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(include=['AIPyS','AIPyS.CLI','AIPyS.classification.bayes','AIPyS.classification.CNN',
                                     'AIPyS.segmentation.cellpose','AIPyS.segmentation.parametric','AIPyS.supportFunctions',
                                     'web_app.Image_labeling','web_app.measure_length','web_app.measure_length','web_app.TableViz']),
     install_requires=required,
     entry_points={
         'console_scripts': [
            'aipys=AIPyS.CLI.aipys:main',
```

### Comparing `AIPyS-0.0.3/web_app/Image_labeling/app.py` & `AIPyS-0.0.4/web_app/Image_labeling/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/web_app/Image_labeling/draft.py` & `AIPyS-0.0.4/web_app/Image_labeling/draft.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/web_app/TableViz/app.py` & `AIPyS-0.0.4/web_app/TableViz/app.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/web_app/TableViz/distplot.py` & `AIPyS-0.0.4/web_app/TableViz/distplot.py`

 * *Files identical despite different names*

### Comparing `AIPyS-0.0.3/web_app/measure_length/app.py` & `AIPyS-0.0.4/web_app/measure_length/app.py`

 * *Files identical despite different names*

