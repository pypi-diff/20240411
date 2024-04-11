# Comparing `tmp/vsensebox-0.0.3.tar.gz` & `tmp/vsensebox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox-0.0.3.tar", last modified: Wed Apr 10 23:09:18 2024, max compression
+gzip compressed data, was "vsensebox-0.0.4.tar", last modified: Thu Apr 11 13:27:33 2024, max compression
```

## Comparing `vsensebox-0.0.3.tar` & `vsensebox-0.0.4.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-10 23:09:12.000000 vsensebox-0.0.3/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 23:09:12.000000 vsensebox-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-10 23:09:12.000000 vsensebox-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 23:09:18.340121 vsensebox-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-10 23:09:12.000000 vsensebox-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-10 23:09:12.000000 vsensebox-0.0.3/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 23:09:12.000000 vsensebox-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-10 23:09:12.000000 vsensebox-0.0.3/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 23:09:12.000000 vsensebox-0.0.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:09:18.340121 vsensebox-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-10 23:09:12.000000 vsensebox-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-10 23:09:12.000000 vsensebox-0.0.3/setup_extra.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-10 23:09:12.000000 vsensebox-0.0.3/tests/pretests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 23:09:12.000000 vsensebox-0.0.3/tests/test_01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/vsensebox/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.328121 vsensebox-0.0.3/vsensebox/config/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/confighelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/detectors.zip
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/config/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/centroid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/deepsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/sort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/config/trackers/trackers.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/detectors/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.332121 vsensebox-0.0.3/vsensebox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/data/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/data/trackers/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)    53701 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/cfgloader_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/gui/uitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/yolo_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/detectors/yolo_ultralytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.336121 vsensebox-0.0.3/vsensebox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/modules/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/box_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/modules/trackers/utils/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox/vsense/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/vsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-10 23:09:12.000000 vsensebox-0.0.3/vsensebox/vsense/vsense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:09:18.340121 vsensebox-0.0.3/vsensebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 23:09:18.000000 vsensebox-0.0.3/vsensebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.724304 vsensebox-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-11 13:27:25.000000 vsensebox-0.0.4/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:27:25.000000 vsensebox-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 13:27:25.000000 vsensebox-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-11 13:27:33.724304 vsensebox-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 13:27:25.000000 vsensebox-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 13:27:25.000000 vsensebox-0.0.4/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 13:27:25.000000 vsensebox-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.712304 vsensebox-0.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 13:27:25.000000 vsensebox-0.0.4/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-11 13:27:25.000000 vsensebox-0.0.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:27:33.724304 vsensebox-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-11 13:27:25.000000 vsensebox-0.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 13:27:25.000000 vsensebox-0.0.4/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.712304 vsensebox-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 13:27:25.000000 vsensebox-0.0.4/tests/pretests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 13:27:25.000000 vsensebox-0.0.4/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.712304 vsensebox-0.0.4/vsensebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.716304 vsensebox-0.0.4/vsensebox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7776 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/confighelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21249 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.716304 vsensebox-0.0.4/vsensebox/config/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.716304 vsensebox-0.0.4/vsensebox/config/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/detectors.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.716304 vsensebox-0.0.4/vsensebox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/config/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/trackers/centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/trackers/deepsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/trackers/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/trackers/sort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/config/trackers/trackers.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/data/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/detectors/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/data/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/data/trackers/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    53488 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/gui/cfgloader_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/gui/uitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/detectors/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/detectors/yolo_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/detectors/yolo_ultralytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.720304 vsensebox-0.0.4/vsensebox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.724304 vsensebox-0.0.4/vsensebox/modules/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/box_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/modules/trackers/utils/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.724304 vsensebox-0.0.4/vsensebox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/utils/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.724304 vsensebox-0.0.4/vsensebox/vsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/vsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-11 13:27:25.000000 vsensebox-0.0.4/vsensebox/vsense/vsense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:27:33.724304 vsensebox-0.0.4/vsensebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-11 13:27:33.000000 vsensebox-0.0.4/vsensebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-11 13:27:33.000000 vsensebox-0.0.4/vsensebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:27:33.000000 vsensebox-0.0.4/vsensebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 13:27:33.000000 vsensebox-0.0.4/vsensebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 13:27:33.000000 vsensebox-0.0.4/vsensebox.egg-info/top_level.txt
```

### Comparing `vsensebox-0.0.3/GETSTARTED.md` & `vsensebox-0.0.4/GETSTARTED.md`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/LICENSE` & `vsensebox-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/PKG-INFO` & `vsensebox-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.3
+Version: 0.0.4
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vsensebox-0.0.3/README.md` & `vsensebox-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/RELEASENOTES.md` & `vsensebox-0.0.4/RELEASENOTES.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Release Notes 
 
 ## **VSenseBox v0.0.x - Hello World!**
 
+* `VSenseBox` [v0.0.4](https://github.com/rathaumons/vsensebox/tree/v0.0.4)
+  - Add minor bug fixes
+  - Add example 03 for multithreading
+  - Improve overall performance
+  - Update and improve documentation
+
 * `VSenseBox` [v0.0.3](https://github.com/rathaumons/vsensebox/tree/v0.0.3)
   - Improve `VSense` performance
   - Update and improve documentation
 
 * `VSenseBox` [v0.0.2](https://github.com/rathaumons/vsensebox/tree/v0.0.2)
   - Add direct YAML file reading to `config()`
   - Update and improve documentation
```

### Comparing `vsensebox-0.0.3/requirements/requirements.txt` & `vsensebox-0.0.4/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/setup.py` & `vsensebox-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/setup_extra.yaml` & `vsensebox-0.0.4/setup_extra.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/tests/pretests.py` & `vsensebox-0.0.4/tests/pretests.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/tests/test_01.py` & `vsensebox-0.0.4/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/__init__.py` & `vsensebox-0.0.4/vsensebox/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # VSenseBox - Python toolbox for visual sensing
 # GNU General Public License v3 or later (GPLv3+)
 # Copyright (C) 2024 UMONS-Numediart
 
 
 from vsensebox.vsense import VSense
-from vsensebox.config.configurator import reset
-from vsensebox.gui import config
+from vsensebox.gui import config, reset
+from vsensebox.utils.about import docs, github
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __author__ = "Ratha SIV"
 __description__ = "VSenseBox - Python toolbox for visual sensing."
 __homepage__ = "https://rathaumons.github.io/vsensebox"
 __url__ = "https://github.com/rathaumons/vsensebox.git"
 
-__all__ = ("_version__", "VSense", "config", "reset")
+__all__ = (
+    "__version__", 
+    "VSense", 
+    "config", 
+    "reset", 
+    "docs", 
+    "github"
+)
```

### Comparing `vsensebox-0.0.3/vsensebox/config/confighelper.py` & `vsensebox-0.0.4/vsensebox/config/confighelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 import json
 import yaml
 from yaml.loader import SafeLoader
 
-from vsensebox.config.strings import UnifiedStrings
+from .strings import USTR
 from vsensebox.utils.commontools import getAbsPathFDS, isExist
 from vsensebox.utils.logtools import add_error_log
 
 
-unified_strings = UnifiedStrings()
-
-
 def isDictString(input_string):
     """Check whether the :obj:`input_string` is a valid raw dictionary.
 
     Parameters
     ----------
     input_string : str
         An input of raw string.
@@ -224,15 +221,15 @@
         with open(output_file, 'w') as dumping:
             dumping.write(header)
             for key, value in doc.items():
                 key = str(key).lower()
                 if str(value) == "None" or value is None:
                     value = "null # NULL=Null=null is None in Python"
                 if key == "detector" or key == "tracker":
-                    value = unified_strings.getUnifiedFormat(value)
+                    value = USTR.getUnifiedFormat(value)
                 dumping.write('%s: %s\n' % (key, value))
     except ValueError as e:
         msg = 'dumpDocDict() -> ' + str(e)
         add_error_log(msg)
         raise ValueError(msg)
 
 def dumpListDocDict(output_file, doc_list, header):
@@ -253,15 +250,15 @@
             sep_index = 1
             for d in doc_list:
                 for key, value in d.items():
                     key = str(key).lower()
                     if str(value) == "None" or value is None:
                         value = "null # NULL=Null=null is None in Python"
                     if key == "detector" or key == "tracker":
-                        value = unified_strings.getUnifiedFormat(value)
+                        value = USTR.getUnifiedFormat(value)
                     dumping.write('%s: %s\n' % (key, value))
                 if sep_index < len(doc_list):
                     dumping.write("---\n")
                     sep_index += 1
     except ValueError as e:
         msg = 'dumpListDocDict() -> ' + str(e)
         add_error_log(msg)
```

### Comparing `vsensebox-0.0.3/vsensebox/config/configurator.py` & `vsensebox-0.0.4/vsensebox/config/configurator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # VSenseBox - Python toolbox for visual sensing
 # GNU General Public License v3 or later (GPLv3+)
 # Copyright (C) 2024 UMONS-Numediart
 
 
-from .strings import UnifiedStrings
+from .strings import USTR
 from .confighelper import getCFGDict, getListCFGDoc, dumpDocDict, dumpListDocDict
-from vsensebox.utils.logtools import add_warning_log, add_error_log, add_info_log
+from vsensebox.utils.logtools import add_warning_log, add_error_log
 from vsensebox.utils.commontools import (joinFPathFull, getGlobalRootDir, 
                                          getAdaptiveAbsPathFDS, normalizePathFDS)
 
-unified_strings = UnifiedStrings()
-internal_root_dir = getGlobalRootDir()
-internal_config_dir = joinFPathFull(internal_root_dir, 'config')
-detectors_config_dir = joinFPathFull(internal_config_dir, 'detectors')
-trackers_config_dir = joinFPathFull(internal_config_dir, 'trackers')
+IN_ROOT_DIR = getGlobalRootDir()
+IN_DATA_DIR = joinFPathFull(IN_ROOT_DIR, 'data')
+IN_CONFIG_DIR = joinFPathFull(IN_ROOT_DIR, 'config')
+DET_CONFIG_DIR = joinFPathFull(IN_CONFIG_DIR, 'detectors')
+TRK_CONFIG_DIR = joinFPathFull(IN_CONFIG_DIR, 'trackers')
+STR_CONFIG_DIR = joinFPathFull(IN_CONFIG_DIR, 'strings')
 
 
 class BaseCGF(object):
 
     """
     An base CFG class used to store the necessary configurations of a module.
 
@@ -27,15 +28,15 @@
         A :class:`MyStrings` object used to store unified strings.
     configs : dict or list[dict], default={}
         A configuration dictionary of a single document or a list of multiple documents 
         of the configurations.
     """
 
     def __init__(self):
-        self.unified_strings = unified_strings
+        self.unified_strings = USTR
         self.configs = {}
     
     def loadDoc(self, input):
         """Load and set dictionary of a single document from a YAML/JSON file or string.
 
         Parameters
         ----------
@@ -126,15 +127,15 @@
             to your current working directory. 
             (2) Set :code:`relative_to_vsensebox_root=True` when all the paths in your configuration 
             file are relative to :code:`{vsensebox root}`.
         """
         super().__init__()
         self.from_dir = ""
         if relative_to_vsensebox_root:
-            self.from_dir = internal_root_dir
+            self.from_dir = IN_ROOT_DIR
         if cfg is not None:
             self.set(cfg)
 
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
@@ -175,17 +176,17 @@
         yolocs_doc = {
             "detector": self.detector,
             "nms": self.nms,
             "conf": self.conf,
             "imgsz": self.imgsz,
             "min_width": self.min_width,
             "classes": self.classes,
-            "class_file": normalizePathFDS(internal_root_dir, self.class_file),
-            "model_cfg_file": normalizePathFDS(internal_root_dir, self.model_cfg_file),
-            "model_file": normalizePathFDS(internal_root_dir, self.model_file),
+            "class_file": normalizePathFDS(IN_ROOT_DIR, self.class_file),
+            "model_cfg_file": normalizePathFDS(IN_ROOT_DIR, self.model_cfg_file),
+            "model_file": normalizePathFDS(IN_ROOT_DIR, self.model_file),
         }
         return yolocs_doc
 
 
 class DCFG_YOLOULT(BaseCGF):
 
     """
@@ -236,15 +237,15 @@
             set relatively to your current working directory. 
             (2) Set :code:`relative_to_vsensebox_root=True` when all the paths in your 
             configuration file are relative to :code:{vsensebox root}.
         """
         super().__init__()
         self.from_dir = ""
         if relative_to_vsensebox_root:
-            self.from_dir = internal_root_dir
+            self.from_dir = IN_ROOT_DIR
         if cfg is not None:
             self.set(cfg)
 
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
@@ -291,15 +292,15 @@
             "imgsz": self.imgsz,
             "half": self.half,
             "min_width": self.min_width,
             "classes": self.classes,
             "device": self.device,
             "max_det": self.max_det,
             "line_width": self.line_width,
-            "model_file": normalizePathFDS(internal_root_dir, self.model_file),
+            "model_file": normalizePathFDS(IN_ROOT_DIR, self.model_file),
         }
         return yolout_doc
 
 
 class TCFG_Centroid(BaseCGF):
 
     """
@@ -332,15 +333,15 @@
             your current working directory. 
             (2) Set :code:`relative_to_vsensebox_root=True` when all the paths in your configuration 
             file are relative to :code:`{vsensebox root}`.
         """
         super().__init__()
         self.from_dir = ""
         if relative_to_vsensebox_root:
-            self.from_dir = internal_root_dir
+            self.from_dir = IN_ROOT_DIR
         if cfg is not None:
             self.set(cfg)
 
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
@@ -414,15 +415,15 @@
             your current working directory. 
             (2) Set :code:`relative_to_vsensebox_root=True` when all the paths in your configuration 
             file are relative to :code:`{vsensebox root}`.
         """
         super().__init__()
         self.from_dir = ""
         if relative_to_vsensebox_root:
-            self.from_dir = internal_root_dir
+            self.from_dir = IN_ROOT_DIR
         if cfg is not None:
             self.set(cfg)
 
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
@@ -505,15 +506,15 @@
             your current working directory. 
             (2) Set :code:`relative_to_vsensebox_root=True` when all the paths in your configuration 
             file are relative to :code:`{vsensebox root}`.
         """
         super().__init__()
         self.from_dir = ""
         if relative_to_vsensebox_root:
-            self.from_dir = internal_root_dir
+            self.from_dir = IN_ROOT_DIR
         if cfg is not None:
             self.set(cfg)
 
     def set(self, input):
         """
         Set configurations according to :obj:`input`.
 
@@ -550,20 +551,11 @@
         """
         deepsort_doc = {
             "tracker": self.tracker,
             "nn_budget": self.nn_budget,
             "batch_size": self.batch_size,
             "nms_max_overlap": self.nms_max_overlap,
             "max_cosine_distance": self.max_cosine_distance,
-            "model_file": normalizePathFDS(internal_root_dir, self.model_file)
+            "model_file": normalizePathFDS(IN_ROOT_DIR, self.model_file)
         }
         return deepsort_doc
 
-def reset():
-    """Reset the internal configurations.
-    """
-    import shutil
-    strings_config_dir = joinFPathFull(internal_config_dir, 'strings')
-    shutil.unpack_archive(joinFPathFull(strings_config_dir, 'strings.zip'), strings_config_dir)
-    shutil.unpack_archive(joinFPathFull(detectors_config_dir, 'detectors.zip'), detectors_config_dir)
-    shutil.unpack_archive(joinFPathFull(trackers_config_dir, 'trackers.zip'), trackers_config_dir)
-    add_info_log("Reset successfully!")
```

### Comparing `vsensebox-0.0.3/vsensebox/config/strings.py` & `vsensebox-0.0.4/vsensebox/config/strings.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 import yaml
 from yaml.loader import SafeLoader
 from vsensebox.utils.commontools import joinFPathFull, getGlobalRootDir
 
 
-default_strings_yaml = joinFPathFull(getGlobalRootDir(), "config/strings/strings.yaml")
+DEFAULT_STR_YAML = joinFPathFull(getGlobalRootDir(), "config/strings/strings.yaml")
 
 class UnifiedStrings(object):
 
     """
     A class used to set up unified strings of VSenseBox based on the internal strings.yaml.
 
     Attributes
@@ -33,15 +33,15 @@
         Unified string of word 'SORT'.
     deepsort : str, auto
         Unified string of word 'DeepSORT'.
     centroid : str, auto
         Unified string of word 'Centroid'.
     """
 
-    def __init__(self, strings_yaml=default_strings_yaml):
+    def __init__(self, strings_yaml=DEFAULT_STR_YAML):
         """Initailize by calling :meth:`load(strings_yaml=strings_yaml)`.
 
         Parameters
         ----------
         strings_yaml : str, default='{vsensebox root}/config/strings/strings.yaml'
             A path of a YAML file which stores the unified strings.
         """
@@ -110,7 +110,9 @@
             res = input_str.title()
         elif input_str.lower in ['top', 'center', 'bottom']:
             res = input_str.title()
         else:
             res = input_str
         
         return res
+
+USTR = UnifiedStrings()
```

### Comparing `vsensebox-0.0.3/vsensebox/config/trackers/trackers.zip` & `vsensebox-0.0.4/vsensebox/config/trackers/trackers.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/gui/assets/settings.ico` & `vsensebox-0.0.4/vsensebox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/gui/cfgloader_ui.py` & `vsensebox-0.0.4/vsensebox/gui/cfgloader_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 import os
 import time
 
 from PyQt6 import QtCore, QtGui, QtWidgets
+
+from vsensebox.gui.uitools import CUR_DIR, UI_TMP
+from vsensebox.config.configurator import IN_ROOT_DIR, IN_CONFIG_DIR
 from vsensebox.config.confighelper import getCFGDict, dumpDocDict
 from vsensebox.utils.about import getVersionString
-from vsensebox.utils.commontools import (joinFPathFull, normalizePathFDS, isExist, 
-                                         isExist, getGlobalRootDir, getAncestorDir)
-
-current_dir = os.path.dirname(__file__)
-vsensebox_root = getGlobalRootDir()
-internal_config_dir = joinFPathFull(vsensebox_root, 'config')
-internal_data_dir = joinFPathFull(vsensebox_root, 'data')
-ui_tmp = joinFPathFull(current_dir, "ui.tmp")
+from vsensebox.utils.commontools import joinFPathFull, normalizePathFDS, isExist, getAncestorDir
 
 
 class Ui_CFGLoader(object):
 
     def setupUi(self, CFGLoader):
         CFGLoader.setObjectName("CFGLoader")
         CFGLoader.resize(560, 600)
@@ -637,27 +633,27 @@
         self.status_lineEdit.setText("")
         self.status_lineEdit.setStyleSheet("color: rgb(0, 0, 0)")
 
     def browseYAMLFile(self):
         self.resetStatus()
         file_filter = "Config file (*.yaml *.json)"
         input_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Browse config file", 
-                                                              internal_config_dir, file_filter)
+                                                              IN_CONFIG_DIR, file_filter)
         if input_file:
             self.yaml_file_lineEdit.setText(input_file)
             self.readYAML(input_file)
             self.save_pushButton.setDisabled(False)
             self.reload_pushButton.setDisabled(False)
 
     def browseFile(self, par_num):
         file_filter = "File (*.*)"
         input_file, _ = QtWidgets.QFileDialog.getOpenFileName(None, "Browse file", 
-                                                              internal_data_dir, file_filter)
-        input_file = normalizePathFDS(vsensebox_root, input_file)
+                                                              IN_ROOT_DIR, file_filter)
         if input_file:
+            input_file = normalizePathFDS(IN_ROOT_DIR, input_file)
             if par_num == 1:
                 self.par01_value_lineEdit.setText(input_file)
             elif par_num == 2:
                 self.par02_value_lineEdit.setText(input_file)
             elif par_num == 3:
                 self.par03_value_lineEdit.setText(input_file)
             elif par_num == 4:
@@ -812,39 +808,39 @@
             self.status_lineEdit.setStyleSheet("color: rgb(255, 50, 50)")
     
     def saveas(self):
         self.resetStatus()
         config_yaml = self.getConfig()
         file_filter = "File (*.yaml)"
         yaml_file, _ = QtWidgets.QFileDialog.getSaveFileName(None, "Save configuration", 
-                                                             internal_config_dir, file_filter)
+                                                             IN_CONFIG_DIR, file_filter)
         if isExist(getAncestorDir(yaml_file)) and yaml_file != '':
             date_time = str(time.strftime("%Y-%m-%d %Hh%Mm%Ss"))
             try:
                 header = "# Modified " + date_time + "\n"
                 config_yaml = self.getConfig()
                 dumpDocDict(yaml_file, config_yaml, header)
                 self.status_lineEdit.setText("Saved " + date_time)
                 self.status_lineEdit.setStyleSheet("color: rgb(50, 255, 50)")
             except Exception as e:
                 print(e)
                 self.status_lineEdit.setText("Failed to save!")
                 self.status_lineEdit.setStyleSheet("color: rgb(255, 50, 50)")
 
     def checkUITMP(self):
-        if isExist(ui_tmp):
-            with open(ui_tmp) as ui_tmp_file:
-                lines = ui_tmp_file.read().splitlines()
+        if isExist(UI_TMP):
+            with open(UI_TMP) as _ui_tmp_file:
+                lines = _ui_tmp_file.read().splitlines()
                 if len(lines) > 0:
                     if isinstance(lines[0], str):
                         self.yaml_file_lineEdit.setText(lines[0])
                         self.readYAML(lines[0])
                         self.save_pushButton.setDisabled(False)
                         self.reload_pushButton.setDisabled(False)
-            os.remove(ui_tmp)
+            os.remove(UI_TMP)
 
     def reload(self):
         self.resetStatus()
         yaml_file = self.yaml_file_lineEdit.text()
         if isExist(yaml_file):
             try:
                 self.clearPar()
@@ -863,12 +859,12 @@
         CFGLoader.close()
 
 
 if __name__ == "__main__":
     import sys
     app = QtWidgets.QApplication(sys.argv)
     CFGLoader = QtWidgets.QWidget()
-    CFGLoader.setWindowIcon(QtGui.QIcon(joinFPathFull(current_dir, "assets/settings.ico")))
+    CFGLoader.setWindowIcon(QtGui.QIcon(joinFPathFull(CUR_DIR, "assets/settings.ico")))
     ui = Ui_CFGLoader()
     ui.setupUi(CFGLoader)
     CFGLoader.show()
     sys.exit(app.exec())
```

### Comparing `vsensebox-0.0.3/vsensebox/modules/detectors/detectors.py` & `vsensebox-0.0.4/vsensebox/modules/detectors/detectors.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/detectors/yolo_classic.py` & `vsensebox-0.0.4/vsensebox/modules/detectors/yolo_classic.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/detectors/yolo_ultralytics.py` & `vsensebox-0.0.4/vsensebox/modules/detectors/yolo_ultralytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             numpy_dets = dets[0].cuda().cpu().to("cpu").numpy()
         dt_boxes_xyxy = numpy_dets.boxes.xyxy
         dt_confidences = numpy_dets.boxes.conf
         dt_classes = numpy_dets.boxes.cls
         dt_keypoints = dets[0].keypoints
         if dt_keypoints is not None:
             for box_xyxy, conf, kp, cl in zip(dt_boxes_xyxy, dt_confidences, 
-                                          reversed(dt_keypoints), dt_classes):
+                                              reversed(dt_keypoints), dt_classes):
                 box_xyxy = box_xyxy.astype(int)
                 box_xywh = to_xywh(box_xyxy)
                 if box_xywh[2] >= self.cfg.min_width:
                     boxes_xywh.append(box_xywh)
                     boxes_xyxy.append(box_xyxy)
                     keypoint = kp.data[0]
                     keypoints.append(keypoint)
```

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/centroid.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/centroid.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,33 @@
         self.previous_ct = []
         self.previous_id = []
         self.current_ct = []
         self.current_id = []
         self.max_spread = cfg.max_spread
         self.pref_y = cfg.pref_y
 
-    def __generateID__(self):
+    def _generateID(self):
         self.used_ids = list(set(self.used_ids))
         if len(self.used_ids) == 0: aID = 0
         else: aID = max(self.used_ids) + 1
         self.used_ids.append(aID)
         return aID
     
-    def __findRepspoint__(self, box_xyxy):
+    def _findRepspoint(self, box_xyxy):
         x = int((box_xyxy[0] + box_xyxy[2]) / 2)
         y = 0
         if self.pref_y.lower() == "center":
             y = int((box_xyxy[1] + box_xyxy[3]) / 2)
         elif self.pref_y.lower() == "bottom":
             y = max(box_xyxy[1], box_xyxy[3])
         else:
             y = min(box_xyxy[1], box_xyxy[3])
         return (x, y)
 
-    def __findPID__(self, point):
+    def _findPID(self, point):
         pindex = -1
         min_d = 8192
         i = 0
         for ct in self.previous_ct:
             d = dist(point, ct)
             if d < min_d:
                 min_d = d
@@ -81,29 +81,29 @@
 
         self.previous_ct = self.current_ct
         self.previous_id = self.current_id
 
         self.current_id = []
         self.used_ids = []
 
-        self.current_ct = [self.__findRepspoint__(b) for b in boxes_xyxy]
+        self.current_ct = [self._findRepspoint(b) for b in boxes_xyxy]
         hang_indexes_in_clist = []
         len_bb = len(boxes_xyxy)
         if len_bb > 0:
             for i in range(0, len_bb):
                 self.current_id.append(-1)
-                pindex = self.__findPID__(self.current_ct[i])
+                pindex = self._findPID(self.current_ct[i])
                 if pindex >= 0:
                     prev_id = self.previous_id[pindex]
                     if prev_id in self.used_ids:
                         hang_indexes_in_clist.append(i)
                     else:
                         self.current_id[i] = prev_id
                         self.used_ids.append(prev_id)
                 else:
                     hang_indexes_in_clist.append(i)
             len_hlist = len(hang_indexes_in_clist)
             if len_hlist > 0:
                 for index in hang_indexes_in_clist:
-                    self.current_id[index] = self.__generateID__()
+                    self.current_id[index] = self._generateID()
         
         return boxes_xyxy, self.current_id
```

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/deepsort.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/deepsort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/sort.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/trackers.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/trackers.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/box_matching.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/box_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/detection.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/detection_yolo.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/generate_detections.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/generate_detections.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/iou_matching.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/kalman_filter.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/linear_assignment.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/nn_matching.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/nn_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/preprocessing.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/sort.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/track.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/modules/trackers/utils/tracker.py` & `vsensebox-0.0.4/vsensebox/modules/trackers/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/utils/about.py` & `vsensebox-0.0.4/vsensebox/utils/about.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.0.3/vsensebox/utils/commontools.py` & `vsensebox-0.0.4/vsensebox/utils/commontools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 import os
 import sys
 import cv2
 import numpy as np
-from pathlib import Path 
 
 
 def getCVMat(img, to_rgb=False):
     """
     :meta private:
     """
     if isinstance(img, str):
@@ -86,14 +85,15 @@
     """
     return os.path.join(main, to_join).replace(os.sep, '/')
 
 def getFileName(input):
     """
     :meta private:
     """
+    from pathlib import Path 
     return Path(input).name
 
 def getGlobalRootDir():
     """
     :meta private:
     """
     current_dir = os.path.dirname(__file__)
```

### Comparing `vsensebox-0.0.3/vsensebox/utils/logtools.py` & `vsensebox-0.0.4/vsensebox/utils/logtools.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 import os
 import time
 import logging
 
-__timestamp__ = str(time.strftime("%Y%m%d_%H%M%S"))
-__vsensebox_root__ = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-__log_dir__ = os.path.join(__vsensebox_root__, "data/logs").replace(os.sep, '/')
-__log_txt_path__ = os.path.join(__log_dir__, "log_" + __timestamp__ + ".txt")
-__max_age__ = 86400 * 1 # 1 DAY
+_TIMESTAMP = str(time.strftime("%Y%m%d_%H%M%S"))
+_VSENSEBOX_ROOT = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
+_LOG_DIR = os.path.join(_VSENSEBOX_ROOT, "data/logs").replace(os.sep, '/')
+_LOG_TXT_PATH = os.path.join(_LOG_DIR, "log_" + _TIMESTAMP + ".txt")
+_MAX_AGE = 86400 * 1 # 1 DAY
 
 # Remove old logs
-if os.path.exists(__log_dir__):
-    for filename in os.listdir(__log_dir__):
+if os.path.exists(_LOG_DIR):
+    for filename in os.listdir(_LOG_DIR):
         if "git" in filename: continue
-        filestamp = os.stat(os.path.join(__log_dir__, filename)).st_mtime
-        if  filestamp < time.time() - __max_age__:
-            os.remove(os.path.join(__log_dir__, filename))
-else: os.makedirs(__log_dir__)
+        filestamp = os.stat(os.path.join(_LOG_DIR, filename)).st_mtime
+        if  filestamp < time.time() - _MAX_AGE:
+            os.remove(os.path.join(_LOG_DIR, filename))
+else: os.makedirs(_LOG_DIR)
 
 # Initial logger
 logging.basicConfig(
-    filename=__log_txt_path__,
+    filename=_LOG_TXT_PATH,
     filemode='a',
     format='%(asctime)s %(levelname)-3s %(message)-3s',
     datefmt='%H:%M:%S',
     level=logging.INFO
 )
 
 # Add header
-with open(__log_txt_path__, 'w+') as log_txt:
+with open(_LOG_TXT_PATH, 'w+') as log_txt:
     log_txt.write("-------------------------------------------------")
     log_txt.write("-------------------------------------------------\n")
     log_txt.write("#################################################")
     log_txt.write("#################################################\n")
     log_txt.write("-------------------------------------------------")
     log_txt.write("-------------------------------------------------\n")
```

### Comparing `vsensebox-0.0.3/vsensebox/utils/visualizetools.py` & `vsensebox-0.0.4/vsensebox/utils/visualizetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # GNU General Public License v3 or later (GPLv3+)
 # Copyright (C) 2024 UMONS-Numediart
 
 
 import cv2
 
 from .commontools import getCVMat
-from .logtools import add_error_log, add_warning_log
+from .logtools import add_warning_log
 
 def draw_boxes(img, 
                ids=[], 
                show_ids=True, 
                boxes_xyxy=[], 
                boxes_confs=[], 
                boxes_color=(255, 255, 0),
```

### Comparing `vsensebox-0.0.3/vsensebox/vsense/vsense.py` & `vsensebox-0.0.4/vsensebox/vsense/vsense.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # VSenseBox - Python toolbox for visual sensing
 # GNU General Public License v3 or later (GPLv3+)
 # Copyright (C) 2024 UMONS-Numediart
 
 
 # Configurations
-from vsensebox.config.configurator import detectors_config_dir, trackers_config_dir, internal_root_dir
+from vsensebox.config.configurator import DET_CONFIG_DIR, TRK_CONFIG_DIR, IN_ROOT_DIR
 from vsensebox.config.confighelper import getCFGDict
 
 # Utils & tools
 from vsensebox.modules.detectors import checkDet
 from vsensebox.modules.trackers import checkTrk
 from vsensebox.utils.commontools import getCVMat, joinFPathFull, getAncestorDir
 
 # Default detector
-default_det = getCFGDict(joinFPathFull(detectors_config_dir, 'default.yaml'))
-default_detector_yaml = joinFPathFull(internal_root_dir, default_det['config_yaml'])
-det_rel_to_root = True if getAncestorDir(default_det['config_yaml']) == 'config/detectors' else False
+DEFAULT_DET_CONFIG = getCFGDict(joinFPathFull(DET_CONFIG_DIR, 'default.yaml'))
+DEFAULT_DET_YAML = joinFPathFull(IN_ROOT_DIR, DEFAULT_DET_CONFIG['config_yaml'])
+DET_YAML_TO_ROOT = True if getAncestorDir(DEFAULT_DET_CONFIG['config_yaml']) == 'config/detectors' else False
 
 # Default tracker
-default_trk = getCFGDict(joinFPathFull(trackers_config_dir, 'default.yaml'))
-default_tracker_yaml = joinFPathFull(internal_root_dir, default_trk['config_yaml'])
-trk_rel_to_root = True if getAncestorDir(default_trk['config_yaml']) == 'config/trackers' else False
+DEFAULT_TRK_CONFIG = getCFGDict(joinFPathFull(TRK_CONFIG_DIR, 'default.yaml'))
+DEFAULT_TRK_YAML = joinFPathFull(IN_ROOT_DIR, DEFAULT_TRK_CONFIG['config_yaml'])
+TRK_YAML_TO_ROOT = True if getAncestorDir(DEFAULT_TRK_CONFIG['config_yaml']) == 'config/trackers' else False
 
 
 class VSense(object):
 
     """
     VSense is used to operate the object detection and tracking.
 
@@ -53,19 +53,19 @@
         config_yaml : str, default=None
             Path of YAML config file.
         img_is_mat : bool, default=False
             Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like object.
         """
         if not img_is_mat: img = getCVMat(img)
         if config_yaml is None:
-            config_yaml = default_detector_yaml
-            self._det_rel_to_root = det_rel_to_root
+            config_yaml = DEFAULT_DET_YAML
+            self._det_rel_to_root = DET_YAML_TO_ROOT
         if self._yaml_det != config_yaml:
             self._detector = checkDet(detector=self._detector, config_yaml=config_yaml, 
-                                    relative_to_vsensebox_root=self._det_rel_to_root)
+                                      relative_to_vsensebox_root=self._det_rel_to_root)
         else:
             self._yaml_det = config_yaml
         img, boxes_xywh, boxes_xyxy, keypoints, confs, cls = self._detector.detect(img)
         self.assets.update(
             boxes_xywh=boxes_xywh, 
             boxes_xyxy=boxes_xyxy, 
             keypoints=keypoints, 
@@ -83,19 +83,19 @@
         config_yaml : str, default=None
             Path of YAML config file.
         img_is_mat : bool, default=False
             Speed up the function by telling whether the :obj:`img` is :obj:`Mat` like object.
         """
         if not img_is_mat: img = getCVMat(img)
         if config_yaml is None:
-            config_yaml = default_tracker_yaml
-            self._trk_rel_to_root = trk_rel_to_root
+            config_yaml = DEFAULT_TRK_YAML
+            self._trk_rel_to_root = TRK_YAML_TO_ROOT
         if self._yaml_trk != config_yaml:
             self._tracker = checkTrk(tracker=self._tracker, config_yaml=config_yaml, 
-                                    relative_to_vsensebox_root=self._trk_rel_to_root)
+                                     relative_to_vsensebox_root=self._trk_rel_to_root)
         else:
             self._yaml_trk = config_yaml
         boxes_xyxy, self.assets.ids = self._tracker.update(
             self.assets.boxes_xyxy, 
             self.assets.boxes_confs, 
             boxes_cls=self.assets.boxes_cls, 
             img=img
```

### Comparing `vsensebox-0.0.3/vsensebox.egg-info/PKG-INFO` & `vsensebox-0.0.4/vsensebox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.0.3
+Version: 0.0.4
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vsensebox-0.0.3/vsensebox.egg-info/SOURCES.txt` & `vsensebox-0.0.4/vsensebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

