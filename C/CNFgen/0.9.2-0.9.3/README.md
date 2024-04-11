# Comparing `tmp/CNFgen-0.9.2.tar.gz` & `tmp/CNFgen-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CNFgen-0.9.2.tar", last modified: Thu May 11 14:51:01 2023, max compression
+gzip compressed data, was "CNFgen-0.9.3.tar", last modified: Thu Apr 11 10:44:20 2024, max compression
```

## Comparing `CNFgen-0.9.2.tar` & `CNFgen-0.9.3.tar`

### file list

```diff
@@ -1,87 +1,126 @@
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.888768 CNFgen-0.9.2/
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.861177 CNFgen-0.9.2/CNFgen.egg-info/
--rw-------   0 massimo    (501) staff       (20)     1234 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/PKG-INFO
--rw-------   0 massimo    (501) staff       (20)     2077 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/SOURCES.txt
--rw-------   0 massimo    (501) staff       (20)        1 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/dependency_links.txt
--rw-------   0 massimo    (501) staff       (20)      135 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/entry_points.txt
--rw-------   0 massimo    (501) staff       (20)       27 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/requires.txt
--rw-------   0 massimo    (501) staff       (20)        7 2023-05-11 14:51:01.000000 CNFgen-0.9.2/CNFgen.egg-info/top_level.txt
--rw-------   0 massimo    (501) staff       (20)      954 2022-08-15 11:20:27.000000 CNFgen-0.9.2/CREDITS.org
--rw-------   0 massimo    (501) staff       (20)    35128 2022-08-15 11:20:27.000000 CNFgen-0.9.2/LICENSE
--rw-------   0 massimo    (501) staff       (20)      113 2022-08-15 11:20:27.000000 CNFgen-0.9.2/MANIFEST.in
--rw-------   0 massimo    (501) staff       (20)     2582 2023-01-15 11:21:57.000000 CNFgen-0.9.2/Makefile
--rw-------   0 massimo    (501) staff       (20)     1234 2023-05-11 14:51:01.888252 CNFgen-0.9.2/PKG-INFO
--rw-------   0 massimo    (501) staff       (20)      944 2022-08-15 11:20:27.000000 CNFgen-0.9.2/PyPI.md
--rw-------   0 massimo    (501) staff       (20)     3263 2022-08-15 11:20:27.000000 CNFgen-0.9.2/README.org
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.863429 CNFgen-0.9.2/cnfgen/
--rw-------   0 massimo    (501) staff       (20)     3498 2023-03-30 20:33:37.000000 CNFgen-0.9.2/cnfgen/__init__.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.867329 CNFgen-0.9.2/cnfgen/clihelpers/
--rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/__init__.py
--rw-r--r--   0 massimo    (501) staff       (20)    12300 2023-04-26 01:25:24.000000 CNFgen-0.9.2/cnfgen/clihelpers/counting_helpers.py
--rw-------   0 massimo    (501) staff       (20)     1915 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/cpls_helpers.py
--rw-------   0 massimo    (501) staff       (20)     1732 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/dimacs_helpers.py
--rw-------   0 massimo    (501) staff       (20)      706 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/formula_helpers.py
--rw-------   0 massimo    (501) staff       (20)    14314 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/graph_helpers.py
--rw-------   0 massimo    (501) staff       (20)     5736 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/ordering_helpers.py
--rw-------   0 massimo    (501) staff       (20)     4353 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/pebbling_helpers.py
--rw-------   0 massimo    (501) staff       (20)    17206 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/php_helpers.py
--rw-------   0 massimo    (501) staff       (20)     1947 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/pitfall_helpers.py
--rw-------   0 massimo    (501) staff       (20)     8535 2023-03-30 20:45:56.000000 CNFgen-0.9.2/cnfgen/clihelpers/simple_helpers.py
--rw-------   0 massimo    (501) staff       (20)    16941 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clihelpers/transformation_helpers.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.870698 CNFgen-0.9.2/cnfgen/clitools/
--rw-------   0 massimo    (501) staff       (20)     1117 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/__init__.py
--rwx------   0 massimo    (501) staff       (20)     9386 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/cmdline.py
--rwx------   0 massimo    (501) staff       (20)    19172 2023-03-30 19:31:28.000000 CNFgen-0.9.2/cnfgen/clitools/cnfgen.py
--rw-------   0 massimo    (501) staff       (20)     5472 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/cnfshuffle.py
--rw-------   0 massimo    (501) staff       (20)    14525 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_args.py
--rw-------   0 massimo    (501) staff       (20)    14232 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_build.py
--rw-------   0 massimo    (501) staff       (20)     5967 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_docs.py
--rwx------   0 massimo    (501) staff       (20)     2972 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/graph_fileinput.py
--rw-------   0 massimo    (501) staff       (20)     6298 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/kthlist2pebbling.py
--rw-------   0 massimo    (501) staff       (20)     1769 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/msg.py
--rw-------   0 massimo    (501) staff       (20)    15414 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/clitools/pbgen.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.878539 CNFgen-0.9.2/cnfgen/families/
--rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/__init__.py
--rw-------   0 massimo    (501) staff       (20)     2336 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/cliquecoloring.py
--rwx------   0 massimo    (501) staff       (20)     2949 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/coloring.py
--rw-------   0 massimo    (501) staff       (20)     1777 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/counting.py
--rw-------   0 massimo    (501) staff       (20)     3028 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/cpls.py
--rw-------   0 massimo    (501) staff       (20)     3874 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/dominatingset.py
--rw-------   0 massimo    (501) staff       (20)     2222 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/graphisomorphism.py
--rw-------   0 massimo    (501) staff       (20)     4309 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/ordering.py
--rwx------   0 massimo    (501) staff       (20)     7136 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pebbling.py
--rw-------   0 massimo    (501) staff       (20)    11935 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pigeonhole.py
--rw-------   0 massimo    (501) staff       (20)     5408 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/pitfall.py
--rw-------   0 massimo    (501) staff       (20)     6300 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/ramsey.py
--rw-------   0 massimo    (501) staff       (20)     4005 2023-03-30 20:22:27.000000 CNFgen-0.9.2/cnfgen/families/randomformulas.py
--rw-r--r--   0 massimo    (501) staff       (20)     4318 2023-03-30 20:22:10.000000 CNFgen-0.9.2/cnfgen/families/randomkxor.py
--rw-------   0 massimo    (501) staff       (20)     6837 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/subgraph.py
--rw-------   0 massimo    (501) staff       (20)     3207 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/subsetcardinality.py
--rw-------   0 massimo    (501) staff       (20)     1651 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/families/tseitin.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.883733 CNFgen-0.9.2/cnfgen/formula/
--rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/__init__.py
--rw-------   0 massimo    (501) staff       (20)     9755 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/basecnf.py
--rw-------   0 massimo    (501) staff       (20)    18010 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/baseopb.py
--rwx------   0 massimo    (501) staff       (20)     2425 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/cnf.py
--rw-------   0 massimo    (501) staff       (20)    13353 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/cnfio.py
--rw-------   0 massimo    (501) staff       (20)     8052 2023-03-30 19:47:51.000000 CNFgen-0.9.2/cnfgen/formula/linear.py
--rw-------   0 massimo    (501) staff       (20)     2632 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/opb.py
--rw-------   0 massimo    (501) staff       (20)     4661 2023-03-30 16:53:11.000000 CNFgen-0.9.2/cnfgen/formula/opbio.py
--rw-------   0 massimo    (501) staff       (20)    64230 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/formula/variables.py
--rwx------   0 massimo    (501) staff       (20)    61042 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/graphs.py
--rw-------   0 massimo    (501) staff       (20)     1189 2022-12-24 07:47:49.000000 CNFgen-0.9.2/cnfgen/info.py
--rw-------   0 massimo    (501) staff       (20)     2378 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/localtypes.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.885254 CNFgen-0.9.2/cnfgen/transformations/
--rw-------   0 massimo    (501) staff       (20)        0 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/__init__.py
--rw-------   0 massimo    (501) staff       (20)     4446 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/shuffle.py
--rw-------   0 massimo    (501) staff       (20)    12741 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/transformations/substitutions.py
-drwx------   0 massimo    (501) staff       (20)        0 2023-05-11 14:51:01.887588 CNFgen-0.9.2/cnfgen/utils/
--rw-------   0 massimo    (501) staff       (20)      105 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/__init__.py
--rw-------   0 massimo    (501) staff       (20)     6938 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/latexoutput.py
--rw-------   0 massimo    (501) staff       (20)     2853 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/opb.py
--rw-------   0 massimo    (501) staff       (20)     5808 2023-04-08 07:46:21.000000 CNFgen-0.9.2/cnfgen/utils/parsedimacs.py
--rw-------   0 massimo    (501) staff       (20)    14980 2022-08-15 11:20:27.000000 CNFgen-0.9.2/cnfgen/utils/solver.py
--rw-------   0 massimo    (501) staff       (20)       18 2023-05-11 14:51:01.000000 CNFgen-0.9.2/cnfgen/version.py
--rw-------   0 massimo    (501) staff       (20)       32 2023-01-15 11:21:57.000000 CNFgen-0.9.2/requirements.txt
--rw-------   0 massimo    (501) staff       (20)       38 2023-05-11 14:51:01.888920 CNFgen-0.9.2/setup.cfg
--rw-------   0 massimo    (501) staff       (20)     1027 2022-08-15 11:20:27.000000 CNFgen-0.9.2/setup.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.244820 CNFgen-0.9.3/
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.244820 CNFgen-0.9.3/CNFgen.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1302 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/PKG-INFO
+-rw-------   0 massimo   (1000) massimo   (1000)     3057 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/SOURCES.txt
+-rw-------   0 massimo   (1000) massimo   (1000)        1 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/dependency_links.txt
+-rw-------   0 massimo   (1000) massimo   (1000)      135 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/entry_points.txt
+-rw-------   0 massimo   (1000) massimo   (1000)       32 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/requires.txt
+-rw-------   0 massimo   (1000) massimo   (1000)        7 2024-04-11 10:44:20.000000 CNFgen-0.9.3/CNFgen.egg-info/top_level.txt
+-rw-------   0 massimo   (1000) massimo   (1000)      954 2022-08-24 16:38:58.000000 CNFgen-0.9.3/CREDITS.org
+-rw-------   0 massimo   (1000) massimo   (1000)    35128 2022-08-24 16:38:58.000000 CNFgen-0.9.3/LICENSE
+-rw-------   0 massimo   (1000) massimo   (1000)      113 2022-08-24 16:38:58.000000 CNFgen-0.9.3/MANIFEST.in
+-rw-------   0 massimo   (1000) massimo   (1000)     2576 2024-04-11 10:43:59.000000 CNFgen-0.9.3/Makefile
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1302 2024-04-11 10:44:20.244820 CNFgen-0.9.3/PKG-INFO
+-rw-------   0 massimo   (1000) massimo   (1000)      944 2022-08-24 16:38:58.000000 CNFgen-0.9.3/PyPI.md
+-rw-------   0 massimo   (1000) massimo   (1000)     3263 2022-08-24 16:38:58.000000 CNFgen-0.9.3/README.org
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.232820 CNFgen-0.9.3/cnfgen/
+-rw-------   0 massimo   (1000) massimo   (1000)     3498 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/__init__.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.236820 CNFgen-0.9.3/cnfgen/clihelpers/
+-rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/__init__.py
+-rw-------   0 massimo   (1000) massimo   (1000)    12300 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/clihelpers/counting_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1915 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/cpls_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1732 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/dimacs_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)      706 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/formula_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)    14314 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/graph_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     5736 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/ordering_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4353 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/pebbling_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)    17206 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/php_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1947 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/pitfall_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     8535 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/clihelpers/simple_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)    16941 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clihelpers/transformation_helpers.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.236820 CNFgen-0.9.3/cnfgen/clitools/
+-rw-------   0 massimo   (1000) massimo   (1000)     1117 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/__init__.py
+-rwx------   0 massimo   (1000) massimo   (1000)     9507 2024-04-11 10:15:11.000000 CNFgen-0.9.3/cnfgen/clitools/cmdline.py
+-rwx------   0 massimo   (1000) massimo   (1000)    19172 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/clitools/cnfgen.py
+-rw-------   0 massimo   (1000) massimo   (1000)     5472 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/cnfshuffle.py
+-rw-------   0 massimo   (1000) massimo   (1000)    14525 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/graph_args.py
+-rw-------   0 massimo   (1000) massimo   (1000)    14232 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/graph_build.py
+-rw-------   0 massimo   (1000) massimo   (1000)     5967 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/graph_docs.py
+-rwx------   0 massimo   (1000) massimo   (1000)     2972 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/graph_fileinput.py
+-rw-------   0 massimo   (1000) massimo   (1000)     6298 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/kthlist2pebbling.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1769 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/msg.py
+-rw-------   0 massimo   (1000) massimo   (1000)    15414 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/clitools/pbgen.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.240820 CNFgen-0.9.3/cnfgen/families/
+-rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/__init__.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2336 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/cliquecoloring.py
+-rwx------   0 massimo   (1000) massimo   (1000)     2949 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/coloring.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1777 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/counting.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3028 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/cpls.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3874 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/dominatingset.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2222 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/graphisomorphism.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4309 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/ordering.py
+-rwx------   0 massimo   (1000) massimo   (1000)     7136 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/pebbling.py
+-rw-------   0 massimo   (1000) massimo   (1000)    11935 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/pigeonhole.py
+-rw-------   0 massimo   (1000) massimo   (1000)     5408 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/pitfall.py
+-rw-------   0 massimo   (1000) massimo   (1000)     6300 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/ramsey.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4005 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/families/randomformulas.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4318 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/families/randomkxor.py
+-rw-------   0 massimo   (1000) massimo   (1000)     6837 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/subgraph.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3207 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/subsetcardinality.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1651 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/families/tseitin.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.240820 CNFgen-0.9.3/cnfgen/formula/
+-rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/__init__.py
+-rw-------   0 massimo   (1000) massimo   (1000)     9755 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/basecnf.py
+-rw-------   0 massimo   (1000) massimo   (1000)    18010 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/baseopb.py
+-rwx------   0 massimo   (1000) massimo   (1000)     2425 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/cnf.py
+-rw-------   0 massimo   (1000) massimo   (1000)    13353 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/cnfio.py
+-rw-------   0 massimo   (1000) massimo   (1000)     8052 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/formula/linear.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2632 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/opb.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4661 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/formula/opbio.py
+-rw-------   0 massimo   (1000) massimo   (1000)    64230 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/formula/variables.py
+-rwx------   0 massimo   (1000) massimo   (1000)    61042 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/graphs.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1189 2022-12-12 21:05:28.000000 CNFgen-0.9.3/cnfgen/info.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2378 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/localtypes.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.240820 CNFgen-0.9.3/cnfgen/transformations/
+-rw-------   0 massimo   (1000) massimo   (1000)        0 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/transformations/__init__.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4446 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/transformations/shuffle.py
+-rw-------   0 massimo   (1000) massimo   (1000)    12741 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/transformations/substitutions.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.240820 CNFgen-0.9.3/cnfgen/utils/
+-rw-------   0 massimo   (1000) massimo   (1000)      105 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/utils/__init__.py
+-rw-------   0 massimo   (1000) massimo   (1000)     6938 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/utils/latexoutput.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2853 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/utils/opb.py
+-rw-------   0 massimo   (1000) massimo   (1000)     5808 2023-05-13 23:08:15.000000 CNFgen-0.9.3/cnfgen/utils/parsedimacs.py
+-rw-------   0 massimo   (1000) massimo   (1000)    14980 2022-08-24 16:38:58.000000 CNFgen-0.9.3/cnfgen/utils/solver.py
+-rw-------   0 massimo   (1000) massimo   (1000)       18 2024-04-11 10:44:19.000000 CNFgen-0.9.3/cnfgen/version.py
+-rw-------   0 massimo   (1000) massimo   (1000)       32 2023-01-13 14:25:23.000000 CNFgen-0.9.3/requirements.txt
+-rw-------   0 massimo   (1000) massimo   (1000)       38 2024-04-11 10:44:20.244820 CNFgen-0.9.3/setup.cfg
+-rw-------   0 massimo   (1000) massimo   (1000)     1038 2023-12-08 23:01:59.000000 CNFgen-0.9.3/setup.py
+drwx------   0 massimo   (1000) massimo   (1000)        0 2024-04-11 10:44:20.244820 CNFgen-0.9.3/tests/
+-rw-------   0 massimo   (1000) massimo   (1000)     1239 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_bipartite.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4020 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_bipartite_cmdline.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1212 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cliquecoloring.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1109 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cnf.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2702 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cnfgen.py
+-rw-------   0 massimo   (1000) massimo   (1000)      826 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cnfgen_transformation.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1322 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cnfshuffle.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1617 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_cpls.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1286 2023-05-13 23:08:15.000000 CNFgen-0.9.3/tests/test_detect_helpers.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2146 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_digraph_cmdline.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2216 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_dimacsparser.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1111 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_domset.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1207 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_evencolouring.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1379 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_flip.py
+-rw-------   0 massimo   (1000) massimo   (1000)    10122 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_graph_io.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1497 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_graphisomorphism.py
+-rw-------   0 massimo   (1000) massimo   (1000)     7530 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_handbook.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2837 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_kthlist2pebbling.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3531 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_ordering_principle.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1501 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_parse_graph_args.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2908 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_pebbling.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1655 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_perfectmatching.py
+-rw-------   0 massimo   (1000) massimo   (1000)     7389 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_pigeonhole_principle.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2156 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_pitfall.py
+-rw-------   0 massimo   (1000) massimo   (1000)      830 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_planted.py
+-rw-------   0 massimo   (1000) massimo   (1000)     6634 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_ramsey.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2191 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_randomcnf.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2394 2023-05-13 23:08:15.000000 CNFgen-0.9.3/tests/test_randxor.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1565 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_rphp.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1685 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_seed.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3505 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_shuffling.py
+-rw-------   0 massimo   (1000) massimo   (1000)     3147 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_simplegraph_cmdline.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4258 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_subgraph.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2443 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_subsetcardinality.py
+-rw-------   0 massimo   (1000) massimo   (1000)     4915 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_substitution.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1713 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_threshold_subst.py
+-rw-------   0 massimo   (1000) massimo   (1000)     1678 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_tiling.py
+-rw-------   0 massimo   (1000) massimo   (1000)     2995 2022-08-24 16:38:58.000000 CNFgen-0.9.3/tests/test_tseitin.py
```

### Comparing `CNFgen-0.9.2/CNFgen.egg-info/PKG-INFO` & `CNFgen-0.9.3/CNFgen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: CNFgen
-Version: 0.9.2
+Version: 0.9.3
 Summary: CNF formula generator
 Home-page: https://massimolauria.net/cnfgen
 Author: Massimo Lauria
 Author-email: massimo.lauria@uniroma1.it
 License: GPL-3
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: networkx<3.0,>=2.3
+Requires-Dist: pydot>=1.2.3
 
 # CNFgen formula generator and tools
 
 This repository provides the command
 
 - `cnfgen` formula generator;
```

### Comparing `CNFgen-0.9.2/CREDITS.org` & `CNFgen-0.9.3/CREDITS.org`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/LICENSE` & `CNFgen-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/Makefile` & `CNFgen-0.9.3/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 	find . -name '*.pyc' -delete
 	find . -name '*.pyo' -delete
 	find . -name 'flycheck*.py' -delete
 
 package:
 	$(MAKE) clean
 	$(MAKE) $(VERSIONFILE)
-	$(PYTHON) setup.py sdist bdist_egg bdist_wheel
+	$(PYTHON) setup.py sdist bdist_wheel
 
 
 testpackage: test
 	$(MAKE) clean
 	$(MAKE) $(VERSIONFILE)
 	$(eval pkgname=$(shell $(PYTHON) setup.py --name)-$(shell $(PYTHON) setup.py --version))
 	$(PYTHON) setup.py sdist
@@ -44,30 +44,30 @@
 	tar xfz $(pkgname).tar.gz && \
 	cd $(pkgname) && \
 	$(PYTHON) setup.py build
 	rm -fr dist/$(pkgname)
 
 upload: testpackage
 	$(MAKE) package
-	twine upload dist/*
+	twine upload --repository cnfgen dist/*
 
 #
 # Development is based on pyenv
 #
-# The environment is based on the latest 3.8 python with is neither
+# The environment is based on the latest 3.12 python with is neither
 # a '-dev' nor an 'rc*' version. At least according to the list produced by
 #
 # $ pyenv install -l
 #
-DEV_DEPENDENCES:=yapf pytest pytest-datadir flake8 'python-lsp-server[all]'
+DEV_DEPENDENCES:=yapf pytest pytest-datadir flake8 pyright
 PKG_DEPENDENCES:=wheel twine keyring
 DOC_DEPENDENCES:='sphinx<6' sphinx-autobuild numpydoc sphinx_rtd_theme sphinx-autodoc-typehints
 
 PYENV:= $(shell command -v pyenv 2> /dev/null)
-PYENV_PYVERSION:=$(shell pyenv install -l | grep '[[:space:]]3.10.[[:digit:]]*' | grep -v 'rc\|dev' | tail -1)
+PYENV_PYVERSION:=$(shell pyenv install -l | grep '[[:space:]]3.12.[[:digit:]]*' | grep -v 'rc\|dev' | tail -1)
 
 docs: docs-install-tools $(VERSIONFILE)
 	. $(VIRTUALENV)/bin/activate && \
 	python setup.py install && \
 	sphinx-apidoc -e -o docs $(PROJECT)  && \
 	$(MAKE) -C docs html && \
 	pip uninstall -y $(PROJECT)
```

### Comparing `CNFgen-0.9.2/PKG-INFO` & `CNFgen-0.9.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: CNFgen
-Version: 0.9.2
+Version: 0.9.3
 Summary: CNF formula generator
 Home-page: https://massimolauria.net/cnfgen
 Author: Massimo Lauria
 Author-email: massimo.lauria@uniroma1.it
 License: GPL-3
-Requires-Python: >=3.6
+Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: networkx<3.0,>=2.3
+Requires-Dist: pydot>=1.2.3
 
 # CNFgen formula generator and tools
 
 This repository provides the command
 
 - `cnfgen` formula generator;
```

### Comparing `CNFgen-0.9.2/PyPI.md` & `CNFgen-0.9.3/PyPI.md`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/README.org` & `CNFgen-0.9.3/README.org`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/__init__.py` & `CNFgen-0.9.3/cnfgen/__init__.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/counting_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/counting_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/cpls_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/cpls_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/dimacs_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/dimacs_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/formula_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/formula_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/graph_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/graph_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/ordering_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/ordering_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/pebbling_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/pebbling_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/php_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/php_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/pitfall_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/pitfall_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/simple_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/simple_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clihelpers/transformation_helpers.py` & `CNFgen-0.9.3/cnfgen/clihelpers/transformation_helpers.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/__init__.py` & `CNFgen-0.9.3/cnfgen/clitools/__init__.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/cmdline.py` & `CNFgen-0.9.3/cnfgen/clitools/cmdline.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 # -*- coding:utf-8 -*-
 """Components for command line interface
 
 CNFgen has many command line entry points to its functionality, and
 some of them expose the same functionality over and over. This module
 contains useful common components.
 
-Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021
+Copyright (C) 2012, 2013, 2014, 2015, 2016, 2019, 2020, 2021, 2023, 2024
 Massimo Lauria <massimo.lauria@uniroma1.it>
 https://github.com/MassimoLauria/cnfgen.git
 
 """
 
 import os
 import sys
 import argparse
 import subprocess
 import tempfile
 import signal
+import importlib
 
 from contextlib import redirect_stdout
 from contextlib import contextmanager
 
 from cnfgen.clitools.graph_args import ObtainGraphAction
 
 
@@ -95,15 +96,17 @@
         sortkey = str
 
     for loader, module_name, _ in pkgutil.walk_packages(package.__path__):
         module_name = package.__name__ + "." + module_name
         if module_name in sys.modules:
             module = sys.modules[module_name]
         else:
-            module = loader.find_module(module_name).load_module(module_name)
+            modspec = importlib.util.find_spec(module_name)
+            module  = importlib.util.module_from_spec(modspec)
+            modspec.loader.exec_module(module)
         for objname in dir(module):
             obj = getattr(module, objname)
             if test(obj):
                 result.append(obj)
     result.sort(key=sortkey)
     return result
```

### Comparing `CNFgen-0.9.2/cnfgen/clitools/cnfgen.py` & `CNFgen-0.9.3/cnfgen/clitools/cnfgen.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/cnfshuffle.py` & `CNFgen-0.9.3/cnfgen/clitools/cnfshuffle.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/graph_args.py` & `CNFgen-0.9.3/cnfgen/clitools/graph_args.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/graph_build.py` & `CNFgen-0.9.3/cnfgen/clitools/graph_build.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/graph_docs.py` & `CNFgen-0.9.3/cnfgen/clitools/graph_docs.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/graph_fileinput.py` & `CNFgen-0.9.3/cnfgen/clitools/graph_fileinput.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/kthlist2pebbling.py` & `CNFgen-0.9.3/cnfgen/clitools/kthlist2pebbling.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/msg.py` & `CNFgen-0.9.3/cnfgen/clitools/msg.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/clitools/pbgen.py` & `CNFgen-0.9.3/cnfgen/clitools/pbgen.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/cliquecoloring.py` & `CNFgen-0.9.3/cnfgen/families/cliquecoloring.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/coloring.py` & `CNFgen-0.9.3/cnfgen/families/coloring.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/counting.py` & `CNFgen-0.9.3/cnfgen/families/counting.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/cpls.py` & `CNFgen-0.9.3/cnfgen/families/cpls.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/dominatingset.py` & `CNFgen-0.9.3/cnfgen/families/dominatingset.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/graphisomorphism.py` & `CNFgen-0.9.3/cnfgen/families/graphisomorphism.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/ordering.py` & `CNFgen-0.9.3/cnfgen/families/ordering.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/pebbling.py` & `CNFgen-0.9.3/cnfgen/families/pebbling.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/pigeonhole.py` & `CNFgen-0.9.3/cnfgen/families/pigeonhole.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/pitfall.py` & `CNFgen-0.9.3/cnfgen/families/pitfall.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/ramsey.py` & `CNFgen-0.9.3/cnfgen/families/ramsey.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/randomformulas.py` & `CNFgen-0.9.3/cnfgen/families/randomformulas.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/randomkxor.py` & `CNFgen-0.9.3/cnfgen/families/randomkxor.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/subgraph.py` & `CNFgen-0.9.3/cnfgen/families/subgraph.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/subsetcardinality.py` & `CNFgen-0.9.3/cnfgen/families/subsetcardinality.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/families/tseitin.py` & `CNFgen-0.9.3/cnfgen/families/tseitin.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/basecnf.py` & `CNFgen-0.9.3/cnfgen/formula/basecnf.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/baseopb.py` & `CNFgen-0.9.3/cnfgen/formula/baseopb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/cnf.py` & `CNFgen-0.9.3/cnfgen/formula/cnf.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/cnfio.py` & `CNFgen-0.9.3/cnfgen/formula/cnfio.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/linear.py` & `CNFgen-0.9.3/cnfgen/formula/linear.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/opb.py` & `CNFgen-0.9.3/cnfgen/formula/opb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/opbio.py` & `CNFgen-0.9.3/cnfgen/formula/opbio.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/formula/variables.py` & `CNFgen-0.9.3/cnfgen/formula/variables.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/graphs.py` & `CNFgen-0.9.3/cnfgen/graphs.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/info.py` & `CNFgen-0.9.3/cnfgen/info.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/localtypes.py` & `CNFgen-0.9.3/cnfgen/localtypes.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/transformations/shuffle.py` & `CNFgen-0.9.3/cnfgen/transformations/shuffle.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/transformations/substitutions.py` & `CNFgen-0.9.3/cnfgen/transformations/substitutions.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/utils/latexoutput.py` & `CNFgen-0.9.3/cnfgen/utils/latexoutput.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/utils/opb.py` & `CNFgen-0.9.3/cnfgen/utils/opb.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/utils/parsedimacs.py` & `CNFgen-0.9.3/cnfgen/utils/parsedimacs.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/cnfgen/utils/solver.py` & `CNFgen-0.9.3/cnfgen/utils/solver.py`

 * *Files identical despite different names*

### Comparing `CNFgen-0.9.2/setup.py` & `CNFgen-0.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,13 +23,13 @@
     entry_points={
         'console_scripts': [
             'cnfgen=cnfgen.clitools.cnfgen:main',
             'pbgen=cnfgen.clitools.pbgen:main',
             'cnfshuffle=cnfgen.clitools.cnfshuffle:main'
         ],
     },
-    install_requires=['networkx>=2.0', 'pydot>=1.2.3'],
-    python_requires='>=3.6',
+    install_requires=['networkx>=2.3,<3.0', 'pydot>=1.2.3'],
+    python_requires='>=3.6,<3.12',
 
     # Package long description in Markdown
     long_description=long_description,
     long_description_content_type='text/markdown')
```

