# Comparing `tmp/lightning-module-enhanced-0.26.tar.gz` & `tmp/lightning-module-enhanced-0.26.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-module-enhanced-0.26.tar", last modified: Sun Mar 24 07:41:32 2024, max compression
+gzip compressed data, was "lightning-module-enhanced-0.26.1.tar", last modified: Thu Apr 11 07:29:39 2024, max compression
```

## Comparing `lightning-module-enhanced-0.26.tar` & `lightning-module-enhanced-0.26.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26/LICENSE
--rw-r--r--   0 mihai     (1000) mihai     (1000)      739 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      121 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.296287 lightning-module-enhanced-0.26/lightning_module_enhanced/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      576 2024-01-21 09:47:06.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      290 2023-02-05 12:57:21.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1683 2022-11-13 18:03:22.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/copy_best_checkpoint.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    16973 2024-02-18 13:18:24.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/metadata_callback.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3290 2024-01-21 09:47:06.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/plot_callback.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3996 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/plot_metrics.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      930 2023-02-05 12:57:21.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/remove_previous_train_artifacts.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    19063 2024-03-23 15:48:25.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/lme.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2893 2023-03-06 07:35:54.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2282 2023-05-18 11:32:36.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/loss.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      293 2023-03-06 07:35:54.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2854 2024-02-17 10:17:42.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/callable_core_metric.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4653 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/core_metric.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2243 2023-10-12 23:09:17.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_accuracy.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1314 2023-05-18 11:32:36.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_confusion_matrix.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1817 2023-06-10 12:15:45.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_f1_score.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     8722 2024-03-23 15:48:25.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/multi_trainer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/lightning_module_enhanced/schedulers/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       91 2022-11-13 18:03:22.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/schedulers/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      924 2024-02-17 10:17:45.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/schedulers/reduce_lr_on_plateau_with_burn_in.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)    11508 2024-03-22 08:00:27.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/trainable_module.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3314 2024-02-18 13:18:24.000000 lightning-module-enhanced-0.26/lightning_module_enhanced/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/
--rw-r--r--   0 mihai     (1000) mihai     (1000)      739 2024-03-24 07:41:32.000000 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1334 2024-03-24 07:41:32.000000 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-03-24 07:41:32.000000 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      189 2024-03-24 07:41:32.000000 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       26 2024-03-24 07:41:32.000000 lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-03-24 07:41:32.300287 lightning-module-enhanced-0.26/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      925 2024-03-24 07:41:18.000000 lightning-module-enhanced-0.26/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.793346 lightning-module-enhanced-0.26.1/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      483 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26.1/LICENSE
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      741 2024-04-11 07:29:39.789346 lightning-module-enhanced-0.26.1/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      121 2023-08-18 08:15:06.000000 lightning-module-enhanced-0.26.1/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.785346 lightning-module-enhanced-0.26.1/lightning_module_enhanced/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      576 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.789346 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      290 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1683 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/copy_best_checkpoint.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    16973 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/metadata_callback.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3290 2024-04-11 07:29:20.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/plot_callback.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4147 2024-04-05 05:49:36.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/plot_metrics.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      930 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/remove_previous_train_artifacts.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    19063 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/lme.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2893 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2282 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/loss.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.789346 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      293 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2854 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/callable_core_metric.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4653 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/core_metric.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2243 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_accuracy.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1314 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_confusion_matrix.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1817 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_f1_score.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     8722 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/multi_trainer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.789346 lightning-module-enhanced-0.26.1/lightning_module_enhanced/schedulers/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       91 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/schedulers/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      924 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/schedulers/reduce_lr_on_plateau_with_burn_in.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    11508 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/trainable_module.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3314 2024-03-24 07:41:58.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-11 07:29:39.789346 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      741 2024-04-11 07:29:39.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1334 2024-04-11 07:29:39.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-04-11 07:29:39.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      189 2024-04-11 07:29:39.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       26 2024-04-11 07:29:39.000000 lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-04-11 07:29:39.793346 lightning-module-enhanced-0.26.1/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      927 2024-04-11 07:29:37.000000 lightning-module-enhanced-0.26.1/setup.py
```

### Comparing `lightning-module-enhanced-0.26/PKG-INFO` & `lightning-module-enhanced-0.26.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-module-enhanced
-Version: 0.26
+Version: 0.26.1
 Summary: Lightning Module Enhanced
 Home-page: https://gitlab.com/mihaicristianpirvu/lightning-module-enhanced
 License: WTFPL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytorch_lightning==2.2.0.post0
```

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/__init__.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/copy_best_checkpoint.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/copy_best_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/metadata_callback.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/metadata_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/plot_callback.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/plot_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/plot_metrics.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/plot_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
         ax.plot([metric_x + 1], [metric_y], "o")
 
     def _do_plot(self, pl_module: "LME", metric_name: str, out_file: str):
         """Plot the figure with the metric"""
         fig = plt.figure()
         ax = fig.gca()
         metric_history = self.history[metric_name]
+        def _norm(x):
+            return np.clip(x, -2 * np.sign(np.median(x)) * np.median(x), 2 * np.sign(np.median(x)) * np.median(x))
         _range = range(1, len(metric_history["train"]) + 1)
-        ax.plot(_range, metric_history["train"], label="train")
+        ax.plot(_range, _norm(metric_history["train"]), label="train")
         if None not in metric_history["val"]:
-            ax.plot(_range, metric_history["val"], label="validation")
+            ax.plot(_range, _norm(metric_history["val"]), label="validation")
         self._plot_best_dot(ax, pl_module, metric_name)
         ax.set_xlabel("Epoch")
         ax.set_ylabel(metric_name)
         fig.legend()
         fig.savefig(out_file)
         plt.close(fig)
```

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/callbacks/remove_previous_train_artifacts.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/callbacks/remove_previous_train_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/lme.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/lme.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/logger.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/loss.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/loss.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/callable_core_metric.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/callable_core_metric.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/core_metric.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/core_metric.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_accuracy.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_accuracy.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_confusion_matrix.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/metrics/multi_class_f1_score.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/metrics/multi_class_f1_score.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/multi_trainer.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/multi_trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/schedulers/reduce_lr_on_plateau_with_burn_in.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/schedulers/reduce_lr_on_plateau_with_burn_in.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/trainable_module.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/trainable_module.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced/utils.py` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/PKG-INFO` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-module-enhanced
-Version: 0.26
+Version: 0.26.1
 Summary: Lightning Module Enhanced
 Home-page: https://gitlab.com/mihaicristianpirvu/lightning-module-enhanced
 License: WTFPL
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytorch_lightning==2.2.0.post0
```

### Comparing `lightning-module-enhanced-0.26/lightning_module_enhanced.egg-info/SOURCES.txt` & `lightning-module-enhanced-0.26.1/lightning_module_enhanced.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-module-enhanced-0.26/setup.py` & `lightning-module-enhanced-0.26.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from os import path
 
 name = "lightning-module-enhanced"
-version = "0.26"
+version = "0.26.1"
 description = "Lightning Module Enhanced"
 url = "https://gitlab.com/mihaicristianpirvu/lightning-module-enhanced"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

