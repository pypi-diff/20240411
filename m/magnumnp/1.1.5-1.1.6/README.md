# Comparing `tmp/magnumnp-1.1.5.tar.gz` & `tmp/magnumnp-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnumnp-1.1.5.tar", last modified: Thu Feb 22 13:02:13 2024, max compression
+gzip compressed data, was "magnumnp-1.1.6.tar", last modified: Thu Apr 11 08:37:32 2024, max compression
```

## Comparing `magnumnp-1.1.5.tar` & `magnumnp-1.1.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.925202 magnumnp-1.1.5/
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-02-22 13:01:58.000000 magnumnp-1.1.5/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35069 2024-02-22 13:01:58.000000 magnumnp-1.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8253 2024-02-22 13:02:13.924202 magnumnp-1.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7554 2024-02-22 13:01:58.000000 magnumnp-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.920202 magnumnp-1.1.5/magnumnp/
--rw-rw-rw-   0 root         (0) root         (0)     1027 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.921202 magnumnp-1.1.5/magnumnp/common/
--rw-rw-rw-   0 root         (0) root         (0)     1366 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2624 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/decorated_tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     8932 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1919 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/material.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/mesh.py
--rw-rw-rw-   0 root         (0) root         (0)     7593 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/state.py
--rw-rw-rw-   0 root         (0) root         (0)    38962 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/tabulate.py
--rw-rw-rw-   0 root         (0) root         (0)     1364 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/time_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     8878 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/common/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.922202 magnumnp-1.1.5/magnumnp/field_terms/
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/anisotropy.py
--rw-rw-rw-   0 root         (0) root         (0)     8514 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/demag.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/demagPBC.py
--rw-rw-rw-   0 root         (0) root         (0)     6734 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/demag_nonequidistant.py
--rw-rw-rw-   0 root         (0) root         (0)     8623 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/dmi.py
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     1877 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/external.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/field_terms.py
--rw-rw-rw-   0 root         (0) root         (0)     6437 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/oersted.py
--rw-rw-rw-   0 root         (0) root         (0)     4936 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/rkky.py
--rw-rw-rw-   0 root         (0) root         (0)     3091 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/rux.py
--rw-rw-rw-   0 root         (0) root         (0)     5560 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/spintorque.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/field_terms/thermal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.923202 magnumnp-1.1.5/magnumnp/loggers/
--rw-rw-rw-   0 root         (0) root         (0)      943 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/loggers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5852 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/loggers/field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/loggers/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7570 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/loggers/scalar_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.923202 magnumnp-1.1.5/magnumnp/solvers/
--rw-rw-rw-   0 root         (0) root         (0)     4661 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/LBFGS.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/eigensolver.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/llg.py
--rw-rw-rw-   0 root         (0) root         (0)     4089 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/minimize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.924202 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/
--rw-rw-rw-   0 root         (0) root         (0)     1119 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1575 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/heun.py
--rw-rw-rw-   0 root         (0) root         (0)     4534 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/rkf45.py
--rw-rw-rw-   0 root         (0) root         (0)     4917 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/rkf56.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/scipy_ode.py
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/scipy_odeint.py
--rw-rw-rw-   0 root         (0) root         (0)     3256 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ode_solvers/torchdiffeq.py
--rw-rw-rw-   0 root         (0) root         (0)     3640 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/ohm_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/steepest_descent.py
--rw-rw-rw-   0 root         (0) root         (0)     3334 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/solvers/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.924202 magnumnp-1.1.5/magnumnp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6669 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/utils/imaging_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2024-02-22 13:01:59.000000 magnumnp-1.1.5/magnumnp/utils/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:02:13.924202 magnumnp-1.1.5/magnumnp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8253 2024-02-22 13:02:13.000000 magnumnp-1.1.5/magnumnp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1710 2024-02-22 13:02:13.000000 magnumnp-1.1.5/magnumnp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 13:02:13.000000 magnumnp-1.1.5/magnumnp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-02-22 13:02:13.000000 magnumnp-1.1.5/magnumnp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-22 13:02:13.000000 magnumnp-1.1.5/magnumnp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 13:02:13.925202 magnumnp-1.1.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1909 2024-02-22 13:02:08.000000 magnumnp-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.015821 magnumnp-1.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-04-11 08:37:19.000000 magnumnp-1.1.6/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35069 2024-04-11 08:37:19.000000 magnumnp-1.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-11 08:37:32.014821 magnumnp-1.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2024-04-11 08:37:19.000000 magnumnp-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.010821 magnumnp-1.1.6/magnumnp/
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.011821 magnumnp-1.1.6/magnumnp/common/
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2624 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/decorated_tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     8932 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1919 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/material.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/mesh.py
+-rw-rw-rw-   0 root         (0) root         (0)     7593 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/state.py
+-rw-rw-rw-   0 root         (0) root         (0)    38962 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/tabulate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/time_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8878 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/common/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.012821 magnumnp-1.1.6/magnumnp/field_terms/
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/anisotropy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8514 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/demag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/demagPBC.py
+-rw-rw-rw-   0 root         (0) root         (0)     6734 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/demag_nonequidistant.py
+-rw-rw-rw-   0 root         (0) root         (0)     8623 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/dmi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/external.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/field_terms.py
+-rw-rw-rw-   0 root         (0) root         (0)     6437 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/oersted.py
+-rw-rw-rw-   0 root         (0) root         (0)     6783 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/rkky.py
+-rw-rw-rw-   0 root         (0) root         (0)     3091 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/rux.py
+-rw-rw-rw-   0 root         (0) root         (0)     5560 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/spintorque.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/field_terms/thermal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.012821 magnumnp-1.1.6/magnumnp/loggers/
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/loggers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5852 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/loggers/field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/loggers/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7570 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/loggers/scalar_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.013821 magnumnp-1.1.6/magnumnp/solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/LBFGS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/eigensolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/llg.py
+-rw-rw-rw-   0 root         (0) root         (0)     4089 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/minimize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.014821 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)     1119 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/heun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4534 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/rkf45.py
+-rw-rw-rw-   0 root         (0) root         (0)     4917 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/rkf56.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/scipy_ode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/scipy_odeint.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ode_solvers/torchdiffeq.py
+-rw-rw-rw-   0 root         (0) root         (0)     3640 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/ohm_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/steepest_descent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/solvers/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.014821 magnumnp-1.1.6/magnumnp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6669 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/utils/imaging_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2024-04-11 08:37:19.000000 magnumnp-1.1.6/magnumnp/utils/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:37:32.014821 magnumnp-1.1.6/magnumnp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-11 08:37:31.000000 magnumnp-1.1.6/magnumnp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-11 08:37:32.000000 magnumnp-1.1.6/magnumnp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:37:32.000000 magnumnp-1.1.6/magnumnp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-11 08:37:32.000000 magnumnp-1.1.6/magnumnp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 08:37:32.000000 magnumnp-1.1.6/magnumnp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 08:37:32.015821 magnumnp-1.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2024-04-11 08:37:30.000000 magnumnp-1.1.6/setup.py
```

### Comparing `magnumnp-1.1.5/LICENSE` & `magnumnp-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/PKG-INFO` & `magnumnp-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.5
+Version: 1.1.6
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Requires-Dist: torch
 Requires-Dist: torchdiffeq
 Requires-Dist: xitorch
 Requires-Dist: tqdm
 
 ![magnum.np](logo.png)
 
-magnum.np 1.1.5
+magnum.np 1.1.6
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -34,15 +34,15 @@
 * Fast FFT Oersted-field optimized for small memory footprint
 * Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
 * Non-Equidistant Mesh for Multilayer Structures
 * Arbitrary Material Parameters varying in space and time
 * Spin-torque model by Slonczewski
 * Spin-torque model by Zhang and Li
 * Spin-Orbit torque (SOT)
-* Antiferromagnetic coupling layers (RKKY)
+* Bilinear and biquadratic Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
 * Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
```

### Comparing `magnumnp-1.1.5/README.md` & `magnumnp-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![magnum.np](logo.png)
 
-magnum.np 1.1.5
+magnum.np 1.1.6
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -12,15 +12,15 @@
 * Fast FFT Oersted-field optimized for small memory footprint
 * Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
 * Non-Equidistant Mesh for Multilayer Structures
 * Arbitrary Material Parameters varying in space and time
 * Spin-torque model by Slonczewski
 * Spin-torque model by Zhang and Li
 * Spin-Orbit torque (SOT)
-* Antiferromagnetic coupling layers (RKKY)
+* Bilinear and biquadratic Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
 * Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
```

### Comparing `magnumnp-1.1.5/magnumnp/__init__.py` & `magnumnp-1.1.6/magnumnp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """magnum.np main module"""
 
-__version__ = '1.1.5'
+__version__ = '1.1.6'
 
 import magnumnp.common.logging as logging
 import torch
 torch.set_default_dtype(torch.float64)
 
 # monkey patch torch versions < 2.0 or on Windows
 try:
```

### Comparing `magnumnp-1.1.5/magnumnp/common/__init__.py` & `magnumnp-1.1.6/magnumnp/common/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/constants.py` & `magnumnp-1.1.6/magnumnp/common/constants.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/decorated_tensor.py` & `magnumnp-1.1.6/magnumnp/common/decorated_tensor.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/io.py` & `magnumnp-1.1.6/magnumnp/common/io.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/logging.py` & `magnumnp-1.1.6/magnumnp/common/logging.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/material.py` & `magnumnp-1.1.6/magnumnp/common/material.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/mesh.py` & `magnumnp-1.1.6/magnumnp/common/mesh.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/state.py` & `magnumnp-1.1.6/magnumnp/common/state.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/tabulate.py` & `magnumnp-1.1.6/magnumnp/common/tabulate.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/time_interpolator.py` & `magnumnp-1.1.6/magnumnp/common/time_interpolator.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/common/timer.py` & `magnumnp-1.1.6/magnumnp/common/timer.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/__init__.py` & `magnumnp-1.1.6/magnumnp/field_terms/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/anisotropy.py` & `magnumnp-1.1.6/magnumnp/field_terms/anisotropy.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/demag.py` & `magnumnp-1.1.6/magnumnp/field_terms/demag.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/demagPBC.py` & `magnumnp-1.1.6/magnumnp/field_terms/demagPBC.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/demag_nonequidistant.py` & `magnumnp-1.1.6/magnumnp/field_terms/demag_nonequidistant.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/dmi.py` & `magnumnp-1.1.6/magnumnp/field_terms/dmi.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/exchange.py` & `magnumnp-1.1.6/magnumnp/field_terms/exchange.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/external.py` & `magnumnp-1.1.6/magnumnp/field_terms/external.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/field_terms.py` & `magnumnp-1.1.6/magnumnp/field_terms/field_terms.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/oersted.py` & `magnumnp-1.1.6/magnumnp/field_terms/oersted.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/rkky.py` & `magnumnp-1.1.6/magnumnp/field_terms/rkky.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 from magnumnp.common import timedmethod, constants
 import torch
 
-__all__ = ["RKKYField"]
+__all__ = ["RKKYField", "BiquadraticRKKYField"]
 
 # TODO: interface should be generalized and simplified
 class RKKYField(object):
     r"""
     Interlayer-Exchange interaction between two layers gives rise to the following energy contribution:
 
     .. math::
@@ -93,15 +93,15 @@
             m1 = 15./8. * state.m[:,:,(self._id1,),:] - 5./4. * state.m[:,:,(self._id1-1,),:] + 3./8.* state.m[:,:,(self._id1-2,),:]
             m2 = 15./8. * state.m[:,:,(self._id2,),:] - 5./4. * state.m[:,:,(self._id2+1,),:] + 3./8.* state.m[:,:,(self._id2+2,),:]
 
         h[:,:,(self._id1,),:] = self._J_rkky * (m2 - (m1*m2).sum(axis = 3, keepdim=True) * m1)
         h[:,:,(self._id2,),:] = self._J_rkky * (m1 - (m1*m2).sum(axis = 3, keepdim=True) * m2)
 
         h /= constants.mu_0 * state.material["Ms"] * state.mesh.dx[2]
-        return torch.nan_to_num(h)
+        return h.nan_to_num(posinf=0, neginf=0)
 
     def E(self, state):
         m1 = state.m[:,:,(self._id1,),:]
         m2 = state.m[:,:,(self._id2,),:]
         if self._order == 1:
             m1 += 0.5 * ( state.m[:,:,(self._id1,),:] - state.m[:,:,(self._id1-1,),:])
             m2 += 0.5 * (-state.m[:,:,(self._id2,),:] + state.m[:,:,(self._id2+1,),:])
@@ -110,7 +110,57 @@
             m2 += 0.25 * (3*state.m[:,:,(self._id2,),:] - 4*state.m[:,:,(self._id2+1,),:] + state.m[:,:,(self._id2+2,),:])
 
         E = (m2*m1).sum()
         E *= -state.mesh.dx[0] * state.mesh.dx[1] * self._J_rkky
         return E
 
 
+
+# TODO: interface should be generalized and simplified
+class BiquadraticRKKYField(object):
+    r"""
+    Biquadratic surface exchange couplong between two layers gives rise to the following energy contribution:
+    .. math::
+        E^\text{biquadratic} = -\int\limits_\Gamma J_\text{biquadratic} \, (\vec{m}_i \cdot \vec{m}_j)^2 \, d\vec{A},
+
+
+    where :math:`\Gamma` is the interface between two layers :math:`i` and :math:`j` with magnetizations :math:`\vec{m}_i` and :math:`\vec{m}_j`, respectively.
+
+    The effective field is given by:
+
+    .. math::
+        \vec{h}^\text{biquadratic}_i = \frac{2 J_\text{biquadratic}} {M_s \Delta z \mu_0} \, (\vec{m}_i \cdot \vec{m}_j) \, \vec{m}_j,
+
+    with the interlayer exchange constant :math:`J_\text{biquadratic}`.
+
+    """
+    def __init__(self, J_rkky_BQ, dir, id1, id2):
+        self._J_rkky_BQ = J_rkky_BQ
+        if dir != "z":
+            raise ValueError("Currently only dir='z' is implemented!")
+        self._dir = dir 
+        self._id1 = min(id1,id2)
+        self._id2 = max(id1,id2)
+
+    @timedmethod
+    def h(self, state):
+        h = state.zeros(state.mesh.n + (3,))
+
+        m1 = state.m[:,:,self._id1,:]
+        m2 = state.m[:,:,self._id2,:]
+
+        m12 = (m1*m2).sum(axis=-1, keepdim=True)
+        h[:,:,self._id1,:] = 2. * self._J_rkky_BQ * m12 * m2
+        h[:,:,self._id2,:] = 2. * self._J_rkky_BQ * m12 * m1
+
+        #TODO: find out why there is a 2x discrepancy compared with oommf
+        h /= constants.mu_0 * state.material["Ms"] * state.mesh.dx[2]
+
+        return h.nan_to_num(posinf=0, neginf=0)
+    
+    def E(self, state):
+        m1 = state.m[:,:,self._id1,:]
+        m2 = state.m[:,:,self._id2,:]
+
+        E = ((m1*m2).sum(dim=-1)**2).sum()
+        E *= -state.mesh.dx[0] * state.mesh.dx[1] * self._J_rkky_BQ
+        return E
```

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/rux.py` & `magnumnp-1.1.6/magnumnp/field_terms/rux.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/spintorque.py` & `magnumnp-1.1.6/magnumnp/field_terms/spintorque.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/field_terms/thermal.py` & `magnumnp-1.1.6/magnumnp/field_terms/thermal.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/loggers/__init__.py` & `magnumnp-1.1.6/magnumnp/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/loggers/field_logger.py` & `magnumnp-1.1.6/magnumnp/loggers/field_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/loggers/logger.py` & `magnumnp-1.1.6/magnumnp/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/loggers/scalar_logger.py` & `magnumnp-1.1.6/magnumnp/loggers/scalar_logger.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/LBFGS.py` & `magnumnp-1.1.6/magnumnp/solvers/LBFGS.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/__init__.py` & `magnumnp-1.1.6/magnumnp/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/eigensolver.py` & `magnumnp-1.1.6/magnumnp/solvers/eigensolver.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/llg.py` & `magnumnp-1.1.6/magnumnp/solvers/llg.py`

 * *Files 16% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 
     @timedmethod
     def step(self, state, dt, **kwargs):
         self._solver.step(state, dt, **kwargs)
         logging.info_blue("[LLG] step: dt= %g  t=%g" % (dt, state.t))
 
     @timedmethod
+    def solve(self, state, tt, **kwargs):
+        logging.info_blue("[LLG] solve: t0=%g  t1=%g Integrating ..." % (tt[0].cpu().numpy(), tt[-1].cpu().numpy()))
+        res = self._solver.solve(state, tt, **kwargs)
+        logging.info_green("[LLG] solve: t0=%g  t1=%g Finished" % (tt[0].cpu().numpy(), tt[-1].cpu().numpy()))
+        return res
+
+    @timedmethod
     def relax(self, state, maxiter = 500, rtol = 1e-6, dt = 1e-11):
         t0 = state.t
         E0 = self.E(state)
 
         for i in range(maxiter):
             self._solver.step(state, dt, alpha = 1.0) #, no_precession = True) # no_precession requires more iterations for SP4 demo!?
```

### Comparing `magnumnp-1.1.5/magnumnp/solvers/minimize.py` & `magnumnp-1.1.6/magnumnp/solvers/minimize.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/__init__.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/heun.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/heun.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/rkf45.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/rkf45.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/rkf56.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/rkf56.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/scipy_ode.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/scipy_ode.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/scipy_odeint.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/scipy_odeint.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,7 +50,21 @@
                     args = (state, llg_args),
                     rtol = rtol or self._rtol,
                     atol = atol or self._atol,
                     tfirst = True)[1]
 
         state.m = state.Tensor(m1.reshape(state.mesh.n + (3,), order = "F"))
         state.t = t1
+
+    def solve(self, state, tt, rtol = None, atol = None, **llg_args):
+        m0 = state.m.detach().cpu().numpy().reshape(-1, order = 'F')
+        res = odeint(self._f_wrapper,
+                     m0,
+                     tt.detach().cpu().numpy()*1e9,
+                     args = (state, llg_args),
+                     rtol = rtol or self._rtol,
+                     atol = atol or self._atol,
+                     tfirst = True)
+
+        state.m = state.Tensor(res[-1].reshape(state.mesh.n + (3,), order = "F"))
+        state.t = tt[-1]
+        return res
```

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ode_solvers/torchdiffeq.py` & `magnumnp-1.1.6/magnumnp/solvers/ode_solvers/torchdiffeq.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,14 +44,28 @@
                      method = self._method,
                      rtol = rtol or self._rtol,
                      atol = atol or self._atol,
                      options = self._options) # TODO: reuse solver object?
         state.m = state.Tensor(res[1])
         state.t = t1
 
+    def solve(self, state, tt, rtol = None, atol = None, **llg_args):
+        res = odeint(lambda t, m: self._f_wrapper(t, m, state, **llg_args),
+                     state.m,
+                     tt*1e9,
+                     method = self._method,
+                     rtol = rtol or self._rtol,
+                     atol = atol or self._atol,
+                     options = self._options) # TODO: reuse solver object?
+        state.m = state.Tensor(res[-1])
+        state.t = tt[-1]
+        return res
+
+
+
 class TorchDiffEqAdjoint(object):
     def __init__(self, f, adjoint_parameters, method = "dopri5", rtol = 1e-5, atol = 1e-5, options = {}):
         self._f = f
         self._adjoint_parameters = adjoint_parameters
         self._method = method
         self._rtol = rtol
         self._atol = atol
@@ -71,7 +85,20 @@
                      method = self._method,
                      rtol = rtol or self._rtol,
                      atol = atol or self._atol,
                      adjoint_params = self._adjoint_parameters,
                      options = self._options) # TODO: reuse solver object?
         state.m = state.Tensor(res[1])
         state.t = t1
+
+    def solve(self, state, tt, rtol = None, atol = None, **llg_args):
+        res = odeint_adjoint(lambda t, m: self._f_wrapper(t, m, state, **llg_args),
+                     state.m,
+                     tt*1e9,
+                     method = self._method,
+                     rtol = rtol or self._rtol,
+                     atol = atol or self._atol,
+                     adjoint_params = self._adjoint_parameters,
+                     options = self._options) # TODO: reuse solver object?
+        state.m = state.Tensor(res[-1])
+        state.t = tt[-1]
+        return res
```

### Comparing `magnumnp-1.1.5/magnumnp/solvers/ohm_solver.py` & `magnumnp-1.1.6/magnumnp/solvers/ohm_solver.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/steepest_descent.py` & `magnumnp-1.1.6/magnumnp/solvers/steepest_descent.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/solvers/string.py` & `magnumnp-1.1.6/magnumnp/solvers/string.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/utils/__init__.py` & `magnumnp-1.1.6/magnumnp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/utils/imaging_tools.py` & `magnumnp-1.1.6/magnumnp/utils/imaging_tools.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp/utils/misc.py` & `magnumnp-1.1.6/magnumnp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/magnumnp.egg-info/PKG-INFO` & `magnumnp-1.1.6/magnumnp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnumnp
-Version: 1.1.5
+Version: 1.1.6
 Summary: magnum.np finite-difference package for the solution of micromagnetic problems
 Home-page: http://gitlab.com/magnum.np/magnum.np
 Author: Florian Bruckner
 Author-email: florian.bruckner@univie.ac.at
 Project-URL: Documentation, https://magnum.np.gitlab.io/magnum.np/
 Project-URL: Changelog, https://gitlab.com/magnum.np/magnum.np/blob/main/CHANGELOG
 Description-Content-Type: text/markdown
@@ -18,15 +18,15 @@
 Requires-Dist: torch
 Requires-Dist: torchdiffeq
 Requires-Dist: xitorch
 Requires-Dist: tqdm
 
 ![magnum.np](logo.png)
 
-magnum.np 1.1.5
+magnum.np 1.1.6
 ===============
 magnum.np is a Python library for the solution of micromagnetic problems with the finite-difference method. It implements state-of-the-art algorithms and is based on [pytorch](http://www.pytorch.org/), which allows to seamlessly run code either on GPU or on CPU. Simulation scripts are written in Python which leads to very readable yet flexible code. Due to [pytorch](http://www.pytorch.org/) integration, extensive postprocessing can be done directly in the simulations scripts. Furthermore [pytorch](http://www.paraview.org/)'s autograd feature makes it possible to solve inverse problems without significant modifications of the code. This manual is meant to give you both a quick start and a reference to magnum.np.
 
 
 Features
 --------
 * Explicit / Implicit time-integration of the Landau-Lifshitz-Gilbert Equation
@@ -34,15 +34,15 @@
 * Fast FFT Oersted-field optimized for small memory footprint
 * Periodic Boundary Conditions in 1D, 2D, and 3D (True and Pseudo-Periodic)
 * Non-Equidistant Mesh for Multilayer Structures
 * Arbitrary Material Parameters varying in space and time
 * Spin-torque model by Slonczewski
 * Spin-torque model by Zhang and Li
 * Spin-Orbit torque (SOT)
-* Antiferromagnetic coupling layers (RKKY)
+* Bilinear and biquadratic Antiferromagnetic coupling layers (RKKY)
 * Dzyaloshinskii-Moriya interaction (interface, bulk, D2d)
 * String method for energy barrier computations
 * Sophisticated domain handling, e.g. for spatially varying material parameters
 * Seamless VTK import / export via [pyvista](https://docs.pyvista.org/)
 * Inverse Problems via [pytorch](http://www.pytorch.org/)'s autograd feature
```

### Comparing `magnumnp-1.1.5/magnumnp.egg-info/SOURCES.txt` & `magnumnp-1.1.6/magnumnp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnumnp-1.1.5/setup.py` & `magnumnp-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='magnumnp',
-      version='v1.1.5',
+      version='v1.1.6',
       description='magnum.np finite-difference package for the solution of micromagnetic problems',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Florian Bruckner',
       author_email='florian.bruckner@univie.ac.at',
       url='http://gitlab.com/magnum.np/magnum.np',
       project_urls = {'Documentation': 'https://magnum.np.gitlab.io/magnum.np/',
```

