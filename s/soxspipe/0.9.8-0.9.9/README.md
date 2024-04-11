# Comparing `tmp/soxspipe-0.9.8.tar.gz` & `tmp/soxspipe-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soxspipe-0.9.8.tar", last modified: Fri Jan 19 13:26:46 2024, max compression
+gzip compressed data, was "soxspipe-0.9.9.tar", last modified: Wed Jan 24 12:06:56 2024, max compression
```

## Comparing `soxspipe-0.9.8.tar` & `soxspipe-0.9.9.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:46.577925 soxspipe-0.9.8/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      453 2024-01-19 12:47:48.000000 soxspipe-0.9.8/.readthedocs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17500 2024-01-19 12:47:48.000000 soxspipe-0.9.8/CHANGES.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-01-19 12:47:48.000000 soxspipe-0.9.8/LICENSE
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      361 2024-01-19 12:47:48.000000 soxspipe-0.9.8/MANIFEST.in
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3931 2024-01-19 13:26:46.577925 soxspipe-0.9.8/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2866 2024-01-19 12:47:48.000000 soxspipe-0.9.8/README.md
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2024-01-19 13:26:46.577925 soxspipe-0.9.8/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1821 2024-01-19 12:47:48.000000 soxspipe-0.9.8/setup.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.645893 soxspipe-0.9.8/soxspipe/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      141 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/__version__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      592 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/advanced_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10806 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/cl_utils.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.705895 soxspipe-0.9.8/soxspipe/commonutils/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      886 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1151 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/combiner.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    75682 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/create_dispersion_map.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    59602 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/data_organiser.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    45153 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/detect_continuum.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36935 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/detect_order_edges.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2932 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/detector_lookup.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3509 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6493 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/filenamer.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3000 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/flux_calibration.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/getpackagepath.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36592 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/horne_extraction.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4422 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/keyword_lookup.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8653 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/polynomials.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3273 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/response_function.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    18476 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/set_of_files.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11892 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/subtract_background.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    67614 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/subtract_sky.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    38382 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/toolkit.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1421 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/commonutils/uncompress.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6907 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/default_settings.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   110592 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/pandas_export.db
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.717895 soxspipe-0.9.8/soxspipe/recipes/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      416 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/__init__.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    51393 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/_base_recipe_.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10544 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_disp_solution.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13737 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_mbias.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8075 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_mdark.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36966 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_mflat.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11801 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_order_centres.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13302 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_spatial_solution.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    15741 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_stare.py
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6155 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/recipes/soxs_straighten.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.765897 soxspipe-0.9.8/soxspipe/resources/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6290 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/package.mplstyle
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2730 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/soxs_detector_parameters.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      853 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/soxs_keywords.yaml
--rwxr-xr-x   0 jenkins   (1003) jenkins   (1004)    45056 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/soxspipe.db
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.481887 soxspipe-0.9.8/soxspipe/resources/static_calibrations/
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:46.169911 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 33557761 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    63360 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_MPH_TAB_NIR_Xe.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8640 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_SPH_TAB_NIR_Xe.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/skylines.fits
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:46.573925 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8674560 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 24629760 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 12340800 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  6197760 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 32820480 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004) 16436160 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8245440 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17280 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   169920 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    60480 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/skylines.fits
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2713 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/xsh_detector_parameters.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9625 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/resources/xsh_keywords.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9670 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/setup.cfg
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3254 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/test_settings_soxs.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6914 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/test_settings_soxs_sim.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10363 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/test_settings_xsh.yaml
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3389 2024-01-19 12:47:48.000000 soxspipe-0.9.8/soxspipe/utKit.py
-drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-19 13:26:45.665894 soxspipe-0.9.8/soxspipe.egg-info/
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3931 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3995 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)       52 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-19 12:52:25.000000 soxspipe-0.9.8/soxspipe.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)      154 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2024-01-19 13:26:45.000000 soxspipe-0.9.8/soxspipe.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:56.030597 soxspipe-0.9.9/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      453 2024-01-24 11:21:53.000000 soxspipe-0.9.9/.readthedocs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17559 2024-01-24 11:21:53.000000 soxspipe-0.9.9/CHANGES.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    35149 2024-01-24 11:21:53.000000 soxspipe-0.9.9/LICENSE
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      361 2024-01-24 11:21:53.000000 soxspipe-0.9.9/MANIFEST.in
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3931 2024-01-24 12:06:56.030597 soxspipe-0.9.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2866 2024-01-24 11:21:53.000000 soxspipe-0.9.9/README.md
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       38 2024-01-24 12:06:56.030597 soxspipe-0.9.9/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1821 2024-01-24 11:21:53.000000 soxspipe-0.9.9/setup.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:54.990561 soxspipe-0.9.9/soxspipe/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      141 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       22 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/__version__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      592 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/advanced_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10806 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/cl_utils.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:55.038563 soxspipe-0.9.9/soxspipe/commonutils/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      886 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1151 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/combiner.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    75682 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/create_dispersion_map.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    59602 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/data_organiser.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    45153 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/detect_continuum.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36935 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/detect_order_edges.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2932 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/detector_lookup.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3509 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6493 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/filenamer.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3000 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/flux_calibration.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      358 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/getpackagepath.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36592 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/horne_extraction.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     4422 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/keyword_lookup.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8653 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/polynomials.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3273 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/response_function.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    18476 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/set_of_files.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11892 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/subtract_background.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    67614 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/subtract_sky.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    38382 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/toolkit.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     1421 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/commonutils/uncompress.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6907 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/default_settings.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   110592 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/pandas_export.db
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:55.050563 soxspipe-0.9.9/soxspipe/recipes/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      416 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/__init__.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    51393 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/_base_recipe_.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10546 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_disp_solution.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13739 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_mbias.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8077 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_mdark.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    36968 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_mflat.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    11801 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_order_centres.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    13304 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_spatial_solution.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    15743 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_stare.py
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6157 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/recipes/soxs_straighten.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:55.058564 soxspipe-0.9.9/soxspipe/resources/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6290 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/resources/package.mplstyle
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2730 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/resources/soxs_detector_parameters.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      853 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/resources/soxs_keywords.yaml
+-rwxr-xr-x   0 jenkins   (1003) jenkins   (1004)    45056 2024-01-24 11:21:53.000000 soxspipe-0.9.9/soxspipe/resources/soxspipe.db
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:54.978561 soxspipe-0.9.9/soxspipe/resources/static_calibrations/
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:55.430576 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 33557761 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    63360 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_MPH_TAB_NIR_Xe.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     8640 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_SPH_TAB_NIR_Xe.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/skylines.fits
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:56.026597 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8674560 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 24629760 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 12340800 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  6197760 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 32820480 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004) 16436160 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)  8245440 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    17280 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    14400 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   169920 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   132480 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)   167040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    60480 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    23040 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    28800 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    46080 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/skylines.fits
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     2713 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/xsh_detector_parameters.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9625 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/resources/xsh_keywords.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     9670 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/setup.cfg
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3254 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/test_settings_soxs.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     6914 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/test_settings_soxs_sim.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)    10363 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/test_settings_xsh.yaml
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3389 2024-01-24 11:21:54.000000 soxspipe-0.9.9/soxspipe/utKit.py
+drwxr-xr-x   0 jenkins   (1003) jenkins   (1004)        0 2024-01-24 12:06:54.998562 soxspipe-0.9.9/soxspipe.egg-info/
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3931 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)     3995 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)       52 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        1 2024-01-24 11:27:25.000000 soxspipe-0.9.9/soxspipe.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)      154 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1003) jenkins   (1004)        9 2024-01-24 12:06:54.000000 soxspipe-0.9.9/soxspipe.egg-info/top_level.txt
```

### Comparing `soxspipe-0.9.8/CHANGES.md` & `soxspipe-0.9.9/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 
 # Release Notes  
 
+## v0.9.9 - January 24, 2024
+
+* **FIXED**: bug fix logger
+
 ## v0.9.8 - January 19, 2024
 
 * **FIXED**: bug fix in collecting settings files from the default location
 
 ## v0.9.7 - December 7, 2023
 
 * **ENHANCEMENT:** the instrument name is now included in the SOF & product filename.
```

### Comparing `soxspipe-0.9.8/LICENSE` & `soxspipe-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/PKG-INFO` & `soxspipe-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soxspipe
-Version: 0.9.8
+Version: 0.9.9
 Summary: A python package and command-line tools to The data-reduction pipeline for the SOXS instrument
 Home-page: https://github.com/thespacedoctor/soxspipe
-Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.9.8.zip
+Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.9.9.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: GPLv3
 Keywords: soxs, eso, data, pipeline, spectra
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `soxspipe-0.9.8/README.md` & `soxspipe-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/setup.py` & `soxspipe-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/advanced_settings.yaml` & `soxspipe-0.9.9/soxspipe/advanced_settings.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/cl_utils.py` & `soxspipe-0.9.9/soxspipe/cl_utils.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/__init__.py` & `soxspipe-0.9.9/soxspipe/commonutils/__init__.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/combiner.py` & `soxspipe-0.9.9/soxspipe/commonutils/combiner.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/create_dispersion_map.py` & `soxspipe-0.9.9/soxspipe/commonutils/create_dispersion_map.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/data_organiser.py` & `soxspipe-0.9.9/soxspipe/commonutils/data_organiser.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/detect_continuum.py` & `soxspipe-0.9.9/soxspipe/commonutils/detect_continuum.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/detect_order_edges.py` & `soxspipe-0.9.9/soxspipe/commonutils/detect_order_edges.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/detector_lookup.py` & `soxspipe-0.9.9/soxspipe/commonutils/detector_lookup.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py` & `soxspipe-0.9.9/soxspipe/commonutils/dispersion_map_to_pixel_arrays.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/filenamer.py` & `soxspipe-0.9.9/soxspipe/commonutils/filenamer.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/flux_calibration.py` & `soxspipe-0.9.9/soxspipe/commonutils/flux_calibration.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/horne_extraction.py` & `soxspipe-0.9.9/soxspipe/commonutils/horne_extraction.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/keyword_lookup.py` & `soxspipe-0.9.9/soxspipe/commonutils/keyword_lookup.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/polynomials.py` & `soxspipe-0.9.9/soxspipe/commonutils/polynomials.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/response_function.py` & `soxspipe-0.9.9/soxspipe/commonutils/response_function.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/set_of_files.py` & `soxspipe-0.9.9/soxspipe/commonutils/set_of_files.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/subtract_background.py` & `soxspipe-0.9.9/soxspipe/commonutils/subtract_background.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/subtract_sky.py` & `soxspipe-0.9.9/soxspipe/commonutils/subtract_sky.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/toolkit.py` & `soxspipe-0.9.9/soxspipe/commonutils/toolkit.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/commonutils/uncompress.py` & `soxspipe-0.9.9/soxspipe/commonutils/uncompress.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/default_settings.yaml` & `soxspipe-0.9.9/soxspipe/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/pandas_export.db` & `soxspipe-0.9.9/soxspipe/pandas_export.db`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/recipes/_base_recipe_.py` & `soxspipe-0.9.9/soxspipe/recipes/_base_recipe_.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_disp_solution.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_disp_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                         error = "Input frames for soxspipe disp_solution need to be single pinhole lamp on and a master-bias and possibly a master dark for UVB/VIS"
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_mbias.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_mbias.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             error = "Input frames not BIAS frames" % locals()
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.error("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
 
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_mdark.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_mdark.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
                 error = "Input frames have differing exposure-times %(exptimes)s" % locals()
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_mflat.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_mflat.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
                         error = f"Input {l} frames for soxspipe mflat need to have a unique exptime"
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_order_centres.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_order_centres.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_spatial_solution.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_spatial_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                         error = f"Input frames for soxspipe spatial_solution need to be LAMP,WAVE, a master-bias, a first-guess dispersion solution table and an order location table. Can optionally supply a master-flat and/or master-dark for UVB/VIS."
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_stare.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_stare.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         #         "Need a **** for %(arm)s - none found with the input files" % locals())
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/recipes/soxs_straighten.py` & `soxspipe-0.9.9/soxspipe/recipes/soxs_straighten.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 "Need a full dispersion/spatial solution for %(arm)s - none found with the input files" % locals())
 
         if error:
             sys.stdout.flush()
             sys.stdout.write("\x1b[1A\x1b[2K")
             self.log.print("# VERIFYING INPUT FRAMES - **ERROR**\n")
             self.log.print(self.inputFrames.summary)
-            self.log.print()
+            self.log.print("")
             raise TypeError(error)
 
         self.imageType = imageTypes[0]
         self.log.debug('completed the ``verify_input_frames`` method')
         return None
 
     def produce_product(
```

### Comparing `soxspipe-0.9.8/soxspipe/resources/package.mplstyle` & `soxspipe-0.9.9/soxspipe/resources/package.mplstyle`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/soxs_detector_parameters.yaml` & `soxspipe-0.9.9/soxspipe/resources/soxs_detector_parameters.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/soxs_keywords.yaml` & `soxspipe-0.9.9/soxspipe/resources/soxs_keywords.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/soxspipe.db` & `soxspipe-0.9.9/soxspipe/resources/soxspipe.db`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/BP_MAP_RP_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_MPH_TAB_NIR_Xe.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_MPH_TAB_NIR_Xe.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_SPECTRAL_FORMAT_TAB_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/SOXS_SPH_TAB_NIR_Xe.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/SOXS_SPH_TAB_NIR_Xe.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/soxs/skylines.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/soxs/skylines.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/BP_MAP_RP_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_UVB.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/SPECTRAL_FORMAT_TAB_VIS.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_MULT_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_NIR.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_UVB_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x1.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_1x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/THEO_TAB_SING_VIS_2x2.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/static_calibrations/xsh/skylines.fits` & `soxspipe-0.9.9/soxspipe/resources/static_calibrations/xsh/skylines.fits`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/xsh_detector_parameters.yaml` & `soxspipe-0.9.9/soxspipe/resources/xsh_detector_parameters.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/resources/xsh_keywords.yaml` & `soxspipe-0.9.9/soxspipe/resources/xsh_keywords.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/setup.cfg` & `soxspipe-0.9.9/soxspipe/setup.cfg`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/test_settings_soxs.yaml` & `soxspipe-0.9.9/soxspipe/test_settings_soxs.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/test_settings_soxs_sim.yaml` & `soxspipe-0.9.9/soxspipe/test_settings_soxs_sim.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/test_settings_xsh.yaml` & `soxspipe-0.9.9/soxspipe/test_settings_xsh.yaml`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe/utKit.py` & `soxspipe-0.9.9/soxspipe/utKit.py`

 * *Files identical despite different names*

### Comparing `soxspipe-0.9.8/soxspipe.egg-info/PKG-INFO` & `soxspipe-0.9.9/soxspipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: soxspipe
-Version: 0.9.8
+Version: 0.9.9
 Summary: A python package and command-line tools to The data-reduction pipeline for the SOXS instrument
 Home-page: https://github.com/thespacedoctor/soxspipe
-Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.9.8.zip
+Download-URL: https://github.com/thespacedoctor/soxspipe/archive/v0.9.9.zip
 Author: David Young
 Author-email: davidrobertyoung@gmail.com
 License: GPLv3
 Keywords: soxs, eso, data, pipeline, spectra
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `soxspipe-0.9.8/soxspipe.egg-info/SOURCES.txt` & `soxspipe-0.9.9/soxspipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

