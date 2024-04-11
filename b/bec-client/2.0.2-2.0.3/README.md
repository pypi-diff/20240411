# Comparing `tmp/bec_client-2.0.2.tar.gz` & `tmp/bec_client-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_client-2.0.2.tar", last modified: Thu Apr 11 08:36:44 2024, max compression
+gzip compressed data, was "bec_client-2.0.3.tar", last modified: Thu Apr 11 12:57:35 2024, max compression
```

## Comparing `bec_client-2.0.2.tar` & `bec_client-2.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.068462 bec_client-2.0.2/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 08:36:44.068462 bec_client-2.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.066462 bec_client-2.0.2/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/bec_ipython_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/bec_magics.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.066462 bec_client-2.0.2/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_client-2.0.2/bec_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.066462 bec_client-2.0.2/bec_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_client-2.0.2/bec_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/high_level_interfaces/spec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.066462 bec_client-2.0.2/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.067462 bec_client-2.0.2/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.067462 bec_client-2.0.2/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_client-2.0.2/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.067462 bec_client-2.0.2/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_client-2.0.2/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 08:36:34.000000 bec_client-2.0.2/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.067462 bec_client-2.0.2/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/cSAXS/csaxs_bl_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.067462 bec_client-2.0.2/bec_client/plugins/flomni/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/flomni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75021 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/flomni/flomni.py
--rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/flomni/flomni_optics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/plugins/flomni/x_ray_eye_align.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-11 01:29:15.000000 bec_client-2.0.2/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:36:44.068462 bec_client-2.0.2/bec_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 08:36:44.000000 bec_client-2.0.2/bec_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-11 08:36:44.069462 bec_client-2.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-11 08:36:42.000000 bec_client-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.047402 bec_client-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 12:57:35.047402 bec_client-2.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.045402 bec_client-2.0.3/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/beamline_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/bec_ipython_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/bec_magics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/bec_startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/callbacks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/callbacks/ipython_live_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/callbacks/live_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/callbacks/move_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/callbacks/scan_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/high_level_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/high_level_interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/high_level_interfaces/spec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.046402 bec_client-2.0.3/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.047402 bec_client-2.0.3/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/cSAXS/csaxs_bl_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.047402 bec_client-2.0.3/bec_client/plugins/flomni/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/flomni/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77116 2024-04-11 12:57:24.000000 bec_client-2.0.3/bec_client/plugins/flomni/flomni.py
+-rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/flomni/flomni_optics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/plugins/flomni/x_ray_eye_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-11 12:02:54.000000 bec_client-2.0.3/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:57:35.047402 bec_client-2.0.3/bec_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      406 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 12:57:35.000000 bec_client-2.0.3/bec_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-11 12:57:35.048403 bec_client-2.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2024-04-11 12:57:33.000000 bec_client-2.0.3/setup.py
```

### Comparing `bec_client-2.0.2/bec_client/beamline_mixin.py` & `bec_client-2.0.3/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/bec_ipython_client.py` & `bec_client-2.0.3/bec_client/bec_ipython_client.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/bec_magics.py` & `bec_client-2.0.3/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/bec_startup.py` & `bec_client-2.0.3/bec_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/callbacks/ipython_live_updates.py` & `bec_client-2.0.3/bec_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/callbacks/live_table.py` & `bec_client-2.0.3/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/callbacks/move_device.py` & `bec_client-2.0.3/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/callbacks/scan_progress.py` & `bec_client-2.0.3/bec_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/callbacks/utils.py` & `bec_client-2.0.3/bec_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/high_level_interfaces/spec_hli.py` & `bec_client-2.0.3/bec_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/main.py` & `bec_client-2.0.3/bec_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_client-2.0.3/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_client-2.0.3/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_client-2.0.3/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/SLS/sls_info.py` & `bec_client-2.0.3/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/XTreme/x-treme.py` & `bec_client-2.0.3/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/cSAXS/beamline_info.py` & `bec_client-2.0.3/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_client-2.0.3/bec_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/flomni/flomni.py` & `bec_client-2.0.3/bec_client/plugins/flomni/flomni.py`

 * *Files 3% similar despite different names*

```diff
@@ -1353,14 +1353,25 @@
         return val
 
     @tomo_stitch_overlap.setter
     def tomo_stitch_overlap(self, val: float):
         self.client.set_global_var("tomo_stitch_overlap", val)
 
     @property
+    def golden_projections_at_0_deg_for_damage_estimation(self):
+        val = self.client.get_global_var("golden_projections_at_0_deg_for_damage_estimation")
+        if val is None:
+            return 0
+        return val
+
+    @golden_projections_at_0_deg_for_damage_estimation.setter
+    def golden_projections_at_0_deg_for_damage_estimation(self, val: float):
+        self.client.set_global_var("golden_projections_at_0_deg_for_damage_estimation", val)
+
+    @property
     def golden_ratio_bunch_size(self):
         val = self.client.get_global_var("golden_ratio_bunch_size")
         if val is None:
             return 20
         return val
 
     @golden_ratio_bunch_size.setter
@@ -1581,14 +1592,20 @@
                     ii = 0
                 else:
                     ii = projection_number
                 while True:
                     angle, subtomo_number = self._golden(ii, self.golden_ratio_bunch_size, 180, 1)
                     if previous_subtomo_number != subtomo_number:
                         self._write_subtomo_to_scilog(subtomo_number)
+                        if (
+                            subtomo_number % 2 == 1
+                            and ii > 10
+                            and self.golden_projections_at_0_deg_for_damage_estimation == 1
+                        ):
+                            self._tomo_scan_at_angle(0, subtomo_number)
                         previous_subtomo_number = subtomo_number
                     self._tomo_scan_at_angle(angle, subtomo_number)
                     ii += 1
                     if (
                         ii > self.golden_max_number_of_projections
                         and self.golden_max_number_of_projections > 0
                     ):
@@ -1605,14 +1622,20 @@
                     ii = projection_number
                 while True:
                     angle, subtomo_number = self._golden_equally_spaced(
                         ii, int(180 / self.tomo_angle_stepsize), 180, 1, 0
                     )
                     if previous_subtomo_number != subtomo_number:
                         self._write_subtomo_to_scilog(subtomo_number)
+                        if (
+                            subtomo_number % 2 == 1
+                            and ii > 10
+                            and self.golden_projections_at_0_deg_for_damage_estimation == 1
+                        ):
+                            self._tomo_scan_at_angle(0, subtomo_number)
                         previous_subtomo_number = subtomo_number
                     self._tomo_scan_at_angle(angle, subtomo_number)
                     ii += 1
                     if (
                         ii > self.golden_max_number_of_projections
                         and self.golden_max_number_of_projections > 0
                     ):
@@ -1786,24 +1809,32 @@
         if self.tomo_type == 2:
             print("\x1b[1mTomo type 2:\x1b[0m Golden ratio tomography")
             print(f"Sorted in bunches of: {self.golden_ratio_bunch_size}")
             if self.golden_max_number_of_projections > 0:
                 print(f"ending after {self.golden_max_number_of_projections} projections")
             else:
                 print("ending by manual interruption")
+            if self.golden_projections_at_0_deg_for_damage_estimation == 1:
+                print(
+                    "repeating prjections at 0 degrees at the beginning of every second subtomogram"
+                )
         if self.tomo_type == 3:
             print(
                 "\x1b[1mTomo type 3:\x1b[0m Equally spaced tomography, golden ratio starting angle"
             )
             print(f"Number of projections per sub-tomogram: {180/self.tomo_angle_stepsize}")
             print(f"Angular step within sub-tomogram:    {self.tomo_angle_stepsize} degrees")
             if self.golden_max_number_of_projections > 0:
                 print(f"ending after {self.golden_max_number_of_projections} projections")
             else:
                 print("ending by manual interruption")
+            if self.golden_projections_at_0_deg_for_damage_estimation == 1:
+                print(
+                    "repeating prjections at 0 degrees at the beginning of every second subtomogram"
+                )
         print(f"\nSample name: {self.sample_name}\n")
 
         user_input = input("Are these parameters correctly set for your scan? [Y/n]")
         if user_input == "y" or user_input == "":
             print("... excellent!")
         else:
             self.tomo_countingtime = self._get_val("<ctime> s", self.tomo_countingtime, float)
@@ -1837,27 +1868,37 @@
                     int,
                 )
                 self.golden_max_number_of_projections = self._get_val(
                     "Stop after number of projections (zero for endless)",
                     self.golden_max_number_of_projections,
                     int,
                 )
+                self.golden_projections_at_0_deg_for_damage_estimation = self._get_val(
+                    "Repeat projections at 0 deg every second subtomo 1/0 ?",
+                    self.golden_projections_at_0_deg_for_damage_estimation,
+                    int,
+                )
 
             if self.tomo_type == 3:
                 numprj = self._get_val(
                     "Number of projections per sub-tomogram",
                     int(180 / self.tomo_angle_stepsize),
                     int,
                 )
                 self.tomo_angle_stepsize = 180 / numprj
                 self.golden_max_number_of_projections = self._get_val(
                     "Stop after number of projections (zero for endless)",
                     self.golden_max_number_of_projections,
                     int,
                 )
+                self.golden_projections_at_0_deg_for_damage_estimation = self._get_val(
+                    "Repeat projections at 0 deg every second subtomo",
+                    self.golden_projections_at_0_deg_for_damage_estimation,
+                    int,
+                )
 
     @staticmethod
     def _get_val(msg: str, default_value, data_type):
         return data_type(input(f"{msg} ({default_value}): ") or default_value)
 
     def rt_off(self):
         dev.rtx.enabled = False
```

### Comparing `bec_client-2.0.2/bec_client/plugins/flomni/flomni_optics_mixin.py` & `bec_client-2.0.3/bec_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/plugins/flomni/x_ray_eye_align.py` & `bec_client-2.0.3/bec_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/prettytable.py` & `bec_client-2.0.3/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/progressbar.py` & `bec_client-2.0.3/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client/signals.py` & `bec_client-2.0.3/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/bec_client.egg-info/SOURCES.txt` & `bec_client-2.0.3/bec_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/setup.cfg` & `bec_client-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_client-2.0.2/setup.py` & `bec_client-2.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

