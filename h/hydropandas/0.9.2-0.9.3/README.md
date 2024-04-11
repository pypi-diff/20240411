# Comparing `tmp/hydropandas-0.9.2.tar.gz` & `tmp/hydropandas-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydropandas-0.9.2.tar", last modified: Wed Oct 18 14:08:11 2023, max compression
+gzip compressed data, was "hydropandas-0.9.3.tar", last modified: Fri Nov  3 13:15:24 2023, max compression
```

## Comparing `hydropandas-0.9.2.tar` & `hydropandas-0.9.3.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.497954 hydropandas-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-10-18 14:08:00.000000 hydropandas-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2023-10-18 14:08:11.497954 hydropandas-0.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.489955 hydropandas-0.9.2/hydropandas/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.489955 hydropandas-0.9.2/hydropandas/data/
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/data/fews_parameterid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/data/knmi_meteostation.json
--rw-r--r--   0 runner    (1001) docker     (127)    51075 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/data/knmi_neerslagstation.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.489955 hydropandas-0.9.2/hydropandas/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/geo.py
--rw-r--r--   0 runner    (1001) docker     (127)    21276 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/gwobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29354 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    12102 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/extensions/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.493955 hydropandas-0.9.2/hydropandas/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20157 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/bro.py
--rw-r--r--   0 runner    (1001) docker     (127)    14556 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/bronhouderportaal_bro.py
--rw-r--r--   0 runner    (1001) docker     (127)    24866 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)    23730 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/fews.py
--rw-r--r--   0 runner    (1001) docker     (127)    64177 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/knmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/menyanthes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/modflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/pastas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/waterinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/wiski.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/io/wow.py
--rw-r--r--   0 runner    (1001) docker     (127)    71746 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/obs_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    42387 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-18 14:08:00.000000 hydropandas-0.9.2/hydropandas/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.489955 hydropandas-0.9.2/hydropandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2023-10-18 14:08:11.000000 hydropandas-0.9.2/hydropandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2023-10-18 14:08:11.000000 hydropandas-0.9.2/hydropandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 14:08:11.000000 hydropandas-0.9.2/hydropandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-10-18 14:08:11.000000 hydropandas-0.9.2/hydropandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-18 14:08:11.000000 hydropandas-0.9.2/hydropandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2023-10-18 14:08:00.000000 hydropandas-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2023-10-18 14:08:00.000000 hydropandas-0.9.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-18 14:08:11.497954 hydropandas-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 14:08:11.493955 hydropandas-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_000_run_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_001_to_from.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_002_obs_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_003_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_004_gwobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_005_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_006_knmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_007_wiski.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_008_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_009_fews.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_011_bro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-18 14:08:00.000000 hydropandas-0.9.2/tests/test_012_wow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.462000 hydropandas-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-11-03 13:15:12.000000 hydropandas-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2023-11-03 13:15:24.458000 hydropandas-0.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.449999 hydropandas-0.9.3/hydropandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.449999 hydropandas-0.9.3/hydropandas/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    18073 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/data/fews_parameterid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/data/knmi_meteostation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51075 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/data/knmi_neerslagstation.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.453999 hydropandas-0.9.3/hydropandas/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21276 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/gwobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29348 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/extensions/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.453999 hydropandas-0.9.3/hydropandas/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20157 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/bro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14556 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/bronhouderportaal_bro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24866 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23730 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/fews.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64177 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/knmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9026 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/menyanthes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/modflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/pastas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/waterinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7153 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/wiski.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/io/wow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73855 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/obs_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43491 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/observation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.453999 hydropandas-0.9.3/hydropandas/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/static/js_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-03 13:15:12.000000 hydropandas-0.9.3/hydropandas/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.449999 hydropandas-0.9.3/hydropandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2023-11-03 13:15:24.000000 hydropandas-0.9.3/hydropandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-03 13:15:24.000000 hydropandas-0.9.3/hydropandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 13:15:24.000000 hydropandas-0.9.3/hydropandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2023-11-03 13:15:24.000000 hydropandas-0.9.3/hydropandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-03 13:15:24.000000 hydropandas-0.9.3/hydropandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-11-03 13:15:12.000000 hydropandas-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2023-11-03 13:15:12.000000 hydropandas-0.9.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-03 13:15:24.462000 hydropandas-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 13:15:24.453999 hydropandas-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_000_run_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8137 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_001_to_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_002_obs_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_003_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_004_gwobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_005_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_006_knmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_007_wiski.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_008_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_009_fews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_011_bro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-03 13:15:12.000000 hydropandas-0.9.3/tests/test_012_wow.py
```

### Comparing `hydropandas-0.9.2/LICENSE` & `hydropandas-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/PKG-INFO` & `hydropandas-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydropandas
-Version: 0.9.2
+Version: 0.9.3
 Summary: Module by Artesia for loading observation data into custom DataFrames.
 Author-email: Onno Ebbens <o.ebbens@artesia-water.nl>
 Maintainer-email: "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.E. Ebbens, D.A. Brakenhoff, R. Calje
```

### Comparing `hydropandas-0.9.2/hydropandas/__init__.py` & `hydropandas-0.9.3/hydropandas/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     read_dino,
     read_excel,
     read_fews,
     read_imod,
     read_knmi,
     read_menyanthes,
     read_modflow,
+    read_pastastore,
     read_pickle,
     read_waterinfo,
     read_wiski,
 )
 from .observation import (
     EvaporationObs,
     GroundwaterObs,
```

### Comparing `hydropandas-0.9.2/hydropandas/data/fews_parameterid.py` & `hydropandas-0.9.3/hydropandas/data/fews_parameterid.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/data/knmi_meteostation.json` & `hydropandas-0.9.3/hydropandas/data/knmi_meteostation.json`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/data/knmi_neerslagstation.json` & `hydropandas-0.9.3/hydropandas/data/knmi_neerslagstation.json`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/extensions/accessor.py` & `hydropandas-0.9.3/hydropandas/extensions/accessor.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/extensions/geo.py` & `hydropandas-0.9.3/hydropandas/extensions/geo.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/extensions/gwobs.py` & `hydropandas-0.9.3/hydropandas/extensions/gwobs.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/extensions/plots.py` & `hydropandas-0.9.3/hydropandas/extensions/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,26 +40,26 @@
             start date for timeseries plot
         tmax : dt.datetime, optional
             end date for timeseries plot
         per_monitoring_well : bool, optional
             if True plot multiple tubes at the same monitoring_well in one
             figure
         **kwargs :
-            will be passed to the Obs.to_interactive_plot method, options
+            will be passed to the Obs.interactive_plot method, options
             include:
 
             - cols : list of str or None
             - hoover_names : list of str
             - plot_freq : list of str
             - plot_legend_names : list of str
             - markers : list of str
             - hoover_names : list of str
             - plot_colors : list of str
             - ylabel : str
-            - add_filter_to_legend : boolean
+            - add_screen_to_legend : boolean
         """
         _color_cycle = (
             "blue",
             "olive",
             "lime",
             "red",
             "orange",
@@ -180,25 +180,25 @@
             see col_name_lat
         zoom_start : int, optional
             start zoom level of the folium ma
         create_interactive_plots : boolean, optional
             if True interactive plots will be created, if False the iplot_fname
             in the meta ditctionary of the observations is used.
         **kwargs :
-            will be passed to the to_interactive_plots method options are:
+            will be passed to the interactive_plots method options are:
 
             - cols : list of str or None
             - hoover_names : list of str
             - plot_legend_names : list of str
             - plot_freq : list of str
             - markers : list of str
             - hoover_names : list of str
             - plot_colors : list of str
             - ylabel : str
-            - add_filter_to_legend : boolean
+            - add_screen_to_legend : boolean
             - tmin : dt.datetime
             - tmax : dt.datetime
 
         Returns
         -------
         m : folium.Map
             the folium map
```

### Comparing `hydropandas-0.9.2/hydropandas/extensions/stats.py` & `hydropandas-0.9.3/hydropandas/extensions/stats.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/bro.py` & `hydropandas-0.9.3/hydropandas/io/bro.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/bronhouderportaal_bro.py` & `hydropandas-0.9.3/hydropandas/io/bronhouderportaal_bro.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/dino.py` & `hydropandas-0.9.3/hydropandas/io/dino.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/fews.py` & `hydropandas-0.9.3/hydropandas/io/fews.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/knmi.py` & `hydropandas-0.9.3/hydropandas/io/knmi.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/menyanthes.py` & `hydropandas-0.9.3/hydropandas/io/menyanthes.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/modflow.py` & `hydropandas-0.9.3/hydropandas/io/modflow.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/waterinfo.py` & `hydropandas-0.9.3/hydropandas/io/waterinfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,14 @@
         zf = zipfile.ZipFile(path)
         f = zf.open("{}.csv".format(name))
     else:
         raise NotImplementedError(
             "File type '{}' not supported!".format(os.path.splitext(path)[-1])
         )
 
-    if index_cols is None:
-        index_cols = ["WAARNEMINGDATUM", "WAARNEMINGTIJD"]
-
     if value_col is None:
         value_col = "NUMERIEKEWAARDE"
 
     if location_col is None:
         location_col = "MEETPUNT_IDENTIFICATIE"
 
     if xcol is None:
@@ -62,19 +59,33 @@
 
     # read data
     df = pd.read_csv(
         f,
         sep=";",
         decimal=",",
         encoding="ISO-8859-1",
-        parse_dates=[index_cols],
         dayfirst=True,
-        index_col="_".join(index_cols),
     )
 
+    if index_cols is None:
+        index_cols = ["WAARNEMINGDATUM"]
+        if "WAARNEMINGTIJD (MET/CET)" in df.columns:
+            index_cols += ["WAARNEMINGTIJD (MET/CET)"]
+        elif "WAARNEMINGTIJD" in df.columns:
+            index_cols += ["WAARNEMINGTIJD"]
+        else:
+            raise KeyError(
+                "expected column with WAARNEMINGSTIJD but could not find one"
+            )
+
+    df.index = pd.to_datetime(
+        df[index_cols[0]] + " " + df[index_cols[1]], dayfirst=True
+    )
+    df.drop(columns=index_cols, inplace=True)
+
     # do some conversions
     df.loc[df[value_col] == 999999999, value_col] = np.NaN
     df[value_col] = df[value_col] / 100.0
 
     # parse metadata into dict
     if return_metadata:
         if len(df[location_col].unique()) > 1:
```

### Comparing `hydropandas-0.9.2/hydropandas/io/wiski.py` & `hydropandas-0.9.3/hydropandas/io/wiski.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/io/wow.py` & `hydropandas-0.9.3/hydropandas/io/wow.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas/obs_collection.py` & `hydropandas-0.9.3/hydropandas/obs_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -721,14 +721,47 @@
         keep_all_obs=keep_all_obs,
         **kwargs,
     )
 
     return oc
 
 
+def read_pastastore(
+    pstore,
+    libname,
+    ObsClass=obs.GroundwaterObs,
+    metadata_mapping=None,
+):
+    """Read pastastore library.
+
+    Parameters
+    ----------
+    pstore : pastastore.PastaStore
+        PastaStore object
+    libname : str
+        name of library (e.g. oseries or stresses)
+    ObsClass : Obs, optional
+        type of Obs to read data as, by default obs.GroundwaterObs
+    metadata_mapping : dict, optional
+        dictionary containing map between metadata field names in pastastore and
+        metadata field names expected by hydropandas, by default None.
+
+    Returns
+    -------
+    ObsCollection
+        ObsCollection containing data
+    """
+    return ObsCollection.from_pastastore(
+        pstore=pstore,
+        libname=libname,
+        ObsClass=ObsClass,
+        metadata_mapping=metadata_mapping,
+    )
+
+
 class ObsCollection(pd.DataFrame):
     """class for a collection of point observations.
 
     An ObsCollection object is a subclass of a pandas.DataFrame and allows for
     additional attributes and methods. Additional attributes are
     defined in the '_metadata' attribute.
 
@@ -1844,14 +1877,51 @@
             keep_all_obs=keep_all_obs,
             **kwargs,
         )
         obs_df = util._obslist_to_frame(obs_list)
 
         return cls(obs_df, name=name, meta=meta)
 
+    @classmethod
+    def from_pastastore(
+        cls, pstore, libname, ObsClass=obs.GroundwaterObs, metadata_mapping=None
+    ):
+        """Read pastastore library.
+
+        Parameters
+        ----------
+        pstore : pastastore.PastaStore
+            PastaStore object
+        libname : str
+            name of library (e.g. oseries or stresses)
+        ObsClass : Obs, optional
+            type of Obs to read data as, by default obs.GroundwaterObs
+        metadata_mapping : dict, optional
+            dictionary containing map between metadata field names in pastastore and
+            metadata field names expected by hydropandas, by default None.
+
+        Returns
+        -------
+        ObsCollection
+            ObsCollection containing data
+        """
+        from .io import pastas
+
+        obs_list = pastas.read_pastastore_library(
+            pstore, libname, ObsClass=ObsClass, metadata_mapping=metadata_mapping
+        )
+        obs_df = util._obslist_to_frame(obs_list)
+
+        meta = {
+            "name": pstore.name,
+            "conntype": pstore.conn.conn_type,
+            "library": libname,
+        }
+        return cls(obs_df, name=pstore.name, meta=meta)
+
     def to_excel(self, path, meta_sheet_name="metadata"):
         """Write an ObsCollection to an excel, the first sheet in the
         excel contains the metadata, the other tabs are the timeseries of each
         observation.
 
         The excel can be read using the read_excel function of hydropandas.
 
@@ -1950,15 +2020,16 @@
             Existing pastastore, if None a new pastastore is created
         pstore_name : str, optional
             Name of the pastastore only used if pstore is None
         col : str, optional
             Name of the column in the Obs dataframe to be used. If None the
             first numeric column in the Obs Dataframe is used.
         kind : str, optional
-            The kind of series that is added to the pastastore
+            The kind of series that is added to the pastastore. Use 'oseries'
+            for observations and anything else for stresses.
         add_metadata : boolean, optional
             If True metadata from the observations added to the pastastore
         conn : pastastore.connectors or None, optional
             type of connector, if None the DictConnector is used. Default is
             None.
         overwrite : boolean, optional
             if True, overwrite existing series in pastastore, default is False
```

### Comparing `hydropandas-0.9.2/hydropandas/observation.py` & `hydropandas-0.9.3/hydropandas/observation.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,14 +741,46 @@
         """
         from .io import wiski
 
         data, metadata = wiski.read_wiski_file(path, **kwargs)
 
         return cls(data, meta=metadata, **metadata)
 
+    @classmethod
+    def from_pastastore(cls, pstore, libname, name, metadata_mapping=None):
+        """Read item from pastastore library.
+
+        Parameters
+        ----------
+        pstore : pastastore.PastaStore
+            pastastore object
+        libname : str
+            name of library containinig item
+        name : str
+            name of item
+        metadata_mapping : dict, optional
+            dictionary containing map between metadata field names in pastastore (keys)
+            and metadata field names expected by hydropandas (values), by default None.
+        """
+        from .io import pastas
+
+        data, metadata = pastas.read_pastastore_item(pstore, libname, name)
+
+        if metadata_mapping is not None:
+            for pstore_name, oc_name in metadata_mapping.items():
+                metadata[oc_name] = metadata.get(pstore_name, None)
+
+        metadata["source"] = "pastastore"
+        kwargs = {}
+        for key, value in metadata.items():
+            if key in cls._metadata:
+                kwargs[key] = value
+
+        return cls(data, meta=metadata, **kwargs)
+
 
 class WaterQualityObs(Obs):
     """class for water quality ((grond)watersamenstelling) point
     observations.
 
     Subclass of the Obs class
     """
```

### Comparing `hydropandas-0.9.2/hydropandas/util.py` & `hydropandas-0.9.3/hydropandas/util.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/hydropandas.egg-info/PKG-INFO` & `hydropandas-0.9.3/hydropandas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydropandas
-Version: 0.9.2
+Version: 0.9.3
 Summary: Module by Artesia for loading observation data into custom DataFrames.
 Author-email: Onno Ebbens <o.ebbens@artesia-water.nl>
 Maintainer-email: "O.N. Ebbens" <o.ebbens@artesia-water.nl>, "R. Calje" <r.calje@artesia-water.nl>, "D.A. Brakenhoff" <d.brakenhoff@artesia-water.nl>, "M.A. Vonk" <m.vonk@artesia-water.nl>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 O.E. Ebbens, D.A. Brakenhoff, R. Calje
```

### Comparing `hydropandas-0.9.2/hydropandas.egg-info/SOURCES.txt` & `hydropandas-0.9.3/hydropandas.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 hydropandas/io/knmi.py
 hydropandas/io/menyanthes.py
 hydropandas/io/modflow.py
 hydropandas/io/pastas.py
 hydropandas/io/waterinfo.py
 hydropandas/io/wiski.py
 hydropandas/io/wow.py
+hydropandas/static/js_collapse.html
+hydropandas/static/style.css
 tests/test_000_run_notebooks.py
 tests/test_001_to_from.py
 tests/test_002_obs_objects.py
 tests/test_003_calculations.py
 tests/test_004_gwobs.py
 tests/test_005_dino.py
 tests/test_006_knmi.py
```

### Comparing `hydropandas-0.9.2/pyproject.toml` & `hydropandas-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 include-package-data = true
 
 [tool.setuptools.dynamic]
 version = { attr = "hydropandas.version.__version__" }
 
 [tool.setuptools.package-data]
 "hydropandas.data" = ["*.json"]
+"hydropandas.static" = ["*.html", "*.css"]
 
 [tool.black]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `hydropandas-0.9.2/readme.md` & `hydropandas-0.9.3/readme.md`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_000_run_notebooks.py` & `hydropandas-0.9.3/tests/test_000_run_notebooks.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_001_to_from.py` & `hydropandas-0.9.3/tests/test_001_to_from.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import os
+
 import pandas as pd
+import pastastore as pst
 import pytest
 from requests.exceptions import ConnectionError
 
 import hydropandas as hpd
 
 # %% BRO
 
@@ -189,15 +192,25 @@
 
 
 # %% PASTASTORE
 def test_to_pastastore():
     dino_gw = test_obscollection_dinozip_gw()
     # drop duplicate
     dino_gw.drop("B22D0155-001", inplace=True)
-    dino_gw.to_pastastore()
+    pstore = dino_gw.to_pastastore()
+    # export to zip for read test
+    pstore.to_zip("test_pastastore.zip")
+
+
+def test_from_pastastore():
+    pstore = pst.PastaStore.from_zip(
+        "test_pastastore.zip", conn=pst.DictConnector("pastas_db")
+    )
+    _ = hpd.read_pastastore(pstore, "oseries")
+    os.remove("test_pastastore.zip")
 
 
 # %% excel
 
 
 def test_to_excel():
     oc = hpd.read_fews(
@@ -321,15 +334,15 @@
     )
 
 
 # %% WATERINFO
 
 
 def test_waterinfo_from_dir():
-    path = "./tests/data/waterinfo-test"
+    path = "./tests/data/2023-waterinfo-test"
     hpd.read_waterinfo(path)
 
 
 # %% MENYANTHES
 
 
 def test_obscollection_menyanthes():
```

### Comparing `hydropandas-0.9.2/tests/test_002_obs_objects.py` & `hydropandas-0.9.3/tests/test_002_obs_objects.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_003_calculations.py` & `hydropandas-0.9.3/tests/test_003_calculations.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_004_gwobs.py` & `hydropandas-0.9.3/tests/test_004_gwobs.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_005_dino.py` & `hydropandas-0.9.3/tests/test_005_dino.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_006_knmi.py` & `hydropandas-0.9.3/tests/test_006_knmi.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_007_wiski.py` & `hydropandas-0.9.3/tests/test_007_wiski.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_008_visualisation.py` & `hydropandas-0.9.3/tests/test_008_visualisation.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_009_fews.py` & `hydropandas-0.9.3/tests/test_009_fews.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_011_bro.py` & `hydropandas-0.9.3/tests/test_011_bro.py`

 * *Files identical despite different names*

### Comparing `hydropandas-0.9.2/tests/test_012_wow.py` & `hydropandas-0.9.3/tests/test_012_wow.py`

 * *Files identical despite different names*

