# Comparing `tmp/RM-Tools-1.4.0.tar.gz` & `tmp/RM-Tools-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RM-Tools-1.4.0.tar", last modified: Tue Mar 26 02:59:45 2024, max compression
+gzip compressed data, was "RM-Tools-1.4.1.tar", last modified: Wed Apr 10 04:24:58 2024, max compression
```

## Comparing `RM-Tools-1.4.0.tar` & `RM-Tools-1.4.1.tar`

### file list

```diff
@@ -1,80 +1,64 @@
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.165566 RM-Tools-1.4.0/
--rw-r--r--   0 cvaneck    (503) staff       (20)     1106 2020-07-23 17:47:25.000000 RM-Tools-1.4.0/LICENSE.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)      161 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/MANIFEST.in
--rw-r--r--   0 cvaneck    (503) staff       (20)     4203 2024-03-26 02:59:45.165066 RM-Tools-1.4.0/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)     2792 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/README.md
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:44.933771 RM-Tools-1.4.0/RM_Tools.egg-info/
--rw-r--r--   0 cvaneck    (503) staff       (20)     4203 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)     1964 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)        1 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)      927 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/entry_points.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)      171 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/requires.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)       30 2024-03-26 02:59:44.000000 RM-Tools-1.4.0/RM_Tools.egg-info/top_level.txt
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:44.987639 RM-Tools-1.4.0/RMtools_1D/
--rw-r--r--   0 cvaneck    (503) staff       (20)       87 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/__init__.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    10298 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/calculate_RMSF.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.009043 RM-Tools-1.4.0/RMtools_1D/cats/
--rw-r--r--   0 cvaneck    (503) staff       (20)     2528 2019-05-13 17:33:13.000000 RM-Tools-1.4.0/RMtools_1D/cats/catComplex.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)     5692 2019-05-13 17:33:13.000000 RM-Tools-1.4.0/RMtools_1D/cats/cat_simple_doQUfit.bat
--rw-r--r--   0 cvaneck    (503) staff       (20)     2104 2019-05-13 17:33:13.000000 RM-Tools-1.4.0/RMtools_1D/cats/catalogue.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)     2826 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/cats/catalogue1.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)    10670 2019-05-13 17:33:13.000000 RM-Tools-1.4.0/RMtools_1D/cats/testCat.dat
--rwxr-xr-x   0 cvaneck    (503) staff       (20)     4897 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/clean_model.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.052947 RM-Tools-1.4.0/RMtools_1D/data/
--rw-r--r--   0 cvaneck    (503) staff       (20)    50612 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)   140348 2022-12-12 07:27:14.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_FDFdirty.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)   115502 2022-12-12 07:27:14.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf
--rw-r--r--   0 cvaneck    (503) staff       (20)   280809 2022-12-12 07:27:14.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_RMSF.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)     1730 2022-12-12 07:27:14.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_RMsynth.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)     1415 2023-11-22 05:32:20.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_RMsynth.json
--rw-r--r--   0 cvaneck    (503) staff       (20)   136375 2022-12-12 07:27:13.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_spectra-plots.pdf
--rw-r--r--   0 cvaneck    (503) staff       (20)    14400 2022-12-12 07:27:14.000000 RM-Tools-1.4.0/RMtools_1D/data/Source1_weight.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50728 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source2.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50710 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source3.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50677 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source4.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50670 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source5.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50727 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source6.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50687 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source7.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50589 2020-09-17 20:30:02.000000 RM-Tools-1.4.0/RMtools_1D/data/Source8.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    27217 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/do_QUfit_1D_mnest.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    21574 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/do_RMclean_1D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    30020 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/do_RMsynth_1D.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    10241 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/do_RMsynth_1D_fromFITS.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    15427 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/mk_test_ascii_data.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.089927 RM-Tools-1.4.0/RMtools_1D/models_ns/
--rw-r--r--   0 cvaneck    (503) staff       (20)       38 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2161 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m1.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     3971 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m11.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     5018 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m111.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2476 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m2.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4258 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m3.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4547 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m4.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2638 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m5.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4802 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m6.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2759 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_1D/models_ns/m7.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    52363 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/rmtools_bwdepol.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     7904 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_1D/rmtools_bwpredict.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.128764 RM-Tools-1.4.0/RMtools_3D/
--rw-r--r--   0 cvaneck    (503) staff       (20)    15333 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/RMpeakfit_3D.py
--rw-r--r--   0 cvaneck    (503) staff       (20)       87 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4374 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/assemble_chunks.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     3598 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/create_chunks.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    21367 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/do_RMclean_3D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    36949 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_3D/do_RMsynth_3D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    21708 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_3D/do_fitIcube.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     5868 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/extract_region.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     1776 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/make_freq_file.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    18516 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMtools_3D/mk_test_cube_data.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    12786 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMtools_3D/rescale_I_model_3D.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2024-03-26 02:59:45.163811 RM-Tools-1.4.0/RMutils/
--rw-r--r--   0 cvaneck    (503) staff       (20)      297 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    95236 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/mpfit.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4778 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/normalize.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    16972 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/util_FITS.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    83900 2024-03-05 04:30:11.000000 RM-Tools-1.4.0/RMutils/util_RM.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    45721 2024-03-26 02:48:53.000000 RM-Tools-1.4.0/RMutils/util_misc.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    10139 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/util_plotFITS.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    75833 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/util_plotTk.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4600 2024-02-19 00:37:51.000000 RM-Tools-1.4.0/RMutils/util_rec.py
--rw-r--r--   0 cvaneck    (503) staff       (20)       38 2024-03-26 02:59:45.165629 RM-Tools-1.4.0/setup.cfg
--rw-r--r--   0 cvaneck    (503) staff       (20)     3094 2024-03-26 02:50:42.000000 RM-Tools-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.766679 RM-Tools-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 04:24:58.766679 RM-Tools-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.766679 RM-Tools-1.4.1/RM_Tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-10 04:24:58.000000 RM-Tools-1.4.1/RM_Tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.758679 RM-Tools-1.4.1/RMtools_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10298 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/calculate_RMSF.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.758679 RM-Tools-1.4.1/RMtools_1D/cats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/cats/catComplex.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/cats/cat_simple_doQUfit.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/cats/catalogue.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/cats/catalogue1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/cats/testCat.dat
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4897 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/clean_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27217 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/do_QUfit_1D_mnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21574 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/do_RMclean_1D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29995 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/do_RMsynth_1D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/do_RMsynth_1D_fromFITS.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15427 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/mk_test_ascii_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.758679 RM-Tools-1.4.1/RMtools_1D/models_ns/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/models_ns/m7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52363 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/rmtools_bwdepol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_1D/rmtools_bwpredict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.762679 RM-Tools-1.4.1/RMtools_3D/
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/RMpeakfit_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/assemble_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/create_chunks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21367 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/do_RMclean_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36920 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/do_RMsynth_3D.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21708 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/do_fitIcube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/extract_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/make_freq_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/mk_test_cube_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMtools_3D/rescale_I_model_3D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:24:58.766679 RM-Tools-1.4.1/RMutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95236 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/mpfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_FITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84116 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_RM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45721 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_plotFITS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75833 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_plotTk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/RMutils/util_rec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 04:24:58.766679 RM-Tools-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-10 04:24:54.000000 RM-Tools-1.4.1/setup.py
```

### Comparing `RM-Tools-1.4.0/LICENSE.txt` & `RM-Tools-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/PKG-INFO` & `RM-Tools-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.0.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.1.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RM-Tools-1.4.0/README.md` & `RM-Tools-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RM_Tools.egg-info/PKG-INFO` & `RM-Tools-1.4.1/RM_Tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.4.0
+Version: 1.4.1
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.0.tar.gz
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.4.1.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RM-Tools-1.4.0/RM_Tools.egg-info/SOURCES.txt` & `RM-Tools-1.4.1/RM_Tools.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -19,29 +19,14 @@
 RMtools_1D/rmtools_bwdepol.py
 RMtools_1D/rmtools_bwpredict.py
 RMtools_1D/cats/catComplex.csv
 RMtools_1D/cats/cat_simple_doQUfit.bat
 RMtools_1D/cats/catalogue.csv
 RMtools_1D/cats/catalogue1.csv
 RMtools_1D/cats/testCat.dat
-RMtools_1D/data/Source1.dat
-RMtools_1D/data/Source1_FDFdirty.dat
-RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf
-RMtools_1D/data/Source1_RMSF.dat
-RMtools_1D/data/Source1_RMsynth.dat
-RMtools_1D/data/Source1_RMsynth.json
-RMtools_1D/data/Source1_spectra-plots.pdf
-RMtools_1D/data/Source1_weight.dat
-RMtools_1D/data/Source2.dat
-RMtools_1D/data/Source3.dat
-RMtools_1D/data/Source4.dat
-RMtools_1D/data/Source5.dat
-RMtools_1D/data/Source6.dat
-RMtools_1D/data/Source7.dat
-RMtools_1D/data/Source8.dat
 RMtools_1D/models_ns/__init__.py
 RMtools_1D/models_ns/m1.py
 RMtools_1D/models_ns/m11.py
 RMtools_1D/models_ns/m111.py
 RMtools_1D/models_ns/m2.py
 RMtools_1D/models_ns/m3.py
 RMtools_1D/models_ns/m4.py
```

### Comparing `RM-Tools-1.4.0/RM_Tools.egg-info/entry_points.txt` & `RM-Tools-1.4.1/RM_Tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/calculate_RMSF.py` & `RM-Tools-1.4.1/RMtools_1D/calculate_RMSF.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/cats/catComplex.csv` & `RM-Tools-1.4.1/RMtools_1D/cats/catComplex.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/cats/cat_simple_doQUfit.bat` & `RM-Tools-1.4.1/RMtools_1D/cats/cat_simple_doQUfit.bat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/cats/catalogue.csv` & `RM-Tools-1.4.1/RMtools_1D/cats/catalogue.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/cats/catalogue1.csv` & `RM-Tools-1.4.1/RMtools_1D/cats/catalogue1.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/cats/testCat.dat` & `RM-Tools-1.4.1/RMtools_1D/cats/testCat.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/clean_model.py` & `RM-Tools-1.4.1/RMtools_1D/clean_model.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/do_QUfit_1D_mnest.py` & `RM-Tools-1.4.1/RMtools_1D/do_QUfit_1D_mnest.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/do_RMclean_1D.py` & `RM-Tools-1.4.1/RMtools_1D/do_RMclean_1D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/do_RMsynth_1D.py` & `RM-Tools-1.4.1/RMtools_1D/do_RMsynth_1D.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,14 @@
     dirtyFDF, lam0Sq_m2 = do_rmsynth_planes(
         dataQ=qArr,
         dataU=uArr,
         lambdaSqArr_m2=lambdaSqArr_m2,
         phiArr_radm2=phiArr_radm2,
         weightArr=weightArr,
         nBits=nBits,
-        verbose=verbose,
         log=log,
         lam0Sq_m2=0 if super_resolution else None,
     )
 
     # Calculate the Rotation Measure Spread Function
     RMSFArr, phi2Arr_radm2, fwhmRMSFArr, fitStatArr, _ = get_rmsf_planes(
         lambdaSqArr_m2=lambdaSqArr_m2,
```

### Comparing `RM-Tools-1.4.0/RMtools_1D/do_RMsynth_1D_fromFITS.py` & `RM-Tools-1.4.1/RMtools_1D/do_RMsynth_1D_fromFITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/mk_test_ascii_data.py` & `RM-Tools-1.4.1/RMtools_1D/mk_test_ascii_data.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m1.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m1.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m11.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m11.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m111.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m111.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m2.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m2.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m3.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m3.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m4.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m4.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m5.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m5.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m6.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m6.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/models_ns/m7.py` & `RM-Tools-1.4.1/RMtools_1D/models_ns/m7.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/rmtools_bwdepol.py` & `RM-Tools-1.4.1/RMtools_1D/rmtools_bwdepol.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_1D/rmtools_bwpredict.py` & `RM-Tools-1.4.1/RMtools_1D/rmtools_bwpredict.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/RMpeakfit_3D.py` & `RM-Tools-1.4.1/RMtools_3D/RMpeakfit_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/assemble_chunks.py` & `RM-Tools-1.4.1/RMtools_3D/assemble_chunks.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/create_chunks.py` & `RM-Tools-1.4.1/RMtools_3D/create_chunks.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/do_RMclean_3D.py` & `RM-Tools-1.4.1/RMtools_3D/do_RMclean_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/do_RMsynth_3D.py` & `RM-Tools-1.4.1/RMtools_3D/do_RMsynth_3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,14 @@
         FDFcube, lam0Sq_m2 = do_rmsynth_planes(
             dataQ=qArr,
             dataU=uArr,
             lambdaSqArr_m2=lambdaSqArr_m2,
             phiArr_radm2=phiArr_radm2,
             weightArr=weightArr,
             nBits=32,
-            verbose=verbose,
             lam0Sq_m2=0 if super_resolution else None,
         )
     else:
         # need lambda0 for RMSF calculation
         lam0Sq_m2 = 0 if super_resolution else None
 
     # Calculate the Rotation Measure Spread Function cube
```

### Comparing `RM-Tools-1.4.0/RMtools_3D/do_fitIcube.py` & `RM-Tools-1.4.1/RMtools_3D/do_fitIcube.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/extract_region.py` & `RM-Tools-1.4.1/RMtools_3D/extract_region.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/make_freq_file.py` & `RM-Tools-1.4.1/RMtools_3D/make_freq_file.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/mk_test_cube_data.py` & `RM-Tools-1.4.1/RMtools_3D/mk_test_cube_data.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMtools_3D/rescale_I_model_3D.py` & `RM-Tools-1.4.1/RMtools_3D/rescale_I_model_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/mpfit.py` & `RM-Tools-1.4.1/RMutils/mpfit.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/normalize.py` & `RM-Tools-1.4.1/RMutils/normalize.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/util_FITS.py` & `RM-Tools-1.4.1/RMutils/util_FITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/util_RM.py` & `RM-Tools-1.4.1/RMutils/util_RM.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,38 +90,38 @@
     dataQ,
     dataU,
     lambdaSqArr_m2,
     phiArr_radm2,
     weightArr=None,
     lam0Sq_m2=None,
     nBits=32,
-    verbose=False,
+    eps=1e-6,
     log=print,
 ):
     """Perform RM-synthesis on Stokes Q and U cubes (1,2 or 3D). This version
     of the routine loops through spectral planes and is faster than the pixel-
     by-pixel code. This version also correctly deals with isolated clumps of
     NaN-flagged voxels within the data-cube (unlikely in interferometric cubes,
     but possible in single-dish cubes). Input data must be in standard python
     [z,y,x] order, where z is the frequency axis in ascending order.
 
     dataQ           ... 1, 2 or 3D Stokes Q data array
     dataU           ... 1, 2 or 3D Stokes U data array
     lambdaSqArr_m2  ... vector of wavelength^2 values (assending freq order)
     phiArr_radm2    ... vector of trial Faraday depth values
     weightArr       ... vector of weights, default [None] is Uniform (all 1s)
+    lam0Sq_m2       ... force a reference lambda^2 value [None, calculated]
     nBits           ... precision of data arrays [32]
-    verbose         ... print feedback during calculation [False]
+    eps             ... NUFFT tolerance [1e-6] (see https://finufft.readthedocs.io/en/latest/python.html#module-finufft)
     log             ... function to be used to output messages [print]
 
     """
 
     # Default data types
     dtFloat = "float" + str(nBits)
-    dtComplex = "complex" + str(2 * nBits)
 
     # Set the weight array
     if weightArr is None:
         weightArr = np.ones(lambdaSqArr_m2.shape, dtype=dtFloat)
     weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
 
     # Sanity check on array sizes
@@ -191,15 +191,15 @@
     # finufft must have matching dtypes, so complex64 matches float32
     a = (lambdaSqArr_m2 - lam0Sq_m2).astype(f"float{pCube.itemsize*8/2:.0f}")
     FDFcube = (
         finufft.nufft1d3(
             x=a,
             c=np.ascontiguousarray(pCube.T),
             s=(phiArr_radm2[::-1] * 2).astype(a.dtype),
-            eps=1e-8,
+            eps=eps,
         )
         * KArr[..., None]
     ).T
 
     # Check for pixels that have Re(FDF)=Im(FDF)=0. across ALL Faraday depths
     # These pixels will be changed to NaN in the output
     zeromap = np.all(FDFcube == 0.0, axis=0)
@@ -224,14 +224,15 @@
     weightArr=None,
     mskArr=None,
     lam0Sq_m2=None,
     double=True,
     fitRMSF=False,
     fitRMSFreal=False,
     nBits=32,
+    eps=1e-6,
     verbose=False,
     log=print,
 ):
     """Calculate the Rotation Measure Spread Function from inputs. This version
     returns a cube (1, 2 or 3D) of RMSF spectra based on the shape of a
     boolean mask array, where flagged data are True and unflagged data False.
     If only whole planes (wavelength channels) are flagged then the RMSF is the
@@ -246,14 +247,15 @@
     weightArr       ... vector of weights, default [None] is no weighting
     maskArr         ... cube of mask values used to shape return cube [None]
     lam0Sq_m2       ... force a reference lambda^2 value (def=calculate) [None]
     double          ... pad the Faraday depth to double-size [True]
     fitRMSF         ... fit the main lobe of the RMSF with a Gaussian [False]
     fitRMSFreal     ... fit RMSF.real, rather than abs(RMSF) [False]
     nBits           ... precision of data arrays [32]
+    eps             ... NUFFT tolerance [1e-6] (see https://finufft.readthedocs.io/en/latest/python.html#module-finufft)
     verbose         ... print feedback during calculation [False]
     log             ... function to be used to output messages [print]
 
     """
 
     # Default data types
     dtFloat = "float" + str(nBits)
@@ -375,15 +377,15 @@
         # Calculate the RMSF for each plane
         a = (lambdaSqArr_m2 - lam0Sq_m2).astype(dtFloat)
         RMSFcube = (
             finufft.nufft1d3(
                 x=a,
                 c=np.ascontiguousarray(weightCube.T),
                 s=(phiArr_radm2[::-1] * 2).astype(a.dtype),
-                eps=1e-8,
+                eps=eps,
             )
             * KArr[..., None]
         ).T
 
         # Clean up one cube worth of memory
         del weightCube
         gc.collect()
```

### Comparing `RM-Tools-1.4.0/RMutils/util_misc.py` & `RM-Tools-1.4.1/RMutils/util_misc.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/util_plotFITS.py` & `RM-Tools-1.4.1/RMutils/util_plotFITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/util_plotTk.py` & `RM-Tools-1.4.1/RMutils/util_plotTk.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/RMutils/util_rec.py` & `RM-Tools-1.4.1/RMutils/util_rec.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.4.0/setup.py` & `RM-Tools-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import setup
 
 NAME = "RM-Tools"
 DESCRIPTION = "RM-synthesis, RM-clean and QU-fitting on polarised radio spectra"
 URL = "https://github.com/CIRADA-Tools/RM-Tools"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.4.0"
+VERSION = "1.4.1"
 DOWNLOAD_URL = (
     "https://github.com/CIRADA-Tools/RM-Tools/archive/v" + VERSION + ".tar.gz"
 )
 
 REQUIRED = [
     "numpy<2",
     "scipy",
```

