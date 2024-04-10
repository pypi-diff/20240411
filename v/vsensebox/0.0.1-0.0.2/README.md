# Comparing `tmp/vsensebox-0.0.1.tar.gz` & `tmp/vsensebox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox-0.0.1.tar", last modified: Tue Apr  9 03:39:43 2024, max compression
+gzip compressed data, was "vsensebox-0.0.2.tar", last modified: Wed Apr 10 21:52:45 2024, max compression
```

## Comparing `vsensebox-0.0.1.tar` & `vsensebox-0.0.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.122563 vsensebox-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-09 03:39:34.000000 vsensebox-0.0.1/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-09 03:39:34.000000 vsensebox-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-09 03:39:34.000000 vsensebox-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 03:39:43.122563 vsensebox-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-09 03:39:34.000000 vsensebox-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-09 03:39:34.000000 vsensebox-0.0.1/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 03:39:34.000000 vsensebox-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.110563 vsensebox-0.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-09 03:39:34.000000 vsensebox-0.0.1/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-09 03:39:34.000000 vsensebox-0.0.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 03:39:43.122563 vsensebox-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-09 03:39:34.000000 vsensebox-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-09 03:39:34.000000 vsensebox-0.0.1/setup_extra.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.110563 vsensebox-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-09 03:39:34.000000 vsensebox-0.0.1/tests/pretests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 03:39:34.000000 vsensebox-0.0.1/tests/test_01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.110563 vsensebox-0.0.1/vsensebox/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.110563 vsensebox-0.0.1/vsensebox/config/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/confighelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.110563 vsensebox-0.0.1/vsensebox/config/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/config/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/detectors.zip
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/config/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/trackers/centroid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/trackers/deepsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/trackers/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/trackers/sort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/config/trackers/trackers.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/data/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/detectors/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/data/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/data/trackers/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.114563 vsensebox-0.0.1/vsensebox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.118563 vsensebox-0.0.1/vsensebox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)    53087 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/gui/cfgloader_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/gui/uitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.118563 vsensebox-0.0.1/vsensebox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.118563 vsensebox-0.0.1/vsensebox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/detectors/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/detectors/yolo_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/detectors/yolo_ultralytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.118563 vsensebox-0.0.1/vsensebox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.118563 vsensebox-0.0.1/vsensebox/modules/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/box_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/modules/trackers/utils/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.122563 vsensebox-0.0.1/vsensebox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/utils/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.122563 vsensebox-0.0.1/vsensebox/vsense/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/vsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-09 03:39:34.000000 vsensebox-0.0.1/vsensebox/vsense/vsense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 03:39:43.122563 vsensebox-0.0.1/vsensebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-09 03:39:43.000000 vsensebox-0.0.1/vsensebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-09 03:39:43.000000 vsensebox-0.0.1/vsensebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 03:39:43.000000 vsensebox-0.0.1/vsensebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 03:39:43.000000 vsensebox-0.0.1/vsensebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 03:39:43.000000 vsensebox-0.0.1/vsensebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-10 21:52:39.000000 vsensebox-0.0.2/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 21:52:39.000000 vsensebox-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 21:52:39.000000 vsensebox-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 21:52:45.451537 vsensebox-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 21:52:39.000000 vsensebox-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-10 21:52:39.000000 vsensebox-0.0.2/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 21:52:39.000000 vsensebox-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-10 21:52:39.000000 vsensebox-0.0.2/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 21:52:39.000000 vsensebox-0.0.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:52:45.451537 vsensebox-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-10 21:52:39.000000 vsensebox-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 21:52:39.000000 vsensebox-0.0.2/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 21:52:39.000000 vsensebox-0.0.2/tests/pretests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 21:52:39.000000 vsensebox-0.0.2/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/confighelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/config/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/detectors.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/deepsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/sort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/trackers.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/detectors/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/trackers/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    53701 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/cfgloader_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/uitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/yolo_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/yolo_ultralytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/box_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox/vsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/vsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/vsense/vsense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/top_level.txt
```

### Comparing `vsensebox-0.0.1/GETSTARTED.md` & `vsensebox-0.0.2/GETSTARTED.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,18 @@
   - For Linux, recommend changing `python3` to `python`: `sudo apt install python-is-python3`
   - If you prefer conda + Python [3.9-3.12]: `conda create --name vsensebox_env python=3.11`
   - Upgrade `pip` and `setuptools`:
     ```
     python -m pip install --upgrade pip
     pip install "setuptools>=67.2.0"
     ```
-  - Recommend uninstalling the official `Ultralytics`: `pip uninstall -y ultralytics`
+  - Recommend uninstalling the official `Ultralytics`: 
+    ```
+    pip uninstall -y ultralytics
+    ```
 
 * Install dependencies/requirments under `vsensebox/requirements/`: 
   - On Windows:
     - With GPU:
       ```
       pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121
       pip install -r requirements.txt
@@ -79,32 +82,38 @@
   - Or install the ones you need directly from the links below:
     ```
     pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yolocls-0.0.0-py3-none-any.whl
     pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_yoloult-0.0.0-py3-none-any.whl
     pip install https://github.com/rathaumons/vsensebox-data/releases/download/v0.0.0/vsensebox_data_deepsort-0.0.0-py3-none-any.whl
     ```
 
-* Quick Test
-  - On your Python terminal:
+* Let's try some basic features of `VSenseBox`
+  - Configurator GUI can be called in Python terminal:
     ```
     import vsensebox
     vsensebox.config()
     ```
-  - Now you should see the Configurator GUI like in the screenshot below.
-    <details><summary><ins>Show Configurator GUI</ins></summary><img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox_config_gui.jpg"></details>
-  - For ***Linux***, if the GUI does not work, you might need to install these:
-    ```
-    sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
-    ```
-  - For ***Ubuntu on WSL 2***, you need to install these:
-    ```
-    sudo apt-get install libgl1-mesa-glx
-    sudo apt-get install xdg-utils
-    sudo apt-get install libegl1
-    ```
+    Now you should see the Configurator GUI like in this scheenshot:
+    <img src="https://raw.githubusercontent.com/rathaROG/screenshot/master/VSenseBox/vsensebox_config_gui.jpg">
+  - You can also easily reset the internal configurations by calling the `reset()`. **THIS CAN'T BE REVERSED!** ⚠️
+    ```
+    vsensebox.reset()
+    ```
+  - For the details of GUI functions and configurations, check [Configurations page](https://rathaumons.github.io/vsensebox/vsensebox/config.html).
+  - Check the [Examples page](https://rathaumons.github.io/vsensebox/examples.html) for some real coding!
+* For ***Linux***, if the GUI does not work, you might need to install these:
+  ```
+  sudo apt-get install '^libxcb.*-dev' libx11-xcb-dev libglu1-mesa-dev libxrender-dev libxi-dev libxkbcommon-dev libxkbcommon-x11-dev
+  ```
+* For ***Ubuntu on WSL 2***, if the GUI does not work, you need to install these:
+  ```
+  sudo apt-get install libgl1-mesa-glx
+  sudo apt-get install xdg-utils
+  sudo apt-get install libegl1
+  ```
 
 ## 📢 FYI
 
 ### 1️⃣ Customized OpenCV
 
 OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPI do not include GPU support. Thus, we build our custom one which includes NVIDIA [CUDA](https://developer.nvidia.com/cuda-downloads) & [cuDNN](https://developer.nvidia.com/rdp/cudnn-download) supports for the [OpenCV DNN module](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html). In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) -> [[Repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/opencv-for-pyppbox/releases)
```

### Comparing `vsensebox-0.0.1/LICENSE` & `vsensebox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/PKG-INFO` & `vsensebox-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.1
+Version: 0.0.2
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
@@ -65,12 +65,12 @@
 
 **[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
-* Integrate with popular object detectors including YOLO v3, v4, v5, v8, V9, and more.
-* Integrate with bbox trackers including Centroid, SORT, and DeepSORT.
+* Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
+* Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
 * Support Python 3.9-3.12 on Windows, Linux, and macOS.
 * Support YAML config file for each individual module.
 * Integrate with PyQt GUI for easy config.
```

### Comparing `vsensebox-0.0.1/README.md` & `vsensebox-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 
 **[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
-* Integrate with popular object detectors including YOLO v3, v4, v5, v8, V9, and more.
-* Integrate with bbox trackers including Centroid, SORT, and DeepSORT.
+* Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
+* Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
 * Support Python 3.9-3.12 on Windows, Linux, and macOS.
 * Support YAML config file for each individual module.
 * Integrate with PyQt GUI for easy config.
```

### Comparing `vsensebox-0.0.1/RELEASENOTES.md` & `vsensebox-0.0.2/RELEASENOTES.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release Notes 
 
 ## **VSenseBox v0.0.x - Hello World!**
 
+* `VSenseBox` [v0.0.2](https://github.com/rathaumons/vsensebox/tree/v0.0.2)
+  - Add direct YAML file reading to `config()`
+  - Update and improve documentation
+
 * `VSenseBox` [v0.0.1](https://github.com/rathaumons/vsensebox/tree/v0.0.1)
   - Fix the wrong paths in yolo_classic *.yaml
 
 * `VSenseBox` [v0.0.0](https://github.com/rathaumons/vsensebox/tree/v0.0.0)
   - Initialize first release 👋
   - Come with full [documentation](https://rathaumons.github.io/vsensebox/) 📄
   - Support both CPU and GPU ready 🚀
```

### Comparing `vsensebox-0.0.1/requirements/requirements.txt` & `vsensebox-0.0.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/setup.py` & `vsensebox-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/setup_extra.yaml` & `vsensebox-0.0.2/setup_extra.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/tests/pretests.py` & `vsensebox-0.0.2/tests/pretests.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/tests/test_01.py` & `vsensebox-0.0.2/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/__init__.py` & `vsensebox-0.0.2/vsensebox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 from vsensebox.vsense import VSense
 from vsensebox.config.configurator import reset
 from vsensebox.gui import config
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Ratha SIV"
 __description__ = "VSenseBox - Python toolbox for visual sensing."
 __homepage__ = "https://rathaumons.github.io/vsensebox"
 __url__ = "https://github.com/rathaumons/vsensebox.git"
 
 __all__ = ("_version__", "VSense", "config", "reset")
```

### Comparing `vsensebox-0.0.1/vsensebox/config/confighelper.py` & `vsensebox-0.0.2/vsensebox/config/confighelper.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/config/configurator.py` & `vsensebox-0.0.2/vsensebox/config/configurator.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/config/detectors/detectors.zip` & `vsensebox-0.0.2/vsensebox/config/detectors/detectors.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/config/strings.py` & `vsensebox-0.0.2/vsensebox/config/strings.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/config/trackers/trackers.zip` & `vsensebox-0.0.2/vsensebox/config/trackers/trackers.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/gui/assets/settings.ico` & `vsensebox-0.0.2/vsensebox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/gui/cfgloader_ui.py` & `vsensebox-0.0.2/vsensebox/gui/cfgloader_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 
 import os
 import time
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 from vsensebox.config.confighelper import getCFGDict, dumpDocDict
 from vsensebox.utils.about import getVersionString
-from vsensebox.utils.commontools import (joinFPathFull, normalizePathFDS,
+from vsensebox.utils.commontools import (joinFPathFull, normalizePathFDS, isExist, 
                                          isExist, getGlobalRootDir, getAncestorDir)
 
 current_dir = os.path.dirname(__file__)
 vsensebox_root = getGlobalRootDir()
 internal_config_dir = joinFPathFull(vsensebox_root, 'config')
 internal_data_dir = joinFPathFull(vsensebox_root, 'data')
+ui_tmp = joinFPathFull(current_dir, "ui.tmp")
 
 
 class Ui_CFGLoader(object):
 
     def setupUi(self, CFGLoader):
         CFGLoader.setObjectName("CFGLoader")
         CFGLoader.resize(560, 600)
@@ -561,14 +562,17 @@
         self.par10_pushButton.clicked.connect(lambda: self.browseFile(10))
         self.par11_pushButton.clicked.connect(lambda: self.browseFile(11))
         self.par12_pushButton.clicked.connect(lambda: self.browseFile(12))
         self.par13_pushButton.clicked.connect(lambda: self.browseFile(13))
         self.par14_pushButton.clicked.connect(lambda: self.browseFile(14))
         self.par15_pushButton.clicked.connect(lambda: self.browseFile(15))
 
+        # task
+        self.checkUITMP()
+
         self.retranslateUi(CFGLoader)
         QtCore.QMetaObject.connectSlotsByName(CFGLoader)
 
     def retranslateUi(self, CFGLoader):
         _translate = QtCore.QCoreApplication.translate
         title = "Configurator | VSenseBox v" + getVersionString() + " (GPLV3+)"
         CFGLoader.setWindowTitle(_translate("CFGLoader", title))
@@ -822,14 +826,26 @@
                 self.status_lineEdit.setText("Saved " + date_time)
                 self.status_lineEdit.setStyleSheet("color: rgb(50, 255, 50)")
             except Exception as e:
                 print(e)
                 self.status_lineEdit.setText("Failed to save!")
                 self.status_lineEdit.setStyleSheet("color: rgb(255, 50, 50)")
 
+    def checkUITMP(self):
+        if isExist(ui_tmp):
+            with open(ui_tmp) as ui_tmp_file:
+                lines = ui_tmp_file.read().splitlines()
+                if len(lines) > 0:
+                    if isinstance(lines[0], str):
+                        self.yaml_file_lineEdit.setText(lines[0])
+                        self.readYAML(lines[0])
+                        self.save_pushButton.setDisabled(False)
+                        self.reload_pushButton.setDisabled(False)
+            os.remove(ui_tmp)
+
     def reload(self):
         self.resetStatus()
         yaml_file = self.yaml_file_lineEdit.text()
         if isExist(yaml_file):
             try:
                 self.clearPar()
                 self.readYAML(yaml_file)
```

### Comparing `vsensebox-0.0.1/vsensebox/modules/detectors/detectors.py` & `vsensebox-0.0.2/vsensebox/modules/detectors/detectors.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/detectors/yolo_classic.py` & `vsensebox-0.0.2/vsensebox/modules/detectors/yolo_classic.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/detectors/yolo_ultralytics.py` & `vsensebox-0.0.2/vsensebox/modules/detectors/yolo_ultralytics.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/centroid.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/centroid.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/deepsort.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/deepsort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/sort.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/trackers.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/trackers.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/box_matching.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/box_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/detection.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/detection_yolo.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/generate_detections.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/generate_detections.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/iou_matching.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/kalman_filter.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/linear_assignment.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/nn_matching.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/nn_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/preprocessing.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/sort.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/track.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/modules/trackers/utils/tracker.py` & `vsensebox-0.0.2/vsensebox/modules/trackers/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/utils/about.py` & `vsensebox-0.0.2/vsensebox/utils/about.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/utils/commontools.py` & `vsensebox-0.0.2/vsensebox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/utils/logtools.py` & `vsensebox-0.0.2/vsensebox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/utils/visualizetools.py` & `vsensebox-0.0.2/vsensebox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox/vsense/vsense.py` & `vsensebox-0.0.2/vsensebox/vsense/vsense.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.1/vsensebox.egg-info/PKG-INFO` & `vsensebox-0.0.2/vsensebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.1
+Version: 0.0.2
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
@@ -65,12 +65,12 @@
 
 **[📗 Documentation](https://rathaumons.github.io/vsensebox/) | [🚀 Getting started](https://rathaumons.github.io/vsensebox/getstarted.html) | [💡 Examples](https://rathaumons.github.io/vsensebox/examples.html)**
 
 </div>
 
 ***VSenseBox*** is a small all-in-one Python toolbox filled with many vision/visual sensing modules such as object detectors and object trackers, etc. These modules are well integrated together and can be easily selected and configurated with minimal coding.
 
-* Integrate with popular object detectors including YOLO v3, v4, v5, v8, V9, and more.
-* Integrate with bbox trackers including Centroid, SORT, and DeepSORT.
+* Integrate with popular object detectors including YOLO v3, v4, v5, v8, v9, and more.
+* Integrate with bbox trackers including Centroid, SORT, DeepSORT, and more TBA.
 * Support Python 3.9-3.12 on Windows, Linux, and macOS.
 * Support YAML config file for each individual module.
 * Integrate with PyQt GUI for easy config.
```

### Comparing `vsensebox-0.0.1/vsensebox.egg-info/SOURCES.txt` & `vsensebox-0.0.2/vsensebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

