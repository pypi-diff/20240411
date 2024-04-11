# Comparing `tmp/ucx-py-cu11-0.36.0.tar.gz` & `tmp/ucx_py_cu11-0.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucx-py-cu11-0.36.0.tar", last modified: Tue Feb 13 21:14:40 2024, max compression
+gzip compressed data, was "ucx_py_cu11-0.37.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `ucx-py-cu11-0.36.0.tar` & `ucx_py_cu11-0.37.0.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-13 21:14:40.835511 ucx-py-cu11-0.36.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      458 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 ucx-py-cu11-0.36.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       11 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1630 2024-02-13 21:14:40.835511 ucx-py-cu11-0.36.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      253 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-02-13 21:14:40.835511 ucx-py-cu11-0.36.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 ucx-py-cu11-0.36.0/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-13 21:14:40.834511 ucx-py-cu11-0.36.0/ucx_py_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1630 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/ucx_py_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      193 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/ucx_py_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/ucx_py_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-02-13 21:14:40.000000 ucx-py-cu11-0.36.0/ucx_py_cu11.egg-info/top_level.txt
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     2331 1993-04-05 07:00:00.000000 PKG-INFO
```

