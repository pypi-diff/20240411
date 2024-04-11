# Comparing `tmp/pygmtsar-2024.3.15.post7.tar.gz` & `tmp/pygmtsar-2024.3.15.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtsar-2024.3.15.post7.tar", last modified: Sat Apr  6 16:13:18 2024, max compression
+gzip compressed data, was "pygmtsar-2024.3.15.post8.tar", last modified: Thu Apr 11 18:25:57 2024, max compression
```

## Comparing `pygmtsar-2024.3.15.post7.tar` & `pygmtsar-2024.3.15.post8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.516048 pygmtsar-2024.3.15.post7/
--rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.3.15.post7/LICENSE.txt
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-06 16:13:18.515703 pygmtsar-2024.3.15.post7/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.3.15.post7/README.md
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.514343 pygmtsar-2024.3.15.post7/pygmtsar/
--rw-r--r--   0 mbg        (501) staff       (20)    20813 2024-03-28 13:09:48.000000 pygmtsar-2024.3.15.post7/pygmtsar/ASF.py
--rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.3.15.post7/pygmtsar/AWS.py
--rw-r--r--   0 mbg        (501) staff       (20)     7454 2024-03-15 10:56:24.000000 pygmtsar-2024.3.15.post7/pygmtsar/ESA.py
--rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.3.15.post7/pygmtsar/GMT.py
--rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/IO.py
--rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.3.15.post7/pygmtsar/NCubeVTK.py
--rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.3.15.post7/pygmtsar/PRM.py
--rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.3.15.post7/pygmtsar/PRM_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    18986 2024-04-05 07:42:45.000000 pygmtsar-2024.3.15.post7/pygmtsar/S1.py
--rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack.py
--rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_align.py
--rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_base.py
--rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_dem.py
--rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_detrend.py
--rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_export.py
--rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_geocode.py
--rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_incidence.py
--rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_landmask.py
--rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_multilooking.py
--rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_orbits.py
--rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_phasediff.py
--rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_prm.py
--rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_ps.py
--rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe.py
--rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe_gmtsar.py
--rw-r--r--   0 mbg        (501) staff       (20)    46250 2024-04-05 20:26:03.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_sbas.py
--rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_stl.py
--rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_tidal.py
--rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_topo.py
--rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans.py
--rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans_inv.py
--rw-r--r--   0 mbg        (501) staff       (20)    26491 2024-03-10 08:58:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap.py
--rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap_snaphu.py
--rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.3.15.post7/pygmtsar/Tiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.3.15.post7/pygmtsar/XYZTiles.py
--rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.3.15.post7/pygmtsar/_Stack_merge.py
--rw-r--r--   0 mbg        (501) staff       (20)     1061 2024-04-05 20:28:55.000000 pygmtsar-2024.3.15.post7/pygmtsar/__init__.py
--rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.3.15.post7/pygmtsar/datagrid.py
--rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.3.15.post7/pygmtsar/tqdm_dask.py
--rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.3.15.post7/pygmtsar/tqdm_joblib.py
--rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.3.15.post7/pygmtsar/utils.py
-drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-06 16:13:18.515366 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/
--rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/PKG-INFO
--rw-r--r--   0 mbg        (501) staff       (20)     1132 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/SOURCES.txt
--rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/dependency_links.txt
--rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/requires.txt
--rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-06 16:13:18.000000 pygmtsar-2024.3.15.post7/pygmtsar.egg-info/top_level.txt
--rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-06 16:13:18.516100 pygmtsar-2024.3.15.post7/setup.cfg
--rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-03-08 07:02:25.000000 pygmtsar-2024.3.15.post7/setup.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.762517 pygmtsar-2024.3.15.post8/
+-rw-r--r--   0 mbg        (501) staff       (20)     1563 2023-04-01 05:11:16.000000 pygmtsar-2024.3.15.post8/LICENSE.txt
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-11 18:25:57.762271 pygmtsar-2024.3.15.post8/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)    11914 2024-03-18 16:22:31.000000 pygmtsar-2024.3.15.post8/README.md
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.760670 pygmtsar-2024.3.15.post8/pygmtsar/
+-rw-r--r--   0 mbg        (501) staff       (20)    20813 2024-03-28 13:09:48.000000 pygmtsar-2024.3.15.post8/pygmtsar/ASF.py
+-rw-r--r--   0 mbg        (501) staff       (20)      927 2024-03-14 06:45:34.000000 pygmtsar-2024.3.15.post8/pygmtsar/AWS.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7454 2024-03-15 10:56:24.000000 pygmtsar-2024.3.15.post8/pygmtsar/ESA.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2219 2024-03-14 06:49:14.000000 pygmtsar-2024.3.15.post8/pygmtsar/GMT.py
+-rw-r--r--   0 mbg        (501) staff       (20)    36535 2024-03-29 04:04:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/IO.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8891 2024-03-16 18:56:07.000000 pygmtsar-2024.3.15.post8/pygmtsar/NCubeVTK.py
+-rw-r--r--   0 mbg        (501) staff       (20)    49194 2024-01-27 11:18:32.000000 pygmtsar-2024.3.15.post8/pygmtsar/PRM.py
+-rw-r--r--   0 mbg        (501) staff       (20)    16841 2024-03-07 06:43:34.000000 pygmtsar-2024.3.15.post8/pygmtsar/PRM_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    18986 2024-04-05 07:42:45.000000 pygmtsar-2024.3.15.post8/pygmtsar/S1.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5556 2024-03-15 05:10:43.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack.py
+-rw-r--r--   0 mbg        (501) staff       (20)    38985 2024-03-09 13:11:05.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_align.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8678 2024-01-18 17:12:46.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_base.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9825 2024-03-16 18:57:36.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_dem.py
+-rw-r--r--   0 mbg        (501) staff       (20)    44173 2024-02-08 18:53:49.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_detrend.py
+-rw-r--r--   0 mbg        (501) staff       (20)    20416 2024-03-19 11:48:48.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_export.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19590 2024-03-30 15:27:55.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_geocode.py
+-rw-r--r--   0 mbg        (501) staff       (20)    19429 2024-02-29 05:37:33.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_incidence.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6278 2024-04-01 07:32:21.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_landmask.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10956 2024-02-18 17:02:14.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_multilooking.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2520 2023-11-04 11:03:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_orbits.py
+-rw-r--r--   0 mbg        (501) staff       (20)    47295 2024-03-29 07:29:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_phasediff.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2008 2023-09-20 16:47:03.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_prm.py
+-rw-r--r--   0 mbg        (501) staff       (20)     6374 2024-04-05 09:31:17.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_ps.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8293 2024-03-15 05:49:32.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe.py
+-rw-r--r--   0 mbg        (501) staff       (20)     7468 2023-10-16 14:06:29.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe_gmtsar.py
+-rw-r--r--   0 mbg        (501) staff       (20)    46640 2024-04-11 04:05:10.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_sbas.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8884 2024-01-01 15:32:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_stl.py
+-rw-r--r--   0 mbg        (501) staff       (20)    23398 2023-11-18 15:14:19.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_tidal.py
+-rw-r--r--   0 mbg        (501) staff       (20)    13575 2024-02-20 05:55:12.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_topo.py
+-rw-r--r--   0 mbg        (501) staff       (20)    11432 2023-11-28 08:51:08.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans.py
+-rw-r--r--   0 mbg        (501) staff       (20)    10270 2023-12-22 16:03:15.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans_inv.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26654 2024-04-11 05:08:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap.py
+-rw-r--r--   0 mbg        (501) staff       (20)     8265 2024-01-01 16:12:16.000000 pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap_snaphu.py
+-rw-r--r--   0 mbg        (501) staff       (20)    15529 2024-03-09 15:12:11.000000 pygmtsar-2024.3.15.post8/pygmtsar/Tiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9802 2024-03-09 15:15:40.000000 pygmtsar-2024.3.15.post8/pygmtsar/XYZTiles.py
+-rw-r--r--   0 mbg        (501) staff       (20)     9446 2024-01-18 07:55:51.000000 pygmtsar-2024.3.15.post8/pygmtsar/_Stack_merge.py
+-rw-r--r--   0 mbg        (501) staff       (20)     1061 2024-04-11 02:26:04.000000 pygmtsar-2024.3.15.post8/pygmtsar/__init__.py
+-rw-r--r--   0 mbg        (501) staff       (20)    26366 2024-03-13 16:52:36.000000 pygmtsar-2024.3.15.post8/pygmtsar/datagrid.py
+-rw-r--r--   0 mbg        (501) staff       (20)     4073 2023-10-14 09:53:33.000000 pygmtsar-2024.3.15.post8/pygmtsar/tqdm_dask.py
+-rw-r--r--   0 mbg        (501) staff       (20)     2073 2023-09-12 09:05:29.000000 pygmtsar-2024.3.15.post8/pygmtsar/tqdm_joblib.py
+-rw-r--r--   0 mbg        (501) staff       (20)     5739 2024-01-31 16:19:27.000000 pygmtsar-2024.3.15.post8/pygmtsar/utils.py
+drwxr-xr-x   0 mbg        (501) staff       (20)        0 2024-04-11 18:25:57.761817 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/
+-rw-r--r--   0 mbg        (501) staff       (20)    13463 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/PKG-INFO
+-rw-r--r--   0 mbg        (501) staff       (20)     1132 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/SOURCES.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        1 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/dependency_links.txt
+-rw-r--r--   0 mbg        (501) staff       (20)      330 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/requires.txt
+-rw-r--r--   0 mbg        (501) staff       (20)        9 2024-04-11 18:25:57.000000 pygmtsar-2024.3.15.post8/pygmtsar.egg-info/top_level.txt
+-rw-r--r--   0 mbg        (501) staff       (20)       38 2024-04-11 18:25:57.762575 pygmtsar-2024.3.15.post8/setup.cfg
+-rw-r--r--   0 mbg        (501) staff       (20)     3140 2024-04-11 03:27:25.000000 pygmtsar-2024.3.15.post8/setup.py
```

### Comparing `pygmtsar-2024.3.15.post7/LICENSE.txt` & `pygmtsar-2024.3.15.post8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/PKG-INFO` & `pygmtsar-2024.3.15.post8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post7
+Version: 2024.3.15.post8
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 Requires-Dist: xarray>=2024.1.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: numba
 Requires-Dist: pandas>=2.2
 Requires-Dist: geopandas
 Requires-Dist: distributed>=2024.1.0
-Requires-Dist: dask[complete]<=2024.1.1
+Requires-Dist: dask[complete]>=2024.4.1
 Requires-Dist: dask_image
 Requires-Dist: joblib
 Requires-Dist: tqdm
 Requires-Dist: scipy==1.11.4
 Requires-Dist: cffi
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: scikit-learn
```

### Comparing `pygmtsar-2024.3.15.post7/README.md` & `pygmtsar-2024.3.15.post8/README.md`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/ASF.py` & `pygmtsar-2024.3.15.post8/pygmtsar/ASF.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/AWS.py` & `pygmtsar-2024.3.15.post8/pygmtsar/AWS.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/ESA.py` & `pygmtsar-2024.3.15.post8/pygmtsar/ESA.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/GMT.py` & `pygmtsar-2024.3.15.post8/pygmtsar/GMT.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/IO.py` & `pygmtsar-2024.3.15.post8/pygmtsar/IO.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/NCubeVTK.py` & `pygmtsar-2024.3.15.post8/pygmtsar/NCubeVTK.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/PRM.py` & `pygmtsar-2024.3.15.post8/pygmtsar/PRM.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/PRM_gmtsar.py` & `pygmtsar-2024.3.15.post8/pygmtsar/PRM_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/S1.py` & `pygmtsar-2024.3.15.post8/pygmtsar/S1.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_align.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_align.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_base.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_base.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_dem.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_dem.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_detrend.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_detrend.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_export.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_export.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_geocode.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_geocode.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_incidence.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_incidence.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_landmask.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_landmask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_multilooking.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_multilooking.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_orbits.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_orbits.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_phasediff.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_phasediff.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_prm.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_prm.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_ps.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_ps.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_reframe_gmtsar.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_reframe_gmtsar.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_sbas.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_sbas.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
         x = x.copy()
         # prevent weight=1
         w = (1 - 1e-6)*w.copy()
         x[nanmask] = 0
         w[nanmask] = 0
         # check if x has enough valid values
         #print (f'{x.size}, {np.sum(nanmask)}, {matrix.shape[1]}')
-        if x.size - np.sum(nanmask) < matrix.shape[1]:
-            return np.nan * np.zeros(matrix.shape[1])
+        #if x.size - np.sum(nanmask) < matrix.shape[1]:
+        #    return np.nan * np.zeros(matrix.shape[1])
 
         try:
             if np.all(w == 1):
                 # least squares solution
                 model = np.linalg.lstsq(matrix, x, rcond=None)
             else:
                 # weighted least squares solution
@@ -746,15 +746,16 @@
     def plot_baseline_deviation(self, baseline_pairs, pairs_best=None, column='stddev'):
         #print ('NOTE: this function is deprecated, use instead Stack.plot_baseline_attribute()')
         self.plot_baseline_attribute(baseline_pairs, pairs_best, column=column, caption='Baseline Deviation')
 
     def plot_baseline_displacement(self, phase, corr=None, caption=None, cmap='turbo',
                                    displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
-                                   los=False, tolerance=np.pi/2, xlabel_rotation=45):
+                                   los=False, tolerance=np.pi/2, xlabel_rotation=45,
+                                   legend=True, legend_alpha=None):
         """
         Performs 1D unwrapping, linear regression, and STL on a given set of phase values.
     
         The linear regression model is represented as:
             y = β0 + β1 * x
     
         Where:
@@ -862,21 +863,23 @@
             errors = errors[~nanmask]
             weights = weights[~nanmask]
             #print ('weights', weights)
             #print (errors.size, weights.size, errors)
             #rmse = np.sqrt(np.sum(errors**2) / errors.size)
             rmse = np.sqrt(np.sum(weights * (errors**2)) / np.sum(weights) / errors.size)
             #print ('weighted PI-scaled rmse', np.round(rmse / np.pi, 2))
-            plt.plot(dates, solution, color='black', linestyle='--', linewidth=2, label='LSQ')
+            lsq_mean = np.nanmean(solution)
+            plt.plot(dates, solution, color='black', linestyle='--', linewidth=2, label=f'LSQ mean={lsq_mean:0.2f} [{unit}]')
+            plt.axhline(y=lsq_mean, color='black', linestyle=':')
             plt.plot(dates, values, color='blue', linestyle='-', linewidth=2,
-                     label=f'LSQ β1 {velocity:0.1f} and β0={intercept:0.1f} [{unit}/year], P-value={p_value:0.2f}')
+                     label=f'LSQ β1={velocity:0.1f} and β0={intercept:0.1f} [{unit}/year], P-value={p_value:0.2f}')
     
         if stl:
             plt.plot(dt_periodic.date, trend, color='blue', linestyle='--', linewidth=2,
-                     label=f'STL β1 {stl_velocity:0.1f} and β0={stl_intercept:0.1f} [{unit}/year]')
+                     label=f'STL β1={stl_velocity:0.1f} and β0={stl_intercept:0.1f} [{unit}/year]')
             plt.plot(dt_periodic.date, seasonal, color='green', linestyle='--', linewidth=1, label='STL Seasonal')
             plt.plot(dt_periodic.date, resid, color='red', linestyle='--', linewidth=1, label='STL Residual')
     
         plt.grid(axis='y')
         if unit == 'rad':
             y_min = np.floor(y_min / np.pi) * np.pi
             y_max = np.ceil(y_max / np.pi) * np.pi
@@ -892,25 +895,27 @@
         plt.xticks(rotation=xlabel_rotation)
         plt.xlabel('Timeline')
         plt.ylabel(f'{name}, [{unit}]')
         plt.title('Displacement' \
                   + (f' RMSE={rmse:0.3f} [{unit}]' if displacement or stl else '') \
                   + (f'\n{caption}' if caption is not None else ''))
         plt.xlim([dates[0], dates[-1]])
-        if displacement or stl:
-            plt.legend()
+        if (displacement or stl) and legend:
+            plt.legend(framealpha=legend_alpha)
 
     def plot_baseline_displacement_los_mm(self, phase, corr=None, caption=None, cmap='turbo',
                                    displacement=True, unwrap=True,
                                    stl=False, stl_freq='W', stl_periods=52, stl_robust=True,
-                                   tolerance=np.pi/2, xlabel_rotation=45):
+                                   tolerance=np.pi/2, xlabel_rotation=45,
+                                   legend=True, legend_alpha=None):
         self.plot_baseline_displacement(phase=phase, corr=corr, caption=caption, cmap=cmap,
                                    displacement=displacement, unwrap=unwrap,
                                    stl=stl, stl_freq=stl_freq, stl_periods=stl_periods, stl_robust=stl_robust,
-                                   los=True, tolerance=tolerance, xlabel_rotation=xlabel_rotation)
+                                   los=True, tolerance=tolerance, xlabel_rotation=xlabel_rotation,
+                                   legend=legend, legend_alpha=legend_alpha)
 
     def rmse(self, data, solution, weight=None):
         """
         Calculate difference between pairs and dates
     
         Use to calculate solution vs pair unwrapped phases difference as
         diff = sbas.stack_vs_cube(phase_unwrap, solution)
```

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_stl.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_stl.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_tidal.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_tidal.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_topo.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_topo.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_trans_inv.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_trans_inv.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,18 @@
                 #print (f'3JUMP {ndate}:', jump, value, '=>', buffer[pair_idx], '?', values.sum(), 'tol', is_tolerance)
                 if is_tolerance:
                     pairs_ok.append(pair_idx)
                     pairs_ok.extend(np.where(matching_rows)[0])
                 #print ()
                 #break
     
+        # return original values when unwrapping is not possible at all
+        if len(pairs_ok) == 0:
+            return buffer
+        # return unwrapped values
         # validity mask
         mask = [idx in pairs_ok for idx in range(buffer.size)]
         #mask = np.isin(np.arange(buffer.size), pairs_ok)
         # output is the same size as input
         #out = np.nan * np.zeros(data.size)
         out = np.full(data.size, np.nan, dtype=np.float32)
         out[~nanmask] = np.where(mask, buffer, np.nan)
```

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Stack_unwrap_snaphu.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Stack_unwrap_snaphu.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/Tiles.py` & `pygmtsar-2024.3.15.post8/pygmtsar/Tiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/XYZTiles.py` & `pygmtsar-2024.3.15.post8/pygmtsar/XYZTiles.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/_Stack_merge.py` & `pygmtsar-2024.3.15.post8/pygmtsar/_Stack_merge.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/__init__.py` & `pygmtsar-2024.3.15.post8/pygmtsar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 
 # This file is part of the PyGMTSAR project: https://github.com/mobigroup/gmtsar
 # 
 # Copyright (c) 2023, Alexey Pechnikov
 # 
 # Licensed under the BSD 3-Clause License (see LICENSE for details)
 # ----------------------------------------------------------------------------
-__version__ = '2024.3.15.post7'
+__version__ = '2024.3.15.post8'
 
 # unified progress indicators
 from .tqdm_joblib import tqdm_joblib
 from .tqdm_dask import tqdm_dask
 # base NetCDF operations and parameters on NetCDF grid
 from .datagrid import datagrid
 # top level module classes
```

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/datagrid.py` & `pygmtsar-2024.3.15.post8/pygmtsar/datagrid.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/tqdm_dask.py` & `pygmtsar-2024.3.15.post8/pygmtsar/tqdm_dask.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/tqdm_joblib.py` & `pygmtsar-2024.3.15.post8/pygmtsar/tqdm_joblib.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar/utils.py` & `pygmtsar-2024.3.15.post8/pygmtsar/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar.egg-info/PKG-INFO` & `pygmtsar-2024.3.15.post8/pygmtsar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtsar
-Version: 2024.3.15.post7
+Version: 2024.3.15.post8
 Summary: PyGMTSAR (Python GMTSAR): Powerful and Accessible Satellite Interferometry
 Home-page: https://github.com/AlexeyPechnikov/gmtsar
 Author: Alexey Pechnikov
 Author-email: alexey@pechnikov.dev
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 License-File: LICENSE.txt
 Requires-Dist: xarray>=2024.1.0
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: numba
 Requires-Dist: pandas>=2.2
 Requires-Dist: geopandas
 Requires-Dist: distributed>=2024.1.0
-Requires-Dist: dask[complete]<=2024.1.1
+Requires-Dist: dask[complete]>=2024.4.1
 Requires-Dist: dask_image
 Requires-Dist: joblib
 Requires-Dist: tqdm
 Requires-Dist: scipy==1.11.4
 Requires-Dist: cffi
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: scikit-learn
```

### Comparing `pygmtsar-2024.3.15.post7/pygmtsar.egg-info/SOURCES.txt` & `pygmtsar-2024.3.15.post8/pygmtsar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygmtsar-2024.3.15.post7/setup.py` & `pygmtsar-2024.3.15.post8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     packages=['pygmtsar'],
     install_requires=['xarray>=2024.1.0',
                       'numpy>=1.22.4',
                       'numba',
                       'pandas>=2.2',
                       'geopandas',
                       'distributed>=2024.1.0',
-                      'dask[complete]<=2024.1.1',
+                      'dask[complete]>=2024.4.1',
                       'dask_image',
                       'joblib',
                       'tqdm',
                       'scipy==1.11.4',
                       'cffi',
                       'shapely>=2.0.2',
                       'scikit-learn',
```

