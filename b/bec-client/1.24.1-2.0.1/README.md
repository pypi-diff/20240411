# Comparing `tmp/bec_client-1.24.1.tar.gz` & `tmp/bec_client-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_client-1.24.1.tar", last modified: Wed Apr 10 15:06:10 2024, max compression
+gzip compressed data, was "bec_client-2.0.1.tar", last modified: Thu Apr 11 06:21:54 2024, max compression
```

## Comparing `bec_client-1.24.1.tar` & `bec_client-2.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 15:06:10.933711 bec_client-1.24.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.931711 bec_client-1.24.1/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_ipython_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_magics.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/high_level_interfaces/spec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client/plugins/flomni/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    73850 2024-04-10 13:07:13.000000 bec_client-1.24.1/bec_client/plugins/flomni/flomni.py
--rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/flomni_optics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/x_ray_eye_align.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-10 15:06:10.934711 bec_client-1.24.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2118 2024-04-10 15:06:09.000000 bec_client-1.24.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.697401 bec_client-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 06:21:54.697401 bec_client-2.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.695401 bec_client-2.0.1/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/beamline_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/bec_ipython_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/bec_magics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/bec_startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_client-2.0.1/bec_client/callbacks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/callbacks/ipython_live_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/callbacks/live_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/callbacks/move_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/callbacks/scan_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/high_level_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_client-2.0.1/bec_client/high_level_interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/high_level_interfaces/spec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_client-2.0.1/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.696401 bec_client-2.0.1/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_client-2.0.1/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 06:21:44.000000 bec_client-2.0.1/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.697401 bec_client-2.0.1/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.697401 bec_client-2.0.1/bec_client/plugins/flomni/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/flomni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75021 2024-04-11 01:23:09.000000 bec_client-2.0.1/bec_client/plugins/flomni/flomni.py
+-rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/flomni/flomni_optics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/plugins/flomni/x_ray_eye_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-10 11:18:35.000000 bec_client-2.0.1/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:21:54.697401 bec_client-2.0.1/bec_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 06:21:54.000000 bec_client-2.0.1/bec_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-11 06:21:54.700401 bec_client-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-11 06:21:52.000000 bec_client-2.0.1/setup.py
```

### Comparing `bec_client-1.24.1/bec_client/beamline_mixin.py` & `bec_client-2.0.1/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/bec_ipython_client.py` & `bec_client-2.0.1/bec_client/bec_ipython_client.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/bec_magics.py` & `bec_client-2.0.1/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/bec_startup.py` & `bec_client-2.0.1/bec_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/callbacks/ipython_live_updates.py` & `bec_client-2.0.1/bec_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/callbacks/live_table.py` & `bec_client-2.0.1/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/callbacks/move_device.py` & `bec_client-2.0.1/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/callbacks/scan_progress.py` & `bec_client-2.0.1/bec_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/callbacks/utils.py` & `bec_client-2.0.1/bec_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/high_level_interfaces/spec_hli.py` & `bec_client-2.0.1/bec_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/main.py` & `bec_client-2.0.1/bec_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_client-2.0.1/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_client-2.0.1/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_client-2.0.1/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/SLS/sls_info.py` & `bec_client-2.0.1/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/XTreme/x-treme.py` & `bec_client-2.0.1/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/cSAXS/beamline_info.py` & `bec_client-2.0.1/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_client-2.0.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/flomni/flomni.py` & `bec_client-2.0.1/bec_client/plugins/flomni/flomni.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,21 +411,15 @@
 
     def laser_tracker_show_all(self):
         dev.rtx.controller.laser_tracker_show_all()
 
     def laser_tracker_on(self):
         dev.rtx.controller.laser_tracker_on()
         time.sleep(0.2)
-        signal = dev.rtx.controller.read_ssi_interferometer(1)
-        if signal < 10000:
-            time.sleep(1)
-            if signal < 10000:
-                print("\x1b[91mThe signal of the tracker is low. Please readjust!\x1b[0m")
-
-    # change hard coded number to a user parameter!
+        self._laser_tracker_check_signalstrength()
 
     def laser_tracker_off(self):
         dev.rtx.controller.laser_tracker_off()
 
     def show_signal_strength_interferometer(self):
         dev.rtx.controller.show_signal_strength_interferometer()
 
@@ -922,15 +916,20 @@
                     f"Could not find default correction file {self.default_correction_file}."
                 )
                 logger.warning("Not applying any correction.")
 
     def reset_tomo_alignment_fit(self):
         self.client.delete_global_var("tomo_alignment_fit")
 
-    def read_alignment_offset(self, dir_path=os.path.expanduser("~/Data10/specES1/internal/")):
+    def read_alignment_offset(
+        self,
+        dir_path=os.path.expanduser("~/Data10/specES1/internal/"),
+        setup="flomni",
+        use_vertical_default_values=True,
+    ):
         """
         Read the alignment offset from the given directory and set the global parameter
         tomo_alignment_fit.
 
         Args:
             dir_path (str, optional): The directory to read the alignment offset from. Defaults to os.path.expanduser("~/Data10/specES1/internal/").
         """
@@ -955,30 +954,59 @@
 
         with open(os.path.join(dir_path, "ptychotomoalign_Ay3.txt"), "r") as file:
             tomo_alignment_fit[1][3] = file.readline()
 
         with open(os.path.join(dir_path, "ptychotomoalign_Cy3.txt"), "r") as file:
             tomo_alignment_fit[1][4] = file.readline()
 
-        self.client.set_global_var("tomo_alignment_fit", tomo_alignment_fit.tolist())
-        # x amp, phase, offset, y amp, phase, offset, 3rd order amp, 3rd order phase
-        #  0 0    0 1    0 2     1 0    1 1    1 2       1 3           1 4
-
-        print("New alignment parameters loaded")
+        print("New alignment parameters loaded:")
         print(
             f"X Amplitude {tomo_alignment_fit[0][0]}, "
             f"X Phase {tomo_alignment_fit[0][1]}, "
             f"X Offset {tomo_alignment_fit[0][2]}, "
             f"Y Amplitude {tomo_alignment_fit[1][0]}, "
             f"Y Phase {tomo_alignment_fit[1][1]}, "
             f"Y Offset {tomo_alignment_fit[1][2]}, "
             f"Y 3rd Order Amplitude {tomo_alignment_fit[1][3]}, "
-            f"Y 3rd Order Phase {tomo_alignment_fit[1][4]}."
+            f"Y 3rd Order Phase {tomo_alignment_fit[1][4]} ."
         )
 
+        if use_vertical_default_values:
+            print(
+                f"Using default values for vertical alignment for setup {setup}. Optional: use_vertical_default_values=False"
+            )
+            if setup == "flomni":
+                tomo_alignment_fit[1][0] = 0
+                tomo_alignment_fit[1][1] = 0
+                tomo_alignment_fit[1][2] = 0
+                tomo_alignment_fit[1][3] = 0
+                tomo_alignment_fit[1][4] = 0
+            elif setup == "omny":
+                tomo_alignment_fit[1][0] = 2.588628
+                tomo_alignment_fit[1][1] = -2.385422
+                tomo_alignment_fit[1][2] = 0
+                tomo_alignment_fit[1][3] = 1.010583
+                tomo_alignment_fit[1][4] = -1.359157
+
+            print("Follwing parameters will be used:")
+            print(
+                f"X Amplitude {tomo_alignment_fit[0][0]}, "
+                f"X Phase {tomo_alignment_fit[0][1]}, "
+                f"X Offset {tomo_alignment_fit[0][2]}, "
+                f"Y Amplitude {tomo_alignment_fit[1][0]}, "
+                f"Y Phase {tomo_alignment_fit[1][1]}, "
+                f"Y Offset {tomo_alignment_fit[1][2]}, "
+                f"Y 3rd Order Amplitude {tomo_alignment_fit[1][3]}, "
+                f"Y 3rd Order Phase {tomo_alignment_fit[1][4]} ."
+            )
+
+        self.client.set_global_var("tomo_alignment_fit", tomo_alignment_fit.tolist())
+        # x amp, phase, offset, y amp, phase, offset, 3rd order amp, 3rd order phase
+        #  0 0    0 1    0 2     1 0    1 1    1 2       1 3           1 4
+
     def get_alignment_offset(self, angle: float):
         """
         Compute the alignment offset for the given angle.
 
         Args:
             angle (float): The angle to compute the alignment offset for.
 
@@ -1693,14 +1721,15 @@
 
     def tomo_scan_projection(self, angle: float):
         scans = builtins.__dict__.get("scans")
 
         # additional_correction = self.align.compute_additional_correction(angle)
         # additional_correction_2 = self.align.compute_additional_correction_2(angle)
         # correction_xeye_mu = self.align.lamni_compute_additional_correction_xeye_mu(angle)
+
         offsets = self.get_alignment_offset(angle)
         sum_offset_x = offsets[0]
         sum_offset_y = (
             offsets[1]
             - self.compute_additional_correction_y(angle)
             - self.compute_additional_correction_y_2(angle)
         )
```

### Comparing `bec_client-1.24.1/bec_client/plugins/flomni/flomni_optics_mixin.py` & `bec_client-2.0.1/bec_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/plugins/flomni/x_ray_eye_align.py` & `bec_client-2.0.1/bec_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/prettytable.py` & `bec_client-2.0.1/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/progressbar.py` & `bec_client-2.0.1/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client/signals.py` & `bec_client-2.0.1/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/bec_client.egg-info/SOURCES.txt` & `bec_client-2.0.1/bec_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/setup.cfg` & `bec_client-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.1/setup.py` & `bec_client-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "1.24.1"
+__version__ = "2.0.1"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

