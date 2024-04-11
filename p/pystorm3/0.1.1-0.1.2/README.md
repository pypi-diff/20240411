# Comparing `tmp/pystorm3-0.1.1.tar.gz` & `tmp/pystorm3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.1.tar", last modified: Thu Apr 11 12:26:43 2024, max compression
+gzip compressed data, was "pystorm3-0.1.2.tar", last modified: Thu Apr 11 12:33:35 2024, max compression
```

## Comparing `pystorm3-0.1.1.tar` & `pystorm3-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.776595 pystorm3-0.1.1/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.1/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:26:43.775595 pystorm3-0.1.1/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-10 16:21:02.000000 pystorm3-0.1.1/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.1/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/signal_processing/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.1/pystorm/signal_processing/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     4742 2024-04-11 12:21:03.000000 pystorm3-0.1.1/pystorm/signal_processing/band_filter.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.1/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2647 2024-04-11 12:22:38.000000 pystorm3-0.1.1/pystorm/timefreq/hilbert.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2377 2024-04-10 16:09:04.000000 pystorm3-0.1.1/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       51 2024-04-10 16:00:40.000000 pystorm3-0.1.1/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    29490 2024-04-11 12:24:01.000000 pystorm3-0.1.1/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)      716 2024-04-11 12:18:49.000000 pystorm3-0.1.1/pystorm/utils/type_safety.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 11:50:54.000000 pystorm3-0.1.1/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      472 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 12:26:43.776595 pystorm3-0.1.1/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.1/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.048623 pystorm3-0.1.2/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.2/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:33:35.047623 pystorm3-0.1.2/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-11 12:31:09.000000 pystorm3-0.1.2/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.2/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.2/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4742 2024-04-11 12:21:03.000000 pystorm3-0.1.2/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.2/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2647 2024-04-11 12:22:38.000000 pystorm3-0.1.2/pystorm/timefreq/hilbert.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2377 2024-04-10 16:09:04.000000 pystorm3-0.1.2/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       51 2024-04-10 16:00:40.000000 pystorm3-0.1.2/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    29490 2024-04-11 12:24:01.000000 pystorm3-0.1.2/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      716 2024-04-11 12:18:49.000000 pystorm3-0.1.2/pystorm/utils/type_safety.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 12:33:30.000000 pystorm3-0.1.2/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:33:35.047623 pystorm3-0.1.2/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      472 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 12:33:35.000000 pystorm3-0.1.2/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 12:33:35.048623 pystorm3-0.1.2/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.2/setup.py
```

### Comparing `pystorm3-0.1.1/LICENSE` & `pystorm3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/PKG-INFO` & `pystorm3-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
@@ -40,17 +40,17 @@
 
 `pip install pystorm3`.
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
-
-### Coming soon
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+
+### Coming soon
 - Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.1/README.md` & `pystorm3-0.1.2/README.md`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 `pip install pystorm3`.
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
-
-### Coming soon
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+
+### Coming soon
 - Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.1/pystorm/signal_processing/band_filter.py` & `pystorm3-0.1.2/pystorm/signal_processing/band_filter.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/pystorm/timefreq/hilbert.py` & `pystorm3-0.1.2/pystorm/timefreq/hilbert.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/pystorm/timefreq/welch_psd.py` & `pystorm3-0.1.2/pystorm/timefreq/welch_psd.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/pystorm/utils/minitorch.py` & `pystorm3-0.1.2/pystorm/utils/minitorch.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/pystorm/utils/type_safety.py` & `pystorm3-0.1.2/pystorm/utils/type_safety.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.1/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.2/pystorm3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
@@ -40,17 +40,17 @@
 
 `pip install pystorm3`.
 
 ## Pystorm functions
 
 ### Currently implemented
 - Power spectral density estimation ([PSD Welch method](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/timefreq/bst_psd.m), physical units only) in source and sensor space (can operate on GPU)
-
-### Coming soon
 - Band-pass filtering (equivalent to ["bst-hfilter-2019"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/math/bst_bandpass_hfilter.m))
 - Hilbert transform
+
+### Coming soon
 - Amplitude envelope correlation (equivalent to ["penv" and "oenv"](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/connectivity/bst_henv.m))
 - Sign flip for parcellated source signal
 - [tPAC](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic.m) (time-resolved Phase-Amplitude Coupling) with [surrogate data z-score](https://github.com/brainstorm-tools/brainstorm3/blob/master/toolbox/process/functions/process_pac_dynamic_sur2.m)
 
 ### Currently not implemented
 - Handling of unconstrained sources
```

### Comparing `pystorm3-0.1.1/setup.py` & `pystorm3-0.1.2/setup.py`

 * *Files identical despite different names*

