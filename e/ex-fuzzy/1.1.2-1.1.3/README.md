# Comparing `tmp/ex_fuzzy-1.1.2.tar.gz` & `tmp/ex_fuzzy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.2.tar", last modified: Wed Apr 10 14:00:24 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.3.tar", last modified: Thu Apr 11 15:42:48 2024, max compression
```

## Comparing `ex_fuzzy-1.1.2.tar` & `ex_fuzzy-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.657128 ex_fuzzy-1.1.2/
--rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4327 2024-04-10 14:00:24.653126 ex_fuzzy-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3278 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.527121 ex_fuzzy-1.1.2/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.627124 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    10541 2024-01-31 11:27:43.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    43120 2024-04-10 13:41:32.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    39155 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.559122 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     4327 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-10 14:00:24.000000 ex_fuzzy-1.1.2/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 14:00:24.658127 ex_fuzzy-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-10 13:55:40.000000 ex_fuzzy-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 14:00:24.650126 ex_fuzzy-1.1.2/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.265662 ex_fuzzy-1.1.3/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5785 2024-04-11 15:42:48.263661 ex_fuzzy-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4736 2024-04-10 16:32:46.000000 ex_fuzzy-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.164651 ex_fuzzy-1.1.3/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.240659 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15674 2024-04-05 10:32:51.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2640 2024-04-05 14:46:18.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    42810 2024-04-11 15:37:23.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    39296 2024-04-11 15:35:59.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    15945 2024-04-04 16:52:41.000000 ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.188652 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     5785 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-11 15:42:48.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 15:42:47.000000 ex_fuzzy-1.1.3/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 15:42:48.266663 ex_fuzzy-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-11 15:42:39.000000 ex_fuzzy-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 15:42:48.258661 ex_fuzzy-1.1.3/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.3/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.2/LICENSE` & `ex_fuzzy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/PKG-INFO` & `ex_fuzzy-1.1.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: ex_fuzzy
-Version: 1.1.2
-Summary: Library to perform explainable AI using fuzzy logic.
-Home-page: https://github.com/Fuminides/ex-fuzzy
-Download-URL: https://pypi.org/project/ex-fuzzy/
-Maintainer: Javier Fumanal Idocin
-Maintainer-email: javierfumanalidocin@gmail.com
-License: GPL-3.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: networkx
-Requires-Dist: matplotlib
-Requires-Dist: pymoo
-Requires-Dist: pandas
-Requires-Dist: scikit-learn
-
 # Ex-Fuzzy
 ex-Fuzzy is a fuzzy toolbox library for Python with special focus in its accesibility to use and visualization of results. In this way, we focus on the ex(-Fuzzy)plainable capacities of approximate reasoning.
 
 Some of the tools available in this library include:
 
 - Support for approximate reasoning using fuzzy association rules, for both classification and regression problems. This includes rule base optimization using genetic algorithms and rule visualization.
 - Precomputed and optimized fuzzy variables and their correspondent linguistic variables (i.e low, medium, high).
@@ -53,16 +26,16 @@
 
 Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
   <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
+  <img src="https://private-user-images.githubusercontent.com/12574757/310877934-89b7184e-5dcc-445f-8b5f-7d4e9388c56f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5MzQtODliNzE4NGUtNWRjYy00NDVmLThiNWYtN2Q0ZTkzODhjNTZmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU0MzQ2YzhjMmQyM2M2MDlhMzc2MGUwMzUxYzFlNDgyNjk1OTU4NTY3ZGQ1Y2RhZDM2N2MzZDY2MTU2ZGVmMTImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bnJll8XpKV6o7R6MXmjNB7wJQY8eYyBMANpwkPQjRo0" width="350" title="Type 2 example">
+  <img src="https://private-user-images.githubusercontent.com/12574757/310877940-cf4453fe-6f82-4f49-b418-c774729022f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5NDAtY2Y0NDUzZmUtNmY4Mi00ZjQ5LWI0MTgtYzc3NDcyOTAyMmY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyNmQwNTFiNzNmYTljN2ZjZjcyYjY2ZTg3NWRjZDMxNmMyNGFmZTBlMGNkOTg4YTdlN2RkODNhYzc0OGE1NmUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Q_LcDf9RsPHi_QKuqMxkaIQ0dKvx8-dSv0u-KcyRNIA" width="350" title="General Type 2 example">
   
 </p>
 
 ## Dependencies
 
 - Numpy
 - Pandas
```

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,24 +44,27 @@
         self.nAnts = nAnts
         self.fl_classifier = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, 
                                             fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
         self.fuzzy_type = fuzzy_type
         self.tolerance = tolerance
 
 
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50):
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, **kwargs) -> None:
         '''
         Trains the model with the given data.
 
         :param X: samples to train.
         :param y: labels for each sample.
+        :param n_gen: number of generations to compute in the genetic optimization.
+        :param pop_size: number of subjects per generation.
+        :param kwargs: additional parameters for the genetic optimization. See fit method in BaseRuleBaseClassifier.
         '''
         fuzzy_vars = utils.construct_partitions(X, self.fuzzy_type)
         candidate_rules = rm.multiclass_mine_rulebase(X, y, fuzzy_vars, self.tolerance, max_depth=self.nAnts)
-        self.fl_classifier.fit(X, y, checkpoints=0, candidate_rules=candidate_rules, n_gen=n_gen, pop_size=pop_size)
+        self.fl_classifier.fit(X, y, checkpoints=0, candidate_rules=candidate_rules, n_gen=n_gen, pop_size=pop_size, **kwargs)
 
 
     def predict(self, X: np.array) -> np.array:
         '''
         Predict for each sample the corresponding class.
 
         :param X: samples to predict.
@@ -106,28 +109,28 @@
                                             fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
         self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
                                             fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
         self.fuzzy_type = fuzzy_type
         self.tolerance = tolerance
 
 
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0):
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, **kwargs) -> None:
         '''
         Trains the model with the given data.
 
         :param X: samples to train.
         :param y: labels for each sample.
         :param n_gen: number of generations to compute in the genetic optimization.
         :param pop_size: number of subjects per generation.
         :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
-        :param n_runner: number of threds to use.
+        :param kwargs: additional parameters for the genetic optimization. See fit method in BaseRuleBaseClassifier.
         '''
-        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints)
+        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, **kwargs)
         self.phase1_rules = self.fl_classifier1.rule_base
-        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules)
+        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules, **kwargs)
         
 
     def predict(self, X: np.array) -> np.array:
         '''
         Predcit for each sample the correspondent class.
 
         :param X: samples to predict.
@@ -169,30 +172,30 @@
                                             fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class) 
         self.fl_classifier2 = evf.BaseFuzzyRulesClassifier(nRules=nRules, linguistic_variables=linguistic_variables, nAnts=nAnts, 
                                             fuzzy_type=fuzzy_type, verbose=verbose, tolerance=tolerance, runner=runner, n_class=n_class)
         self.fuzzy_type = fuzzy_type
         self.tolerance = tolerance
 
 
-    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, n_runner:int=1):
+    def fit(self, X: np.array, y: np.array, n_gen:int=30, pop_size:int=50, checkpoints:int=0, **kwargs) -> None:
         '''
         Trains the model with the given data.
 
         :param X: samples to train.
         :param y: labels for each sample.
         :param n_gen: number of generations to compute in the genetic optimization.
         :param pop_size: number of subjects per generation.
         :param checkpoints: if bigger than 0, will save the best subject per x generations in a text file.
-        :param n_runner: number of threds to use.
+        :param kwargs: additional parameters for the genetic optimization. See fit method in BaseRuleBaseClassifier.
         '''
         candidate_rules = rm.multiclass_mine_rulebase(X, y, self.fl_classifier1.lvs, self.tolerance)
 
-        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, candidate_rules=candidate_rules)
+        self.fl_classifier1.fit(X, y, n_gen, pop_size, checkpoints, candidate_rules=candidate_rules, **kwargs)
         self.phase1_rules = self.fl_classifier1.rule_base
-        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules)
+        self.fl_classifier2.fit(X, y, n_gen, pop_size, checkpoints, initial_rules=self.phase1_rules, **kwargs)
 
 
     def predict(self, X: np.array) -> np.array:
         '''
         Predcit for each sample the correspondent class.
 
         :param X: samples to predict.
```

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 class BaseFuzzyRulesClassifier(ClassifierMixin):
     '''
     Class that is used as a classifier for a fuzzy rule based system. Supports precomputed and optimization of the linguistic variables.
     '''
 
     def __init__(self,  nRules: int = 30, nAnts: int = 4, fuzzy_type: fs.FUZZY_SETS = fs.FUZZY_SETS.t1, tolerance: float = 0.0,
                  n_linguist_variables: int = 3, verbose=False, linguistic_variables: list[fs.fuzzyVariable] = None,
-                 domain: list[float] = None, n_class: int=None, precomputed_rules: rules.MasterRuleBase =None, runner: int=1) -> None:
+                 domain: list[float] = None, n_class: int=None, precomputed_rules: rules.MasterRuleBase=None, runner: int=1) -> None:
         '''
         Inits the optimizer with the corresponding parameters.
 
         :param nRules: number of rules to optimize.
         :param nAnts: max number of antecedents to use.
         :param fuzzy type: FUZZY_SET enum type in fuzzy_sets module. The kind of fuzzy set used.
         :param tolerance: tolerance for the dominance score of the rules.
@@ -96,30 +96,29 @@
 
             # If not, then we need the parameters sumistered by the user.
             self.lvs = None
             self.fuzzy_type = fuzzy_type
             self.n_linguist_variables = n_linguist_variables
             self.domain = domain
 
-        self.alpha_ = 0.950
-        self.beta_ = 0.025
-        self.gamma_ = 0.025
+        self.alpha_ = 0.0
+        self.beta_ = 0.0
 
     def customized_loss(self, loss_function):
         '''
         Function to customize the loss function used for the optimization.
 
         :param loss_function: function that takes as input the true labels and the predicted labels and returns a float.
         :return: None
         '''
         self.custom_loss = loss_function
 
 
     def fit(self, X: np.array, y: np.array, n_gen:int=70, pop_size:int=30,
-            checkpoints:int=0, candidate_rules:rules.MasterRuleBase=None, initial_rules:rules.MasterRuleBase=None):
+            checkpoints:int=0, candidate_rules:rules.MasterRuleBase=None, initial_rules:rules.MasterRuleBase=None, random_state:int=33) -> None:
         '''
         Fits a fuzzy rule based classifier using a genetic algorithm to the given data.
 
         :param X: numpy array samples x features
         :param y: labels. integer array samples (x 1)
         :param n_gen: integer. Number of generations to run the genetic algorithm.
         :param pop_size: integer. Population size for each gneration.
@@ -146,20 +145,20 @@
                 self.nRules = len(initial_rules.get_rules())
                 self.nAnts = len(initial_rules.get_rules()[0].antecedents)
 
             if self.lvs is None:
                 # If Fuzzy variables need to be optimized.
                 problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, tolerance=self.tolerance, n_classes=len(np.unique(y)),
                                     n_linguist_variables=self.n_linguist_variables, fuzzy_type=self.fuzzy_type, domain=self.domain, thread_runner=self.thread_runner,
-                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
+                                    alpha=self.alpha_, beta=self.beta_)
             else:
                 # If Fuzzy variables are already precomputed.
                 problem = FitRuleBase(X, y, nRules=self.nRules, nAnts=self.nAnts, n_classes=len(np.unique(y)),
                                     linguistic_variables=self.lvs, domain=self.domain, tolerance=self.tolerance, thread_runner=self.thread_runner,
-                                    alpha=self.alpha_, beta=self.beta_, gamma=self.gamma_)
+                                    alpha=self.alpha_, beta=self.beta_)
         else:
             self.fuzzy_type = candidate_rules.fuzzy_type()
             self.n_linguist_variables = candidate_rules.n_linguist_variables()
             problem = ExploreRuleBases(X, y, n_classes=len(np.unique(y)), candidate_rules=candidate_rules, thread_runner=self.thread_runner, nRules=self.nRules)
 
         if self.custom_loss is not None:
             problem.fitness_func = self.custom_loss
@@ -209,14 +208,15 @@
                         f.write(checkpoint_rules)     
 
         else:
             res = minimize(problem,
                         algorithm,
                         # termination,
                         ("n_gen", n_gen),
+                        seed=random_state,
                         copy_algorithm=False,
                         save_history=False,
                         verbose=self.verbose)
         
         pop = res.pop
         fitness_last_gen = pop.get('F')
         best_solution = np.argmin(fitness_last_gen)
@@ -347,26 +347,24 @@
         Get the rulebase obtained after fitting the classifier to the data.
 
         :return: a matrix format for the rulebase.
         '''
         return self.rule_base.get_rulebase_matrix()
     
 
-    def reparametrice_loss(self, alpha:float, beta:float, gamma:float) -> None:
+    def reparametrice_loss(self, alpha:float, beta:float) -> None:
         '''
         Changes the parameters in the loss function. 
 
         :note: Does not check for convexity preservation. The user can play with these parameters as it wills.
         :param alpha: controls the MCC term.
         :param beta: controls the average rule size loss.
-        :param gamma: controls the number of rules loss.
         '''
         self.alpha_ = alpha
         self.beta_ = beta
-        self.gamma_ = gamma
 
 
 
 class ExploreRuleBases(Problem):
     '''
     Class to model as pymoo problem the fitting of a rulebase to a set of data given a series of candidate rules for a classification problem using Evolutionary strategies
     Supports type 1 and t2.
@@ -488,15 +486,15 @@
             
 
             out["F"] = 1 - score
         except rules.RuleError:
             out["F"] = 1
 
     
-    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.95, beta:float=0.025, gamma:float=0.025, precomputed_truth=None) -> float:
+    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.0, beta:float=0.0, precomputed_truth=None) -> float:
         '''
         Fitness function for the optimization problem.
         :param ruleBase: RuleBase object
         :param X: array of train samples. X shape = (n_samples, n_features)
         :param y: array of train labels. y shape = (n_samples,)
         :param tolerance: float. Tolerance for the size evaluation.
         :return: float. Fitness value.
@@ -504,15 +502,15 @@
         ev_object = evr.evalRuleBase(ruleBase, X, y, precomputed_truth=precomputed_truth)
         ev_object.add_rule_weights()
 
         score_acc = ev_object.classification_eval()
         score_rules_size = ev_object.size_antecedents_eval(tolerance)
         score_nrules = ev_object.effective_rulesize_eval(tolerance)
 
-        score = score_acc * alpha + (1 - alpha) * (score_rules_size * beta + score_nrules * gamma)
+        score = score_acc + score_rules_size * alpha + score_nrules * beta
 
         return score
     
 
 
 class FitRuleBase(Problem):
     '''
@@ -560,15 +558,15 @@
         ['Low', 'Medium', 'High'],
         ['Low', 'Medium', 'High', 'Very High'],
         ['Very Low', 'Low', 'Medium', 'High', 'Very High']
     ]
 
     def __init__(self, X: np.array, y: np.array, nRules: int, nAnts: int, n_classes: int, thread_runner: StarmapParallelization=None, 
                  linguistic_variables:list[fs.fuzzyVariable]=None, n_linguist_variables:int=3, fuzzy_type=fs.FUZZY_SETS.t1, domain:list=None,
-                 tolerance:float=0.01, alpha:float=0.950, beta:float=0.025, gamma:float=0.025) -> None:
+                 tolerance:float=0.01, alpha:float=0.0, beta:float=0.0) -> None:
         '''
         Cosntructor method. Initializes the classifier with the number of antecedents, linguist variables and the kind of fuzzy set desired.
 
         :param X: np array or pandas dataframe samples x features.
         :param y: np vector containing the target classes. vector sample
         :param nRules: number of rules to optimize.
         :param nAnts: max number of antecedents to use.
@@ -667,15 +665,14 @@
             varbound = np.concatenate(
                 (antecedent_bounds, final_consequent_bounds), axis=0)
 
         nVar = len(varbound)
         self.single_gen_size = nVar
         self.alpha_ = alpha
         self.beta_ = beta
-        self.gamma_ = gamma
 
         if thread_runner is not None:
             super().__init__(
                 vars=vars,
                 n_var=nVar,
                 n_obj=1,
                 elementwise=True,
@@ -903,31 +900,30 @@
             those features are the parameters to optimize.
 
         :param out: dict where the F field is the fitness. It is used from the outside.
         '''
         ruleBase = self._construct_ruleBase(x, self.fuzzy_type)
 
         if len(ruleBase.get_rules()) > 0:
-            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self.alpha_, self.beta_, self.gamma_, self._precomputed_truth)
+            score = self.fitness_func(ruleBase, self.X, self.y, self.tolerance, self.alpha_, self.beta_, self._precomputed_truth)
         else:
             score = 0.0
         
         out["F"] = 1 - score
     
 
-    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.975, beta:float=0.0125, gamma:float=0.0125, precomputed_truth:np.array=None) -> float:
+    def fitness_func(self, ruleBase: rules.RuleBase, X:np.array, y:np.array, tolerance:float, alpha:float=0.0, beta:float=0.0, precomputed_truth:np.array=None) -> float:
         '''
         Fitness function for the optimization problem.
         :param ruleBase: RuleBase object
         :param X: array of train samples. X shape = (n_samples, n_features)
         :param y: array of train labels. y shape = (n_samples,)
         :param tolerance: float. Tolerance for the size evaluation.
         :param alpha: float. Weight for the accuracy term.
         :param beta: float. Weight for the average rule size term.
-        :param gamma: float. Weight for the number of rules term.
         :param precomputed_truth: np array. If given, it will be used as the truth values for the evaluation.
         :return: float. Fitness value.
         '''
         if precomputed_truth is None:
             precomputed_truth = rules.compute_antecedents_memberships(ruleBase.antecedents, X)
 
         ev_object = evr.evalRuleBase(ruleBase, X, y, precomputed_truth=precomputed_truth)
@@ -935,14 +931,14 @@
         ruleBase.purge_rules(tolerance)
 
         if len(ruleBase.get_rules()) > 0: 
             score_acc = ev_object.classification_eval()
             score_rules_size = ev_object.size_antecedents_eval(tolerance)
             score_nrules = ev_object.effective_rulesize_eval(tolerance)
 
-            score = score_acc * alpha + score_rules_size * beta + score_nrules * gamma
+            score = score_acc + score_rules_size * alpha + score_nrules * beta
         else:
             score = 0.0
             
         return score
```

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,20 +807,20 @@
         Computes the output of the t1 inference system.
 
         Return an array in shape samples.
 
         :param x: array with the values of the inputs.
         :return: array with the output of the inference system for each sample.
         '''
-        res = np.zeros((x.shape[0], 2))
+        res = np.zeros((x.shape[0]))
 
         antecedent_memberships = self.compute_rule_antecedent_memberships(x)
 
         for sample in range(antecedent_memberships.shape[0]):
-            res[sample, :] = centroid.center_of_masses(
+            res[sample] = centroid.center_of_masses(
                 self.consequent_centroids_rules, antecedent_memberships[sample])
 
         return res
 
     def forward(self, x: np.array) -> np.array:
         '''
         Same as inference() in the t1 case.
@@ -957,14 +957,18 @@
         '''
         Returns the winning rule for each sample. Takes into account dominance scores if already computed.
 
         :param X: array with the values of the inputs.
         :param precomputed_truth: if not None, the antecedent memberships are already computed. (Used for sped up in genetic algorithms)
         :return: array with the winning rule for each sample.
         '''
+        # Raise an error if there no rules
+        if len(self.get_rules()) == 0:
+            raise RuleError('No rules to predict!')
+        
         consequents = sum([[self.consequent_names[ix]]*len(self[ix].rules)
                           for ix in range(len(self.rule_bases))], [])  # The sum is for flatenning the list
         winning_rules = self._winning_rules(X, precomputed_truth=precomputed_truth)
 
         return np.array([consequents[ix] for ix in winning_rules])
```

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.3/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ex-fuzzy
-Version: 1.1.2
+Name: ex_fuzzy
+Version: 1.1.3
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -53,16 +53,16 @@
 
 Use plots to visualize any kind of fuzzy sets, and use graphs to visualize rules or print them on screen.
 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/12574757/210235257-17b22ede-762b-406c-880a-497e06964f17.png" width="350" title="Fuzzy graph">
   <img src="https://user-images.githubusercontent.com/12574757/210235264-be98fff9-d1b6-4f3b-8b93-b11e0466a48c.png" width="350" title="Type 1 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/b37e2f4e-0e19-4d4b-a504-b121e41c9399" width="350" title="Type 2 example">
-  <img src="https://github.com/Fuminides/exFuzzy/assets/12574757/8e3c036f-2ab7-4281-8ef8-b8891fbf354a" width="350" title="General Type 2 example">
+  <img src="https://private-user-images.githubusercontent.com/12574757/310877934-89b7184e-5dcc-445f-8b5f-7d4e9388c56f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5MzQtODliNzE4NGUtNWRjYy00NDVmLThiNWYtN2Q0ZTkzODhjNTZmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU0MzQ2YzhjMmQyM2M2MDlhMzc2MGUwMzUxYzFlNDgyNjk1OTU4NTY3ZGQ1Y2RhZDM2N2MzZDY2MTU2ZGVmMTImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bnJll8XpKV6o7R6MXmjNB7wJQY8eYyBMANpwkPQjRo0" width="350" title="Type 2 example">
+  <img src="https://private-user-images.githubusercontent.com/12574757/310877940-cf4453fe-6f82-4f49-b418-c774729022f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI3NTk5NTAsIm5iZiI6MTcxMjc1OTY1MCwicGF0aCI6Ii8xMjU3NDc1Ny8zMTA4Nzc5NDAtY2Y0NDUzZmUtNmY4Mi00ZjQ5LWI0MTgtYzc3NDcyOTAyMmY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDEwVDE0MzQxMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTcyNmQwNTFiNzNmYTljN2ZjZjcyYjY2ZTg3NWRjZDMxNmMyNGFmZTBlMGNkOTg4YTdlN2RkODNhYzc0OGE1NmUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Q_LcDf9RsPHi_QKuqMxkaIQ0dKvx8-dSv0u-KcyRNIA" width="350" title="General Type 2 example">
   
 </p>
 
 ## Dependencies
 
 - Numpy
 - Pandas
```

### Comparing `ex_fuzzy-1.1.2/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.3/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/setup.py` & `ex_fuzzy-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.2/tests/test_centroids.py` & `ex_fuzzy-1.1.3/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/tests/test_classification.py` & `ex_fuzzy-1.1.3/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/tests/test_eval_tools.py` & `ex_fuzzy-1.1.3/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.3/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.2/tests/test_utils.py` & `ex_fuzzy-1.1.3/tests/test_utils.py`

 * *Files identical despite different names*

