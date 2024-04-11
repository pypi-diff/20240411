# Comparing `tmp/gwalk-2.2.0.tar.gz` & `tmp/gwalk-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwalk-2.2.0.tar", last modified: Wed Apr  3 18:11:04 2024, max compression
+gzip compressed data, was "gwalk-2.2.1.tar", last modified: Thu Apr 11 14:49:14 2024, max compression
```

## Comparing `gwalk-2.2.0.tar` & `gwalk-2.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173928 gwalk-2.2.0/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      339 2023-12-12 01:57:59.000000 gwalk-2.2.0/MANIFEST.in
--rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-03 18:11:04.173809 gwalk-2.2.0/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.2.0/README.md
--rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-03 18:10:57.000000 gwalk-2.2.0/__version__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      515 2023-08-15 23:07:31.000000 gwalk-2.2.0/pyproject.toml
--rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2024-04-03 18:11:04.174216 gwalk-2.2.0/setup.cfg
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5617 2023-12-12 01:57:59.000000 gwalk-2.2.0/setup.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.109295 gwalk-2.2.0/src/
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.127414 gwalk-2.2.0/src/gwalk/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-03 18:10:57.000000 gwalk-2.2.0/src/gwalk/__version__.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.130660 gwalk-2.2.0/src/gwalk/c_utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/c_utils/dbg.h
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.132444 gwalk-2.2.0/src/gwalk/catalog/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    29447 2023-05-02 15:45:34.000000 gwalk-2.2.0/src/gwalk/catalog/catalog.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/coordinates.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.143574 gwalk-2.2.0/src/gwalk/catalog/prior/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/CIP_prior_functions.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/callister_prior.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/catalog/prior/prior_methods.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5712 2023-05-02 15:46:03.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:14.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3070 2023-05-02 15:46:22.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2p1.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3071 2023-05-02 15:46:27.000000 gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_3.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.149861 gwalk-2.2.0/src/gwalk/density/
--rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/density/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/density/mesh.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.158645 gwalk-2.2.0/src/gwalk/multivariate_normal/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_decomposition.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_mahalanobis_distance.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
--rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition_numpy.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    37193 2024-04-03 17:24:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/pdf.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11805 2024-04-03 18:08:34.000000 gwalk-2.2.0/src/gwalk/multivariate_normal/utils.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     6816 2023-12-12 01:57:59.000000 gwalk-2.2.0/src/gwalk/optimize_likelihood_grid.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.159953 gwalk-2.2.0/src/gwalk/plots/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/axis.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/likelihood_corner.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/percentile_levels.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/plots/walker_plot.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.164101 gwalk-2.2.0/src/gwalk/tools/
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/NAL_event_pipeline.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/collect.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/example_script.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/fit_catalog_samples.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/tools/fit_likelihood_grid.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/load_best_fits.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/plot_mesh_norm_corner.py
--rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/tools/populate_nal_figures.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.2.0/src/gwalk/tools/test_catalog_samples.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.164965 gwalk-2.2.0/src/gwalk/utils/
--rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/utils/__init__.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.2.0/src/gwalk/utils/hist.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-04-25 18:43:04.000000 gwalk-2.2.0/src/gwalk/utils/multivariate_normal.py
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173412 gwalk-2.2.0/src/gwalk.egg-info/
--rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/PKG-INFO
--rw-r--r--   0 vdelfave (669582709) staff       (20)     2057 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/SOURCES.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/dependency_links.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)      131 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/requires.txt
--rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2024-04-03 18:11:04.000000 gwalk-2.2.0/src/gwalk.egg-info/top_level.txt
-drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-03 18:11:04.173072 gwalk-2.2.0/tests/
--rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_decomposition.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3984 2023-12-12 01:57:59.000000 gwalk-2.2.0/tests/test_dpgmm.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_grid.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_kl.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_maha.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)    14181 2024-04-03 18:09:35.000000 gwalk-2.2.0/tests/test_object.py
--rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-04-25 18:43:04.000000 gwalk-2.2.0/tests/test_pdf.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.347604 gwalk-2.2.1/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      339 2023-12-12 01:57:59.000000 gwalk-2.2.1/MANIFEST.in
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-11 14:49:14.347478 gwalk-2.2.1/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2029 2022-11-15 19:49:14.000000 gwalk-2.2.1/README.md
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-11 14:49:05.000000 gwalk-2.2.1/__version__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      515 2023-08-15 23:07:31.000000 gwalk-2.2.1/pyproject.toml
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       63 2024-04-11 14:49:14.347895 gwalk-2.2.1/setup.cfg
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5617 2023-12-12 01:57:59.000000 gwalk-2.2.1/setup.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.268312 gwalk-2.2.1/src/
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.284818 gwalk-2.2.1/src/gwalk/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      307 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       20 2024-04-11 14:49:05.000000 gwalk-2.2.1/src/gwalk/__version__.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.286491 gwalk-2.2.1/src/gwalk/c_utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1236 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/c_utils/dbg.h
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.306447 gwalk-2.2.1/src/gwalk/catalog/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    29447 2023-05-02 15:45:34.000000 gwalk-2.2.1/src/gwalk/catalog/catalog.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17506 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/coordinates.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.307647 gwalk-2.2.1/src/gwalk/catalog/prior/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4574 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/prior/CIP_prior_functions.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/prior/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11432 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/prior/callister_prior.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4176 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/catalog/prior/prior_methods.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5702 2024-04-09 15:33:18.000000 gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3203 2024-04-09 15:30:06.000000 gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_2.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3202 2024-04-09 15:30:01.000000 gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_2p1.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3203 2024-04-09 15:30:13.000000 gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_3.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.308264 gwalk-2.2.1/src/gwalk/density/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)       23 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/density/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    50044 2023-01-24 15:58:53.000000 gwalk-2.2.1/src/gwalk/density/mesh.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.333512 gwalk-2.2.1/src/gwalk/multivariate_normal/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      108 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    24841 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/_decomposition.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6289 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/_mahalanobis_distance.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    25977 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    27446 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/bounded_multivariate_normal.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    17947 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13587 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/decomposition_numpy.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    37193 2024-04-03 17:24:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11599 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/pdf.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11805 2024-04-03 18:08:34.000000 gwalk-2.2.1/src/gwalk/multivariate_normal/utils.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     6816 2023-12-12 01:57:59.000000 gwalk-2.2.1/src/gwalk/optimize_likelihood_grid.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.335414 gwalk-2.2.1/src/gwalk/plots/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/plots/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     7254 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/plots/axis.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     8166 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/plots/likelihood_corner.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1578 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/plots/percentile_levels.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      686 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/plots/walker_plot.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.341424 gwalk-2.2.1/src/gwalk/tools/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5546 2023-01-24 15:58:53.000000 gwalk-2.2.1/src/gwalk/tools/NAL_event_pipeline.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2937 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/collect.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13900 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/example_script.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13076 2023-01-24 15:58:53.000000 gwalk-2.2.1/src/gwalk/tools/fit_catalog_samples.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     1681 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/tools/fit_likelihood_grid.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     5595 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/load_best_fits.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4668 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/plot_mesh_norm_corner.py
+-rwxr-xr-x   0 vdelfave (669582709) staff       (20)     4068 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/tools/populate_nal_figures.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    11425 2023-01-24 15:58:53.000000 gwalk-2.2.1/src/gwalk/tools/test_catalog_samples.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.342210 gwalk-2.2.1/src/gwalk/utils/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        0 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/utils/__init__.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3186 2022-11-15 19:49:15.000000 gwalk-2.2.1/src/gwalk/utils/hist.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      133 2023-04-25 18:43:04.000000 gwalk-2.2.1/src/gwalk/utils/multivariate_normal.py
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.347070 gwalk-2.2.1/src/gwalk.egg-info/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      932 2024-04-11 14:49:14.000000 gwalk-2.2.1/src/gwalk.egg-info/PKG-INFO
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     2057 2024-04-11 14:49:14.000000 gwalk-2.2.1/src/gwalk.egg-info/SOURCES.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        1 2024-04-11 14:49:14.000000 gwalk-2.2.1/src/gwalk.egg-info/dependency_links.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)      131 2024-04-11 14:49:14.000000 gwalk-2.2.1/src/gwalk.egg-info/requires.txt
+-rw-r--r--   0 vdelfave (669582709) staff       (20)        6 2024-04-11 14:49:14.000000 gwalk-2.2.1/src/gwalk.egg-info/top_level.txt
+drwxr-xr-x   0 vdelfave (669582709) staff       (20)        0 2024-04-11 14:49:14.346716 gwalk-2.2.1/tests/
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    13966 2023-04-25 18:43:04.000000 gwalk-2.2.1/tests/test_decomposition.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3984 2023-12-12 01:57:59.000000 gwalk-2.2.1/tests/test_dpgmm.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3304 2023-04-25 18:43:04.000000 gwalk-2.2.1/tests/test_grid.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     5810 2023-04-25 18:43:04.000000 gwalk-2.2.1/tests/test_kl.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     3882 2023-04-25 18:43:04.000000 gwalk-2.2.1/tests/test_maha.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)    14181 2024-04-03 18:09:35.000000 gwalk-2.2.1/tests/test_object.py
+-rw-r--r--   0 vdelfave (669582709) staff       (20)     4824 2023-04-25 18:43:04.000000 gwalk-2.2.1/tests/test_pdf.py
```

### Comparing `gwalk-2.2.0/PKG-INFO` & `gwalk-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.2.0
+Version: 2.2.1
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.2.0/README.md` & `gwalk-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/pyproject.toml` & `gwalk-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/setup.py` & `gwalk-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/c_utils/dbg.h` & `gwalk-2.2.1/src/gwalk/c_utils/dbg.h`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/catalog.py` & `gwalk-2.2.1/src/gwalk/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/coordinates.py` & `gwalk-2.2.1/src/gwalk/catalog/coordinates.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/prior/CIP_prior_functions.py` & `gwalk-2.2.1/src/gwalk/catalog/prior/CIP_prior_functions.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/prior/callister_prior.py` & `gwalk-2.2.1/src/gwalk/catalog/prior/callister_prior.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/prior/prior_methods.py` & `gwalk-2.2.1/src/gwalk/catalog/prior/prior_methods.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_1.py` & `gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 '''\
 Read samples from GWTC-1_sample_release and convert to source frame
 '''
 
 ######## Imports ########
-from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
-from gwalk.catalog.coordinates import z_from_lum_dist_interp
-from gwalk.catalog.coordinates import source_from_detector
-from gwalk.catalog.coordinates import detector_from_source
-from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
+from gwalk.catalog.coordinates import z_of_lum_dist_interp
 from gwalk.catalog.coordinates import coord_labels
-from gwalk.catalog.coordinates import lambdatilde_of_eta_lam1_lam2
-from gwalk.catalog.coordinates import deltalambda_of_eta_lam1_lam2
+from basil_core.astro.coordinates import m1_m2_of_mc_eta, mc_eta_of_m1_m2
+from basil_core.astro.coordinates import detector_of_source, source_of_detector
+from basil_core.astro.coordinates import chieff_of_m1_m2_chi1z_chi2z
+from basil_core.astro.coordinates import lambda_tilde_of_eta_lambda1_lambda2
+from basil_core.astro.coordinates import delta_lambda_of_eta_lambda1_lambda2
 from os.path import join, isfile
 from xdata.database import Database
 
 ######## Functions ########
 #### Database handling ####
 
 def get_samples(
@@ -108,15 +107,15 @@
     pdict["cos_tilt_1"] = name_dict["costilt1"]
     pdict["cos_tilt_2"] = name_dict["costilt2"]
 
     ## Find redshift
     # Load luminosity distance in Mpc
     lum_dist = np.copy(name_dict["luminosity_distance_Mpc"])
     # Find redshift
-    Z = z_from_lum_dist_interp(lum_dist, nbins = z_bins)
+    Z = z_of_lum_dist_interp(lum_dist, nbins = z_bins)
     # Append to dictionary
     pdict["redshift"] = np.copy(Z)
 
 
 
     pdict["cos_theta_jn"] = name_dict["costheta_jn"]
     pdict["luminosity_distance"] = name_dict["luminosity_distance_Mpc"]
@@ -124,25 +123,25 @@
     pdict["dec"] = name_dict["declination"]
     pdict["mass_1"] = name_dict["m1_detector_frame_Msun"]
     pdict["mass_2"] = name_dict["m2_detector_frame_Msun"]
     pdict["a_1"] = name_dict["spin1"]
     pdict["a_2"] = name_dict["spin2"]
 
     # Find source frame masses
-    mc, eta = mc_eta_from_m1m2(name_dict["m1_detector_frame_Msun"],
+    mc, eta = mc_eta_of_m1_m2(name_dict["m1_detector_frame_Msun"],
                                name_dict["m2_detector_frame_Msun"])
-    m1_source = source_from_detector(name_dict["m1_detector_frame_Msun"], Z)
-    m2_source = source_from_detector(name_dict["m2_detector_frame_Msun"], Z)
-    mc_source, eta_source = mc_eta_from_m1m2(m1_source, m2_source)
+    m1_source = source_of_detector(name_dict["m1_detector_frame_Msun"], Z)
+    m2_source = source_of_detector(name_dict["m2_detector_frame_Msun"], Z)
+    mc_source, eta_source = mc_eta_of_m1_m2(m1_source, m2_source)
     # Find Chieff
     spin_1z = pdict["a_1"]*pdict["cos_tilt_1"]
     spin_2z = pdict["a_2"]*pdict["cos_tilt_2"]
     spin_1xy = pdict["a_1"]*np.power(1 - pdict["cos_tilt_1"]**2, 0.5)
     spin_2xy = pdict["a_2"]*np.power(1 - pdict["cos_tilt_2"]**2, 0.5)
-    chieff = chieff_from_m1m2s1s2(m1_source, m2_source, spin_1z, spin_2z)
+    chieff = chieff_of_m1_m2_chi1z_chi2z(m1_source, m2_source, spin_1z, spin_2z)
     # Append to dictionary
     pdict["mass_1_source"] = m1_source
     pdict["mass_2_source"] = m2_source
     pdict["chirp_mass_source"] = mc_source
     pdict["chirp_mass"] = mc
     pdict["symmetric_mass_ratio"] = eta
     pdict["chi_eff"] = chieff
```

### Comparing `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2.py` & `gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_2p1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 #!/home/xevra/.local/bin/python3
 '''\
 Generate the likelihood function of each event
 '''
 
 ######## Imports ########
 import numpy as np
-from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
-from gwalk.catalog.coordinates import z_from_lum_dist_interp
-from gwalk.catalog.coordinates import source_from_detector
-from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
+from basil_core.astro.coordinates import m1_m2_of_mc_eta, mc_eta_of_m1_m2
+from basil_core.astro.coordinates import detector_of_source, source_of_detector
+from basil_core.astro.coordinates import chieff_of_m1_m2_chi1z_chi2z
+from basil_core.astro.coordinates import lambda_tilde_of_eta_lambda1_lambda2
+from basil_core.astro.coordinates import delta_lambda_of_eta_lambda1_lambda2
 from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
                 names,
                 group = "PublicationSamples",
                ):
     '''Get the posterior samples we need
-
     Parameters
     ----------
     fname_event: str
         Input file name  for catalog samples
     names: list
         Input list of names to draw from catalog samples
     group: str
@@ -81,15 +81,15 @@
                        )
 
     # Generate some things not given
     pdict["inv_lum_dist"] = np.power(pdict["luminosity_distance"],-1.)
 
     # Check on spin coordinates
     if not "chi_eff" in pdict:
-        pdict["chi_eff"] = chieff_from_m1m2s1s2(
+        pdict["chi_eff"] = chieff_of_m1_m2_chi1z_chi2z(
                                                 pdict["mass_1_source"],
                                                 pdict["mass_2_source"],
                                                 pdict["a_1"],
                                                 pdict["a_2"],
                                                )
     # Check aligned spin
     if not "spin_1z" in pdict:
```

### Comparing `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_2p1.py` & `gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/home/xevra/.local/bin/python3
 '''\
 Generate the likelihood function of each event
 '''
 
 ######## Imports ########
 import numpy as np
-from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
-from gwalk.catalog.coordinates import z_from_lum_dist_interp
-from gwalk.catalog.coordinates import source_from_detector
-from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
+from basil_core.astro.coordinates import m1_m2_of_mc_eta, mc_eta_of_m1_m2
+from basil_core.astro.coordinates import detector_of_source, source_of_detector
+from basil_core.astro.coordinates import chieff_of_m1_m2_chi1z_chi2z
+from basil_core.astro.coordinates import lambda_tilde_of_eta_lambda1_lambda2
+from basil_core.astro.coordinates import delta_lambda_of_eta_lambda1_lambda2
 from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
                 names,
                 group = "PublicationSamples",
                ):
     '''Get the posterior samples we need
+
     Parameters
     ----------
     fname_event: str
         Input file name  for catalog samples
     names: list
         Input list of names to draw from catalog samples
     group: str
@@ -80,15 +82,15 @@
                        )
 
     # Generate some things not given
     pdict["inv_lum_dist"] = np.power(pdict["luminosity_distance"],-1.)
 
     # Check on spin coordinates
     if not "chi_eff" in pdict:
-        pdict["chi_eff"] = chieff_from_m1m2s1s2(
+        pdict["chi_eff"] = chieff_of_m1_m2_chi1z_chi2z(
                                                 pdict["mass_1_source"],
                                                 pdict["mass_2_source"],
                                                 pdict["a_1"],
                                                 pdict["a_2"],
                                                )
     # Check aligned spin
     if not "spin_1z" in pdict:
```

### Comparing `gwalk-2.2.0/src/gwalk/catalog/read_catalog_GWTC_3.py` & `gwalk-2.2.1/src/gwalk/catalog/read_catalog_GWTC_3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/home/xevra/.local/bin/python3
 '''\
 Generate the likelihood function of each event
 '''
 
 ######## Imports ########
 import numpy as np
-from gwalk.catalog.coordinates import m1m2_from_mc_eta, mc_eta_from_m1m2
-from gwalk.catalog.coordinates import z_from_lum_dist_interp
-from gwalk.catalog.coordinates import source_from_detector
-from gwalk.catalog.coordinates import chieff_from_m1m2s1s2
 from gwalk.catalog.coordinates import coord_labels
+from basil_core.astro.coordinates import m1_m2_of_mc_eta, mc_eta_of_m1_m2
+from basil_core.astro.coordinates import detector_of_source, source_of_detector
+from basil_core.astro.coordinates import chieff_of_m1_m2_chi1z_chi2z
+from basil_core.astro.coordinates import lambda_tilde_of_eta_lambda1_lambda2
+from basil_core.astro.coordinates import delta_lambda_of_eta_lambda1_lambda2
 from xdata.database import Database
 from os.path import join, isfile
 
 ######## Functions ########
 #### Database handling ####
 def get_samples(
                 fname_event,
@@ -80,15 +81,15 @@
                        )
 
     # Generate some things not given
     pdict["inv_lum_dist"] = np.power(pdict["luminosity_distance"],-1.)
 
     # Check on spin coordinates
     if not "chi_eff" in pdict:
-        pdict["chi_eff"] = chieff_from_m1m2s1s2(
+        pdict["chi_eff"] = chieff_of_m1_m2_chi1z_chi2z(
                                                 pdict["mass_1_source"],
                                                 pdict["mass_2_source"],
                                                 pdict["a_1"],
                                                 pdict["a_2"],
                                                )
     # Check aligned spin
     if not "spin_1z" in pdict:
```

### Comparing `gwalk-2.2.0/src/gwalk/density/mesh.py` & `gwalk-2.2.1/src/gwalk/density/mesh.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/_decomposition.c` & `gwalk-2.2.1/src/gwalk/multivariate_normal/_decomposition.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/_mahalanobis_distance.c` & `gwalk-2.2.1/src/gwalk/multivariate_normal/_mahalanobis_distance.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c` & `gwalk-2.2.1/src/gwalk/multivariate_normal/_multivariate_normal_pdf_utils.c`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/bounded_multivariate_normal.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/bounded_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/decomposition_numpy.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/decomposition_numpy.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/object.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/object.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/pdf.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/pdf.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/multivariate_normal/utils.py` & `gwalk-2.2.1/src/gwalk/multivariate_normal/utils.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/optimize_likelihood_grid.py` & `gwalk-2.2.1/src/gwalk/optimize_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/plots/axis.py` & `gwalk-2.2.1/src/gwalk/plots/axis.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/plots/likelihood_corner.py` & `gwalk-2.2.1/src/gwalk/plots/likelihood_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/plots/percentile_levels.py` & `gwalk-2.2.1/src/gwalk/plots/percentile_levels.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/plots/walker_plot.py` & `gwalk-2.2.1/src/gwalk/plots/walker_plot.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/NAL_event_pipeline.py` & `gwalk-2.2.1/src/gwalk/tools/NAL_event_pipeline.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/collect.py` & `gwalk-2.2.1/src/gwalk/tools/collect.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/example_script.py` & `gwalk-2.2.1/src/gwalk/tools/example_script.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/fit_catalog_samples.py` & `gwalk-2.2.1/src/gwalk/tools/fit_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/fit_likelihood_grid.py` & `gwalk-2.2.1/src/gwalk/tools/fit_likelihood_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/load_best_fits.py` & `gwalk-2.2.1/src/gwalk/tools/load_best_fits.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/plot_mesh_norm_corner.py` & `gwalk-2.2.1/src/gwalk/tools/plot_mesh_norm_corner.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/populate_nal_figures.py` & `gwalk-2.2.1/src/gwalk/tools/populate_nal_figures.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/tools/test_catalog_samples.py` & `gwalk-2.2.1/src/gwalk/tools/test_catalog_samples.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk/utils/hist.py` & `gwalk-2.2.1/src/gwalk/utils/hist.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/src/gwalk.egg-info/PKG-INFO` & `gwalk-2.2.1/src/gwalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwalk
-Version: 2.2.0
+Version: 2.2.1
 Home-page: https://gitlab.com/xevra/gwalk
 Author: Vera Del Favero
 Author-email: xevra86@gmail.com
 Maintainer: Vera Del Favero
 Maintainer-email: xevra86@gmail.com
 License: MIT Lisence
 Keywords: Gravitational Wave,Likelihood
```

### Comparing `gwalk-2.2.0/src/gwalk.egg-info/SOURCES.txt` & `gwalk-2.2.1/src/gwalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_decomposition.py` & `gwalk-2.2.1/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_dpgmm.py` & `gwalk-2.2.1/tests/test_dpgmm.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_grid.py` & `gwalk-2.2.1/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_kl.py` & `gwalk-2.2.1/tests/test_kl.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_maha.py` & `gwalk-2.2.1/tests/test_maha.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_object.py` & `gwalk-2.2.1/tests/test_object.py`

 * *Files identical despite different names*

### Comparing `gwalk-2.2.0/tests/test_pdf.py` & `gwalk-2.2.1/tests/test_pdf.py`

 * *Files identical despite different names*

