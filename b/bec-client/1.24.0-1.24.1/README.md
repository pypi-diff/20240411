# Comparing `tmp/bec_client-1.24.0.tar.gz` & `tmp/bec_client-1.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_client-1.24.0.tar", last modified: Wed Apr 10 13:44:07 2024, max compression
+gzip compressed data, was "bec_client-1.24.1.tar", last modified: Wed Apr 10 15:06:10 2024, max compression
```

## Comparing `bec_client-1.24.0.tar` & `bec_client-1.24.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.363772 bec_client-1.24.0/
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 13:44:07.363772 bec_client-1.24.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.361772 bec_client-1.24.0/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/beamline_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/bec_ipython_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/bec_magics.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/bec_startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.361772 bec_client-1.24.0/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 13:43:56.000000 bec_client-1.24.0/bec_client/callbacks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/callbacks/ipython_live_updates.py
--rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/callbacks/live_table.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/callbacks/move_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/callbacks/scan_progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.361772 bec_client-1.24.0/bec_client/high_level_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 13:43:56.000000 bec_client-1.24.0/bec_client/high_level_interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/high_level_interfaces/spec_hli.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.361772 bec_client-1.24.0/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.362772 bec_client-1.24.0/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/LamNI/load_additional_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.362772 bec_client-1.24.0/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 13:43:56.000000 bec_client-1.24.0/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.362772 bec_client-1.24.0/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 13:43:56.000000 bec_client-1.24.0/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 13:43:56.000000 bec_client-1.24.0/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.362772 bec_client-1.24.0/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.362772 bec_client-1.24.0/bec_client/plugins/flomni/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/flomni/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    73850 2024-04-10 13:07:13.000000 bec_client-1.24.0/bec_client/plugins/flomni/flomni.py
--rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/flomni/flomni_optics_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/plugins/flomni/x_ray_eye_align.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/progressbar.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-10 11:18:35.000000 bec_client-1.24.0/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 13:44:07.363772 bec_client-1.24.0/bec_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1521 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 13:44:07.000000 bec_client-1.24.0/bec_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-10 13:44:07.364772 bec_client-1.24.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2118 2024-04-10 13:44:05.000000 bec_client-1.24.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 15:06:10.933711 bec_client-1.24.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.931711 bec_client-1.24.1/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       93 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/beamline_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4787 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_ipython_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_magics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/bec_startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/callbacks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9948 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/ipython_live_updates.py
+-rw-rw-rw-   0 root         (0) root         (0)    11955 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/live_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/move_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/scan_progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/high_level_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/high_level_interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/high_level_interfaces/spec_hli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5508 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      872 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    54693 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.932711 bec_client-1.24.1/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 15:06:00.000000 bec_client-1.24.1/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client/plugins/flomni/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    73850 2024-04-10 13:07:13.000000 bec_client-1.24.1/bec_client/plugins/flomni/flomni.py
+-rw-rw-rw-   0 root         (0) root         (0)     6391 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/flomni_optics_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8902 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/plugins/flomni/x_ray_eye_align.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)    11165 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/progressbar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-04-10 11:18:35.000000 bec_client-1.24.1/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 15:06:10.933711 bec_client-1.24.1/bec_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1521 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 15:06:10.000000 bec_client-1.24.1/bec_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-10 15:06:10.934711 bec_client-1.24.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2024-04-10 15:06:09.000000 bec_client-1.24.1/setup.py
```

### Comparing `bec_client-1.24.0/bec_client/beamline_mixin.py` & `bec_client-1.24.1/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/bec_ipython_client.py` & `bec_client-1.24.1/bec_client/bec_ipython_client.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/bec_magics.py` & `bec_client-1.24.1/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/bec_startup.py` & `bec_client-1.24.1/bec_client/bec_startup.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/callbacks/ipython_live_updates.py` & `bec_client-1.24.1/bec_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/callbacks/live_table.py` & `bec_client-1.24.1/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/callbacks/move_device.py` & `bec_client-1.24.1/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/callbacks/scan_progress.py` & `bec_client-1.24.1/bec_client/callbacks/scan_progress.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/callbacks/utils.py` & `bec_client-1.24.1/bec_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/high_level_interfaces/spec_hli.py` & `bec_client-1.24.1/bec_client/high_level_interfaces/spec_hli.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/main.py` & `bec_client-1.24.1/bec_client/main.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_client-1.24.1/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_client-1.24.1/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_client-1.24.1/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/SLS/sls_info.py` & `bec_client-1.24.1/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/XTreme/x-treme.py` & `bec_client-1.24.1/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/cSAXS/beamline_info.py` & `bec_client-1.24.1/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/cSAXS/csaxs_bl_checks.py` & `bec_client-1.24.1/bec_client/plugins/cSAXS/csaxs_bl_checks.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/flomni/flomni.py` & `bec_client-1.24.1/bec_client/plugins/flomni/flomni.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/flomni/flomni_optics_mixin.py` & `bec_client-1.24.1/bec_client/plugins/flomni/flomni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/plugins/flomni/x_ray_eye_align.py` & `bec_client-1.24.1/bec_client/plugins/flomni/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/prettytable.py` & `bec_client-1.24.1/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/progressbar.py` & `bec_client-1.24.1/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client/signals.py` & `bec_client-1.24.1/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/bec_client.egg-info/SOURCES.txt` & `bec_client-1.24.1/bec_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/setup.cfg` & `bec_client-1.24.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_client-1.24.0/setup.py` & `bec_client-1.24.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 
-__version__ = "1.24.0"
+__version__ = "1.24.1"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

