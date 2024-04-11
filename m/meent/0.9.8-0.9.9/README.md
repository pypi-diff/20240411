# Comparing `tmp/meent-0.9.8.tar.gz` & `tmp/meent-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meent-0.9.8.tar", last modified: Fri Mar  8 07:45:19 2024, max compression
+gzip compressed data, was "meent-0.9.9.tar", last modified: Thu Apr 11 03:16:19 2024, max compression
```

## Comparing `meent-0.9.8.tar` & `meent-0.9.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.349849 meent-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-08 07:45:14.000000 meent-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-08 07:45:19.349849 meent-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-03-08 07:45:14.000000 meent-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.337849 meent-0.9.8/meent/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-08 07:45:14.000000 meent-0.9.8/meent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-03-08 07:45:14.000000 meent-0.9.8/meent/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.333849 meent-0.9.8/meent/nk_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.337849 meent-0.9.8/meent/nk_data/filmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-08 07:45:14.000000 meent-0.9.8/meent/nk_data/filmetrics/Al2O3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-08 07:45:14.000000 meent-0.9.8/meent/nk_data/filmetrics/Si.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-03-08 07:45:14.000000 meent-0.9.8/meent/nk_data/filmetrics/Si3N4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-03-08 07:45:14.000000 meent-0.9.8/meent/nk_data/filmetrics/SiO2.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.337849 meent-0.9.8/meent/nk_data/matlab/
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-03-08 07:45:14.000000 meent-0.9.8/meent/nk_data/matlab/p_Si.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.337849 meent-0.9.8/meent/on_jax/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.341849 meent-0.9.8/meent/on_jax/emsolver/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    38784 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.341849 meent-0.9.8/meent/on_jax/modeler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.341849 meent-0.9.8/meent/on_jax/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_jax/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.341849 meent-0.9.8/meent/on_numpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.341849 meent-0.9.8/meent/on_numpy/emsolver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11441 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    27387 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent/on_numpy/modeler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_numpy/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent/on_torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent/on_torch/emsolver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20221 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/convolution_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/field_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/rcwa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/scattering_method.py
--rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/smm_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/emsolver/transfer_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/mee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent/on_torch/modeler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/modeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18450 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/modeler/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent/on_torch/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/optimizer/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-08 07:45:14.000000 meent-0.9.8/meent/on_torch/optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 07:45:19.345849 meent-0.9.8/meent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-08 07:45:19.000000 meent-0.9.8/meent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-03-08 07:45:19.000000 meent-0.9.8/meent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 07:45:19.000000 meent-0.9.8/meent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-08 07:45:19.000000 meent-0.9.8/meent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-08 07:45:19.000000 meent-0.9.8/meent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 07:45:19.349849 meent-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-08 07:45:14.000000 meent-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.588226 meent-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-11 03:16:15.000000 meent-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 03:16:19.588226 meent-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-11 03:16:15.000000 meent-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.576226 meent-0.9.9/meent/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 03:16:15.000000 meent-0.9.9/meent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-11 03:16:15.000000 meent-0.9.9/meent/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.576226 meent-0.9.9/meent/nk_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/nk_data/filmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 03:16:15.000000 meent-0.9.9/meent/nk_data/filmetrics/Al2O3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-11 03:16:15.000000 meent-0.9.9/meent/nk_data/filmetrics/Si.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-11 03:16:15.000000 meent-0.9.9/meent/nk_data/filmetrics/Si3N4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-11 03:16:15.000000 meent-0.9.9/meent/nk_data/filmetrics/SiO2.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/nk_data/matlab/
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-11 03:16:15.000000 meent-0.9.9/meent/nk_data/matlab/p_Si.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/on_jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/on_jax/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16856 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12769 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38784 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/on_jax/modeler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.580226 meent-0.9.9/meent/on_jax/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_jax/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_numpy/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11441 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27387 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9893 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_numpy/modeler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_numpy/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_torch/emsolver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18869 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20221 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/convolution_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/field_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/rcwa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/scattering_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10516 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/smm_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/emsolver/transfer_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/mee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.584226 meent-0.9.9/meent/on_torch/modeler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/modeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31872 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/modeler/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.588226 meent-0.9.9/meent/on_torch/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/optimizer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-11 03:16:15.000000 meent-0.9.9/meent/on_torch/optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:19.588226 meent-0.9.9/meent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-11 03:16:19.000000 meent-0.9.9/meent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-11 03:16:19.000000 meent-0.9.9/meent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:16:19.000000 meent-0.9.9/meent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 03:16:19.000000 meent-0.9.9/meent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:16:19.000000 meent-0.9.9/meent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:16:19.588226 meent-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-11 03:16:15.000000 meent-0.9.9/setup.py
```

### Comparing `meent-0.9.8/LICENSE` & `meent-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/PKG-INFO` & `meent-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meent
-Version: 0.9.8
+Version: 0.9.9
 Home-page: https://github.com/kc-ml2/meent
 Author: KC ML2
 Author-email: yongha@kc-ml2.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.3
```

### Comparing `meent-0.9.8/README.md` & `meent-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/main.py` & `meent-0.9.9/meent/main.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/nk_data/filmetrics/Al2O3.txt` & `meent-0.9.9/meent/nk_data/filmetrics/Al2O3.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/nk_data/filmetrics/Si.txt` & `meent-0.9.9/meent/nk_data/filmetrics/Si.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/nk_data/filmetrics/Si3N4.txt` & `meent-0.9.9/meent/nk_data/filmetrics/Si3N4.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/nk_data/filmetrics/SiO2.txt` & `meent-0.9.9/meent/nk_data/filmetrics/SiO2.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/nk_data/matlab/p_Si.mat` & `meent-0.9.9/meent/nk_data/matlab/p_Si.mat`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/_base.py` & `meent-0.9.9/meent/on_jax/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/convolution_matrix.py` & `meent-0.9.9/meent/on_jax/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/field_distribution.py` & `meent-0.9.9/meent/on_jax/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/primitives.py` & `meent-0.9.9/meent/on_jax/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/rcwa.py` & `meent-0.9.9/meent/on_jax/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/scattering_method.py` & `meent-0.9.9/meent/on_jax/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/smm_util.py` & `meent-0.9.9/meent/on_jax/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/emsolver/transfer_method.py` & `meent-0.9.9/meent/on_jax/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/mee.py` & `meent-0.9.9/meent/on_jax/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/modeler/modeling.py` & `meent-0.9.9/meent/on_jax/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/optimizer/loss.py` & `meent-0.9.9/meent/on_jax/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_jax/optimizer/optimizer.py` & `meent-0.9.9/meent/on_jax/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/_base.py` & `meent-0.9.9/meent/on_numpy/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/convolution_matrix.py` & `meent-0.9.9/meent/on_numpy/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/field_distribution.py` & `meent-0.9.9/meent/on_numpy/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/rcwa.py` & `meent-0.9.9/meent/on_numpy/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/scattering_method.py` & `meent-0.9.9/meent/on_numpy/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/smm_util.py` & `meent-0.9.9/meent/on_numpy/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/emsolver/transfer_method.py` & `meent-0.9.9/meent/on_numpy/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/mee.py` & `meent-0.9.9/meent/on_numpy/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_numpy/modeler/modeling.py` & `meent-0.9.9/meent/on_numpy/modeler/modeling.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/_base.py` & `meent-0.9.9/meent/on_torch/emsolver/_base.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/convolution_matrix.py` & `meent-0.9.9/meent/on_torch/emsolver/convolution_matrix.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/field_distribution.py` & `meent-0.9.9/meent/on_torch/emsolver/field_distribution.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/primitives.py` & `meent-0.9.9/meent/on_torch/emsolver/primitives.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/rcwa.py` & `meent-0.9.9/meent/on_torch/emsolver/rcwa.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/scattering_method.py` & `meent-0.9.9/meent/on_torch/emsolver/scattering_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/smm_util.py` & `meent-0.9.9/meent/on_torch/emsolver/smm_util.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/emsolver/transfer_method.py` & `meent-0.9.9/meent/on_torch/emsolver/transfer_method.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/mee.py` & `meent-0.9.9/meent/on_torch/mee.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/optimizer/loss.py` & `meent-0.9.9/meent/on_torch/optimizer/loss.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent/on_torch/optimizer/optimizer.py` & `meent-0.9.9/meent/on_torch/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/meent.egg-info/PKG-INFO` & `meent-0.9.9/meent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meent
-Version: 0.9.8
+Version: 0.9.9
 Home-page: https://github.com/kc-ml2/meent
 Author: KC ML2
 Author-email: yongha@kc-ml2.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.3
```

### Comparing `meent-0.9.8/meent.egg-info/SOURCES.txt` & `meent-0.9.9/meent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meent-0.9.8/setup.py` & `meent-0.9.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             ],
     'pytorch': ['torch>=2.0.0',
                 'tqdm>=4.64.1',
                 ],
 }
 setup(
     name='meent',
-    version='0.9.8',
+    version='0.9.9',
     url='https://github.com/kc-ml2/meent',
     author='KC ML2',
     author_email='yongha@kc-ml2.com',
     packages=['meent'] + find_packages(include=['meent.*']),
     install_requires=[
         'numpy>=1.23.3',
         'scipy>=1.9.1',
```

