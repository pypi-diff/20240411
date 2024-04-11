# Comparing `tmp/treat2p-0.0.3.tar.gz` & `tmp/treat2p-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treat2p-0.0.3.tar", last modified: Mon Apr  8 17:56:35 2024, max compression
+gzip compressed data, was "treat2p-0.0.4.tar", last modified: Thu Apr 11 10:25:05 2024, max compression
```

## Comparing `treat2p-0.0.3.tar` & `treat2p-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      845 2024-04-08 17:56:35.377806 treat2p-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1280 2024-04-08 17:56:25.000000 treat2p-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 17:56:35.377806 treat2p-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-08 17:56:25.000000 treat2p-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/treat2p/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17525 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/calculations.py
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     4905 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/normalisation.py
--rw-rw-rw-   0 root         (0) root         (0)    13631 2024-04-08 17:56:25.000000 treat2p-0.0.3/treat2p/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 17:56:35.377806 treat2p-0.0.3/treat2p.egg-info/
--rw-r--r--   0 root         (0) root         (0)      845 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-08 17:56:35.000000 treat2p-0.0.3/treat2p.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-11 10:25:05.810577 treat2p-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1280 2024-04-11 10:24:56.000000 treat2p-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 10:25:05.814577 treat2p-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-11 10:24:56.000000 treat2p-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/treat2p/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17760 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/calculations.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     4905 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/normalisation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13631 2024-04-11 10:24:56.000000 treat2p-0.0.4/treat2p/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 10:25:05.810577 treat2p-0.0.4/treat2p.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      845 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 10:25:05.000000 treat2p-0.0.4/treat2p.egg-info/top_level.txt
```

### Comparing `treat2p-0.0.3/PKG-INFO` & `treat2p-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.3
+Version: 0.0.4
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `treat2p-0.0.3/README.md` & `treat2p-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/setup.py` & `treat2p-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/treat2p/calculations.py` & `treat2p-0.0.4/treat2p/calculations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 def estimate_slow_trend(
     F,
     *,
     window=120,
     slow_trend_percentile=10,
     fps=30,
     step=10,
+    fit=False,
+    polyfit_order=2,
     filter_savgol=True,
     filter_lowpass=False,
     filter_percentiles=True,
     savgol_window_length=50,
     savgol_polyorder=2,
     lowpass_order=3,
     lowpass_fcut=0.001,  # in Hz
@@ -74,14 +76,20 @@
             padlen=None,
             padtype="odd",
             method=lowpass_method,
             irlen=None,
             axis=0,
         )
 
+    if fit:
+        if fit == "poly":
+            span = np.arange(0, len(slow_trend))
+            poly = np.polyfit(span, slow_trend, polyfit_order)
+            slow_trend = np.polyval(poly, span)
+
     return np.asarray(slow_trend)[0 : len(F)]
 
 
 @filter_save_kwargs("F_Cell", "F_Neu")
 def neuropil_factor_ARDSIP(
     F_Cell,
     F_Neu,
```

### Comparing `treat2p-0.0.3/treat2p/core.py` & `treat2p-0.0.4/treat2p/core.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/treat2p/corrections.py` & `treat2p-0.0.4/treat2p/corrections.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/treat2p/normalisation.py` & `treat2p-0.0.4/treat2p/normalisation.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/treat2p/utils.py` & `treat2p-0.0.4/treat2p/utils.py`

 * *Files identical despite different names*

### Comparing `treat2p-0.0.3/treat2p.egg-info/PKG-INFO` & `treat2p-0.0.4/treat2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treat2p
-Version: 0.0.3
+Version: 0.0.4
 Summary: Projects specific python code pipeline for analysis
 Home-page: https://gitlab.pasteur.fr/haisslab/analysis-packages/treat2p
 Author: Timothé Jost-MOUSSEAU
 Author-email: timothe.jost-mousseau@pasteur.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

