# Comparing `tmp/vsensebox-0.0.2.tar.gz` & `tmp/vsensebox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox-0.0.2.tar", last modified: Wed Apr 10 21:52:45 2024, max compression
+gzip compressed data, was "vsensebox-0.0.3.tar", last modified: Wed Apr 10 23:09:18 2024, max compression
```

## Comparing `vsensebox-0.0.2.tar` & `vsensebox-0.0.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-10 21:52:39.000000 vsensebox-0.0.2/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 21:52:39.000000 vsensebox-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 21:52:39.000000 vsensebox-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 21:52:45.451537 vsensebox-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 21:52:39.000000 vsensebox-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-10 21:52:39.000000 vsensebox-0.0.2/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 21:52:39.000000 vsensebox-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-10 21:52:39.000000 vsensebox-0.0.2/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 21:52:39.000000 vsensebox-0.0.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:52:45.451537 vsensebox-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-10 21:52:39.000000 vsensebox-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 21:52:39.000000 vsensebox-0.0.2/setup_extra.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 21:52:39.000000 vsensebox-0.0.2/tests/pretests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 21:52:39.000000 vsensebox-0.0.2/tests/test_01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/config/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/confighelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.439537 vsensebox-0.0.2/vsensebox/config/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/detectors.zip
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/config/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/centroid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/deepsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/sort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/config/trackers/trackers.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/detectors/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.443537 vsensebox-0.0.2/vsensebox/data/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/data/trackers/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)    53701 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/cfgloader_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/gui/uitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/yolo_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/detectors/yolo_ultralytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.447537 vsensebox-0.0.2/vsensebox/modules/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/box_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/modules/trackers/utils/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox/vsense/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/vsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-10 21:52:39.000000 vsensebox-0.0.2/vsensebox/vsense/vsense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:52:45.451537 vsensebox-0.0.2/vsensebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 21:52:45.000000 vsensebox-0.0.2/vsensebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-10 23:09:12.000000 vsensebox-0.0.3/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 23:09:12.000000 vsensebox-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 23:09:12.000000 vsensebox-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 23:09:18.340121 vsensebox-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 23:09:12.000000 vsensebox-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-10 23:09:12.000000 vsensebox-0.0.3/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 23:09:12.000000 vsensebox-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-10 23:09:12.000000 vsensebox-0.0.3/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 23:09:12.000000 vsensebox-0.0.3/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:09:18.340121 vsensebox-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-10 23:09:12.000000 vsensebox-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 23:09:12.000000 vsensebox-0.0.3/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 23:09:12.000000 vsensebox-0.0.3/tests/pretests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 23:09:12.000000 vsensebox-0.0.3/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/vsensebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/vsensebox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/confighelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/detectors.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/deepsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/sort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/trackers.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/detectors/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/data/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/trackers/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    53701 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/cfgloader_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/uitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/yolo_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/yolo_ultralytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/modules/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/box_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/vsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/vsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/vsense/vsense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/top_level.txt
```

### Comparing `vsensebox-0.0.2/GETSTARTED.md` & `vsensebox-0.0.3/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/LICENSE` & `vsensebox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/PKG-INFO` & `vsensebox-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.2
+Version: 0.0.3
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vsensebox-0.0.2/README.md` & `vsensebox-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/RELEASENOTES.md` & `vsensebox-0.0.3/RELEASENOTES.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release Notes 
 
 ## **VSenseBox v0.0.x - Hello World!**
 
+* `VSenseBox` [v0.0.3](https://github.com/rathaumons/vsensebox/tree/v0.0.3)
+  - Improve `VSense` performance
+  - Update and improve documentation
+
 * `VSenseBox` [v0.0.2](https://github.com/rathaumons/vsensebox/tree/v0.0.2)
   - Add direct YAML file reading to `config()`
   - Update and improve documentation
 
 * `VSenseBox` [v0.0.1](https://github.com/rathaumons/vsensebox/tree/v0.0.1)
   - Fix the wrong paths in yolo_classic *.yaml
```

### Comparing `vsensebox-0.0.2/requirements/requirements.txt` & `vsensebox-0.0.3/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/setup.py` & `vsensebox-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/setup_extra.yaml` & `vsensebox-0.0.3/setup_extra.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/tests/pretests.py` & `vsensebox-0.0.3/tests/pretests.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/tests/test_01.py` & `vsensebox-0.0.3/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/__init__.py` & `vsensebox-0.0.3/vsensebox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 from vsensebox.vsense import VSense
 from vsensebox.config.configurator import reset
 from vsensebox.gui import config
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = "Ratha SIV"
 __description__ = "VSenseBox - Python toolbox for visual sensing."
 __homepage__ = "https://rathaumons.github.io/vsensebox"
 __url__ = "https://github.com/rathaumons/vsensebox.git"
 
 __all__ = ("_version__", "VSense", "config", "reset")
```

### Comparing `vsensebox-0.0.2/vsensebox/config/confighelper.py` & `vsensebox-0.0.3/vsensebox/config/confighelper.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/config/configurator.py` & `vsensebox-0.0.3/vsensebox/config/configurator.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/config/detectors/detectors.zip` & `vsensebox-0.0.3/vsensebox/config/detectors/detectors.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/config/strings.py` & `vsensebox-0.0.3/vsensebox/config/strings.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/config/trackers/trackers.zip` & `vsensebox-0.0.3/vsensebox/config/trackers/trackers.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/gui/assets/settings.ico` & `vsensebox-0.0.3/vsensebox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/gui/cfgloader_ui.py` & `vsensebox-0.0.3/vsensebox/gui/cfgloader_ui.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/gui/uitools.py` & `vsensebox-0.0.3/vsensebox/gui/uitools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/detectors/detectors.py` & `vsensebox-0.0.3/vsensebox/modules/detectors/detectors.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/detectors/yolo_classic.py` & `vsensebox-0.0.3/vsensebox/modules/detectors/yolo_classic.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/detectors/yolo_ultralytics.py` & `vsensebox-0.0.3/vsensebox/modules/detectors/yolo_ultralytics.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/centroid.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/centroid.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/deepsort.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/deepsort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/sort.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/trackers.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/trackers.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/box_matching.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/box_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/detection_yolo.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/generate_detections.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/generate_detections.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/iou_matching.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/kalman_filter.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/linear_assignment.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/nn_matching.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/nn_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/preprocessing.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/sort.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/track.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/modules/trackers/utils/tracker.py` & `vsensebox-0.0.3/vsensebox/modules/trackers/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/utils/about.py` & `vsensebox-0.0.3/vsensebox/utils/about.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/utils/commontools.py` & `vsensebox-0.0.3/vsensebox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/utils/logtools.py` & `vsensebox-0.0.3/vsensebox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/utils/visualizetools.py` & `vsensebox-0.0.3/vsensebox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.2/vsensebox/vsense/vsense.py` & `vsensebox-0.0.3/vsensebox/vsense/vsense.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         A :class:`VSenseAssets` object used to store assets of VSense.
     """
 
     def __init__(self):
         self.assets = VSenseAssets()
         self._detector = None
         self._tracker = None
+        self._yaml_det = None
+        self._yaml_trk = None
         self._det_rel_to_root = False
         self._trk_rel_to_root = False
 
     def detect(self, img, config_yaml=None, img_is_mat=False):
         """Detect objects in the given image :obj:`img`.
 
         Parameters
@@ -53,16 +55,19 @@
         img_is_mat : bool, default=False
             Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like object.
         """
         if not img_is_mat: img = getCVMat(img)
         if config_yaml is None:
             config_yaml = default_detector_yaml
             self._det_rel_to_root = det_rel_to_root
-        self._detector = checkDet(detector=self._detector, config_yaml=config_yaml, 
-                                  relative_to_vsensebox_root=self._det_rel_to_root)
+        if self._yaml_det != config_yaml:
+            self._detector = checkDet(detector=self._detector, config_yaml=config_yaml, 
+                                    relative_to_vsensebox_root=self._det_rel_to_root)
+        else:
+            self._yaml_det = config_yaml
         img, boxes_xywh, boxes_xyxy, keypoints, confs, cls = self._detector.detect(img)
         self.assets.update(
             boxes_xywh=boxes_xywh, 
             boxes_xyxy=boxes_xyxy, 
             keypoints=keypoints, 
             boxes_confs=confs,
             boxes_cls=cls
@@ -80,16 +85,19 @@
         img_is_mat : bool, default=False
             Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like object.
         """
         if not img_is_mat: img = getCVMat(img)
         if config_yaml is None:
             config_yaml = default_tracker_yaml
             self._trk_rel_to_root = trk_rel_to_root
-        self._tracker = checkTrk(tracker=self._tracker, config_yaml=config_yaml, 
-                                 relative_to_vsensebox_root=self._trk_rel_to_root)
+        if self._yaml_trk != config_yaml:
+            self._tracker = checkTrk(tracker=self._tracker, config_yaml=config_yaml, 
+                                    relative_to_vsensebox_root=self._trk_rel_to_root)
+        else:
+            self._yaml_trk = config_yaml
         boxes_xyxy, self.assets.ids = self._tracker.update(
             self.assets.boxes_xyxy, 
             self.assets.boxes_confs, 
             boxes_cls=self.assets.boxes_cls, 
             img=img
         )
```

### Comparing `vsensebox-0.0.2/vsensebox.egg-info/PKG-INFO` & `vsensebox-0.0.3/vsensebox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.2
+Version: 0.0.3
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vsensebox-0.0.2/vsensebox.egg-info/SOURCES.txt` & `vsensebox-0.0.3/vsensebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

