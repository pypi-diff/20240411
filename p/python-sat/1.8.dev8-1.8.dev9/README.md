# Comparing `tmp/python-sat-1.8.dev8.tar.gz` & `tmp/python-sat-1.8.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sat-1.8.dev8.tar", last modified: Sat Apr  6 03:31:03 2024, max compression
+gzip compressed data, was "python-sat-1.8.dev9.tar", last modified: Sun Apr  7 06:20:31 2024, max compression
```

## Comparing `python-sat-1.8.dev8.tar` & `python-sat-1.8.dev9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.863770 python-sat-1.8.dev8/
--rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/LICENSE.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/MANIFEST.in
--rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-06 03:31:03.863645 python-sat-1.8.dev8/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567    14570 2024-03-16 05:05:09.000000 python-sat-1.8.dev8/README.rst
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.834119 python-sat-1.8.dev8/allies/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-1.8.dev8/allies/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    13551 2023-11-24 02:09:08.000000 python-sat-1.8.dev8/allies/approxmc.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    16698 2023-11-24 05:11:48.000000 python-sat-1.8.dev8/allies/unigen.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.836878 python-sat-1.8.dev8/cardenc/
--rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/bitwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-1.8.dev8/cardenc/card.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/clset.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/common.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/itot.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/ladder.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/mto.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/pairwise.hh
--rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/ptypes.hh
--rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/pycard.cc
--rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/seqcounter.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/sortcard.hh
--rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/cardenc/utils.hh
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.839308 python-sat-1.8.dev8/examples/
--rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/examples/__init__.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18174 2024-04-05 11:52:59.000000 python-sat-1.8.dev8/examples/fm.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2024-02-23 12:49:50.000000 python-sat-1.8.dev8/examples/genhard.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25762 2024-04-05 10:59:25.000000 python-sat-1.8.dev8/examples/hitman.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    21484 2024-04-05 11:52:23.000000 python-sat-1.8.dev8/examples/lbx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    16112 2024-04-05 12:04:10.000000 python-sat-1.8.dev8/examples/lsu.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    20509 2024-04-05 11:53:17.000000 python-sat-1.8.dev8/examples/mcsls.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     5741 2024-04-05 12:12:36.000000 python-sat-1.8.dev8/examples/models.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    10747 2024-04-05 11:53:33.000000 python-sat-1.8.dev8/examples/musx.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    25841 2024-04-05 11:50:00.000000 python-sat-1.8.dev8/examples/optux.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567    67511 2024-04-05 12:47:02.000000 python-sat-1.8.dev8/examples/rc2.py
--rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/examples/usage.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.841280 python-sat-1.8.dev8/pysat/
--rw-r--r--   0 aign0002 (892519254) 907548567      669 2024-04-05 12:47:38.000000 python-sat-1.8.dev8/pysat/__init__.py
--rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/_fileio.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/_utils.py
--rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/pysat/card.py
--rw-r--r--   0 aign0002 (892519254) 907548567    45094 2024-03-18 05:43:24.000000 python-sat-1.8.dev8/pysat/engines.py
--rw-r--r--   0 aign0002 (892519254) 907548567   192658 2024-03-31 04:44:45.000000 python-sat-1.8.dev8/pysat/formula.py
--rw-r--r--   0 aign0002 (892519254) 907548567    16649 2024-03-16 04:25:34.000000 python-sat-1.8.dev8/pysat/pb.py
--rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-1.8.dev8/pysat/process.py
--rw-r--r--   0 aign0002 (892519254) 907548567   226003 2024-03-18 05:36:00.000000 python-sat-1.8.dev8/pysat/solvers.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.862892 python-sat-1.8.dev8/python_sat.egg-info/
--rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/PKG-INFO
--rw-r--r--   0 aign0002 (892519254) 907548567     2090 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/SOURCES.txt
--rw-r--r--   0 aign0002 (892519254) 907548567        1 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/dependency_links.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      148 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/requires.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       23 2024-04-06 03:31:03.000000 python-sat-1.8.dev8/python_sat.egg-info/top_level.txt
--rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/requirements.txt
--rw-r--r--   0 aign0002 (892519254) 907548567      108 2024-04-06 03:31:03.864042 python-sat-1.8.dev8/setup.cfg
--rw-r--r--   0 aign0002 (892519254) 907548567     6664 2024-03-27 04:48:33.000000 python-sat-1.8.dev8/setup.py
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.853219 python-sat-1.8.dev8/solvers/
--rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-1.8.dev8/solvers/cadical103.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-1.8.dev8/solvers/cadical153.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   644206 2023-08-25 01:25:36.000000 python-sat-1.8.dev8/solvers/cadical170.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   691268 2024-03-16 04:33:34.000000 python-sat-1.8.dev8/solvers/cadical195.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/glucose30.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/glucose41.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-1.8.dev8/solvers/glucose421.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/lingeling.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplechrono.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplecm.zip
--rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/maplesat.zip
--rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/mergesat3.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minicard.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minisat22.tar.gz
--rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/minisatgh.zip
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.857486 python-sat-1.8.dev8/solvers/patches/
--rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-1.8.dev8/solvers/patches/cadical103.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    69395 2024-03-17 07:15:43.000000 python-sat-1.8.dev8/solvers/patches/cadical153.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    92210 2024-03-17 07:14:50.000000 python-sat-1.8.dev8/solvers/patches/cadical195.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/glucose30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/glucose41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    68942 2023-07-15 01:30:10.000000 python-sat-1.8.dev8/solvers/patches/glucose421.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/gluecard30.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/gluecard41.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/lingeling.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-1.8.dev8/solvers/patches/maplechrono.patch
--rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-1.8.dev8/solvers/patches/maplecm.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/maplesat.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-1.8.dev8/solvers/patches/mergesat3.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minicard.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minisat22.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/solvers/patches/minisatgh.patch
--rw-r--r--   0 aign0002 (892519254) 907548567    32315 2024-03-17 07:15:51.000000 python-sat-1.8.dev8/solvers/prepare.py
--rw-r--r--   0 aign0002 (892519254) 907548567   285751 2024-03-16 04:32:47.000000 python-sat-1.8.dev8/solvers/pysolvers.cc
-drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-06 03:31:03.862435 python-sat-1.8.dev8/tests/
--rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-1.8.dev8/tests/test_accum_stats.py
--rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmost.py
--rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmost1.py
--rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_atmostk.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1299 2024-03-17 06:23:23.000000 python-sat-1.8.dev8/tests/test_boolengine.py
--rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-1.8.dev8/tests/test_cnfplus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_equals1.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-1.8.dev8/tests/test_process.py
--rw-r--r--   0 aign0002 (892519254) 907548567     1260 2024-03-17 06:23:42.000000 python-sat-1.8.dev8/tests/test_propagate.py
--rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-1.8.dev8/tests/test_unique_model.py
--rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-1.8.dev8/tests/test_unique_mus.py
--rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-1.8.dev8/tests/test_warmstart.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.781447 python-sat-1.8.dev9/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1109 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/LICENSE.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      217 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/MANIFEST.in
+-rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-07 06:20:31.781339 python-sat-1.8.dev9/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567    14570 2024-03-16 05:05:09.000000 python-sat-1.8.dev9/README.rst
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.726046 python-sat-1.8.dev9/allies/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-04-14 00:41:27.000000 python-sat-1.8.dev9/allies/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    13551 2023-11-24 02:09:08.000000 python-sat-1.8.dev9/allies/approxmc.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    16698 2023-11-24 05:11:48.000000 python-sat-1.8.dev9/allies/unigen.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.729801 python-sat-1.8.dev9/cardenc/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1375 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/bitwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2468 2023-03-02 05:23:11.000000 python-sat-1.8.dev9/cardenc/card.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1874 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/clset.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1303 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/common.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     4646 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/itot.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     2325 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/ladder.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    11355 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/mto.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     1008 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/pairwise.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567      918 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/ptypes.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567    15865 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/pycard.cc
+-rw-r--r--   0 aign0002 (892519254) 907548567     4851 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/seqcounter.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     8355 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/sortcard.hh
+-rw-r--r--   0 aign0002 (892519254) 907548567     5117 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/cardenc/utils.hh
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.735776 python-sat-1.8.dev9/examples/
+-rw-------   0 aign0002 (892519254) 907548567        0 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/examples/__init__.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18174 2024-04-05 11:52:59.000000 python-sat-1.8.dev9/examples/fm.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    18986 2024-02-23 12:49:50.000000 python-sat-1.8.dev9/examples/genhard.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25762 2024-04-05 10:59:25.000000 python-sat-1.8.dev9/examples/hitman.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    21484 2024-04-05 11:52:23.000000 python-sat-1.8.dev9/examples/lbx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    16112 2024-04-05 12:04:10.000000 python-sat-1.8.dev9/examples/lsu.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    20509 2024-04-05 11:53:17.000000 python-sat-1.8.dev9/examples/mcsls.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     5741 2024-04-05 12:12:36.000000 python-sat-1.8.dev9/examples/models.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    10747 2024-04-05 11:53:33.000000 python-sat-1.8.dev9/examples/musx.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    25841 2024-04-05 11:50:00.000000 python-sat-1.8.dev9/examples/optux.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567    67511 2024-04-05 12:47:02.000000 python-sat-1.8.dev9/examples/rc2.py
+-rwxr-xr-x   0 aign0002 (892519254) 907548567     2183 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/examples/usage.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.742012 python-sat-1.8.dev9/pysat/
+-rw-r--r--   0 aign0002 (892519254) 907548567      669 2024-04-07 06:16:33.000000 python-sat-1.8.dev9/pysat/__init__.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     5814 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/pysat/_fileio.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1340 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/pysat/_utils.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    30043 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/pysat/card.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    45094 2024-03-18 05:43:24.000000 python-sat-1.8.dev9/pysat/engines.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   192658 2024-03-31 04:44:45.000000 python-sat-1.8.dev9/pysat/formula.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    16649 2024-03-16 04:25:34.000000 python-sat-1.8.dev9/pysat/pb.py
+-rw-r--r--   0 aign0002 (892519254) 907548567    11968 2023-03-05 06:22:14.000000 python-sat-1.8.dev9/pysat/process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   226003 2024-03-18 05:36:00.000000 python-sat-1.8.dev9/pysat/solvers.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.780598 python-sat-1.8.dev9/python_sat.egg-info/
+-rw-r--r--   0 aign0002 (892519254) 907548567     1523 2024-04-07 06:20:31.000000 python-sat-1.8.dev9/python_sat.egg-info/PKG-INFO
+-rw-r--r--   0 aign0002 (892519254) 907548567     2090 2024-04-07 06:20:31.000000 python-sat-1.8.dev9/python_sat.egg-info/SOURCES.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567        1 2024-04-07 06:20:31.000000 python-sat-1.8.dev9/python_sat.egg-info/dependency_links.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      148 2024-04-07 06:20:31.000000 python-sat-1.8.dev9/python_sat.egg-info/requires.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       23 2024-04-07 06:20:31.000000 python-sat-1.8.dev9/python_sat.egg-info/top_level.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567       39 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/requirements.txt
+-rw-r--r--   0 aign0002 (892519254) 907548567      108 2024-04-07 06:20:31.781713 python-sat-1.8.dev9/setup.cfg
+-rw-r--r--   0 aign0002 (892519254) 907548567     6664 2024-04-07 06:16:21.000000 python-sat-1.8.dev9/setup.py
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.759439 python-sat-1.8.dev9/solvers/
+-rw-r--r--   0 aign0002 (892519254) 907548567   547031 2023-03-02 05:10:30.000000 python-sat-1.8.dev9/solvers/cadical103.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   596433 2023-03-03 10:16:48.000000 python-sat-1.8.dev9/solvers/cadical153.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   644206 2023-08-25 01:25:36.000000 python-sat-1.8.dev9/solvers/cadical170.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   691268 2024-03-16 04:33:34.000000 python-sat-1.8.dev9/solvers/cadical195.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    50813 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/glucose30.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82779 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/glucose41.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    88105 2023-07-11 23:37:13.000000 python-sat-1.8.dev9/solvers/glucose421.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567   501731 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/lingeling.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    82656 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/maplechrono.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    94949 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/maplecm.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567    77088 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/maplesat.zip
+-rw-r--r--   0 aign0002 (892519254) 907548567   179223 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/mergesat3.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567  1529188 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/minicard.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    43879 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/minisat22.tar.gz
+-rw-r--r--   0 aign0002 (892519254) 907548567    75209 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/minisatgh.zip
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.775824 python-sat-1.8.dev9/solvers/patches/
+-rw-r--r--   0 aign0002 (892519254) 907548567    51588 2023-03-02 05:15:52.000000 python-sat-1.8.dev9/solvers/patches/cadical103.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    69395 2024-03-17 07:15:43.000000 python-sat-1.8.dev9/solvers/patches/cadical153.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    92447 2024-04-07 06:10:23.000000 python-sat-1.8.dev9/solvers/patches/cadical195.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    93207 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/glucose30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    89206 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/glucose41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    68942 2023-07-15 01:30:10.000000 python-sat-1.8.dev9/solvers/patches/glucose421.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   117955 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/gluecard30.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   137342 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/gluecard41.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    54848 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/lingeling.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    90618 2023-01-14 22:24:35.000000 python-sat-1.8.dev9/solvers/patches/maplechrono.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567   114715 2023-01-14 21:29:08.000000 python-sat-1.8.dev9/solvers/patches/maplecm.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    82379 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/maplesat.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    88893 2023-01-14 22:24:31.000000 python-sat-1.8.dev9/solvers/patches/mergesat3.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    51757 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/minicard.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    42627 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/minisat22.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    60626 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/solvers/patches/minisatgh.patch
+-rw-r--r--   0 aign0002 (892519254) 907548567    32315 2024-04-07 06:10:30.000000 python-sat-1.8.dev9/solvers/prepare.py
+-rw-r--r--   0 aign0002 (892519254) 907548567   285751 2024-03-16 04:32:47.000000 python-sat-1.8.dev9/solvers/pysolvers.cc
+drwxr-xr-x   0 aign0002 (892519254) 907548567        0 2024-04-07 06:20:31.779852 python-sat-1.8.dev9/tests/
+-rw-r--r--   0 aign0002 (892519254) 907548567      987 2023-07-12 00:04:49.000000 python-sat-1.8.dev9/tests/test_accum_stats.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      429 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/tests/test_atmost.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      707 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/tests/test_atmost1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      998 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/tests/test_atmostk.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1299 2024-03-17 06:23:23.000000 python-sat-1.8.dev9/tests/test_boolengine.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     2432 2023-07-12 00:04:57.000000 python-sat-1.8.dev9/tests/test_cnfplus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      784 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/tests/test_equals1.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1007 2023-03-05 06:31:37.000000 python-sat-1.8.dev9/tests/test_process.py
+-rw-r--r--   0 aign0002 (892519254) 907548567     1285 2024-04-06 08:24:37.000000 python-sat-1.8.dev9/tests/test_propagate.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      890 2023-07-12 00:05:05.000000 python-sat-1.8.dev9/tests/test_unique_model.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      937 2023-01-13 10:53:42.000000 python-sat-1.8.dev9/tests/test_unique_mus.py
+-rw-r--r--   0 aign0002 (892519254) 907548567      650 2023-07-12 00:05:10.000000 python-sat-1.8.dev9/tests/test_warmstart.py
```

### Comparing `python-sat-1.8.dev8/LICENSE.txt` & `python-sat-1.8.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/PKG-INFO` & `python-sat-1.8.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 1.8.dev8
+Version: 1.8.dev9
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `python-sat-1.8.dev8/README.rst` & `python-sat-1.8.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/allies/approxmc.py` & `python-sat-1.8.dev9/allies/approxmc.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/allies/unigen.py` & `python-sat-1.8.dev9/allies/unigen.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/bitwise.hh` & `python-sat-1.8.dev9/cardenc/bitwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/card.hh` & `python-sat-1.8.dev9/cardenc/card.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/clset.hh` & `python-sat-1.8.dev9/cardenc/clset.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/common.hh` & `python-sat-1.8.dev9/cardenc/common.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/itot.hh` & `python-sat-1.8.dev9/cardenc/itot.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/ladder.hh` & `python-sat-1.8.dev9/cardenc/ladder.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/mto.hh` & `python-sat-1.8.dev9/cardenc/mto.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/pairwise.hh` & `python-sat-1.8.dev9/cardenc/pairwise.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/ptypes.hh` & `python-sat-1.8.dev9/cardenc/ptypes.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/pycard.cc` & `python-sat-1.8.dev9/cardenc/pycard.cc`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/seqcounter.hh` & `python-sat-1.8.dev9/cardenc/seqcounter.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/sortcard.hh` & `python-sat-1.8.dev9/cardenc/sortcard.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/cardenc/utils.hh` & `python-sat-1.8.dev9/cardenc/utils.hh`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/fm.py` & `python-sat-1.8.dev9/examples/fm.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/genhard.py` & `python-sat-1.8.dev9/examples/genhard.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/hitman.py` & `python-sat-1.8.dev9/examples/hitman.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/lbx.py` & `python-sat-1.8.dev9/examples/lbx.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/lsu.py` & `python-sat-1.8.dev9/examples/lsu.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/mcsls.py` & `python-sat-1.8.dev9/examples/mcsls.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/models.py` & `python-sat-1.8.dev9/examples/models.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/musx.py` & `python-sat-1.8.dev9/examples/musx.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/optux.py` & `python-sat-1.8.dev9/examples/optux.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/rc2.py` & `python-sat-1.8.dev9/examples/rc2.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/examples/usage.py` & `python-sat-1.8.dev9/examples/usage.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/__init__.py` & `python-sat-1.8.dev9/pysat/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ##  Created on: Mar 4, 2017
 ##      Author: Alexey S. Ignatiev
 ##      E-mail: aignatiev@ciencias.ulisboa.pt
 ##
 
 # current version
 #==============================================================================
-VERSION = (1, 8, 'dev', 8)
+VERSION = (1, 8, 'dev', 9)
 
 
 # PEP440 Format
 #==============================================================================
 __version__ = '%d.%d.%s%d' % VERSION if len(VERSION) == 4 else \
               '%d.%d.%d' % VERSION
```

### Comparing `python-sat-1.8.dev8/pysat/_fileio.py` & `python-sat-1.8.dev9/pysat/_fileio.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/_utils.py` & `python-sat-1.8.dev9/pysat/_utils.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/card.py` & `python-sat-1.8.dev9/pysat/card.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/engines.py` & `python-sat-1.8.dev9/pysat/engines.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/formula.py` & `python-sat-1.8.dev9/pysat/formula.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/pb.py` & `python-sat-1.8.dev9/pysat/pb.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/process.py` & `python-sat-1.8.dev9/pysat/process.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/pysat/solvers.py` & `python-sat-1.8.dev9/pysat/solvers.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/python_sat.egg-info/PKG-INFO` & `python-sat-1.8.dev9/python_sat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sat
-Version: 1.8.dev8
+Version: 1.8.dev9
 Summary: A Python library for prototyping with SAT oracles
 Home-page: https://github.com/pysathq/pysat
 Author: Alexey Ignatiev, Joao Marques-Silva, Antonio Morgado
 Author-email: alexey.ignatiev@monash.edu, joao.marques-silva@univ-toulouse.fr, ajrmorgado@gmail.com
 License: MIT
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
```

### Comparing `python-sat-1.8.dev8/python_sat.egg-info/SOURCES.txt` & `python-sat-1.8.dev9/python_sat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/setup.py` & `python-sat-1.8.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/cadical103.tar.gz` & `python-sat-1.8.dev9/solvers/cadical103.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/cadical153.tar.gz` & `python-sat-1.8.dev9/solvers/cadical153.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/cadical170.tar.gz` & `python-sat-1.8.dev9/solvers/cadical170.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/cadical195.tar.gz` & `python-sat-1.8.dev9/solvers/cadical195.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/glucose30.tar.gz` & `python-sat-1.8.dev9/solvers/glucose30.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/glucose41.tar.gz` & `python-sat-1.8.dev9/solvers/glucose41.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/glucose421.tar.gz` & `python-sat-1.8.dev9/solvers/glucose421.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/lingeling.tar.gz` & `python-sat-1.8.dev9/solvers/lingeling.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/maplechrono.zip` & `python-sat-1.8.dev9/solvers/maplechrono.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/maplecm.zip` & `python-sat-1.8.dev9/solvers/maplecm.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/maplesat.zip` & `python-sat-1.8.dev9/solvers/maplesat.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/mergesat3.tar.gz` & `python-sat-1.8.dev9/solvers/mergesat3.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/minicard.tar.gz` & `python-sat-1.8.dev9/solvers/minicard.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/minisat22.tar.gz` & `python-sat-1.8.dev9/solvers/minisat22.tar.gz`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/minisatgh.zip` & `python-sat-1.8.dev9/solvers/minisatgh.zip`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/cadical103.patch` & `python-sat-1.8.dev9/solvers/patches/cadical103.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/cadical153.patch` & `python-sat-1.8.dev9/solvers/patches/cadical153.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/cadical195.patch` & `python-sat-1.8.dev9/solvers/patches/cadical195.patch`

 * *Files 0% similar despite different names*

```diff
@@ -2830,15 +2830,15 @@
    FATAL ("learned unit %d contradicts solution", unit);
  }
  
 -} // namespace CaDiCaL
 +} // namespace CaDiCaL195
 diff -Naur solvers/cadical195/solver.cpp solvers/cdc195/solver.cpp
 --- solvers/cadical195/solver.cpp	2024-02-29 02:59:11
-+++ solvers/cdc195/solver.cpp	2024-03-17 17:49:46
++++ solvers/cdc195/solver.cpp	2024-04-07 16:10:03
 @@ -2,7 +2,7 @@
  
  /*------------------------------------------------------------------------*/
  
 -namespace CaDiCaL {
 +namespace CaDiCaL195 {
  
@@ -2977,49 +2977,54 @@
 +  traverse_clauses(getter);
 +  dest = getter.clauses;
 +}
 +
  const char *Solver::write_dimacs (const char *path, int min_max_var) {
    LOG_API_CALL_BEGIN ("write_dimacs", path, min_max_var);
    REQUIRE_VALID_STATE ();
-@@ -1628,4 +1716,91 @@
+@@ -1628,4 +1716,99 @@
    va_end (ap);
  }
  
 -} // namespace CaDiCaL
 +//=================================================================================================
 +// Propagate and check
 +bool Solver::prop_check(const vector<int>& assump, vector<int>& prop, int psaving) {
 +  prop.clear();
 +
 +  if (internal->unsat || internal->unsat_constraint) {
 +    return false;
 +  }
 +
-+  // dealing with phase saving //TODO check how to do this
-+  int old_psave = internal->opts.rephase; // note: these can be made (very) slightly more efficient by accessing the table directly
-+  int old_lucky = internal->opts.lucky;
-+  internal->opts.lucky = psaving;
-+  internal->opts.rephase = psaving;
-+
-+  int old_resetall = internal->opts.restoreall;
++  // saving default options
++  int old_ilb    = internal->opts.ilb;
++  int old_psave  = internal->opts.rephase; // note: these can be made (very) slightly more efficient by accessing the table directly
++  int old_lucky  = internal->opts.lucky;
++  int old_resall = internal->opts.restoreall;
++
++  // resetting the above options
++  internal->opts.ilb        = 0;
++  internal->opts.lucky      = psaving;
++  internal->opts.rephase    = psaving;
 +  internal->opts.restoreall = 2;
++
 +  int tmp = internal->already_solved ();
-+  if (!tmp) {
++  if (!tmp)
 +    tmp = internal->restore_clauses ();
-+  }
 +  if (tmp) {
-+    internal->opts.restoreall = old_resetall;
-+    internal->opts.rephase = old_psave;
-+    internal->opts.lucky = old_lucky;
++    // restoring default option values
++    internal->opts.ilb        = old_ilb;
++    internal->opts.lucky      = old_lucky;
++    internal->opts.rephase    = old_psave;
++    internal->opts.restoreall = old_resall;
 +    internal->reset_solving();
 +    internal->report_solving(tmp);
 +    return false;
 +  }
-+  internal->opts.restoreall = old_resetall;
++  internal->opts.restoreall = old_resall;
 +
 +  bool st = true;
 +  int level = internal->level;
 +  bool noconfl = true;
 +  Clause *old_conflict = internal->conflict;
 +
 +  // propagate each assumption at a new decision level
@@ -3057,17 +3062,20 @@
 +      int conflict_val = *conflict_ptr;
 +      prop.push_back(conflict_val);
 +    }
 +    // backtrack
 +    internal->backtrack(level);
 +  }
 +
++  // restoring default ilb value
++  internal->opts.ilb = old_ilb;
++
 +  // restore phase saving
 +  internal->opts.rephase = old_psave;
-+  internal->opts.lucky = old_lucky;
++  internal->opts.lucky   = old_lucky;
 +  // reset conflict
 +  internal->conflict = old_conflict;
 +  internal->reset_solving();
 +  internal->report_solving(tmp);
 +
 +  // return
 +  return st && noconfl;
```

### Comparing `python-sat-1.8.dev8/solvers/patches/glucose30.patch` & `python-sat-1.8.dev9/solvers/patches/glucose30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/glucose41.patch` & `python-sat-1.8.dev9/solvers/patches/glucose41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/glucose421.patch` & `python-sat-1.8.dev9/solvers/patches/glucose421.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/gluecard30.patch` & `python-sat-1.8.dev9/solvers/patches/gluecard30.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/gluecard41.patch` & `python-sat-1.8.dev9/solvers/patches/gluecard41.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/lingeling.patch` & `python-sat-1.8.dev9/solvers/patches/lingeling.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/maplechrono.patch` & `python-sat-1.8.dev9/solvers/patches/maplechrono.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/maplecm.patch` & `python-sat-1.8.dev9/solvers/patches/maplecm.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/maplesat.patch` & `python-sat-1.8.dev9/solvers/patches/maplesat.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/mergesat3.patch` & `python-sat-1.8.dev9/solvers/patches/mergesat3.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/minicard.patch` & `python-sat-1.8.dev9/solvers/patches/minicard.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/minisat22.patch` & `python-sat-1.8.dev9/solvers/patches/minisat22.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/patches/minisatgh.patch` & `python-sat-1.8.dev9/solvers/patches/minisatgh.patch`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/prepare.py` & `python-sat-1.8.dev9/solvers/prepare.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/solvers/pysolvers.cc` & `python-sat-1.8.dev9/solvers/pysolvers.cc`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_accum_stats.py` & `python-sat-1.8.dev9/tests/test_accum_stats.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_atmost1.py` & `python-sat-1.8.dev9/tests/test_atmost1.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_atmostk.py` & `python-sat-1.8.dev9/tests/test_atmostk.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_boolengine.py` & `python-sat-1.8.dev9/tests/test_boolengine.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_cnfplus.py` & `python-sat-1.8.dev9/tests/test_cnfplus.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_equals1.py` & `python-sat-1.8.dev9/tests/test_equals1.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_process.py` & `python-sat-1.8.dev9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_propagate.py` & `python-sat-1.8.dev9/tests/test_propagate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pysat.card import *
 from pysat.solvers import Solver
 
 solvers = ['cadical153',
+           'cadical195',
            'gluecard30',
            'gluecard41',
            'glucose30',
            'glucose41',
            'glucose42',
            'maplechrono',
            'maplecm',
```

### Comparing `python-sat-1.8.dev8/tests/test_unique_model.py` & `python-sat-1.8.dev9/tests/test_unique_model.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_unique_mus.py` & `python-sat-1.8.dev9/tests/test_unique_mus.py`

 * *Files identical despite different names*

### Comparing `python-sat-1.8.dev8/tests/test_warmstart.py` & `python-sat-1.8.dev9/tests/test_warmstart.py`

 * *Files identical despite different names*

