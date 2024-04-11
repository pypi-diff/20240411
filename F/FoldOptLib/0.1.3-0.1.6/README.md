# Comparing `tmp/FoldOptLib-0.1.3.tar.gz` & `tmp/FoldOptLib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoldOptLib-0.1.3.tar", last modified: Wed Mar 27 02:33:14 2024, max compression
+gzip compressed data, was "FoldOptLib-0.1.6.tar", last modified: Thu Apr 11 00:54:48 2024, max compression
```

## Comparing `FoldOptLib-0.1.3.tar` & `FoldOptLib-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.367012 FoldOptLib-0.1.3/FoldOptLib/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/examples/misc_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/fold_modelling/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/fold_modelling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/fold_modelling/base_fold_frame_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/fold_modelling/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/fold_modelling/simple_fold_frame_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_fold.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_fold_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_svariogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/helper/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/helper/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/input/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/input/input_data_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/input/input_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib/ipywidgets_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/ipywidgets_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/ipywidgets_interface/knowledge_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/FoldOptLib/objective_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/axial_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/geological_knowledge.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/lambda_objective_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/least_squares.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/objective_functions/von_mises_fisher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/FoldOptLib/optimisers/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/optimisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/optimisers/axial_surface_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/optimisers/base_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/optimisers/fold_optimiser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/optimisers/fourier_optimiser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/FoldOptLib/splot/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/splot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/splot/splot_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/FoldOptLib/visualisation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/FoldOptLib/visualisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 02:33:14.371012 FoldOptLib-0.1.3/FoldOptLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 02:33:14.000000 FoldOptLib-0.1.3/FoldOptLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-27 02:33:14.000000 FoldOptLib-0.1.3/FoldOptLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 02:33:14.000000 FoldOptLib-0.1.3/FoldOptLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-27 02:33:14.000000 FoldOptLib-0.1.3/FoldOptLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-27 02:33:14.000000 FoldOptLib-0.1.3/FoldOptLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 02:33:14.375012 FoldOptLib-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-27 02:33:13.000000 FoldOptLib-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.530541 FoldOptLib-0.1.6/FoldOptLib/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.530541 FoldOptLib-0.1.6/FoldOptLib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/examples/misc_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.534541 FoldOptLib-0.1.6/FoldOptLib/fold_modelling/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/fold_modelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/fold_modelling/base_fold_frame_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/fold_modelling/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/fold_modelling/simple_fold_frame_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.534541 FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_fold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_fold_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_svariogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.534541 FoldOptLib-0.1.6/FoldOptLib/helper/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/helper/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.534541 FoldOptLib-0.1.6/FoldOptLib/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/input/input_data_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/input/input_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.534541 FoldOptLib-0.1.6/FoldOptLib/ipywidgets_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/ipywidgets_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/ipywidgets_interface/knowledge_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/FoldOptLib/objective_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/axial_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/geological_knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/lambda_objective_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/objective_functions/von_mises_fisher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/FoldOptLib/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/optimisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13956 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/optimisers/axial_surface_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/optimisers/base_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/optimisers/fold_optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/optimisers/fourier_optimiser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/FoldOptLib/splot/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/splot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/splot/splot_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/FoldOptLib/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/FoldOptLib/visualisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/FoldOptLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 00:54:48.000000 FoldOptLib-0.1.6/FoldOptLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-11 00:54:48.000000 FoldOptLib-0.1.6/FoldOptLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:54:48.000000 FoldOptLib-0.1.6/FoldOptLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 00:54:48.000000 FoldOptLib-0.1.6/FoldOptLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 00:54:48.000000 FoldOptLib-0.1.6/FoldOptLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:54:48.538541 FoldOptLib-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-11 00:54:36.000000 FoldOptLib-0.1.6/setup.py
```

### Comparing `FoldOptLib-0.1.3/FoldOptLib/__init__.py` & `FoldOptLib-0.1.6/FoldOptLib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # from .fold_modelling import FoldModel, BaseFoldFrameBuilder
-from .helper import _helper, utils
+from .helper import utils
 from .input import CheckInputData, InputDataProcessor
 from .objective_functions import GeologicalKnowledgeFunctions, VonMisesFisher, LeastSquaresFunctions, \
     loglikelihood_fourier_series, loglikelihood_axial_surface, gaussian_log_likelihood, loglikelihood, \
     is_axial_plane_compatible
 from .optimisers import FourierSeriesOptimiser, AxialSurfaceOptimiser
 from .splot import SPlotProcessor
 from .ipywidgets_interface import create_value_widgets, on_add_button_click, on_constraint_change, \
```

### Comparing `FoldOptLib-0.1.3/FoldOptLib/examples/misc_functions.py` & `FoldOptLib-0.1.6/FoldOptLib/examples/misc_functions.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/fold_modelling/base_fold_frame_builder.py` & `FoldOptLib-0.1.6/FoldOptLib/fold_modelling/base_fold_frame_builder.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/fold_modelling/engine.py` & `FoldOptLib-0.1.6/FoldOptLib/fold_modelling/engine.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_fold.py` & `FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_fold.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_fold_frame.py` & `FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_fold_frame.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/from_loopstructural/_svariogram.py` & `FoldOptLib-0.1.6/FoldOptLib/from_loopstructural/_svariogram.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/helper/_helper.py` & `FoldOptLib-0.1.6/FoldOptLib/helper/_helper.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/helper/utils.py` & `FoldOptLib-0.1.6/FoldOptLib/helper/utils.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/input/input_data_checker.py` & `FoldOptLib-0.1.6/FoldOptLib/input/input_data_checker.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/input/input_data_processor.py` & `FoldOptLib-0.1.6/FoldOptLib/input/input_data_processor.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/ipywidgets_interface/knowledge_input.py` & `FoldOptLib-0.1.6/FoldOptLib/ipywidgets_interface/knowledge_input.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/axial_plane.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/axial_plane.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/gaussian.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/gaussian.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/geological_knowledge.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/geological_knowledge.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/lambda_objective_function.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/lambda_objective_function.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/least_squares.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/least_squares.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/objective_functions/von_mises_fisher.py` & `FoldOptLib-0.1.6/FoldOptLib/objective_functions/von_mises_fisher.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/optimisers/axial_surface_optimiser.py` & `FoldOptLib-0.1.6/FoldOptLib/optimisers/axial_surface_optimiser.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/optimisers/base_optimiser.py` & `FoldOptLib-0.1.6/FoldOptLib/optimisers/base_optimiser.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/optimisers/fold_optimiser.py` & `FoldOptLib-0.1.6/FoldOptLib/optimisers/fold_optimiser.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/optimisers/fourier_optimiser.py` & `FoldOptLib-0.1.6/FoldOptLib/optimisers/fourier_optimiser.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib/splot/splot_processor.py` & `FoldOptLib-0.1.6/FoldOptLib/splot/splot_processor.py`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/FoldOptLib.egg-info/PKG-INFO` & `FoldOptLib-0.1.6/FoldOptLib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: FoldOptLib
-Version: 0.1.3
+Version: 0.1.6
 Summary: Open source Fold Geometry Optimisers for LoopStructural and Map2Loop
 Home-page: https://github.com/Loop3D/FoldOptLib
 Author: Rabii Chaarani
 Author-email: rabii.chaarani@monash.edu
 License: MIT
 Keywords: earth sciences,geology,3-D modelling,structural geology,uncertainty,fold geometry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 License-File: LICENSE
+Requires-Dist: loopstructural>=1.4.10
+Requires-Dist: ipywidgets
+Requires-Dist: mplstereonet
+Requires-Dist: scipy>=1.11.3
 
 # FoldOptLib - Fold Geometry Optimisation Library
 
 ## Installation 
 to install the library, run the following command:  
-``` pip install foldoptlib```   
-
-
+``` pip install foldoptlib```   or 
+``` conda install -c conda-forge foldoptlib```
```

### Comparing `FoldOptLib-0.1.3/FoldOptLib.egg-info/SOURCES.txt` & `FoldOptLib-0.1.6/FoldOptLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/LICENSE` & `FoldOptLib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FoldOptLib-0.1.3/PKG-INFO` & `FoldOptLib-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: FoldOptLib
-Version: 0.1.3
+Version: 0.1.6
 Summary: Open source Fold Geometry Optimisers for LoopStructural and Map2Loop
 Home-page: https://github.com/Loop3D/FoldOptLib
 Author: Rabii Chaarani
 Author-email: rabii.chaarani@monash.edu
 License: MIT
 Keywords: earth sciences,geology,3-D modelling,structural geology,uncertainty,fold geometry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 License-File: LICENSE
+Requires-Dist: loopstructural>=1.4.10
+Requires-Dist: ipywidgets
+Requires-Dist: mplstereonet
+Requires-Dist: scipy>=1.11.3
 
 # FoldOptLib - Fold Geometry Optimisation Library
 
 ## Installation 
 to install the library, run the following command:  
-``` pip install foldoptlib```   
-
-
+``` pip install foldoptlib```   or 
+``` conda install -c conda-forge foldoptlib```
```

### Comparing `FoldOptLib-0.1.3/setup.py` & `FoldOptLib-0.1.6/setup.py`

 * *Files identical despite different names*

