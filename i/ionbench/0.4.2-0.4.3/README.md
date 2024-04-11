# Comparing `tmp/ionbench-0.4.2.tar.gz` & `tmp/ionbench-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionbench-0.4.2.tar", last modified: Fri Apr  5 15:58:00 2024, max compression
+gzip compressed data, was "ionbench-0.4.3.tar", last modified: Thu Apr 11 17:27:16 2024, max compression
```

## Comparing `ionbench-0.4.2.tar` & `ionbench-0.4.3.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.267327 ionbench-0.4.2/
--rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5369 2024-04-05 15:58:00.257357 ionbench-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.398327 ionbench-0.4.2/ionbench/
--rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.2/ionbench/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.547619 ionbench-0.4.2/ionbench/benchmarker/
--rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.2/ionbench/benchmarker/__init__.py
--rw-rw-rw-   0        0        0    38265 2024-04-04 14:59:14.000000 ionbench-0.4.2/ionbench/benchmarker/benchmarker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.309470 ionbench-0.4.2/ionbench/data/
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.643812 ionbench-0.4.2/ionbench/data/loewe2016/
--rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
--rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
--rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.2/ionbench/data/loewe2016/ikr.csv
--rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.2/ionbench/data/loewe2016/ikur.csv
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.697722 ionbench-0.4.2/ionbench/data/moreno2016/
--rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.2/ionbench/data/moreno2016/ina.csv
--rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.2/ionbench/data/moreno2016/moreno2016.mmt
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.772463 ionbench-0.4.2/ionbench/data/staircase/
--rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.2/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
--rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.2/ionbench/data/staircase/dataHH.csv
--rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.2/ionbench/data/staircase/dataMM.csv
--rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.2/ionbench/data/staircase/fink-2008-ikr-mm.mmt
--rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.2/ionbench/data/staircase/staircase-pace.mmt
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.792975 ionbench-0.4.2/ionbench/data/test/
--rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.2/ionbench/data/test/data.csv
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.839650 ionbench-0.4.2/ionbench/modification/
--rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.2/ionbench/modification/__init__.py
--rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.2/ionbench/modification/modification.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:58.865497 ionbench-0.4.2/ionbench/optimisers/
--rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.2/ionbench/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.382740 ionbench-0.4.2/ionbench/optimisers/external_optimisers/
--rw-rw-rw-   0        0        0     5632 2024-04-05 09:00:28.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
--rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Bot2012.py
--rw-rw-rw-   0        0        0     5153 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
--rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
--rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
--rw-rw-rw-   0        0        0     3223 2024-03-21 15:12:02.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
--rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
--rw-rw-rw-   0        0        0    10669 2024-03-26 10:17:05.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
--rw-rw-rw-   0        0        0     7970 2024-03-25 15:17:59.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
--rw-rw-rw-   0        0        0    10097 2024-03-21 13:12:06.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
--rw-rw-rw-   0        0        0     4293 2024-03-21 13:12:06.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
--rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/__init__.py
--rw-rw-rw-   0        0        0    15056 2024-03-28 15:05:33.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
--rw-rw-rw-   0        0        0     8595 2024-03-25 15:17:59.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     7612 2024-03-25 15:17:58.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5125 2024-03-21 13:03:27.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
--rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
--rw-rw-rw-   0        0        0     6680 2024-04-05 09:00:28.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
--rw-rw-rw-   0        0        0     4418 2024-03-26 10:13:34.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
--rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
--rw-rw-rw-   0        0        0     3221 2024-04-05 12:40:19.000000 ionbench-0.4.2/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.521098 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/
--rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/cmaes_pints.py
--rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
--rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/pso_pints.py
--rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/snes_pints.py
--rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.2/ionbench/optimisers/pints_optimisers/xnes_pints.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.677281 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/
--rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-21 13:11:58.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
--rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/lm_scipy.py
--rw-rw-rw-   0        0        0     2900 2024-03-21 16:55:00.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
--rw-rw-rw-   0        0        0     2905 2024-03-21 16:55:01.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/powell_scipy.py
--rw-rw-rw-   0        0        0     2320 2024-03-21 16:55:01.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
--rw-rw-rw-   0        0        0     2009 2024-03-28 14:52:14.000000 ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.790619 ionbench-0.4.2/ionbench/problems/
--rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.2/ionbench/problems/__init__.py
--rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/loewe2016.py
--rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/moreno2016.py
--rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.2/ionbench/problems/staircase.py
--rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.2/ionbench/problems/test.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.826542 ionbench-0.4.2/ionbench/tracker/
--rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.2/ionbench/tracker/__init__.py
--rw-rw-rw-   0        0        0    16883 2024-04-05 09:42:13.000000 ionbench-0.4.2/ionbench/tracker/tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:57:59.897269 ionbench-0.4.2/ionbench/uncertainty/
--rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.2/ionbench/uncertainty/__init__.py
--rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.2/ionbench/uncertainty/fim.py
--rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.2/ionbench/uncertainty/profile_likelihood.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.121371 ionbench-0.4.2/ionbench/utils/
--rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.2/ionbench/utils/__init__.py
--rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.2/ionbench/utils/autodiff.py
--rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.2/ionbench/utils/cache.py
--rw-rw-rw-   0        0        0     4897 2024-04-05 08:53:05.000000 ionbench-0.4.2/ionbench/utils/classes_pints.py
--rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.2/ionbench/utils/multistart.py
--rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.2/ionbench/utils/particle_optimisers.py
--rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.2/ionbench/utils/population_optimisers.py
--rw-rw-rw-   0        0        0     2460 2024-04-05 15:06:52.000000 ionbench-0.4.2/ionbench/utils/scipy_setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.243783 ionbench-0.4.2/ionbench.egg-info/
--rw-rw-rw-   0        0        0     5369 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3565 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-05 15:57:58.000000 ionbench-0.4.2/ionbench.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 15:58:00.269474 ionbench-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     8469 2024-04-05 15:47:35.000000 ionbench-0.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 15:58:00.230158 ionbench-0.4.2/test/
--rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.2/test/test_modifications.py
--rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.2/test/test_multistart.py
--rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.2/test/test_optimisers.py
--rw-rw-rw-   0        0        0    29511 2024-03-28 14:36:40.000000 ionbench-0.4.2/test/test_problems.py
--rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.2/test/test_uncertainty.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.101991 ionbench-0.4.3/
+-rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5369 2024-04-11 17:27:16.038478 ionbench-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.185270 ionbench-0.4.3/ionbench/
+-rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.3/ionbench/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.464520 ionbench-0.4.3/ionbench/benchmarker/
+-rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.3/ionbench/benchmarker/__init__.py
+-rw-rw-rw-   0        0        0    38630 2024-04-11 14:47:04.000000 ionbench-0.4.3/ionbench/benchmarker/benchmarker.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:12.954381 ionbench-0.4.3/ionbench/data/
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.548807 ionbench-0.4.3/ionbench/data/loewe2016/
+-rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
+-rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
+-rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.3/ionbench/data/loewe2016/ikr.csv
+-rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.3/ionbench/data/loewe2016/ikur.csv
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.583124 ionbench-0.4.3/ionbench/data/moreno2016/
+-rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.3/ionbench/data/moreno2016/ina.csv
+-rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.3/ionbench/data/moreno2016/moreno2016.mmt
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.703981 ionbench-0.4.3/ionbench/data/staircase/
+-rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.3/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
+-rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.3/ionbench/data/staircase/dataHH.csv
+-rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.3/ionbench/data/staircase/dataMM.csv
+-rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.3/ionbench/data/staircase/fink-2008-ikr-mm.mmt
+-rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.3/ionbench/data/staircase/staircase-pace.mmt
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.820213 ionbench-0.4.3/ionbench/data/test/
+-rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.3/ionbench/data/test/data.csv
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.896718 ionbench-0.4.3/ionbench/modification/
+-rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.3/ionbench/modification/__init__.py
+-rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.3/ionbench/modification/modification.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:13.937620 ionbench-0.4.3/ionbench/optimisers/
+-rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.3/ionbench/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:14.737033 ionbench-0.4.3/ionbench/optimisers/external_optimisers/
+-rw-rw-rw-   0        0        0     6106 2024-04-11 14:14:58.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
+-rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Bot2012.py
+-rw-rw-rw-   0        0        0     5552 2024-04-11 12:48:07.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
+-rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
+-rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
+-rw-rw-rw-   0        0        0     3223 2024-04-10 19:26:38.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
+-rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
+-rw-rw-rw-   0        0        0    10669 2024-04-11 13:13:49.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
+-rw-rw-rw-   0        0        0     7882 2024-04-11 11:58:47.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
+-rw-rw-rw-   0        0        0     9966 2024-04-11 08:50:28.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
+-rw-rw-rw-   0        0        0     4293 2024-04-10 19:26:06.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
+-rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/__init__.py
+-rw-rw-rw-   0        0        0    16043 2024-04-11 16:06:14.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
+-rw-rw-rw-   0        0        0     9144 2024-04-11 11:58:59.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     7873 2024-04-10 19:44:28.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5543 2024-04-11 13:02:08.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
+-rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
+-rw-rw-rw-   0        0        0     6786 2024-04-10 20:06:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
+-rw-rw-rw-   0        0        0     4531 2024-04-10 20:06:09.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
+-rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
+-rw-rw-rw-   0        0        0     3221 2024-04-05 12:40:19.000000 ionbench-0.4.3/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.218385 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/
+-rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/cmaes_pints.py
+-rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
+-rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/pso_pints.py
+-rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/snes_pints.py
+-rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.3/ionbench/optimisers/pints_optimisers/xnes_pints.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.464508 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/
+-rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     2567 2024-04-10 14:53:34.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
+-rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/lm_scipy.py
+-rw-rw-rw-   0        0        0     2893 2024-04-10 12:52:14.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
+-rw-rw-rw-   0        0        0     2898 2024-04-10 19:25:15.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/powell_scipy.py
+-rw-rw-rw-   0        0        0     2632 2024-04-10 15:40:25.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
+-rw-rw-rw-   0        0        0     1841 2024-04-10 13:20:06.000000 ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.575691 ionbench-0.4.3/ionbench/problems/
+-rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.3/ionbench/problems/__init__.py
+-rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/loewe2016.py
+-rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/moreno2016.py
+-rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.3/ionbench/problems/staircase.py
+-rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.3/ionbench/problems/test.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.610028 ionbench-0.4.3/ionbench/tracker/
+-rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.3/ionbench/tracker/__init__.py
+-rw-rw-rw-   0        0        0    17362 2024-04-10 15:25:47.000000 ionbench-0.4.3/ionbench/tracker/tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.672549 ionbench-0.4.3/ionbench/uncertainty/
+-rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.3/ionbench/uncertainty/__init__.py
+-rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.3/ionbench/uncertainty/fim.py
+-rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.3/ionbench/uncertainty/profile_likelihood.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:15.857985 ionbench-0.4.3/ionbench/utils/
+-rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.3/ionbench/utils/__init__.py
+-rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.3/ionbench/utils/autodiff.py
+-rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.3/ionbench/utils/cache.py
+-rw-rw-rw-   0        0        0     4897 2024-04-05 08:53:05.000000 ionbench-0.4.3/ionbench/utils/classes_pints.py
+-rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.3/ionbench/utils/multistart.py
+-rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.3/ionbench/utils/particle_optimisers.py
+-rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.3/ionbench/utils/population_optimisers.py
+-rw-rw-rw-   0        0        0     2216 2024-04-10 15:35:53.000000 ionbench-0.4.3/ionbench/utils/scipy_setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.026953 ionbench-0.4.3/ionbench.egg-info/
+-rw-rw-rw-   0        0        0     5369 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3565 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 17:27:12.000000 ionbench-0.4.3/ionbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:27:16.140020 ionbench-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     8469 2024-04-11 17:22:24.000000 ionbench-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:27:16.010904 ionbench-0.4.3/test/
+-rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.3/test/test_modifications.py
+-rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.3/test/test_multistart.py
+-rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.3/test/test_optimisers.py
+-rw-rw-rw-   0        0        0    29297 2024-04-11 17:20:14.000000 ionbench-0.4.3/test/test_problems.py
+-rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.3/test/test_uncertainty.py
```

### Comparing `ionbench-0.4.2/LICENSE.txt` & `ionbench-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/PKG-INFO` & `ionbench-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.2
+Version: 0.4.3
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.2/README.md` & `ionbench-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/__init__.py` & `ionbench-0.4.3/ionbench/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/benchmarker/benchmarker.py` & `ionbench-0.4.3/ionbench/benchmarker/benchmarker.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,15 @@
             penalty = self.parameter_penalty(parametersMG) + self.rate_penalty(parametersMG)
             assert penalty.data > 0
             penalty.backward()
             grad = np.zeros(self.n_parameters())
             for i in range(self.n_parameters()):
                 grad[i] = parametersMG[i].grad if parametersMG[i].grad is not None else 0
             cost = float(penalty.data)
-            error = cost * np.array(len(self.DATA))
+            error = cost * np.ones(len(self.DATA))
             J = np.zeros((len(self.DATA), self.n_parameters()))
             for i in range(len(self.DATA)):
                 J[i,] = grad
             self.tracker.update(parameters, incrementSolveCounter=False, solveType='grad', cost=cost,
                                 solveTime=0)
         else:
             # Inside any bounds, so we can get sensitivities
@@ -591,14 +591,21 @@
         except myokit.lib.markov.LinearModelError as e:
             if 'eigenvalues' in str(e):
                 warnings.warn(
                     'Positive eigenvalues found so steady state is unstable. Will use states defined in problem instead.')
                 state = None
             else:
                 raise
+        except np.linalg.LinAlgError as e:
+            if 'infs or NaNs' in str(e):
+                # Infs or NaNs in matrix, caused error in myokit steady state
+                warnings.warn('Infs or NaNs in matrix so steady state is invalid. Will use states defined in problem instead.')
+                state = None
+            else:
+                raise
         if state is not None:
             if np.any(np.array(state) < 0):
                 npstate = np.array(state)
                 if np.all(np.abs(npstate[npstate < 0]) < 1e-12):
                     # If the negative values are very close to zero, then we can assume they are zero
                     state = [max(0, s) / np.sum(npstate) for s in npstate]
                 else:
```

### Comparing `ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt` & `ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt` & `ionbench-0.4.3/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/loewe2016/ikr.csv` & `ionbench-0.4.3/ionbench/data/loewe2016/ikr.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/loewe2016/ikur.csv` & `ionbench-0.4.3/ionbench/data/loewe2016/ikur.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/moreno2016/ina.csv` & `ionbench-0.4.3/ionbench/data/moreno2016/ina.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/moreno2016/moreno2016.mmt` & `ionbench-0.4.3/ionbench/data/moreno2016/moreno2016.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/staircase/beattie-2017-ikr-hh.mmt` & `ionbench-0.4.3/ionbench/data/staircase/beattie-2017-ikr-hh.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/staircase/dataHH.csv` & `ionbench-0.4.3/ionbench/data/staircase/dataHH.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/staircase/dataMM.csv` & `ionbench-0.4.3/ionbench/data/staircase/dataMM.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/staircase/fink-2008-ikr-mm.mmt` & `ionbench-0.4.3/ionbench/data/staircase/fink-2008-ikr-mm.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/data/staircase/staircase-pace.mmt` & `ionbench-0.4.3/ionbench/data/staircase/staircase-pace.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/modification/modification.py` & `ionbench-0.4.3/ionbench/modification/modification.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/DE_Zhou2009.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/DE_Zhou2009.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,22 @@
     def get_L():
         # Get the number of parameters to perturb in crossover
         L = 1
         while np.random.rand() < CR and L < bm.n_parameters():
             L += 1
         return L
 
-    cost_func = ionbench.utils.cache.get_cached_cost(bm)
+    signed_error = ionbench.utils.cache.get_cached_signed_error(bm)
+    grad = ionbench.utils.cache.get_cached_grad(bm, residuals=True)
+
+    def cost_func(x):
+        """
+        Cost function needs to use the signed_error function so that they use the same cache.
+        """
+        return bm.rmse(signed_error(x) + bm.DATA, bm.DATA)
 
     # Ensure popSize is defined
     if popSize is None:
         popSize = 10 * bm.n_parameters()
 
     # Generate initial population
     pop = [None] * popSize
@@ -72,15 +79,15 @@
                 costMean += p.cost / popSize
             print(f'Average cost is {costMean}')
         if gen > 0 and gen % 1000 == 0:
             # Run lm on each point
             if debug:
                 print('Running lm on each point')
             for i in range(popSize):
-                out = scipy.optimize.least_squares(bm.signed_error, pop[i].x, method='lm', diff_step=1e-3, max_nfev=1000)
+                out = scipy.optimize.least_squares(bm.signed_error, pop[i].x, method='lm', jac=grad, max_nfev=1000)
                 pop[i].x = out.x
                 pop[i].cost = out.cost
 
         for i in range(popSize):
             # Find trial point
             if debug:
                 print(f'Working on individual {i}')
@@ -103,15 +110,21 @@
                 if j == n:
                     for k in range(L):
                         trial.x[(j + k) % bm.n_parameters()] = nu[(j + k) % bm.n_parameters()]
             if debug:
                 print(f'Perturbed point after crossover with L {L} and n {n}')
                 print(trial.x)
             # Save best out of trial or pop[i]
-            trial.find_cost()
+            try:
+                trial.find_cost()
+            except Exception as e:
+                print(e)
+                print('Error in trial.find_cost()')
+                print(trial.x)
+                raise e
             if trial.cost < pop[i].cost:
                 if debug:
                     print(f'Point accepted since trail cost is {trial.cost} and ith cost is {pop[i].cost}')
                 pop[i] = trial
 
         if bm.is_converged():
             break
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Bot2012.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Bot2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Cairns2017.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Cairns2017.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# Only works with positive parameters, crossover isn't defined for the possibility of negative parameters
-
+"""
+Describes the genetic algorithm from Cairns et al. 2017.
+This algorithm uses a crossover method which is based on the binary representation of the parameters. It does not work (is not defined for) negative parameters and struggles to identify parameters under 1e-6.
+"""
 import numpy as np
 import ionbench
 import ionbench.utils.population_optimisers as pop_opt
 import copy
 
 
 # noinspection PyShadowingNames
@@ -74,23 +76,27 @@
                 num1 = par1.x[i]
                 num2 = par2.x[i]
                 # Want to convert to integer and maintain 6 decimal places of accuracy
                 num1 = int(np.round(num1 * 1e6))
                 num2 = int(np.round(num2 * 1e6))
                 # Then map to binary string
                 # Find length of binary strings
-                binStrLen = int(np.log2(max(num1, num2))) + 1
-                bin1 = format(num1, '0' + str(binStrLen) + 'b')
-                bin2 = format(num2, '0' + str(binStrLen) + 'b')
-                # Random position between 0 and binStrLen (inclusive)
-                randPos = np.random.randint(0, binStrLen + 1)
-                # Crossover in binary
-                binNew = bin1[:randPos] + bin2[randPos:]
-                # Convert back to decimal float
-                numNew = int(binNew, 2) / 1e6
+                if num1 == num2:
+                    # Don't do crossover as not different, also avoids avoids issue with log2(0)
+                    numNew = num1/1e6
+                else:
+                    binStrLen = int(np.log2(max(num1, num2))) + 1
+                    bin1 = format(num1, '0' + str(binStrLen) + 'b')
+                    bin2 = format(num2, '0' + str(binStrLen) + 'b')
+                    # Random position between 0 and binStrLen (inclusive)
+                    randPos = np.random.randint(0, binStrLen + 1)
+                    # Crossover in binary
+                    binNew = bin1[:randPos] + bin2[randPos:]
+                    # Convert back to decimal float
+                    numNew = int(binNew, 2) / 1e6
                 child.x[i] = numNew
             newPop.append(child)
 
         # Mutation
         for j in range(popSize):
             for i in range(bm.n_parameters()):
                 # Change of mutation is 0.1%
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
-The module provides the PSO followed by TRR algorithm given by Loewe et al. 2016.
-It runs PSO followed by TRR once complete on the best M particles.
+The module provides the hybrid PSO and TRR algorithm given by Loewe et al. 2016.
+It runs TRR on each particle on every PSO iteration.
 The particles are clamped differently to other PSO algorithms.
 No initial position or velocity sampling given, so we assume ionBench defaults.
-The maximum number of TRR iterations to run on the final M particles is undefined, so we do not set a limit.
 """
 import numpy as np
 import scipy
 import ionbench
 
 
 # noinspection PyShadowingNames
-def run(bm, x0=None, n=96, K=5, maxIter=1000, phi1=2.05, phi2=2.05, M=12, debug=False):
+def run(bm, x0=None, n=96, K=5, maxIter=1000, phi1=2.05, phi2=2.05, debug=False):
     """
-    Runs the particle swarm optimisation from Loewe et al. 2016 followed by trust region reflective. If the benchmarker is bounded, the solver will search in the interval [lb,ub], otherwise the solver will search in the interval [0,2*default].
+    Runs the hybrid particle swarm optimisation - trust region reflective algorithm from Loewe et al. 2016. If the benchmarker is bounded, the solver will search in the interval [lb,ub], otherwise the solver will search in the interval [0,2*default].
 
     Notes on using this optimiser:
         It is unclear the specifics of the optimisation used in Loewe et al. 2016. It does not describe the method for sampling the initial positions or velocities of the particles (we use uniform distribution between bounds for position and expect Loewe et al. 2016 did similarly, and zeros for the initial velocities, waiting for them to be set by TRR). The initial velocities may be different to those used in the Loewe et al. 2016, but luckily the algorithm quickly overwrites the velocities after the first iteration based on the movement under TRR, so it is only a difference between randomly sampled points and running TRR (our method) or randomly sampling points, moving them in a random direction and applying the bounds then applying TRR (a method with a non-zero random velocity).
         The TRR method in Loewe et al. 2016 using Matlab's lsqnonlin implementation. As a Python based substitute we have used Scipy. Unfortunately, the Scipy implementation does not allow a maximum number of iterations to be specified. We have specified the maximum number of cost function evaluations (which appears to not include calls to calculate the gradient), which is strictly more than the number of iterations, but still of a comparable size. There may also be differences in how the radius of the trust region is calculated and updated between these two implementations.
 
     Parameters
     ----------
@@ -31,16 +30,14 @@
         Number of function calls allowed in TRR. Note that this uses the function calls reported by scipy, similar in scale to the number of iterations of TRR used in Loewe et al. 2016. This is not the true number of function calls to the benchmarker as this appears to not include finite difference gradient calculations. The default is 5.
     maxIter : int, optional
         Maximum number of iterations. The default is 1000.
     phi1 : float, optional
         Scale of the acceleration towards a particle's best positions. The default is 2.05.
     phi2 : float, optional
         Scale of the acceleration towards the best point seen across all particles. The default is 2.05.
-    M : int, optional
-        The number of particles to run TRR on once PSO has completed. The default is 12.
     debug : bool, optional
         If True, debug information will be printed, reporting that status of the optimisation each generation. The default is False.
 
     Returns
     -------
     xbest : list
         The best parameters identified.
@@ -113,47 +110,51 @@
             p.set_cost()
             if p.currentCost < Gcost[L]:
                 Gcost[L] = p.currentCost
                 Gpos[L] = np.copy(p.position)
 
         # Update velocities
         for p in particleList:
+            old_position = np.copy(p.position)
+
             # Update velocity
             localAcc = phi1 * np.random.rand() * (p.bestPosition - p.position)
             globalAcc = phi2 * np.random.rand() * (Gpos[L] - p.position)
             p.velocity = constFactor * (p.velocity + localAcc + globalAcc)
 
             # Move particle
             p.position += p.velocity
 
             # Clamp
             p.clamp()
 
+            bounds = ionbench.utils.scipy_setup.minimize_bounds(bm)
+            try:
+                out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad, max_nfev=2 * K,
+                                               bounds=bounds, verbose=verbose)
+                p.velocity = p.transform(out.x) - old_position
+                p.position = p.transform(out.x)
+                p.set_cost(bm.rmse(out.fun+bm.DATA, bm.DATA))
+            except ValueError as e:
+                if 'Residuals are not finite' in str(e):
+                    # Reset cost as it may be changed by clamp
+                    p.set_cost()
+                else:
+                    raise e
+
+
         if debug:
             print("Positions renewed")
-            print(f'Finished population: {L}')
+            print(f'Finished population {L}')
             print(f'Best cost so far: {Gcost[L]}')
             print(f'Found at position: {Gpos[L]}')
 
         if bm.is_converged():
             break
 
-    # Iterations of TRR
-    if debug:
-        print("Beginning TRR")
-
-    costs = [p.currentCost for p in particleList]
-    particleList = [p for _, p in sorted(zip(costs, particleList), key=lambda pair: pair[0])]
-    for p in particleList[:M]:
-        bounds = (bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
-        out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
-                                           bounds=bounds, verbose=verbose)
-        p.position = p.transform(out.x)
-        p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
-
     bm.evaluate()
     return Particle().untransform(Gpos[L])
 
 
 # noinspection PyUnusedLocal,PyShadowingNames
 def get_modification(modNum=1):
     """
@@ -169,8 +170,8 @@
     return mod
 
 
 if __name__ == '__main__':
     bm = ionbench.problems.staircase.HH()
     mod = get_modification()
     mod.apply(bm)
-    run(bm, n=20, maxIter=5, debug=True, **mod.kwargs)
+    run(bm, n=5, debug=True, **mod.kwargs)
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/SA_Vanier1999.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/SA_Vanier1999.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     x0 : list, optional
         Initial parameter guess. Population is generated by randomly perturbing this initial guess +-50%, then applying the appropriate bounds. If x0=None (the default), then the population will be sampled uniformly between the bounds.
     tempInitial : float, optional
         Set to 1 in Vanier 1999, but changes with the scale of the cost function/problem. If no value is set, the default, then the cost of x0 is used.
     N : float, optional
         Number of moves per temperature update. Vanier 1999 varies this problem specifically, between 5 and 300. The default is 5.
     maxIter : int, optional
-        Maximum number of iterations. Sets the budget which controls how fast the temperature decreases, smaller maxIter means faster decrease in temperature to ensure temperature approaches 0 (although it will terminate before reaching 0). The default is 1000.
+        Maximum number of iterations. The default is 1000.
     debug : bool, optional
         If True, debug information will be printed, reporting that status of the optimisation each generation. The default is False.
 
     Returns
     -------
     xbest : list
         The best parameters in the final simplex.
@@ -201,15 +201,18 @@
     for i in range(maxIter):
         # Take a modified nelder mead step
         simplex.step()
         # Regenerate the logarithmically distributed noise used in SA modification
         simplex.regen_noise()
         # Annealing schedule
         if i % N == 0:
-            temp = tempInitial * (1 - i / maxIter)  # Proportional decrease in temperature
+            if i < 1000:
+                temp = tempInitial * (1 - i / 1000)  # Proportional decrease in temperature
+            else:
+                temp = 0
 
         for p in simplex.points:
             if p.cost < bestCost:
                 bestCost = p.cost
                 bestPos = np.copy(p.x)
         if debug:
             print(f'Best cost so far is {bestCost}')
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/__init__.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         """
         p = np.zeros(len(x))
         for i in range(len(p)):
             p[i] = lb[i] + (ub[i] - lb[i]) * np.sin(x[i]) ** 2
         return p
 
     signed_error = ionbench.utils.cache.get_cached_signed_error(bm)
+    grad = ionbench.utils.cache.get_cached_grad(bm, returnCost=True, residuals=True)
 
     # sample initial point
     if x0 is None:
         x0 = bm.sample()
     # Transform to fitting space
     x0 = fitting_params(x0)
 
@@ -123,15 +124,15 @@
     bestCost = np.inf  # Best unweighted cost found so far
     wInit = None  # Initial weights
     w = None  # Current weights
     while True:
         # Initialisation routine for every weight update/reset
         falphaOld = np.inf  # Stores the weighted SSE from the previous iteration in curvilinear GD, for termination criteria of curvilinear gradient descent
         # find residuals and jacobian. Residuals will be used to find weights, J will be used in first iteration of curvilinear GD
-        r0, J = bm.grad(model_params(x0), returnCost=True, residuals=True)
+        r0, J = grad(model_params(x0))
         currentCost = np.sqrt(np.mean(r0 ** 2))
         if debug:
             print(f'Starting out optimisation loop. Weight counter {weightCounter}')
 
         # initial weights at the start of optimisation. Only run once.
         if setInitialWeights:
             wInit = 10 / (10 + np.abs(r0))
@@ -186,15 +187,15 @@
         for k in range(maxInnerIter):
             # Update number of curvilinear GD iterations
             iterCounter += 1
             if debug:
                 print(f'Curvilinear GD Iteration: {k} of {maxInnerIter}')
             if k > 0:
                 # If first iteration of GD, r0 and J have already been calculated
-                r0, J = bm.grad(model_params(x0), returnCost=True, residuals=True)
+                r0, J = grad(model_params(x0))
 
             # apply weights to residuals and jacobian
             r0 = np.diag(w) @ r0
             J = np.diag(w) @ J
 
             # transform jacobian into fitting space
             for i in range(bm.n_parameters()):
@@ -238,38 +239,54 @@
 
             # Run Brent's method to optimise SSE with respect to alpha
             try:
                 out = scipy.optimize.brent(SSE, brack=(0, 1, 1e9), tol=1e-8, full_output=True)
                 alpha = out[0]
                 falphaNew = out[1]
             except ValueError as e:
-                # Option 1: SSE(1e9) is smaller than SSE(1)
-                if SSE(1e9) <= SSE(1):
+                # Failed. Time to find out why and try to recover
+                # Option 1: NaNs in either SSE(0) or SSE(1e9) but not SSE(1) so step still viable
+                if (np.isnan(SSE(0)) or np.isnan(SSE(1e9))) and not np.isnan(SSE(1)):
+                    # If SSE(1) is NOT WORSE than SSE(0) or SSE(1e9), then we can assume that it is a good step
+                    if debug:
+                        print(
+                            f'NaNs were found. SSE(0): {SSE(0)}, SSE(1): {SSE(1)}, SSE(1e9): {SSE(1e9)}. Will try to continue if possible')
+                    if not SSE(1) > SSE(0) and not SSE(1) > SSE(1e9):
+                        alpha = 1
+                        falphaNew = SSE(alpha)
+                    else:
+                        print(f'Failed. SSE(0): {SSE(0)}, SSE(1): {SSE(1)}, SSE(1e9): {SSE(1e9)}')
+                        raise e
+                # Option 2: SSE(1e9) is best - take full step
+                elif SSE(1e9) <= SSE(1) and SSE(1e9) <= SSE(0):
+                    # SSE(1e9)<SSE(1),SSE(0)
                     alpha = 1e9
                     falphaNew = SSE(alpha)
                     if debug:
-                        print('Alpha was minimised by taking the full step')
+                        print('Alpha was minimised (at least approximately) by taking the full step')
+                # Option 3: SSE(0) is smallest - start with even smaller step than 1
                 elif SSE(0) <= SSE(1):
-                    # Error when SSE(1) is larger than SSE(0). In this case, it is likely that 1 is just too large a step size, so we probably have SSE(0)<SSE(1)<SSE(1e9). In which case, any tiny step size will be good enough to start brent optimisation
-                    assert SSE(0) <= SSE(1e9)  # This shouldn't be triggered
+                    # SSE(0)<SSE(1),SSE(1e9)
                     if debug:
                         print(
-                            f'SSE(0) {SSE(0)} seems to be smaller than SSE(1) {SSE(1)}, I am going to assume it is also smaller than SSE(1e9) {SSE(1e9)} and that SSE(1e-6) {SSE(1e-6)} is smaller than them all')
+                            f'SSE(0) {SSE(0)} is smaller than SSE(1) {SSE(1)}, trying smaller steps for the initial guesses (1e-6 and 1e-9). If not, will assume converged')
                     if SSE(1e-6) < SSE(0):
                         initStep = 1e-6
                     elif SSE(1e-9) < SSE(0):
                         initStep = 1e-9
                     else:
+                        # The step needed would be too small so assume converged
                         x0 = model_params(x0)
                         bm.evaluate()
                         return x0
                     out = scipy.optimize.brent(SSE, brack=(0, initStep, 1e9), tol=1e-8, full_output=True)
                     alpha = out[0]
                     falphaNew = out[1]
                 else:
+                    print(f'Failed. SSE(0): {SSE(0)}, SSE(1): {SSE(1)}, SSE(1e9): {SSE(1e9)}')
                     raise e
 
             # Take new step
             x0 = x0 + L(alpha)
 
             if debug:
                 print(f'Optimal alpha was {alpha}')
@@ -300,14 +317,17 @@
             print(f'Weight counter incremented to {weightCounter}')
         if iterCounter >= maxIter:
             if debug:
                 print(
                     f'Reached maximum number of iterations so terminating early. iterCounter: {iterCounter}, maxIter: {maxIter}')
             break
 
+        if bm.is_converged():
+            break
+
     x0 = model_params(x0)
     bm.evaluate()
     return x0
 
 
 # noinspection PyShadowingNames
 def get_modification(modNum=1):
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,21 +126,28 @@
 
             # Move particle
             p.position += p.velocity
 
             # Clamp
             p.clamp()
 
-            bounds = (bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
-            out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
-                                               max_nfev=2 * K,
-                                               bounds=bounds, verbose=verbose)
-            p.velocity = p.transform(out.x) - old_position
-            p.position = p.transform(out.x)
-            p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
+            bounds = ionbench.utils.scipy_setup.minimize_bounds(bm)
+            try:
+                out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
+                                                   max_nfev=2 * K,
+                                                   bounds=bounds, verbose=verbose)
+                p.velocity = p.transform(out.x) - old_position
+                p.position = p.transform(out.x)
+                p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
+            except ValueError as e:
+                if 'Residuals are not finite' in str(e):
+                    # Reset cost as it may be changed by clamp
+                    p.set_cost()
+                else:
+                    raise e
 
         if debug:
             print("Positions renewed")
             print(f'Finished population {L}')
             print(f'Best cost so far: {Gcost[L]}')
             print(f'Found at position: {Gpos[L]}')
 
@@ -150,19 +157,28 @@
     # Iterations of TRR
     if debug:
         print("Beginning TRR")
 
     costs = [p.currentCost for p in particleList]
     particleList = [p for _, p in sorted(zip(costs, particleList), key=lambda pair: pair[0])]
     for p in particleList[:M]:
-        bounds = (bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
-        out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
-                                           bounds=bounds, verbose=verbose)
-        p.position = p.transform(out.x)
-        p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
+        bounds = ionbench.utils.scipy_setup.minimize_bounds(bm)
+        try:
+            out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
+                                               bounds=bounds, verbose=verbose)
+            p.position = p.transform(out.x)
+            p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
+        except ValueError as e:
+            if 'Residuals are not finite' in str(e):
+                pass
+            else:
+                raise e
+        if p.currentCost < Gcost[L]:
+            Gcost[L] = p.currentCost
+            Gpos[L] = np.copy(p.position)
 
     bm.evaluate()
     return Particle().untransform(Gpos[L])
 
 
 # noinspection PyUnusedLocal,PyShadowingNames
 def get_modification(modNum=1):
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
-The module provides the hybrid PSO and TRR algorithm given by Loewe et al. 2016.
-It runs TRR on each particle on every PSO iteration.
+The module provides the PSO followed by TRR algorithm given by Loewe et al. 2016.
+It runs PSO followed by TRR once complete on the best M particles.
 The particles are clamped differently to other PSO algorithms.
 No initial position or velocity sampling given, so we assume ionBench defaults.
+The maximum number of TRR iterations to run on the final M particles is undefined, so we do not set a limit.
 """
 import numpy as np
 import scipy
 import ionbench
 
 
 # noinspection PyShadowingNames
-def run(bm, x0=None, n=96, K=5, maxIter=1000, phi1=2.05, phi2=2.05, debug=False):
+def run(bm, x0=None, n=96, maxIter=1000, phi1=2.05, phi2=2.05, M=12, debug=False):
     """
-    Runs the hybrid particle swarm optimisation - trust region reflective algorithm from Loewe et al. 2016. If the benchmarker is bounded, the solver will search in the interval [lb,ub], otherwise the solver will search in the interval [0,2*default].
+    Runs the particle swarm optimisation from Loewe et al. 2016 followed by trust region reflective. If the benchmarker is bounded, the solver will search in the interval [lb,ub], otherwise the solver will search in the interval [0,2*default].
 
     Notes on using this optimiser:
         It is unclear the specifics of the optimisation used in Loewe et al. 2016. It does not describe the method for sampling the initial positions or velocities of the particles (we use uniform distribution between bounds for position and expect Loewe et al. 2016 did similarly, and zeros for the initial velocities, waiting for them to be set by TRR). The initial velocities may be different to those used in the Loewe et al. 2016, but luckily the algorithm quickly overwrites the velocities after the first iteration based on the movement under TRR, so it is only a difference between randomly sampled points and running TRR (our method) or randomly sampling points, moving them in a random direction and applying the bounds then applying TRR (a method with a non-zero random velocity).
         The TRR method in Loewe et al. 2016 using Matlab's lsqnonlin implementation. As a Python based substitute we have used Scipy. Unfortunately, the Scipy implementation does not allow a maximum number of iterations to be specified. We have specified the maximum number of cost function evaluations (which appears to not include calls to calculate the gradient), which is strictly more than the number of iterations, but still of a comparable size. There may also be differences in how the radius of the trust region is calculated and updated between these two implementations.
 
     Parameters
     ----------
     bm : Benchmarker
         A benchmarker to evaluate the performance of the optimisation algorithm.
     x0 : list, optional
         Initial parameter guess. Population is generated by randomly perturbing this initial guess +-50%, then applying the appropriate bounds. If x0=None (the default), then the population will be sampled uniformly between the bounds.
     n : int, optional
         Number of particles. The default is 96.
-    K : int, optional
-        Number of function calls allowed in TRR. Note that this uses the function calls reported by scipy, similar in scale to the number of iterations of TRR used in Loewe et al. 2016. This is not the true number of function calls to the benchmarker as this appears to not include finite difference gradient calculations. The default is 5.
     maxIter : int, optional
         Maximum number of iterations. The default is 1000.
     phi1 : float, optional
         Scale of the acceleration towards a particle's best positions. The default is 2.05.
     phi2 : float, optional
         Scale of the acceleration towards the best point seen across all particles. The default is 2.05.
+    M : int, optional
+        The number of particles to run TRR on once PSO has completed. The default is 12.
     debug : bool, optional
         If True, debug information will be printed, reporting that status of the optimisation each generation. The default is False.
 
     Returns
     -------
     xbest : list
         The best parameters identified.
@@ -110,43 +111,56 @@
             p.set_cost()
             if p.currentCost < Gcost[L]:
                 Gcost[L] = p.currentCost
                 Gpos[L] = np.copy(p.position)
 
         # Update velocities
         for p in particleList:
-            old_position = np.copy(p.position)
-
             # Update velocity
             localAcc = phi1 * np.random.rand() * (p.bestPosition - p.position)
             globalAcc = phi2 * np.random.rand() * (Gpos[L] - p.position)
             p.velocity = constFactor * (p.velocity + localAcc + globalAcc)
 
             # Move particle
             p.position += p.velocity
 
             # Clamp
             p.clamp()
 
-            bounds = (bm.input_parameter_space(bm.lb), bm.input_parameter_space(bm.ub))
-            out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad, max_nfev=2 * K,
-                                               bounds=bounds, verbose=verbose)
-            p.velocity = p.transform(out.x) - old_position
-            p.position = p.transform(out.x)
-            p.set_cost(bm.rmse(out.fun+bm.DATA, bm.DATA))
-
         if debug:
             print("Positions renewed")
-            print(f'Finished population {L}')
+            print(f'Finished population: {L}')
             print(f'Best cost so far: {Gcost[L]}')
             print(f'Found at position: {Gpos[L]}')
 
         if bm.is_converged():
             break
 
+    # Iterations of TRR
+    if debug:
+        print("Beginning TRR")
+
+    costs = [p.currentCost for p in particleList]
+    particleList = [p for _, p in sorted(zip(costs, particleList), key=lambda pair: pair[0])]
+    for p in particleList[:M]:
+        bounds = ionbench.utils.scipy_setup.minimize_bounds(bm)
+        try:
+            out = scipy.optimize.least_squares(signed_error, p.untransform(p.position), method='trf', jac=grad,
+                                               bounds=bounds, verbose=verbose)
+            p.position = p.transform(out.x)
+            p.set_cost(bm.rmse(out.fun + bm.DATA, bm.DATA))
+        except ValueError as e:
+            if 'Residuals are not finite' in str(e):
+                pass
+            else:
+                raise e
+        if p.currentCost < Gcost[L]:
+            Gcost[L] = p.currentCost
+            Gpos[L] = np.copy(p.position)
+
     bm.evaluate()
     return Particle().untransform(Gpos[L])
 
 
 # noinspection PyUnusedLocal,PyShadowingNames
 def get_modification(modNum=1):
     """
@@ -162,8 +176,8 @@
     return mod
 
 
 if __name__ == '__main__':
     bm = ionbench.problems.staircase.HH()
     mod = get_modification()
     mod.apply(bm)
-    run(bm, n=5, debug=True, **mod.kwargs)
+    run(bm, n=20, maxIter=5, debug=True, **mod.kwargs)
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+This module describes the pattern search algorithm from Kohjitani et al. 2022.
+This algorithm is a simple pattern search algorithm that explores neighbouring points around a base point, and moves to the best neighbouring point if an improvement is found.
+The step size is reduced if no improvements are found in the neighbouring points.
+The algorithm terminates when the step size is sufficiently small.
+"""
 import ionbench
 import numpy as np
 
 
 # noinspection PyShadowingNames
 def run(bm, x0=None, maxIter=1000, CrtStp=2e-5, Stp=1 / 100, RedFct=1 / 4, maxfev=20000, debug=False):
     """
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/ppso_Chen2012.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/ppso_Chen2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Cabo2022.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Cabo2022.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,18 @@
             if p.currentCost < Gcost[L]:
                 Gcost[L] = p.currentCost
                 Gpos[L] = np.copy(p.position)
 
         # Renew velocities
         c1 = 1.496
         c2 = 1.496
-        w = 0.7298 - (0.7298-0.3)*L/maxIter
+        if L < 1000:  # Dependence of w on maxIter has been removed
+            w = 0.7298 - (0.7298-0.3)*L/1000
+        else:
+            w = 0.3
         ringPos = best_in_ring(particleList)
         for i, p in enumerate(particleList):
             localAcc = c1 * np.random.rand() * (p.bestPosition - p.position)
             globalAcc = c2 * np.random.rand() * (ringPos[i] - p.position)
             p.velocity = w * p.velocity + localAcc + globalAcc
         if debug:
             print("Velocities renewed")
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/pso_Seemann2009.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/pso_Seemann2009.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,16 +76,19 @@
         for p in particleList:
             p.set_cost()
             if p.currentCost < Gcost[L]:
                 Gcost[L] = p.currentCost
                 Gpos[L] = np.copy(p.position)
 
         # Renew velocities
-        c1 = 0.5 + L / maxIter * 2
-        c2 = 2.5 - c1
+        if L < 1000:  # Dependence of c1 and c2 on maxIter has been removed
+            c1 = 2.5 - L / 1000 * 2
+        else:
+            c1 = 0.5
+        c2 = 3 - c1
         w = np.random.uniform(0.5, 1)
         for p in particleList:
             localAcc = c1 * np.random.rand() * (p.bestPosition - p.position)
             globalAcc = c2 * np.random.rand() * (Gpos[L] - p.position)
             p.velocity = w * p.velocity + localAcc + globalAcc
         if debug:
             print("Velocities renewed")
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py` & `ionbench-0.4.3/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/cmaes_pints.py` & `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/cmaes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/nelderMead_pints.py` & `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/nelderMead_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/pso_pints.py` & `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/pso_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/snes_pints.py` & `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/snes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/pints_optimisers/xnes_pints.py` & `ionbench-0.4.3/ionbench/optimisers/pints_optimisers/xnes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 import ionbench.problems.staircase
 import scipy.optimize
+from ionbench.utils.scipy_setup import minimize_bounds
 
 
 # noinspection PyShadowingNames
-def run(bm, x0=None, gtol=0.001, maxIter=1000, debug=False):
+def run(bm, x0=None, xtol=1e-4, ftol=1e-4, maxIter=1000, maxfev=20000, debug=False):
     """
-    Runs Conjugate Gradient Descent optimiser from Scipy.
+    Runs Nelder-Mead optimiser from Scipy. Bounds are automatically loaded from the benchmarker if present.
 
     Parameters
     ----------
     bm : Benchmarker
         A benchmarker to evaluate the performance of the optimisation algorithm.
     x0 : list, optional
         Initial parameter vector from which to start optimisation. Default is None, in which case a randomly sampled parameter vector is retrieved from bm.sample().
-    gtol : float, optional
-        Tolerance in for the gradient. Gradient norm must be less than gtol before algorithm successfully terminates. The default is 0.001.
+    xtol : float, optional
+        Tolerance in parameters. Used as a termination criterion. The default is 1e-4.
+    ftol : float, optional
+        Tolerance in cost. Used as a termination criterion. The default is 1e-4.
     maxIter : int, optional
-        Maximum number of iterations of Conjugate Gradient Descent to use. The default is 1000.
+        Maximum number of iterations of Nelder-Mead to use. The default is 1000.
+    maxfev : int, optional
+        Maximum number of cost function evaluations. The default is 20000.
     debug : bool, optional
         If True, prints out the cost and parameters found by the algorithm. The default is False.
 
     Returns
     -------
     xbest : list
-        The best parameters identified by Conjugate Gradient Descent.
+        The best parameters identified by Nelder-Mead.
     """
     cost = ionbench.utils.cache.get_cached_cost(bm)
-    grad = ionbench.utils.cache.get_cached_grad(bm)
 
     if x0 is None:
         x0 = bm.sample()
         if debug:
             print('Sampling x0')
             print(x0)
 
-    out = scipy.optimize.minimize(cost, x0, jac=grad, method='CG', options={'disp': debug, 'gtol': gtol, 'maxiter': maxIter})
+    if bm.parametersBounded:
+        bounds = minimize_bounds(bm)
+        out = scipy.optimize.minimize(cost, x0, method='nelder-mead', options={'disp': debug, 'xatol': xtol, 'fatol': ftol, 'maxiter': maxIter, 'maxfev': maxfev}, bounds=bounds)
+    else:
+        out = scipy.optimize.minimize(cost, x0, method='nelder-mead', options={'disp': debug, 'xatol': xtol, 'fatol': ftol, 'maxiter': maxIter, 'maxfev': maxfev})
 
     if debug:
         print(f'Cost of {out.fun} found at:')
         print(out.x)
 
     bm.evaluate()
     return out.x
 
 
 # noinspection PyShadowingNames
 def get_modification(modNum=1):
     """
-    modNum = 1 -> Sachse2003
-    modNum = 2 -> Vanier1999
+    modNum = 1 -> Balser1990
+    modNum = 2 -> Davies2011
+    modNum = 4 -> Moreno2016
 
     Returns
     -------
     mod : modification
-        Modification corresponding to inputted modNum. Default is modNum = 1, so Sachse2003.
+        Modification corresponding to inputted modNum. Default is modNum = 1, so Balser1990.
 
     """
 
     if modNum == 1:
-        mod = ionbench.modification.Sachse2003()
+        mod = ionbench.modification.Balser1990()
     elif modNum == 2:
-        mod = ionbench.modification.Vanier1999()
+        mod = ionbench.modification.Davies2011()
+    elif modNum == 3:
+        mod = ionbench.modification.Moreno2016()
     else:
-        mod = ionbench.modification.Empty(name='conjugateGD_scipy_scipy')
+        mod = ionbench.modification.Empty(name='nelderMead_scipy')
     return mod
 
 
 if __name__ == '__main__':
-    bm = ionbench.problems.staircase.HH(sensitivities=True)
+    bm = ionbench.problems.staircase.HH()
     mod = get_modification()
     mod.apply(bm)
     run(bm, debug=True, **mod.kwargs)
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/lm_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/lm_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/powell_scipy.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,82 +2,82 @@
 import scipy.optimize
 from ionbench.utils.scipy_setup import minimize_bounds
 
 
 # noinspection PyShadowingNames
 def run(bm, x0=None, xtol=1e-4, ftol=1e-4, maxIter=1000, maxfev=20000, debug=False):
     """
-    Runs Nelder-Mead optimiser from Scipy. Bounds are automatically loaded from the benchmarker if present.
+    Runs Powell's Simplex optimiser from Scipy. Bounds are automatically loaded from the benchmarker if present.
 
     Parameters
     ----------
     bm : Benchmarker
         A benchmarker to evaluate the performance of the optimisation algorithm.
     x0 : list, optional
         Initial parameter vector from which to start optimisation. Default is None, in which case a randomly sampled parameter vector is retrieved from bm.sample().
     xtol : float, optional
         Tolerance in parameters. Used as a termination criterion. The default is 1e-4.
     ftol : float, optional
         Tolerance in cost. Used as a termination criterion. The default is 1e-4.
     maxIter : int, optional
-        Maximum number of iterations of Nelder-Mead to use. The default is 1000.
+        Maximum number of iterations of Powell's Simplex to use. The default is 1000.
     maxfev : int, optional
         Maximum number of cost function evaluations. The default is 20000.
     debug : bool, optional
         If True, prints out the cost and parameters found by the algorithm. The default is False.
 
     Returns
     -------
     xbest : list
-        The best parameters identified by Nelder-Mead.
+        The best parameters identified by Powell's Simplex.
     """
     cost = ionbench.utils.cache.get_cached_cost(bm)
 
     if x0 is None:
         x0 = bm.sample()
         if debug:
             print('Sampling x0')
             print(x0)
 
     if bm.parametersBounded:
-        bounds = minimize_bounds(bm, debug)
-        out = scipy.optimize.minimize(cost, x0, method='nelder-mead', options={'disp': debug, 'xatol': xtol, 'fatol': ftol, 'maxiter': maxIter, 'maxfev': maxfev}, bounds=bounds)
+        bounds = minimize_bounds(bm)
+        out = scipy.optimize.minimize(cost, x0, method='powell', options={'disp': debug, 'xtol': xtol, 'ftol': ftol, 'maxiter': maxIter, 'maxfev': maxfev}, bounds=bounds)
     else:
-        out = scipy.optimize.minimize(cost, x0, method='nelder-mead', options={'disp': debug, 'xatol': xtol, 'fatol': ftol, 'maxiter': maxIter, 'maxfev': maxfev})
+        out = scipy.optimize.minimize(cost, x0, method='powell', options={'disp': debug, 'xtol': xtol, 'ftol': ftol, 'maxiter': maxIter, 'maxfev': maxfev})
 
     if debug:
         print(f'Cost of {out.fun} found at:')
         print(out.x)
 
     bm.evaluate()
     return out.x
 
 
 # noinspection PyShadowingNames
 def get_modification(modNum=1):
     """
-    modNum = 1 -> Balser1990
-    modNum = 2 -> Davies2011
-    modNum = 4 -> Moreno2016
+    modNum = 1 -> Sachse2003
+    modNum = 2 -> Seemann2009
+    modNum = 3 -> Wilhelms2012a
 
     Returns
     -------
     mod : modification
-        Modification corresponding to inputted modNum. Default is modNum = 1, so Balser1990.
+        Modification corresponding to inputted modNum. Default is modNum = 1, so Sachse2003.
 
     """
 
     if modNum == 1:
-        mod = ionbench.modification.Balser1990()
+        mod = ionbench.modification.Sachse2003()
     elif modNum == 2:
-        mod = ionbench.modification.Davies2011()
+        mod = ionbench.modification.Seemann2009()
     elif modNum == 3:
-        mod = ionbench.modification.Moreno2016()
+        mod = ionbench.modification.Wilhelms2012a()
     else:
-        mod = ionbench.modification.Empty(name='nelderMead_scipy')
+        mod = ionbench.modification.Empty(name='powell_scipy')
     return mod
 
 
 if __name__ == '__main__':
     bm = ionbench.problems.staircase.HH()
     mod = get_modification()
     mod.apply(bm)
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/powell_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,77 @@
+"""
+This module contains the conjugate gradient descent method implemented using scipy.optimize.minimize.
+It is an unconstrained optimiser and will struggle with the staircase problems due to the discontinuous nature of the cost/penalty function.
+"""
 import ionbench.problems.staircase
 import scipy.optimize
-from ionbench.utils.scipy_setup import minimize_bounds
 
 
 # noinspection PyShadowingNames
-def run(bm, x0=None, xtol=1e-4, ftol=1e-4, maxIter=1000, maxfev=20000, debug=False):
+def run(bm, x0=None, gtol=0.001, maxIter=1000, debug=False):
     """
-    Runs Powell's Simplex optimiser from Scipy. Bounds are automatically loaded from the benchmarker if present.
+    Runs Conjugate Gradient Descent optimiser from Scipy.
 
     Parameters
     ----------
     bm : Benchmarker
         A benchmarker to evaluate the performance of the optimisation algorithm.
     x0 : list, optional
         Initial parameter vector from which to start optimisation. Default is None, in which case a randomly sampled parameter vector is retrieved from bm.sample().
-    xtol : float, optional
-        Tolerance in parameters. Used as a termination criterion. The default is 1e-4.
-    ftol : float, optional
-        Tolerance in cost. Used as a termination criterion. The default is 1e-4.
+    gtol : float, optional
+        Tolerance in for the gradient. Gradient norm must be less than gtol before algorithm successfully terminates. The default is 0.001.
     maxIter : int, optional
-        Maximum number of iterations of Powell's Simplex to use. The default is 1000.
-    maxfev : int, optional
-        Maximum number of cost function evaluations. The default is 20000.
+        Maximum number of iterations of Conjugate Gradient Descent to use. The default is 1000.
     debug : bool, optional
         If True, prints out the cost and parameters found by the algorithm. The default is False.
 
     Returns
     -------
     xbest : list
-        The best parameters identified by Powell's Simplex.
+        The best parameters identified by Conjugate Gradient Descent.
     """
     cost = ionbench.utils.cache.get_cached_cost(bm)
+    grad = ionbench.utils.cache.get_cached_grad(bm)
 
     if x0 is None:
         x0 = bm.sample()
         if debug:
             print('Sampling x0')
             print(x0)
 
-    if bm.parametersBounded:
-        bounds = minimize_bounds(bm, debug)
-        out = scipy.optimize.minimize(cost, x0, method='powell', options={'disp': debug, 'xtol': xtol, 'ftol': ftol, 'maxiter': maxIter, 'maxfev': maxfev}, bounds=bounds)
-    else:
-        out = scipy.optimize.minimize(cost, x0, method='powell', options={'disp': debug, 'xtol': xtol, 'ftol': ftol, 'maxiter': maxIter, 'maxfev': maxfev})
+    out = scipy.optimize.minimize(cost, x0, jac=grad, method='CG', options={'disp': debug, 'gtol': gtol, 'maxiter': maxIter})
 
     if debug:
         print(f'Cost of {out.fun} found at:')
         print(out.x)
 
     bm.evaluate()
     return out.x
 
 
 # noinspection PyShadowingNames
 def get_modification(modNum=1):
     """
     modNum = 1 -> Sachse2003
-    modNum = 2 -> Seemann2009
-    modNum = 3 -> Wilhelms2012a
+    modNum = 2 -> Vanier1999
 
     Returns
     -------
     mod : modification
         Modification corresponding to inputted modNum. Default is modNum = 1, so Sachse2003.
 
     """
 
     if modNum == 1:
         mod = ionbench.modification.Sachse2003()
     elif modNum == 2:
-        mod = ionbench.modification.Seemann2009()
-    elif modNum == 3:
-        mod = ionbench.modification.Wilhelms2012a()
+        mod = ionbench.modification.Vanier1999()
     else:
-        mod = ionbench.modification.Empty(name='powell_scipy')
+        mod = ionbench.modification.Empty(name='conjugateGD_scipy_scipy')
     return mod
 
 
 if __name__ == '__main__':
-    bm = ionbench.problems.staircase.HH()
+    bm = ionbench.problems.staircase.HH(sensitivities=True)
     mod = get_modification()
     mod.apply(bm)
     run(bm, debug=True, **mod.kwargs)
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,20 +28,23 @@
     grad = ionbench.utils.cache.get_cached_grad(bm)
 
     if x0 is None:
         x0 = bm.sample()
         if debug:
             print('Sampling x0')
             print(x0)
-
-    if bm.parametersBounded:
-        bounds = minimize_bounds(bm, debug)
-        out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', options={'disp': debug, 'maxiter': maxIter}, bounds=bounds)
+    if bm.ratesBounded or 'staircase' in bm.NAME:
+        constraints = {'type': 'eq', 'fun': lambda p: bm.parameter_penalty(bm.original_parameter_space(p))+bm.rate_penalty(bm.original_parameter_space(p))}
+    else:
+        constraints = ()
+    if bm.parametersBounded or 'staircase' in bm.NAME:
+        bounds = minimize_bounds(bm)
+        out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', constraints=constraints, options={'disp': debug, 'maxiter': maxIter}, bounds=bounds)
     else:
-        out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', options={'disp': debug, 'maxiter': maxIter})
+        out = scipy.optimize.minimize(cost, x0, jac=grad, method='SLSQP', constraints=constraints, options={'disp': debug, 'maxiter': maxIter})
 
     if debug:
         print(f'Cost of {out.fun} found at:')
         print(out.x)
 
     bm.evaluate()
     return out.x
```

### Comparing `ionbench-0.4.2/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py` & `ionbench-0.4.3/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,15 @@
         If True, prints out the cost and parameters found by the algorithm. The default is False.
 
     Returns
     -------
     xbest : list
         The best parameters identified by Trust Region Reflective.
     """
-    if bm.parametersBounded:
-        bounds = (bm.lb, bm.ub)
-        out = least_squares(bm, x0, debug, method='trf', maxIter=maxIter, bounds=bounds)
-    else:
-        out = least_squares(bm, x0, debug, method='trf', maxIter=maxIter)
+    out = least_squares(bm, x0, debug, method='trf', maxIter=maxIter)
 
     bm.evaluate()
     return out.x
 
 
 # noinspection PyShadowingNames
 def get_modification(modNum=1):
```

### Comparing `ionbench-0.4.2/ionbench/problems/loewe2016.py` & `ionbench-0.4.3/ionbench/problems/loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/problems/moreno2016.py` & `ionbench-0.4.3/ionbench/problems/moreno2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/problems/staircase.py` & `ionbench-0.4.3/ionbench/problems/staircase.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/problems/test.py` & `ionbench-0.4.3/ionbench/problems/test.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/tracker/tracker.py` & `ionbench-0.4.3/ionbench/tracker/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,17 @@
             if solveType == 'cost':
                 self.solveCount += 1
                 self.costTimes.append(solveTime)
             elif solveType == 'grad':
                 self.gradSolveCount += 1
                 self.gradTimes.append(solveTime)
             self.check_repeated_param(estimatedParams, solveType)
-            self.evals.append((estimatedParams, solveType))
+        else:
+            solveType = 'none'
+        self.evals.append((estimatedParams, solveType))
         self.modelSolves.append(self.solveCount)
         self.gradSolves.append(self.gradSolveCount)
         if cost < self.bestCost:
             self.bestParams = estimatedParams
             self.bestCost = cost
         self.bestCosts.append(self.bestCost)
 
@@ -221,18 +223,22 @@
         i = self.when_converged(threshold)
         if i is None:
             print('Convergence reason:              Optimiser terminated early.')
             i = len(self.bestCosts) - 1
         else:
             print('Convergence reason:              ' + ('Cost threshold' if self.cost_threshold(threshold,
                                                                                                 i) else 'Cost unchanged'))
-        print('Cost evaluations at convergence: ' + str(self.modelSolves[i]))
-        print('Grad evaluations at convergence: ' + str(self.gradSolves[i]))
-        print('Best cost at convergence:        {0:.6f}'.format(self.bestCosts[i]))
-        costTime, gradTime = self.total_solve_time(i)
+        print('Cost evaluations at convergence: ' + str(self.modelSolves[i] if len(self.modelSolves) > 0 else None))
+        print('Grad evaluations at convergence: ' + str(self.gradSolves[i] if len(self.gradSolves) > 0 else None))
+        print('Best cost at convergence:        {0:.6f}'.format(self.bestCosts[i] if len(self.bestCosts) > 0 else self.bestCost))
+        if len(self.modelSolves) > 0:
+            costTime, gradTime = self.total_solve_time(i)
+        else:
+            costTime = 0
+            gradTime = 0
         print('Model solve time at convergence: {0:.6f}'.format(costTime))
         print('Grad solve time at convergence:  {0:.6f}'.format(gradTime))
 
     def when_converged(self, threshold):
         """
         Returns the tracking index at convergence, defined using the two termination criteria: cost threshold and cost unchanged. For example, tracker.bestCosts[tracker.when_converged(threshold)] will return the best cost at convergence.
 
@@ -308,15 +314,16 @@
             return (False, None) if returnIndex else False
         fsig = np.inf
         evalsUnchanged = 0
         for i in range(index):
             if np.abs(self.bestCosts[i] - fsig) > 1e-7:
                 evalsUnchanged = 0
                 fsig = self.bestCosts[i]
-            else:
+            elif self.evals[i][-1] != 'none':
+                # Only increment if the model is solved. Not if a penalty function is used.
                 evalsUnchanged += 1
             if evalsUnchanged >= max_unchanged_evals:
                 return (True, i) if returnIndex else True
         return (False, None) if returnIndex else False
 
     def total_solve_time(self, i):
         """
@@ -350,15 +357,16 @@
             Specifies the type of solve that param corresponds to. 'grad' refers to solving with sensitivities and 'cost' refers to one without. The allows check_repeated_params to ignore any cases where the parameters are first solved as a cost and then again as a grad which is common, expected and optimal for line search based gradient descent methods.
 
         Returns
         -------
         None.
 
         """
-        for (p, st) in self.evals:
-            if all(p == param):
-                if st == solveType:
-                    warnings.warn(
-                        f'Duplicate solve. Both as {st}. This means the implementation of this optimiser can to be improved and the number of function evaluations can be reduced.')
-                elif st == 'grad' and solveType == 'cost':
-                    warnings.warn(
-                        f'Duplicate solve. First as {st}, then as {solveType}. Cost can be found for free from a gradient solve. This means the implementation of this optimiser can to be improved and the number of function evaluations can be reduced.')
+        if solveType != 'none':
+            for (p, st) in self.evals:
+                if all(p == param) and st != 'none':
+                    if st == solveType:
+                        warnings.warn(
+                            f'Duplicate solve. Both as {st}. This means the implementation of this optimiser can to be improved and the number of function evaluations can be reduced.')
+                    elif st == 'grad' and solveType == 'cost':
+                        warnings.warn(
+                            f'Duplicate solve. First as {st}, then as {solveType}. Cost can be found for free from a gradient solve. This means the implementation of this optimiser can to be improved and the number of function evaluations can be reduced.')
```

### Comparing `ionbench-0.4.2/ionbench/uncertainty/fim.py` & `ionbench-0.4.3/ionbench/uncertainty/fim.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/uncertainty/profile_likelihood.py` & `ionbench-0.4.3/ionbench/uncertainty/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/autodiff.py` & `ionbench-0.4.3/ionbench/utils/autodiff.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/cache.py` & `ionbench-0.4.3/ionbench/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/classes_pints.py` & `ionbench-0.4.3/ionbench/utils/classes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/multistart.py` & `ionbench-0.4.3/ionbench/utils/multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/particle_optimisers.py` & `ionbench-0.4.3/ionbench/utils/particle_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/population_optimisers.py` & `ionbench-0.4.3/ionbench/utils/population_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/ionbench/utils/scipy_setup.py` & `ionbench-0.4.3/ionbench/utils/scipy_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,49 +35,37 @@
             print('Sampling x0')
             print(x0)
 
     if debug:
         verbose = 2
     else:
         verbose = 1
-
-    out = scipy.optimize.least_squares(signed_error, x0, method=method, jac=grad, verbose=verbose, max_nfev=maxIter,
+    if bm.parametersBounded or 'staircase' in bm.NAME:
+        bounds = minimize_bounds(bm)
+    else:
+        bounds = (-np.inf, np.inf)
+    out = scipy.optimize.least_squares(signed_error, x0, method=method, bounds=bounds, jac=grad, verbose=verbose, max_nfev=maxIter,
                                        **kwargs)
 
     if debug:
         print(f'Cost of {out.cost} found at:')
         print(out.x)
 
     return out
 
 
-def minimize_bounds(bm, debug):
+def minimize_bounds(bm):
     """
     Map the benchmarker bounds to the scipy bounds format.
     Parameters
     ----------
     bm : Benchmarker
         A benchmarker object.
-    debug : bool
-        If True, prints out the bounds before and after mapping.
     Returns
     -------
-    bounds : list
-        A list of tuples containing the lower and upper bounds for each parameter. None indicates no bound.
+    bounds : scipy.optimize.Bounds
+        Scipy bounds object which restricts scipy optimisation to remain inside parameter bounds.
     """
     lb = bm.input_parameter_space(bm.lb)
     ub = bm.input_parameter_space(bm.ub)
-    bounds = []
-    for i in range(bm.n_parameters()):
-        if lb[i] == np.inf:
-            lb[i] = None
-        if ub[i] == np.inf:
-            ub[i] = None
-        bounds.append((lb[i], ub[i]))
-    if debug:
-        print('Bounds transformed')
-        print('Old Bounds:')
-        print(bm.lb)
-        print(bm.ub)
-        print('New bounds')
-        print(bounds)
+    bounds = scipy.optimize.Bounds(lb=lb, ub=ub, keep_feasible=True)
     return bounds
```

### Comparing `ionbench-0.4.2/ionbench.egg-info/PKG-INFO` & `ionbench-0.4.3/ionbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.2
+Version: 0.4.3
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.2/ionbench.egg-info/SOURCES.txt` & `ionbench-0.4.3/ionbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/setup.py` & `ionbench-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name="ionbench",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.2",  # Required
+    version="0.4.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A benchmarking tool for comparing different parameter optimization algorithms for ion channel models",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ionbench-0.4.2/test/test_modifications.py` & `ionbench-0.4.3/test/test_modifications.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/test/test_multistart.py` & `ionbench-0.4.3/test/test_multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/test/test_optimisers.py` & `ionbench-0.4.3/test/test_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.2/test/test_problems.py` & `ionbench-0.4.3/test/test_problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pytest
+import scipy.stats
+
 import ionbench
 import numpy as np
 import matplotlib.pyplot as plt
 import myokit
 
 
 class Problem:
@@ -244,16 +246,15 @@
             self.bm.cost(self.bm._TRUE_PARAMETERS)
 
     @pytest.mark.filterwarnings("ignore:Current:UserWarning")
     def test_grad(self, plotting=False):
         self.bm.reset()
         self.bm.use_sensitivities()
         # Check gradient calculator is accurate
-        a = grad_check(bm=self.bm, x0=self.bm.sample(),
-                       plotting=plotting)  # Within 1% to account for solver noise and finite difference error
+        a = grad_check(bm=self.bm, x0=self.bm.sample(), plotting=plotting)
         assert a < 0.01
         # Same under log transforms
         self.bm.log_transform([True] + [False] * (self.bm.n_parameters() - 1))
         assert grad_check(bm=self.bm, x0=self.bm.sample(), plotting=plotting) < 0.01
         # Same under scale factor and log transforms
         self.bm.useScaleFactors = True
         assert grad_check(bm=self.bm, x0=self.bm.sample(), plotting=plotting) < 0.01
@@ -262,36 +263,33 @@
         assert grad_check(bm=self.bm, x0=self.bm.sample(), plotting=plotting) < 0.01
         # Reset bm
         self.bm.useScaleFactors = False
 
     @pytest.mark.filterwarnings("ignore:Current:UserWarning")
     def test_grad_bounds(self, plotting=False):
         self.bm.reset()
-        mod = ionbench.modification.Modification(parameterBounds='Sampler')
+        mod = ionbench.modification.Modification(parameterBounds='on')
         mod.apply(self.bm)
         self.bm.use_sensitivities()
         x0 = self.bm.sample()
         # Put two parameter outside of bounds
         self.bm.lb[0] = self.bm.ub[0]
         self.bm.lb[2] = self.bm.ub[2]
         # Check gradient calculator is accurate when outside of bounds
-        a = grad_check(bm=self.bm, x0=x0,
-                       plotting=plotting)  # Within 1% to account for solver noise and finite difference error
+        a = grad_check(bm=self.bm, x0=x0, plotting=plotting)
         assert a < 0.01
         # Handles rate bounds as well
         self.bm.add_rate_bounds()
         self.bm.lb = np.copy(self.bm._LOWER_BOUND)
         tmp = self.bm.RATE_MIN
         self.bm.RATE_MIN = self.bm.RATE_MAX
-        a = grad_check(bm=self.bm, x0=x0,
-                       plotting=plotting)  # Within 1% to account for solver noise and finite difference error
+        a = grad_check(bm=self.bm, x0=x0, plotting=plotting)
         assert a < 0.01
         self.bm.useScaleFactors = True
-        a = grad_check(bm=self.bm, x0=self.bm.input_parameter_space(x0),
-                       plotting=plotting)  # Within 1% to account for solver noise and finite difference error
+        a = grad_check(bm=self.bm, x0=self.bm.input_parameter_space(x0), plotting=plotting)
         assert a < 0.01
         self.bm.RATE_MIN = tmp
 
     @pytest.mark.cheap
     def test_steady_state(self):
         self.bm.reset()
         # Test steady state is right for random parameters
@@ -462,15 +460,15 @@
 
 class Loewe(Problem):
     @pytest.mark.cheap
     def test_sampler(self):
         self.bm.reset()
         # Check sampler is inside the right bounds and doesn't just return default rates, across all transforms
         # Get bounds from a modification
-        mod = ionbench.modification.Modification(parameterBounds='Sampler')
+        mod = ionbench.modification.Modification(parameterBounds='on')
         mod.apply(self.bm)
         lb = self.bm.lb
         ub = self.bm.ub
         self.bm.parametersBounded = False
         # Sampler in bounds
         assert sampler_bounds(self.bm, lb, ub)
         # Sampled different to default
@@ -623,27 +621,28 @@
     return all(np.abs(p1 - p2) < 1e-10)
 
 
 def grad_check(bm, x0, plotting=False):
     """
     Test function for checking gradient matches perturbing the cost function
     """
-    if plotting:
-        paramVec = np.linspace(0.999 * x0[0], 1.001 * x0[0], 10)
-    else:
-        paramVec = [0.999 * x0[0], 1.001 * x0[0]]
-    nPoints = len(paramVec)
+    nPoints = 50
+    paramVec = np.linspace(0.999 * x0[0], 1.001 * x0[0], nPoints)
+    if 'staircase' in bm.NAME:
+        bm.sim.set_tolerance(bm._TOLERANCES[0]/100, bm._TOLERANCES[1]/100)  # Use tighter tolerances here to avoid solver noise
     costs = np.zeros(nPoints)
     for i in range(nPoints):
         p = np.copy(x0)
         p[0] = paramVec[i]
         costs[i] = bm.cost(p)
+    if 'staircase' in bm.NAME:
+        bm.sim.set_tolerance(*bm._TOLERANCES)
     grad = bm.grad(x0)
 
     centreCost = bm.cost(x0)
     if plotting:
         plt.plot(paramVec, costs)
         plt.plot(paramVec, centreCost + grad[0] * (paramVec - x0[0]))
         plt.legend(['ODE cost', 'Grad'])
         plt.show()
-    actualGrad = (costs[-1] - costs[0]) / (paramVec[-1] - paramVec[0])
-    return (actualGrad - grad[0]) ** 2 / actualGrad
+    actualGrad, _, _, _, _ = scipy.stats.linregress(paramVec, costs)
+    return (actualGrad - grad[0])**2 / actualGrad
```

### Comparing `ionbench-0.4.2/test/test_uncertainty.py` & `ionbench-0.4.3/test/test_uncertainty.py`

 * *Files identical despite different names*

