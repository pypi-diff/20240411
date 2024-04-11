# Comparing `tmp/psyke-0.8.2.dev1.tar.gz` & `tmp/psyke-0.8.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.2.dev1.tar", last modified: Tue Apr  9 23:25:49 2024, max compression
+gzip compressed data, was "psyke-0.8.2.dev3.tar", last modified: Wed Apr 10 21:24:15 2024, max compression
```

## Comparing `psyke-0.8.2.dev1.tar` & `psyke-0.8.2.dev3.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-09 23:25:47.000000 psyke-0.8.2.dev1/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.095816 psyke-0.8.2.dev1/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    11056 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21894 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.099816 psyke-0.8.2.dev1/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:25:48.000000 psyke-0.8.2.dev1/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 23:25:49.000000 psyke-0.8.2.dev1/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.091817 psyke-0.8.2.dev1/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.103817 psyke-0.8.2.dev1/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-09 23:24:38.000000 psyke-0.8.2.dev1/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 23:24:40.000000 psyke-0.8.2.dev1/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-09 23:24:40.000000 psyke-0.8.2.dev1/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-09 23:24:40.000000 psyke-0.8.2.dev1/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:25:49.107817 psyke-0.8.2.dev1/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-09 23:24:40.000000 psyke-0.8.2.dev1/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.298854 psyke-0.8.2.dev3/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-10 21:24:13.000000 psyke-0.8.2.dev3/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.302854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 21:24:15.000000 psyke-0.8.2.dev3/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.298854 psyke-0.8.2.dev3/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.306854 psyke-0.8.2.dev3/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.310855 psyke-0.8.2.dev3/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 21:23:08.000000 psyke-0.8.2.dev3/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 21:23:10.000000 psyke-0.8.2.dev3/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-10 21:23:10.000000 psyke-0.8.2.dev3/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-10 21:23:10.000000 psyke-0.8.2.dev3/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:24:15.314854 psyke-0.8.2.dev3/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-10 21:23:10.000000 psyke-0.8.2.dev3/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.2.dev1/LICENSE` & `psyke-0.8.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/PKG-INFO` & `psyke-0.8.2.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.2.dev1
+Version: 0.8.2.dev3
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.2.dev1/README.md` & `psyke-0.8.2.dev3/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/__init__.py` & `psyke-0.8.2.dev3/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/clustering/__init__.py` & `psyke-0.8.2.dev3/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/clustering/cream/__init__.py` & `psyke-0.8.2.dev3/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/clustering/exact/__init__.py` & `psyke-0.8.2.dev3/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/clustering/utils.py` & `psyke-0.8.2.dev3/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/cart/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/cart/predictor.py` & `psyke-0.8.2.dev3/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,47 +36,37 @@
         return ClassificationCube()
 
     def _sort_cubes(self):
         cubes = [(cube.diversity, i, cube) for i, cube in enumerate(self._hypercubes)]
         cubes.sort()
         self._hypercubes = [cube[2] for cube in cubes]
 
-    def _last_cube_as_default(self, theory):
-        last_clause = list(theory.clauses)[-1]
-        theory.retract(last_clause)
-        theory.assertZ(clause(
-            last_clause.head, [last_in_body(last_clause.body)] if self._output is Target.REGRESSION else []))
-        last_cube = self._hypercubes[-1]
-        for dimension in last_cube.dimensions.keys():
-            last_cube[dimension] = [-np.inf, np.inf]
-        return theory
-
     def extract(self, dataframe: pd.DataFrame) -> Theory:
         theory = PedagogicalExtractor.extract(self, dataframe)
         self._surrounding = HyperCube.create_surrounding_cube(dataframe, output=self._output)
         self._surrounding.update(dataframe, self.predictor)
         return theory
 
     def predict_counter(self, data: dict[str, float]):
-        cube = self._find_cube(data)
+        cube = self._find_cube(data.copy())
         if cube is None:
             print("The extracted knowledge is not exhaustive; impossible to predict this instance")
         else:
             print("The output is", self._predict_from_cubes(data))
 
         point = Point(list(data.keys()), list(data.values()))
         cubes = self._hypercubes if cube is None else [c for c in self._hypercubes if cube.output != c.output]
         cubes = sorted([(cube.surface_distance(point), cube.volume(), cube) for cube in cubes])
         outputs = []
         for _, _, c in cubes:
             if c.output not in outputs:
                 outputs.append(c.output)
                 print("The output may be", c.output, 'if')
 
-                for d in c.dimensions.keys():
+                for d in point.dimensions.keys():
                     lower, upper = c[d]
                     p = point[d]
                     if p < lower:
                         print('    ', d, '=', round(lower, 1))
                     elif p > upper:
                         print('    ', d, '=', round(upper, 1))
 
@@ -87,22 +77,22 @@
         subcubes = cube.subcubes(self._hypercubes)
         for c in [c for c in subcubes if sum(c in sc and c != sc for sc in subcubes) == 0]:
             for d in c.finite_dimensions:
                 conditions[d].append(Outside(*c.dimensions[d]))
         return conditions
 
     def predict_why(self, data: dict[str, float]):
-        cube = self._find_cube(data)
+        cube = self._find_cube(data.copy())
         if cube is None:
             print("The extracted knowledge is not exhaustive; impossible to predict this instance")
         else:
             output = self._predict_from_cubes(data)
             print(f"The output is {output} because")
             conditions = self.__get_local_conditions(cube)
-            for d in conditions:
+            for d in data.keys():
                 simplified = HyperCubeExtractor.__simplify(conditions[d])
                 for i, condition in enumerate(simplified):
                     if i == 0:
                         print('    ', d, 'is', end=' ')
                     else:
                         print('and', end=' ')
                     if isinstance(condition, Outside):
@@ -145,34 +135,33 @@
 
     @staticmethod
     def _create_head(dataframe: pd.DataFrame, variables: list[Var], output: float | LinearRegression) -> Struct:
         return create_head(dataframe.columns[-1], variables[:-1], output) \
             if not isinstance(output, LinearRegression) else \
             create_head(dataframe.columns[-1], variables[:-1], variables[-1])
 
-    def _ignore_dimensions(self, cube: HyperCube) -> Iterable[str]:
-        return [d for d in cube.dimensions if cube[d][0] == -np.inf or cube[d][1] == np.inf]
-
     def __drop(self, dataframe: pd.DataFrame):
         self._hypercubes = [cube for cube in self._hypercubes if cube.count(dataframe) > 1]
 
     def _create_theory(self, dataframe: pd.DataFrame) -> Theory:
         self.__drop(dataframe)
+        if self._default_surrounding_cube:
+            self._hypercubes[-1].set_default()
+
         new_theory = mutable_theory()
         for cube in self._hypercubes:
             logger.info(cube.output)
             logger.info(cube.dimensions)
             variables = create_variable_list([], dataframe)
             variables[dataframe.columns[-1]] = to_var(dataframe.columns[-1])
             head = HyperCubeExtractor._create_head(dataframe, list(variables.values()),
                                                    self.unscale(cube.output, dataframe.columns[-1]))
-            body = cube.body(variables, self._ignore_dimensions(cube), self.unscale, self.normalization)
+            body = cube.body(variables, self._dimensions_to_ignore, self.unscale, self.normalization)
             new_theory.assertZ(clause(head, body))
-        new_theory = HyperCubeExtractor._prettify_theory(new_theory)
-        return self._last_cube_as_default(new_theory) if self._default_surrounding_cube else new_theory
+        return HyperCubeExtractor._prettify_theory(new_theory)
 
     @staticmethod
     def _prettify_theory(theory: Theory) -> Theory:
         visitor = Simplifier()
         new_clauses = []
         for c in theory.clauses:
             body = c.body
```

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,22 +20,17 @@
                  output: Target = Target.CONSTANT, gauss_components: int = 5, ranks: list[(str, float)] = [],
                  ignore_threshold: float = 0.0, discretization=None, normalization=None,
                  seed: int = get_default_random_seed()):
         super().__init__(predictor, Target.CLASSIFICATION if isinstance(predictor, ClassifierMixin) else output,
                          discretization, normalization)
         self.clustering = clustering(depth, error_threshold, self._output, gauss_components, discretization,
                                      normalization, seed)
-        self.ranks = ranks
-        self.ignore_threshold = ignore_threshold
         self._default_surrounding_cube = True
+        self._dimensions_to_ignore = [dimension for dimension, relevance in ranks if relevance < ignore_threshold]
 
     def _extract(self, dataframe: pd.DataFrame) -> Theory:
         if not isinstance(self.clustering, HyperCubeClustering):
             raise TypeError("clustering must be a HyperCubeClustering")
 
         self.clustering.fit(dataframe)
         self._hypercubes = self.clustering.get_hypercubes()
-        for cube in self._hypercubes:
-            for dimension, relevance in self.ranks:
-                if relevance < self.ignore_threshold:
-                    cube[dimension] = [-np.inf, np.inf]
         return self._create_theory(dataframe)
```

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         return self._create_theory(dataframe)
 
     def _create_ranges(self, cube, iteration):
         ranges = {}
         for (feature, (a, b)) in cube.dimensions.items():
             n_bins = self.grid.get(feature, iteration)
             if n_bins == 1:
-                ranges[feature] = [(-np.inf, np.inf)]
+                ranges[feature] = [(a, b)]
+                self._dimensions_to_ignore.append(feature)
             else:
                 size = (b - a) / n_bins
                 ranges[feature] = [(a + size * i, a + size * (i + 1)) for i in range(n_bins)]
         return ranges
 
     def _cubes_to_split(self, cube, surrounding, iteration, dataframe, fake, keep_empty=False):
         to_split = []
```

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/hypercube.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
                  output: float | LinearRegression | str = 0.0):
         self._dimensions = self._fit_dimension(dimension) if dimension is not None else {}
         self._limits = limits if limits is not None else set()
         self._output = output
         self._diversity = 0.0
         self._error = 0.0
         self._barycenter = Point([], [])
+        self._default = False
 
     def __contains__(self, obj: dict[str, float] | HyperCube) -> bool:
         """
         Note that a point is inside a hypercube if ALL its dimensions' values satisfy:
             min_dim <= object dimension < max_dim
         :param obj: an N-dimensional object (point or hypercube)
         :return: true if the object is inside the hypercube, false otherwise
@@ -113,14 +114,21 @@
         self._dimensions[key] = value
 
     def __hash__(self) -> int:
         result = [hash(name + str(dimension[0]) + str(dimension[1])) for name, dimension in self.dimensions.items()]
         return sum(result)
 
     @property
+    def is_default(self) -> bool:
+        return self._default
+
+    def set_default(self):
+        self._default = True
+
+    @property
     def dimensions(self) -> Dimensions:
         return self._dimensions
 
     @property
     def finite_dimensions(self) -> Dimensions:
         return {k: v for k, v in self._dimensions.items() if np.isfinite(v[0]) and np.isfinite(v[1])}
 
@@ -208,20 +216,16 @@
         return HyperCube(self.dimensions.copy(), self._limits.copy(), self.output)
 
     def count(self, dataset: pd.DataFrame) -> int:
         return self.filter_dataframe(dataset.iloc[:, :-1]).shape[0]
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
         dimensions = dict(self.dimensions)
-        # TODO: there is something strange in the tests here
-        # print('search', [name for name in dimensions.keys()], 'in', (variables.keys()))
-        for dimension in ignore:
-            del dimensions[dimension]
         return [create_term(variables[name], Between(unscale(values[0], name), unscale(values[1], name)))
-                for name, values in dimensions.items()]
+                for name, values in dimensions.items() if name not in ignore and not self.is_default]
 
     @staticmethod
     def create_surrounding_cube(dataset: pd.DataFrame, closed: bool = False,
                                 output=None) -> GenericCube:
         output = Target.CONSTANT if output is None else output
         dimensions = {
             column: (min(dataset[column]) - HyperCube.EPSILON * 2, max(dataset[column]) + HyperCube.EPSILON * 2)
@@ -278,18 +282,20 @@
     def get_first(self, feature: str) -> float:
         return self[feature][0]
 
     def get_second(self, feature: str) -> float:
         return self[feature][1]
 
     def has_volume(self) -> bool:
-        return all([dimension[1] - dimension[0] > HyperCube.EPSILON for dimension in self._dimensions.values()])
+        return all([dimension[1] - dimension[0] > HyperCube.EPSILON for dimension in self._dimensions.values()
+                    if np.isfinite(dimension[0]) and np.isfinite(dimension[1])])
 
     def volume(self) -> float:
-        return reduce(lambda a, b: a * b, [dimension[1] - dimension[0] for dimension in self._dimensions.values()], 1)
+        return reduce(lambda a, b: a * b, [dimension[1] - dimension[0] for dimension in self._dimensions.values()
+                                           if np.isfinite(dimension[0]) and np.isfinite(dimension[1])], 1)
 
     def diagonal(self) -> float:
         return reduce(
             lambda a, b: a + b, [(dimension[1] - dimension[0]) ** 2 for dimension in self._dimensions.values()], 0
         ) ** 0.5
 
     @property
@@ -300,15 +306,15 @@
     def corners(self) -> Iterable[Point]:
         return [
             Point(list(self._dimensions.keys()), values) for values in itertools.product(*self._dimensions.values())
         ]
 
     def surface_distance(self, point: Point) -> float:
         s = 0
-        for d in self.dimensions.keys():
+        for d in point.dimensions.keys():
             lower, upper = self[d]
             p = point[d]
             if p > upper:
                 s += (p - upper)**2
             elif p < lower:
                 s += (lower - p)**2
         return s**0.5
@@ -405,28 +411,28 @@
 
     # TODO: why this is not a property?
     def init_diversity(self, std: float) -> None:
         self._diversity = std
 
 
 class RegressionCube(HyperCube):
-    def __init__(self, dimension: dict[str, tuple] = None):
-        super().__init__(dimension=dimension, output=LinearRegression())
+    def __init__(self, dimension: dict[str, tuple] = None, output=LinearRegression()):
+        super().__init__(dimension=dimension, output=output)
 
     def update(self, dataset: pd.DataFrame, predictor) -> None:
         filtered = self.filter_dataframe(dataset.iloc[:, :-1])
         if len(filtered > 0):
             predictions = predictor.predict(filtered)
             self._output.fit(filtered, predictions)
             self._diversity = self._error = (abs(self._output.predict(filtered) - predictions)).mean()
             means = filtered.describe().loc['mean']
             self._barycenter = Point(means.index.values, means.values)
 
     def copy(self) -> RegressionCube:
-        return RegressionCube(self.dimensions.copy())
+        return RegressionCube(self.dimensions.copy(), output=self._output)
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
         intercept = self.output.intercept_ if normalization is None else unscale(sum(
             [-self.output.coef_[i] * normalization[name][0] / normalization[name][1] for i, name in
              enumerate(self.dimensions.keys())], self.output.intercept_), list(normalization.keys())[-1])
         coefs = self.output.coef_ if normalization is None else [
             self.output.coef_[i] / normalization[name][1] * normalization[list(normalization.keys())[-1]][1] for
@@ -451,16 +457,16 @@
             self._barycenter = Point(means.index.values, means.values)
 
     def copy(self) -> ClassificationCube:
         return ClassificationCube(self.dimensions.copy(), self._limits.copy(), self._output)
 
 
 class ClosedCube(HyperCube):
-    def __init__(self, dimension: dict[str, tuple] = None):
-        super().__init__(dimension=dimension)
+    def __init__(self, dimension: dict[str, tuple] = None, output: str | LinearRegression | float = 0.0):
+        super().__init__(dimension=dimension, output=output)
 
     def __contains__(self, obj: dict[str, float] | ClosedCube) -> bool:
         """
        Note that an object is inside a hypercube if ALL its dimensions' values satisfy:
            min_dim <= object dimension <= max_dim
        :param obj: an N-dimensional object (point or hypercube)
        :return: true if the object is inside the hypercube, false otherwise
@@ -475,28 +481,28 @@
 
     def filter_indices(self, dataset: pd.DataFrame) -> ndarray:
         v = np.array([v for _, v in self._dimensions.items()])
         ds = dataset.to_numpy(copy=True)
         return np.all((v[:, 0] <= ds) & (ds <= v[:, 1]), axis=1)
 
     def copy(self) -> ClosedCube:
-        return ClosedCube(self.dimensions.copy())
+        return ClosedCube(self.dimensions.copy(), output=self._output)
 
 
 class ClosedRegressionCube(ClosedCube, RegressionCube):
-    def __init__(self, dimension: dict[str, tuple] = None):
-        super().__init__(dimension=dimension)
+    def __init__(self, dimension: dict[str, tuple] = None, output: LinearRegression = LinearRegression()):
+        super().__init__(dimension=dimension, output=output)
 
     def copy(self) -> ClosedRegressionCube:
-        return ClosedRegressionCube(self.dimensions.copy())
+        return ClosedRegressionCube(self.dimensions.copy(), output=self._output)
 
 
 class ClosedClassificationCube(ClosedCube, ClassificationCube):
-    def __init__(self, dimension: dict[str, tuple] = None):
-        super().__init__(dimension=dimension)
+    def __init__(self, dimension: dict[str, tuple] = None, output: str = None):
+        super().__init__(dimension=dimension, output=output)
 
     def copy(self) -> ClosedClassificationCube:
-        return ClosedClassificationCube(self.dimensions.copy())
+        return ClosedClassificationCube(self.dimensions.copy(), output=self._output)
 
 
 GenericCube = Union[HyperCube, ClassificationCube, RegressionCube,
                     ClosedCube, ClosedRegressionCube, ClosedClassificationCube]
```

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.2.dev3/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/real/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/real/utils.py` & `psyke-0.8.2.dev3/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/trepan/__init__.py` & `psyke-0.8.2.dev3/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/extraction/trepan/utils.py` & `psyke-0.8.2.dev3/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/hypercubepredictor.py` & `psyke-0.8.2.dev3/psyke/hypercubepredictor.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from psyke.extraction.hypercubic import RegressionCube, GenericCube, Point
 
 
 class HyperCubePredictor(EvaluableModel):
     def __init__(self, output=Target.CONSTANT, discretization=None, normalization=None):
         super().__init__(discretization, normalization)
         self._hypercubes = []
+        self._dimensions_to_ignore = []
         self._output = output
         self._surrounding = None
 
     def _predict(self, dataframe: pd.DataFrame) -> Iterable:
         return np.array([self._predict_from_cubes(row.to_dict()) for _, row in dataframe.iterrows()])
 
     def _brute_predict(self, dataframe: pd.DataFrame, criterion: str = 'corner', n: int = 2) -> Iterable:
@@ -71,18 +72,24 @@
             return None
         elif self._output == Target.CLASSIFICATION:
             return HyperCubePredictor._get_cube_output(cube, data)
         else:
             return round(HyperCubePredictor._get_cube_output(cube, data), get_int_precision())
 
     def _find_cube(self, data: dict[str, float]) -> GenericCube | None:
+        for dimension in self._dimensions_to_ignore:
+            del data[dimension]
+        found = None
         for cube in self._hypercubes:
             if data in cube:
-                return cube
-        return None
+                found = cube.copy()
+                break
+        if found is None and self._hypercubes[-1].is_default:
+            found = self._hypercubes[-1].copy()
+        return found
 
     @property
     def n_rules(self):
         return len(list(self._hypercubes))
 
     @property
     def volume(self):
```

### Comparing `psyke-0.8.2.dev1/psyke/schema/__init__.py` & `psyke-0.8.2.dev3/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/tuning/__init__.py` & `psyke-0.8.2.dev3/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/tuning/crash/__init__.py` & `psyke-0.8.2.dev3/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/tuning/orchid/__init__.py` & `psyke-0.8.2.dev3/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/tuning/pedro/__init__.py` & `psyke-0.8.2.dev3/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/__init__.py` & `psyke-0.8.2.dev3/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/dataframe.py` & `psyke-0.8.2.dev3/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/logic.py` & `psyke-0.8.2.dev3/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/metrics.py` & `psyke-0.8.2.dev3/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/plot.py` & `psyke-0.8.2.dev3/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke/utils/sorted.py` & `psyke-0.8.2.dev3/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/psyke.egg-info/PKG-INFO` & `psyke-0.8.2.dev3/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.2.dev1
+Version: 0.8.2.dev3
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.2.dev1/psyke.egg-info/SOURCES.txt` & `psyke-0.8.2.dev3/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/setup.py` & `psyke-0.8.2.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/__init__.py` & `psyke-0.8.2.dev3/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.2.dev3/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.2.dev3/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.2.dev3/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/real/test_real.py` & `psyke-0.8.2.dev3/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.2.dev3/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.2.dev3/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/utils/test_prune.py` & `psyke-0.8.2.dev3/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/utils/test_simplify.py` & `psyke-0.8.2.dev3/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.2.dev3/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev1/test/resources/tests/__init__.py` & `psyke-0.8.2.dev3/test/resources/tests/__init__.py`

 * *Files identical despite different names*

