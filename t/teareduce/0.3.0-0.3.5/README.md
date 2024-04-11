# Comparing `tmp/teareduce-0.3.0.tar.gz` & `tmp/teareduce-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teareduce-0.3.0.tar", last modified: Mon Apr  8 19:37:29 2024, max compression
+gzip compressed data, was "teareduce-0.3.5.tar", last modified: Thu Apr 11 08:01:38 2024, max compression
```

## Comparing `teareduce-0.3.0.tar` & `teareduce-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.757660 teareduce-0.3.0/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.3.0/LICENSE.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-08 19:37:29.757423 teareduce-0.3.0/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.3.0/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)     1624 2024-01-12 07:48:48.000000 teareduce-0.3.0/pyproject.toml
--rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-04-08 19:37:29.757713 teareduce-0.3.0/setup.cfg
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.748712 teareduce-0.3.0/src/
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.755976 teareduce-0.3.0/src/teareduce/
--rw-r--r--   0 cardiel    (501) staff       (20)      982 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.3.0/src/teareduce/avoid_astropy_warnings.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1685 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/correct_pincushion_distortion.py
--rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.3.0/src/teareduce/cosmicrays.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.3.0/src/teareduce/ctext.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.3.0/src/teareduce/draw_rectangle.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.3.0/src/teareduce/elapsed_time.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.3.0/src/teareduce/imshow.py
--rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.3.0/src/teareduce/peaks_spectrum.py
--rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.3.0/src/teareduce/polfit.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.3.0/src/teareduce/robust_std.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5916 2024-04-08 18:48:08.000000 teareduce-0.3.0/src/teareduce/sdistortion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.3.0/src/teareduce/sliceregion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5426 2024-04-04 14:31:46.000000 teareduce-0.3.0/src/teareduce/statsummary.py
--rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-04-08 19:29:51.000000 teareduce-0.3.0/src/teareduce/version.py
--rw-r--r--   0 cardiel    (501) staff       (20)    68706 2024-04-04 14:24:28.000000 teareduce-0.3.0/src/teareduce/wavecal.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.3.0/src/teareduce/zscale.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-08 19:37:29.757123 teareduce-0.3.0/src/teareduce.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      715 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       77 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-04-08 19:37:29.000000 teareduce-0.3.0/src/teareduce.egg-info/top_level.txt
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-11 08:01:38.999846 teareduce-0.3.5/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.3.5/LICENSE.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     2302 2024-04-11 08:01:38.999648 teareduce-0.3.5/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.3.5/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)     1646 2024-04-11 06:52:28.000000 teareduce-0.3.5/pyproject.toml
+-rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-04-11 08:01:38.999889 teareduce-0.3.5/setup.cfg
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-11 08:01:38.992489 teareduce-0.3.5/src/
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-11 08:01:38.998491 teareduce-0.3.5/src/teareduce/
+-rw-r--r--   0 cardiel    (501) staff       (20)     1034 2024-04-11 06:50:31.000000 teareduce-0.3.5/src/teareduce/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.3.5/src/teareduce/avoid_astropy_warnings.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1685 2024-04-08 19:29:51.000000 teareduce-0.3.5/src/teareduce/correct_pincushion_distortion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.3.5/src/teareduce/cosmicrays.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.3.5/src/teareduce/ctext.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.3.5/src/teareduce/draw_rectangle.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.3.5/src/teareduce/elapsed_time.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.3.5/src/teareduce/imshow.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     8049 2024-04-11 06:49:24.000000 teareduce-0.3.5/src/teareduce/numsplines.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.3.5/src/teareduce/peaks_spectrum.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.3.5/src/teareduce/polfit.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.3.5/src/teareduce/robust_std.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5916 2024-04-08 18:48:08.000000 teareduce-0.3.5/src/teareduce/sdistortion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.3.5/src/teareduce/sliceregion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5426 2024-04-04 14:31:46.000000 teareduce-0.3.5/src/teareduce/statsummary.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-04-11 06:50:31.000000 teareduce-0.3.5/src/teareduce/version.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    68706 2024-04-04 14:24:28.000000 teareduce-0.3.5/src/teareduce/wavecal.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.3.5/src/teareduce/zscale.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-11 08:01:38.999364 teareduce-0.3.5/src/teareduce.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)     2302 2024-04-11 08:01:38.000000 teareduce-0.3.5/src/teareduce.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      743 2024-04-11 08:01:38.000000 teareduce-0.3.5/src/teareduce.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-11 08:01:38.000000 teareduce-0.3.5/src/teareduce.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       83 2024-04-11 08:01:38.000000 teareduce-0.3.5/src/teareduce.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-04-11 08:01:38.000000 teareduce-0.3.5/src/teareduce.egg-info/top_level.txt
```

### Comparing `teareduce-0.3.0/LICENSE.txt` & `teareduce-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/PKG-INFO` & `teareduce-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.3.0
+Version: 0.3.5
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: astropy
 Requires-Dist: importlib_resources
+Requires-Dist: lmfit
 Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `teareduce-0.3.0/README.md` & `teareduce-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/pyproject.toml` & `teareduce-0.3.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 # (include packages imported in the different modules; otherwise
 # a ModuleNotFoundError is raised when using $ pip install -e .)
 requires = ["setuptools >= 43.0.0", "wheel", "numpy",
-            "astropy", "matplotlib", "scipy", "tqdm"]
+            "astropy", "matplotlib", "scipy", "lmfit", "tqdm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "teareduce"
 dynamic = ["version"]
 description = "Utilities for astronomical data reduction"
 readme = "README.md"
@@ -29,14 +29,15 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 
 dependencies = [
     "astropy",
     "importlib_resources",  # required with python < 3.9
+    "lmfit",
     "matplotlib",
     "numpy >= 1.20",
     "scipy",
     "tqdm",
 ]
 
 [project.optional-dependencies]
```

### Comparing `teareduce-0.3.0/src/teareduce/__init__.py` & `teareduce-0.3.5/src/teareduce/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .avoid_astropy_warnings import avoid_astropy_warnings
 from .correct_pincushion_distortion import correct_pincushion_distortion
 from .cosmicrays import cr2images, apply_cr2images_ccddata, crmedian
 from .ctext import ctext
 from .draw_rectangle import draw_rectangle
 from .elapsed_time import elapsed_time
 from .imshow import imshow
+from .numsplines import AdaptiveLSQUnivariateSpline
 from .peaks_spectrum import find_peaks_spectrum, refine_peaks_spectrum
 from .polfit import polfit_residuals, polfit_residuals_with_sigma_rejection
 from .robust_std import robust_std
 from .sdistortion import fit_sdistortion
 from .sliceregion import SliceRegion1D, SliceRegion2D
 from .statsummary import ifc_statsummary, statsummary
 from .version import version
```

### Comparing `teareduce-0.3.0/src/teareduce/avoid_astropy_warnings.py` & `teareduce-0.3.5/src/teareduce/avoid_astropy_warnings.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/correct_pincushion_distortion.py` & `teareduce-0.3.5/src/teareduce/correct_pincushion_distortion.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/cosmicrays.py` & `teareduce-0.3.5/src/teareduce/cosmicrays.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/ctext.py` & `teareduce-0.3.5/src/teareduce/ctext.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/draw_rectangle.py` & `teareduce-0.3.5/src/teareduce/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/elapsed_time.py` & `teareduce-0.3.5/src/teareduce/elapsed_time.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/imshow.py` & `teareduce-0.3.5/src/teareduce/imshow.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/peaks_spectrum.py` & `teareduce-0.3.5/src/teareduce/peaks_spectrum.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/polfit.py` & `teareduce-0.3.5/src/teareduce/polfit.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/robust_std.py` & `teareduce-0.3.5/src/teareduce/robust_std.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/sdistortion.py` & `teareduce-0.3.5/src/teareduce/sdistortion.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/sliceregion.py` & `teareduce-0.3.5/src/teareduce/sliceregion.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/statsummary.py` & `teareduce-0.3.5/src/teareduce/statsummary.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/wavecal.py` & `teareduce-0.3.5/src/teareduce/wavecal.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce/zscale.py` & `teareduce-0.3.5/src/teareduce/zscale.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.3.0/src/teareduce.egg-info/PKG-INFO` & `teareduce-0.3.5/src/teareduce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.3.0
+Version: 0.3.5
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,14 +18,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: astropy
 Requires-Dist: importlib_resources
+Requires-Dist: lmfit
 Requires-Dist: matplotlib
 Requires-Dist: numpy>=1.20
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `teareduce-0.3.0/src/teareduce.egg-info/SOURCES.txt` & `teareduce-0.3.5/src/teareduce.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/teareduce/avoid_astropy_warnings.py
 src/teareduce/correct_pincushion_distortion.py
 src/teareduce/cosmicrays.py
 src/teareduce/ctext.py
 src/teareduce/draw_rectangle.py
 src/teareduce/elapsed_time.py
 src/teareduce/imshow.py
+src/teareduce/numsplines.py
 src/teareduce/peaks_spectrum.py
 src/teareduce/polfit.py
 src/teareduce/robust_std.py
 src/teareduce/sdistortion.py
 src/teareduce/sliceregion.py
 src/teareduce/statsummary.py
 src/teareduce/version.py
```

