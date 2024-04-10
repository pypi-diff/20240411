# Comparing `tmp/od-metrics-1.0.0.tar.gz` & `tmp/od-metrics-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "od-metrics-1.0.0.tar", last modified: Mon Apr  1 21:50:04 2024, max compression
+gzip compressed data, was "od-metrics-1.0.1.tar", last modified: Wed Apr 10 22:05:53 2024, max compression
```

## Comparing `od-metrics-1.0.0.tar` & `od-metrics-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-01 21:49:53.000000 od-metrics-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4343 2024-04-01 21:50:04.769223 od-metrics-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-01 21:49:53.000000 od-metrics-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-01 21:49:53.000000 od-metrics-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      781 2024-04-01 21:50:04.769223 od-metrics-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-01 21:49:53.000000 od-metrics-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.765223 od-metrics-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.765223 od-metrics-1.0.0/src/od_metrics/
--rw-r--r--   0 root         (0) root         (0)      111 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2199 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/constants.py
--rw-r--r--   0 root         (0) root         (0)    46890 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/od_metrics.py
--rw-r--r--   0 root         (0) root         (0)     4268 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/utils.py
--rw-r--r--   0 root         (0) root         (0)    23209 2024-04-01 21:49:53.000000 od-metrics-1.0.0/src/od_metrics/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/src/od_metrics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4343 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-01 21:50:04.000000 od-metrics-1.0.0/src/od_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 21:50:04.769223 od-metrics-1.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)    12219 2024-04-01 21:49:53.000000 od-metrics-1.0.0/tests/test_pycoco_equivalence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-10 22:05:42.000000 od-metrics-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-04-10 22:05:53.452681 od-metrics-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4873 2024-04-10 22:05:42.000000 od-metrics-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-10 22:05:42.000000 od-metrics-1.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      781 2024-04-10 22:05:53.452681 od-metrics-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-10 22:05:42.000000 od-metrics-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.448681 od-metrics-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.448681 od-metrics-1.0.1/src/od_metrics/
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/constants.py
+-rw-r--r--   0 root         (0) root         (0)    46880 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/od_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/utils.py
+-rw-r--r--   0 root         (0) root         (0)    23245 2024-04-10 22:05:42.000000 od-metrics-1.0.1/src/od_metrics/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/src/od_metrics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 22:05:53.000000 od-metrics-1.0.1/src/od_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:05:53.452681 od-metrics-1.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)    12838 2024-04-10 22:05:42.000000 od-metrics-1.0.1/tests/test_odmetrics.py
```

### Comparing `od-metrics-1.0.0/LICENSE` & `od-metrics-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.0/PKG-INFO` & `od-metrics-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-metrics
-Version: 1.0.0
+Version: 1.0.1
 Summary: Object Detection metrics.
 Home-page: https://github.com/EMalagoli92/OD-metrics
 Author: EMalagoli92
 Author-email: emala.892@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,60 +13,75 @@
 License-File: LICENSE
 Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0
 Requires-Dist: pydantic==2.5.2
 
 <div align="center">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
-  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_dark.svg">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
+  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
+  <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
+    <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <br>
+  <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
-    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License: MIT">
-  </a>
+    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
+  <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
+    <img src="https://mybinder.org/badge_logo.svg"></a>
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
 </p>
 
 <p align="center">
   <strong>
-    A metrics package for Object Detection.
+    A python library for Object Detection metrics.
   </strong>
 </p>
 
-## Supported Metrics
-Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
-and Intersection over Union `IoU`.
-
 
 ## Why OD-Metrics?
 - **User-friendly**: simple to set and simple to use;
 - **Highly Customizable**: every parameters that occur in the definition of `mAP`
 and `mAR` can be set by user to custom values;
 - **Compatibility with [COCOAPI](https://github.com/cocodataset/cocoapi)**: each
 calculated metric is tested to coincide with COCOAPI metrics. 
 
+
+## Supported Metrics
+Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
+and `IoU` (Intersection over Union).
+
+## Documentation
+For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
+
+
+## Try live Demo
+Try OD-Metrics samples [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb)
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
+
+
 ## Installation
 Install from PyPI
 ```
 pip install od-metrics
 ```
 Install from Github
 ```
 pip install git+https://github.com/EMalagoli92/OD-Metrics
 ```
 
-## Documentation
-For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
-
 
 ## Simple Example
 
 ``` python
 from od_metrics import ODMetrics
 
 # Ground truths
```

#### html2text {}

```diff
@@ -1,40 +1,49 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.0 Summary: Object Detection
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.1 Summary: Object Detection
 metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
 EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
 Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
-                                logo_light.svg]
+                            images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
     3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
   img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
- 331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
-                    AA mmeettrriiccss ppaacckkaaggee ffoorr OObbjjeecctt DDeetteeccttiioonn..
-## Supported Metrics Supported metrics include `mAP` (Mean Average Precision),
-`mAR` (Mean Average Recall) and Intersection over Union `IoU`. ## Why OD-
-Metrics? - **User-friendly**: simple to set and simple to use; - **Highly
-Customizable**: every parameters that occur in the definition of `mAP` and
-`mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
+   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+ [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
+                                     _M_I_T_]
+      _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+      _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
+                AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
+## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
+**Highly Customizable**: every parameters that occur in the definition of `mAP`
+and `mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
 (https://github.com/cocodataset/cocoapi)**: each calculated metric is tested to
-coincide with COCOAPI metrics. ## Installation Install from PyPI ``` pip
-install od-metrics ``` Install from Github ``` pip install git+https://
-github.com/EMalagoli92/OD-Metrics ``` ## Documentation For help, usage and API
-reference, please refer to [Documentation](https://emalagoli92.github.io/OD-
-Metrics/) ## Simple Example ``` python from od_metrics import ODMetrics #
-Ground truths y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41,
-62]], "labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132,
-59, 45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [
-[25, 27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
+coincide with COCOAPI metrics. ## Supported Metrics Supported metrics include
+`mAP` (Mean Average Precision), `mAR` (Mean Average Recall) and `IoU`
+(Intersection over Union). ## Documentation For help, usage and API reference,
+please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/) ##
+Try live Demo Try OD-Metrics samples [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/
+HEAD?labpath=samples%2Fsamples.ipynb) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]##
+Installation Install from PyPI ``` pip install od-metrics ``` Install from
+Github ``` pip install git+https://github.com/EMalagoli92/OD-Metrics ``` ##
+Simple Example ``` python from od_metrics import ODMetrics # Ground truths
+y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41, 62]],
+"labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132, 59,
+45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [[25,
+27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
 "scores": [.88, .70, .80] }, { # image 2 "boxes": [[64, 111, 64, 58], [26, 140,
 60, 47], [19, 18, 43, 35]], "labels": [0, 1, 0], "scores": [.71, .54, .74] } ]
 metrics = ODMetrics() output = metrics.compute(y_true, y_pred) print(output)
 """ {'mAP@[.5 | all | 100]': 0.2574257425742574, 'mAP@[.5:.95 | all | 100]':
 0.10297029702970294, 'mAP@[.5:.95 | large | 100]': -1.0, 'mAP@[.5:.95 | medium
 | 100]': 0.10297029702970294, 'mAP@[.5:.95 | small | 100]': -1.0, 'mAP@[.75 |
 all | 100]': 0.0, 'mAR@[.5 | all | 100]': 0.25, 'mAR@[.5:.95 | all | 100]':
```

### Comparing `od-metrics-1.0.0/README.md` & `od-metrics-1.0.1/src/od_metrics.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,87 @@
+Metadata-Version: 2.1
+Name: od-metrics
+Version: 1.0.1
+Summary: Object Detection metrics.
+Home-page: https://github.com/EMalagoli92/OD-metrics
+Author: EMalagoli92
+Author-email: emala.892@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy==1.24.3
+Requires-Dist: parameterized==0.9.0
+Requires-Dist: pydantic==2.5.2
+
 <div align="center">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
-  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_dark.svg">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
+  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
+  <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
+    <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <br>
+  <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
-    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License: MIT">
-  </a>
+    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
+  <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
+    <img src="https://mybinder.org/badge_logo.svg"></a>
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
 </p>
 
 <p align="center">
   <strong>
-    A metrics package for Object Detection.
+    A python library for Object Detection metrics.
   </strong>
 </p>
 
-## Supported Metrics
-Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
-and Intersection over Union `IoU`.
-
 
 ## Why OD-Metrics?
 - **User-friendly**: simple to set and simple to use;
 - **Highly Customizable**: every parameters that occur in the definition of `mAP`
 and `mAR` can be set by user to custom values;
 - **Compatibility with [COCOAPI](https://github.com/cocodataset/cocoapi)**: each
 calculated metric is tested to coincide with COCOAPI metrics. 
 
+
+## Supported Metrics
+Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
+and `IoU` (Intersection over Union).
+
+## Documentation
+For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
+
+
+## Try live Demo
+Try OD-Metrics samples [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb)
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
+
+
 ## Installation
 Install from PyPI
 ```
 pip install od-metrics
 ```
 Install from Github
 ```
 pip install git+https://github.com/EMalagoli92/OD-Metrics
 ```
 
-## Documentation
-For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
-
 
 ## Simple Example
 
 ``` python
 from od_metrics import ODMetrics
 
 # Ground truths
```

#### html2text {}

```diff
@@ -1,33 +1,49 @@
+Metadata-Version: 2.1 Name: od-metrics Version: 1.0.1 Summary: Object Detection
+metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
+EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
+Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
+Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
-                                logo_light.svg]
+                            images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
     3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
   img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
- 331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
-                    AA mmeettrriiccss ppaacckkaaggee ffoorr OObbjjeecctt DDeetteeccttiioonn..
-## Supported Metrics Supported metrics include `mAP` (Mean Average Precision),
-`mAR` (Mean Average Recall) and Intersection over Union `IoU`. ## Why OD-
-Metrics? - **User-friendly**: simple to set and simple to use; - **Highly
-Customizable**: every parameters that occur in the definition of `mAP` and
-`mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
+   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+ [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
+                                     _M_I_T_]
+      _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+      _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
+                AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
+## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
+**Highly Customizable**: every parameters that occur in the definition of `mAP`
+and `mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
 (https://github.com/cocodataset/cocoapi)**: each calculated metric is tested to
-coincide with COCOAPI metrics. ## Installation Install from PyPI ``` pip
-install od-metrics ``` Install from Github ``` pip install git+https://
-github.com/EMalagoli92/OD-Metrics ``` ## Documentation For help, usage and API
-reference, please refer to [Documentation](https://emalagoli92.github.io/OD-
-Metrics/) ## Simple Example ``` python from od_metrics import ODMetrics #
-Ground truths y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41,
-62]], "labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132,
-59, 45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [
-[25, 27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
+coincide with COCOAPI metrics. ## Supported Metrics Supported metrics include
+`mAP` (Mean Average Precision), `mAR` (Mean Average Recall) and `IoU`
+(Intersection over Union). ## Documentation For help, usage and API reference,
+please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/) ##
+Try live Demo Try OD-Metrics samples [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/
+HEAD?labpath=samples%2Fsamples.ipynb) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]##
+Installation Install from PyPI ``` pip install od-metrics ``` Install from
+Github ``` pip install git+https://github.com/EMalagoli92/OD-Metrics ``` ##
+Simple Example ``` python from od_metrics import ODMetrics # Ground truths
+y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41, 62]],
+"labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132, 59,
+45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [[25,
+27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
 "scores": [.88, .70, .80] }, { # image 2 "boxes": [[64, 111, 64, 58], [26, 140,
 60, 47], [19, 18, 43, 35]], "labels": [0, 1, 0], "scores": [.71, .54, .74] } ]
 metrics = ODMetrics() output = metrics.compute(y_true, y_pred) print(output)
 """ {'mAP@[.5 | all | 100]': 0.2574257425742574, 'mAP@[.5:.95 | all | 100]':
 0.10297029702970294, 'mAP@[.5:.95 | large | 100]': -1.0, 'mAP@[.5:.95 | medium
 | 100]': 0.10297029702970294, 'mAP@[.5:.95 | small | 100]': -1.0, 'mAP@[.75 |
 all | 100]': 0.0, 'mAR@[.5 | all | 100]': 0.25, 'mAR@[.5:.95 | all | 100]':
```

### Comparing `od-metrics-1.0.0/setup.cfg` & `od-metrics-1.0.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = od-metrics
-version = 1.0.0
+version = 1.0.1
 author = EMalagoli92
 author_email = emala.892@gmail.com
 description = Object Detection metrics.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EMalagoli92/OD-metrics
 classifiers =
```

### Comparing `od-metrics-1.0.0/src/od_metrics/constants.py` & `od-metrics-1.0.1/src/od_metrics/constants.py`

 * *Files identical despite different names*

### Comparing `od-metrics-1.0.0/src/od_metrics/od_metrics.py` & `od-metrics-1.0.1/src/od_metrics/od_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from functools import reduce, partial
 from collections import defaultdict
 import operator
 from typing import Literal, Any, Callable, cast
 import numpy as np
 
 from .constants import DEFAULT_COCO, _STANDARD_OUTPUT
-from .utils import to_array, get_indexes, get_suffix, _Missing
+from .utils import get_indexes, get_suffix, _Missing
 from .validators import ConstructorModel, ComputeModel, MeanModel
 
 
 class ODMetrics:
     """
     ODMetrics class.
 
@@ -895,16 +895,16 @@
         # label_ids
         if label_ids is _Missing:
             raise TypeError("`label_ids` must be passed.")
 
         # Default
         default_value = {
             "iou_threshold": self.iou_thresholds,
-            "label_id": to_array(label_ids),
-            "area_range_key": to_array(list(self.area_ranges.keys())),
+            "label_id": np.array(label_ids),
+            "area_range_key": np.array(list(self.area_ranges.keys())),
             "max_detection_threshold": self.max_detection_thresholds,
             }
 
         mean_model = MeanModel.model_validate(
             {
                 "iou_threshold": iou_threshold,
                 "area_range_key": area_range_key,
```

### Comparing `od-metrics-1.0.0/src/od_metrics/utils.py` & `od-metrics-1.0.1/src/od_metrics/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 """Utility module."""
 
 from __future__ import annotations
 
 __all__ = [
     "_Missing",
-    "to_array",
     "get_indexes",
     "get_suffix",
     ]
 
-from typing import Literal, Any
+from typing import Literal
 import numpy as np
 
 
 class _Missing:
     """Sentinel class for missing values."""
 
 
-def to_array(
-        input_: Any,
-        ) -> np.ndarray:
-    """
-    Trasform input to `np.ndarray`.
-
-    Parameters
-    ----------
-    input_ : Any | None, optional
-        Input to be converted.
-
-    Returns
-    -------
-    np.ndarray
-        Input converted to `np.ndarray`.
-    """
-    if not isinstance(input_, np.ndarray):
-        output = np.array(input_)
-    else:
-        output = input_
-
-    if output.ndim == 0:
-        output = output.reshape(-1)
-    return output
-
-
 def get_indexes(
         array1: np.ndarray,
         array2: np.ndarray
         ) -> np.ndarray:
     """
     Get a list of indices.
 
@@ -141,16 +114,18 @@
     """
     if box_format == "xywh":
         return bbox
     if box_format == "xyxy":
         return xyxy_xywh(bbox)
     if box_format == "cxcywh":
         return cxcywh_xywh(bbox)
-    raise ValueError("`box_format` can be `'xyxy'`, `'xywh'`, `'cxcywh'`. "
-                     f"Found {box_format}")
+    raise ValueError(  # pragma: no cover
+        "`box_format` can be `'xyxy'`, `'xywh'`, `'cxcywh'`. "
+        f"Found {box_format}"
+        )
 
 
 def get_suffix(
         iou_threshold: np.ndarray,
         area_range_key: np.ndarray,
         max_detection_threshold: np.ndarray,
         ) -> str:
```

### Comparing `od-metrics-1.0.0/src/od_metrics/validators.py` & `od-metrics-1.0.1/src/od_metrics/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from functools import reduce
 from collections import Counter
 from typing import Any, Literal, Optional, Union
 from typing_extensions import Self
 import numpy as np
 
-from pydantic import BaseModel, field_validator, model_validator,\
+from pydantic import BaseModel, field_validator, model_validator, \
     ValidationInfo, ConfigDict
 
 from .utils import to_xywh
 
 
 def _common_validator(
         name: str,
@@ -223,16 +223,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _common_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name],
             dtype=float,
@@ -267,16 +267,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _common_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name],
             dtype=int,
@@ -311,16 +311,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _area_ranges_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name]
             )
@@ -676,16 +676,16 @@
 
         Returns
         -------
         dict
             Ground truth or predictions annotations.
         """
         if info.context is None or "box_format" not in info.context:
-            raise ValueError("Missing required context or `box_format` "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or `box_format` information.")
         box_format = info.context["box_format"]
 
         # y_true
         y_true_input = [YTrueInputModel(**v) for v in data["y_true"]]
         y_pred_input = [YPredInputModel(**v) for v in data["y_pred"]]
 
         if len(y_true_input) != len(y_pred_input):
@@ -746,16 +746,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _common_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name],
             dtype=float,
@@ -785,16 +785,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _common_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name],
             dtype=str,
@@ -824,16 +824,16 @@
         """
         if (
                 info.context is None
                 or "default_flag" not in info.context
                 or "default_value" not in info.context
                 or info.field_name is None
                 ):
-            raise ValueError("Missing required context or field name "
-                             "information.")
+            raise ValueError(  # pragma: no cover
+                "Missing required context or field name information.")
 
         return _common_validator(
             name=info.field_name,
             value=value,
             default_flag=info.context["default_flag"],
             default_value=info.context["default_value"][info.field_name],
             dtype=int,
```

### Comparing `od-metrics-1.0.0/src/od_metrics.egg-info/PKG-INFO` & `od-metrics-1.0.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,70 @@
-Metadata-Version: 2.1
-Name: od-metrics
-Version: 1.0.0
-Summary: Object Detection metrics.
-Home-page: https://github.com/EMalagoli92/OD-metrics
-Author: EMalagoli92
-Author-email: emala.892@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy==1.24.3
-Requires-Dist: parameterized==0.9.0
-Requires-Dist: pydantic==2.5.2
-
 <div align="center">
 <picture>
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_dark.svg">
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
-  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/logo_light.svg">
+  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_dark.svg">
+  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
+  <img width="400" height="400" src="https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/images/logo_light.svg">
 </picture>
 </div>
 <p align="center">
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1" />
   <img src="https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1" />
+  <a href="https://codecov.io/gh/EMalagoli92/OD-Metrics">
+    <img src="https://codecov.io/gh/EMalagoli92/OD-Metrics/graph/badge.svg?token=U7VJTKGYN6"></a>
+  <br>
+  <img src="https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat">
   <a href="https://github.com/EMalagoli92/OD-Metrics/blob/main/LICENSE">
-    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="License: MIT">
-  </a>
+    <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat" alt="License: MIT"></a><br>
+  <a href="https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb">
+    <img src="https://mybinder.org/badge_logo.svg"></a>
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
 </p>
 
 <p align="center">
   <strong>
-    A metrics package for Object Detection.
+    A python library for Object Detection metrics.
   </strong>
 </p>
 
-## Supported Metrics
-Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
-and Intersection over Union `IoU`.
-
 
 ## Why OD-Metrics?
 - **User-friendly**: simple to set and simple to use;
 - **Highly Customizable**: every parameters that occur in the definition of `mAP`
 and `mAR` can be set by user to custom values;
 - **Compatibility with [COCOAPI](https://github.com/cocodataset/cocoapi)**: each
 calculated metric is tested to coincide with COCOAPI metrics. 
 
+
+## Supported Metrics
+Supported metrics include `mAP` (Mean Average Precision), `mAR` (Mean Average Recall)
+and `IoU` (Intersection over Union).
+
+## Documentation
+For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
+
+
+## Try live Demo
+Try OD-Metrics samples [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/HEAD?labpath=samples%2Fsamples.ipynb)
+  <a href="https://colab.research.google.com/github/EMalagoli92/OD-Metrics/blob/main/samples/samples.ipynb">
+    <img src="https://img.shields.io/badge/Open%20in%20Colab-blue?logo=google-colab&style=flat&labelColor=555"></a>
+
+
 ## Installation
 Install from PyPI
 ```
 pip install od-metrics
 ```
 Install from Github
 ```
 pip install git+https://github.com/EMalagoli92/OD-Metrics
 ```
 
-## Documentation
-For help, usage and API reference, please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/)
-
 
 ## Simple Example
 
 ``` python
 from od_metrics import ODMetrics
 
 # Ground truths
```

#### html2text {}

```diff
@@ -1,40 +1,42 @@
-Metadata-Version: 2.1 Name: od-metrics Version: 1.0.0 Summary: Object Detection
-metrics. Home-page: https://github.com/EMalagoli92/OD-metrics Author:
-EMalagoli92 Author-email: emala.892@gmail.com Classifier: Programming Language
-:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.9 Description-Content-
-Type: text/markdown License-File: LICENSE Requires-Dist: numpy==1.24.3
-Requires-Dist: parameterized==0.9.0 Requires-Dist: pydantic==2.5.2
   [https://raw.githubusercontent.com/EMalagoli92/OD-Metrics/main/docs/assets/
-                                logo_light.svg]
+                            images/logo_light.svg]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
  EMalagoli92/3f159a4246243b883a5c817ca2d34baa/raw/unit_test.json?kill_cache=1]
    [https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/
 EMalagoli92/d23fd688b541d4b303d2baa6ee87e51a/raw/mypy.json?kill_cache=1][https:
  //img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
     3ab4a977b9a0e4ccb7178dd1fa51e1b0/raw/pylint.json?kill_cache=1][https://
   img.shields.io/endpoint?url=https://gist.githubusercontent.com/EMalagoli92/
- 331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_L_i_c_e_n_s_e_:_ _M_I_T_]
-                    AA mmeettrriiccss ppaacckkaaggee ffoorr OObbjjeecctt DDeetteeccttiioonn..
-## Supported Metrics Supported metrics include `mAP` (Mean Average Precision),
-`mAR` (Mean Average Recall) and Intersection over Union `IoU`. ## Why OD-
-Metrics? - **User-friendly**: simple to set and simple to use; - **Highly
-Customizable**: every parameters that occur in the definition of `mAP` and
-`mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
+   331395960725a4b47d4ca4977a24e949/raw/version.json?kill_cache=1]_[_h_t_t_p_s_:_/_/
+    _c_o_d_e_c_o_v_._i_o_/_g_h_/_E_M_a_l_a_g_o_l_i_9_2_/_O_D_-_M_e_t_r_i_c_s_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_U_7_V_J_T_K_G_Y_N_6_]
+ [https://img.shields.io/badge/python-%3E=3.9-yellow.svg?style=flat]_[_L_i_c_e_n_s_e_:
+                                     _M_I_T_]
+      _[_h_t_t_p_s_:_/_/_m_y_b_i_n_d_e_r_._o_r_g_/_b_a_d_g_e___l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+      _O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]
+                AA ppyytthhoonn lliibbrraarryy ffoorr OObbjjeecctt DDeetteeccttiioonn mmeettrriiccss..
+## Why OD-Metrics? - **User-friendly**: simple to set and simple to use; -
+**Highly Customizable**: every parameters that occur in the definition of `mAP`
+and `mAR` can be set by user to custom values; - **Compatibility with [COCOAPI]
 (https://github.com/cocodataset/cocoapi)**: each calculated metric is tested to
-coincide with COCOAPI metrics. ## Installation Install from PyPI ``` pip
-install od-metrics ``` Install from Github ``` pip install git+https://
-github.com/EMalagoli92/OD-Metrics ``` ## Documentation For help, usage and API
-reference, please refer to [Documentation](https://emalagoli92.github.io/OD-
-Metrics/) ## Simple Example ``` python from od_metrics import ODMetrics #
-Ground truths y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41,
-62]], "labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132,
-59, 45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [
-[25, 27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
+coincide with COCOAPI metrics. ## Supported Metrics Supported metrics include
+`mAP` (Mean Average Precision), `mAR` (Mean Average Recall) and `IoU`
+(Intersection over Union). ## Documentation For help, usage and API reference,
+please refer to [Documentation](https://emalagoli92.github.io/OD-Metrics/) ##
+Try live Demo Try OD-Metrics samples [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/EMalagoli92/OD-metrics/
+HEAD?labpath=samples%2Fsamples.ipynb) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
+_O_p_e_n_%_2_0_i_n_%_2_0_C_o_l_a_b_-_b_l_u_e_?_l_o_g_o_=_g_o_o_g_l_e_-_c_o_l_a_b_&_s_t_y_l_e_=_f_l_a_t_&_l_a_b_e_l_C_o_l_o_r_=_5_5_5_]##
+Installation Install from PyPI ``` pip install od-metrics ``` Install from
+Github ``` pip install git+https://github.com/EMalagoli92/OD-Metrics ``` ##
+Simple Example ``` python from od_metrics import ODMetrics # Ground truths
+y_true = [ { # image 1 "boxes": [[25, 16, 38, 56], [129, 123, 41, 62]],
+"labels": [0, 1] }, { # image 2 "boxes": [[123, 11, 43, 55], [38, 132, 59,
+45]], "labels": [0, 0] } ] # Predictions y_pred = [ { # image 1 "boxes": [[25,
+27, 37, 54], [119, 111, 40, 67], [124, 9, 49, 67]], "labels": [0, 1, 1],
 "scores": [.88, .70, .80] }, { # image 2 "boxes": [[64, 111, 64, 58], [26, 140,
 60, 47], [19, 18, 43, 35]], "labels": [0, 1, 0], "scores": [.71, .54, .74] } ]
 metrics = ODMetrics() output = metrics.compute(y_true, y_pred) print(output)
 """ {'mAP@[.5 | all | 100]': 0.2574257425742574, 'mAP@[.5:.95 | all | 100]':
 0.10297029702970294, 'mAP@[.5:.95 | large | 100]': -1.0, 'mAP@[.5:.95 | medium
 | 100]': 0.10297029702970294, 'mAP@[.5:.95 | small | 100]': -1.0, 'mAP@[.75 |
 all | 100]': 0.0, 'mAR@[.5 | all | 100]': 0.25, 'mAR@[.5:.95 | all | 100]':
```

### Comparing `od-metrics-1.0.0/tests/test_pycoco_equivalence.py` & `od-metrics-1.0.1/tests/test_odmetrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 """Unittest pycocotools equivalence."""
 
 from __future__ import annotations
 
 import unittest
 import copy
-from typing import Any
+from typing import Any, Literal
+from functools import partial
 import numpy as np
-from parameterized import parameterized_class
+from parameterized import parameterized, parameterized_class
 
 from src.od_metrics import ODMetrics, iou
 from src.od_metrics.constants import DEFAULT_COCO
-from tests.utils import annotations_generator, pycoco_converter,\
-    test_equality, rename_dict, xywh_to
+from tests.utils import annotations_generator, pycoco_converter, \
+    test_equality, rename_dict, xywh_to, apply_function
 from tests.config import TESTS
 
 try:
     import pycocotools
     from pycocotools import mask as maskUtils
     from pycocotools.coco import COCO
     from pycocotools.cocoeval import COCOeval
-    _PYCOCOTOOLS_AVAILABLE = True
-except ImportError:
-    _PYCOCOTOOLS_AVAILABLE = False
-
-# pylint: disable=E1101
+except ImportError:  # pragma: no cover
+    print(  # pragma: no cover
+        "This unittest needs `pycocotools`. Please intall by "
+        "running `pip install pycocotools`"
+        )
 
 
-@unittest.skipUnless(
-    _PYCOCOTOOLS_AVAILABLE,
-    "This unittest needs `pycocotools`. Please intall by "
-    "running `pip install pycocotools`"
-    )
 @parameterized_class(TESTS)
-class TestPyCocoEquivalenceMetrics(unittest.TestCase):
-    """Test equivalence: ODMetrics and `pycocotools.COCOeval()` method."""
+class TestBaseODMetrics(unittest.TestCase):
+    """Test `od_metrics.ODMetrics` class core functionalties."""
 
     metrics_settings: dict
     compute_settings: dict
     annotations_settings: dict
     mean_evaluator_settings: dict
     exceptions: dict
+    y_true: list | None
+    y_pred: list | None
+    to_cover: dict
 
     def get_pycoco_params(
             self,
             od_metrics_params: dict[str, Any],
             pycoco_params: pycocotools.cocoeval.Params,
             real_max_detections: int | None,
             ) -> pycocotools.cocoeval.Params:
@@ -131,54 +130,62 @@
                 pycoco_stats,
                 od_metrics_stats,
                 )
         return True
 
     # pylint: disable=R0915, R0912, R0914
     def test_equivalence(self) -> None:
-        """Test equivalence: od-metrics and `pycocotools`."""
+        """Test equivalence: `od_metrics.ODMetrics` class and `pycocotools`."""
         # Get annotations
-        y_true_od_metrics = annotations_generator(
-            **self.annotations_settings["y_true"])
-        y_pred_od_metrics = annotations_generator(
-            **self.annotations_settings["y_pred"], include_score=True)
+        if getattr(self, "y_true", None):
+            y_true_od_metrics = self.y_true
+        else:
+            y_true_od_metrics = annotations_generator(
+                **self.annotations_settings["y_true"])
+        if getattr(self, "y_pred", None):
+            y_pred_od_metrics = self.y_pred
+        else:
+            y_pred_od_metrics = annotations_generator(
+                **self.annotations_settings["y_pred"], include_score=True)
         # max detections: Only used for max_detections_thresholds=None case
         real_max_detections = (
             max(detect["boxes"].shape[0] for detect in y_pred_od_metrics)
             if "max_detection_thresholds" in self.metrics_settings and
                self.metrics_settings["max_detection_thresholds"] is None
             else None
         )
 
         # Prepare pycoco annotations
-        y_true_pycoco = pycoco_converter(y_true_od_metrics)
-        y_pred_pycoco = pycoco_converter(y_pred_od_metrics)
+        if self.to_cover.get("pycoco_converter", True):
+            y_true_pycoco = pycoco_converter(y_true_od_metrics)
+            y_pred_pycoco = pycoco_converter(y_pred_od_metrics)
+        else:
+            y_true_pycoco = None
+            y_pred_pycoco = None
 
         # Run Od_metrics evaluation
         # Init
         _init_exception = self.exceptions.get("init", None)
         if _init_exception is None:
             od_metrics_obj = ODMetrics(**self.metrics_settings)
         else:
             with self.assertRaises(_init_exception):
                 od_metrics_obj = ODMetrics(**self.metrics_settings)
             return
         # Box format
-        y_true_od_metrics = [
-            ann | {
-                "boxes": [
-                    list(xywh_to(box, od_metrics_obj.box_format))
-                    for box in ann["boxes"]]} for ann in y_true_od_metrics
-            ]
-        y_pred_od_metrics = [
-            ann | {
-                "boxes": [
-                    list(xywh_to(box, od_metrics_obj.box_format))
-                    for box in ann["boxes"]]} for ann in y_pred_od_metrics
-            ]
+        if self.to_cover.get("box_format_converter", True):
+            convert_fn = partial(xywh_to, box_format=od_metrics_obj.box_format)
+            y_true_od_metrics = [
+                ann | {"boxes": apply_function(ann["boxes"], convert_fn)}
+                for ann in y_true_od_metrics
+                ]
+            y_pred_od_metrics = [
+                ann | {"boxes": apply_function(ann["boxes"], convert_fn)}
+                for ann in y_pred_od_metrics
+                ]
 
         # Compute
         _compute_exception = self.exceptions.get("compute", None)
         if _compute_exception is None:
             od_metrics_output = od_metrics_obj.compute(
                 y_true=y_true_od_metrics,
                 y_pred=y_pred_od_metrics,
@@ -211,66 +218,37 @@
         pycoco_obj.params = params
         pycoco_obj.evaluate()
         pycoco_obj.accumulate()
         if is_default_coco:
             pycoco_obj.summarize()
 
         # Test IoUs equivalence
-        _iou_excpetion = self.exceptions.get("iou", None)
-        if _iou_excpetion is None:
-            with self.subTest("Test IoU"):
-                self.assertTrue(self._test_ious(
-                    od_metrics_ious=od_metrics_output["IoU"],
-                    pycoco_ious=pycoco_obj.ious
-                    )
+        with self.subTest("Test IoU"):
+            self.assertTrue(self._test_ious(
+                od_metrics_ious=od_metrics_output["IoU"],
+                pycoco_ious=pycoco_obj.ious
                 )
-        else:
-            with self.assertRaises(_iou_excpetion):
-                with self.subTest("Test IoU"):
-                    self._test_ious(
-                        od_metrics_ious=od_metrics_output["IoU"],
-                        pycoco_ious=pycoco_obj.ious
-                        )
-            return
+            )
 
         # Test aggregate equivalence
-        _aggregate_exception = self.exceptions.get("aggregate", None)
-        if _aggregate_exception is None:
-            with self.subTest("Test aggregate"):
-                self.assertTrue(self._test_aggregate(
-                    od_metrics_output=od_metrics_output,
-                    pycoco_eval=pycoco_obj.eval
-                    )
+        with self.subTest("Test aggregate"):
+            self.assertTrue(self._test_aggregate(
+                od_metrics_output=od_metrics_output,
+                pycoco_eval=pycoco_obj.eval
                 )
-        else:
-            with self.assertRaises(_aggregate_exception):
-                self._test_aggregate(
-                    od_metrics_output=od_metrics_output,
-                    pycoco_eval=pycoco_obj.eval
-                    )
-            return
+            )
 
         # Test summary equivalence
-        _summarize_exception = self.exceptions.get("summarize", None)
-        if _summarize_exception is None:
-            with self.subTest("Test summarize"):
-                self.assertTrue(self._test_summary(
-                    od_metrics_output=od_metrics_output,
-                    pycoco_stats=pycoco_obj.stats,
-                    is_default_coco=is_default_coco,
-                    )
+        with self.subTest("Test summarize"):
+            self.assertTrue(self._test_summary(
+                od_metrics_output=od_metrics_output,
+                pycoco_stats=pycoco_obj.stats,
+                is_default_coco=is_default_coco,
                 )
-        else:
-            with self.assertRaises(_summarize_exception):
-                self._test_summary(
-                    od_metrics_output=od_metrics_output,
-                    pycoco_stats=pycoco_obj.stats,
-                    is_default_coco=is_default_coco,
-                    )
-            return
+            )
 
         # Test mean evalautor
         _mean_evaluator_exception = self.exceptions.get("mean_evaluator", None)
         if _mean_evaluator_exception is None:
             with self.subTest("Test mean evaluator"):
                 od_metrics_output["mean_evaluator"](
                     **self.mean_evaluator_settings)
@@ -291,36 +269,52 @@
             and (np.array_equal(od_metrics_obj.max_detection_thresholds,
                                 DEFAULT_COCO["max_detection_thresholds"]))
             and (od_metrics_obj.area_ranges
                  == DEFAULT_COCO["area_ranges"])
         )
 
 
-@unittest.skipUnless(
-    _PYCOCOTOOLS_AVAILABLE,
-    "This unittest needs `pycocotools`. Please intall by "
-    "running `pip install pycocotools`"
-    )
-class TestPyCocoEquivalenceIoU(unittest.TestCase):
-    """Test equivalence: od-metrics and `pycocotools` iou function."""
+class TestMiscODMetrics(unittest.TestCase):
+    """Test `od_metrics.ODMetrics` class additional functionalties."""
+
+    def test_get_mean_exceptions(self) -> None:
+        """Test `_get_mean()` method exceptions."""
+        metrics = ODMetrics()
+        with self.assertRaises(TypeError):
+            metrics._get_mean(results=None)  # pylint: disable=W0212
+        with self.assertRaises(TypeError):
+            metrics._get_mean(label_ids=None)  # pylint: disable=W0212
+
+
+class TestIoU(unittest.TestCase):
+    """Test `od_metrics.iou()` function."""
 
     HIGH = 100000
     SIZE = 3000
 
-    def test_iou(self) -> None:
-        """Test IoU."""
-        iscrowd = list(map(
-            bool,
-            np.random.randint(
-                low=0,
-                high=2,
-                size=[self.SIZE]
-                ).tolist()
+    @parameterized.expand([(None), ("random")])
+    def test_pycoco_equivalence(
+            self,
+            iscrowd_mode: Literal["random", None],
+            ) -> None:
+        """Test equivalence: `od_metrics` and `pycocotools` iou function."""
+        if iscrowd_mode == "random":
+            iscrowd = list(map(
+                bool,
+                np.random.randint(
+                    low=0,
+                    high=2,
+                    size=[self.SIZE]
+                    ).tolist()
+                )
             )
-        )
+            iscrowd_pycoco = iscrowd
+        else:
+            iscrowd = None
+            iscrowd_pycoco = [False] * self.SIZE
         y_pred = np.random.randint(
             low=1,
             high=self.HIGH,
             size=[self.SIZE, 4]
             )
         y_true = np.random.randint(
             low=1,
@@ -329,14 +323,43 @@
             )
 
         od_metrics_ious = iou(
             y_true=y_true,
             y_pred=y_pred,
             iscrowd=iscrowd
             )
-        pycoco_ious = maskUtils.iou(y_pred, y_true, iscrowd)
+        pycoco_ious = maskUtils.iou(y_pred, y_true, iscrowd_pycoco)
 
         self.assertTrue(test_equality(od_metrics_ious, pycoco_ious))
 
+    def test_length_exception(self) -> None:
+        """Test exception `iscrowd` and `y_true` different length."""
+        iscrowd = list(map(
+            bool,
+            np.random.randint(
+                low=0,
+                high=2,
+                size=[self.SIZE + 1]
+                ).tolist()
+            )
+        )
+        y_pred = np.random.randint(
+            low=1,
+            high=self.HIGH,
+            size=[self.SIZE, 4]
+            )
+        y_true = np.random.randint(
+            low=1,
+            high=self.HIGH,
+            size=[self.SIZE, 4]
+            )
+
+        with self.assertRaises(ValueError):
+            iou(
+                y_true=y_true,
+                y_pred=y_pred,
+                iscrowd=iscrowd,
+                )
+
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()  # pragma: no cover
```

