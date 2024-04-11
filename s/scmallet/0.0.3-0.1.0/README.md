# Comparing `tmp/scmallet-0.0.3.tar.gz` & `tmp/scmallet-0.1.0.tar.gz`

## Comparing `scmallet-0.0.3.tar` & `scmallet-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.3/.codecov.yaml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.0.3/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.0.3/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/binarize.py
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/eval_model.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/infer.py
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/input.py
--rw-r--r--   0        0        0    26591 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/mallet.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/topic_metrices.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.0.3/src/scmallet/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.0.3/tests/test_basic.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.0.3/LICENSE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.0.3/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.0/.codecov.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.1.0/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.1.0/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/__init__.py
+-rw-r--r--   0        0        0     4516 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/binarize.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/eval_model.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/infer.py
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/input.py
+-rw-r--r--   0        0        0    26620 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/mallet.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/topic_metrices.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.1.0/src/scmallet/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.1.0/tests/test_basic.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.1.0/LICENSE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.1.0/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.1.0/PKG-INFO
```

### Comparing `scmallet-0.0.3/.cruft.json` & `scmallet-0.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/.pre-commit-config.yaml` & `scmallet-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `scmallet-0.1.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/.github/workflows/build.yaml` & `scmallet-0.1.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/.github/workflows/release.yaml` & `scmallet-0.1.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/.github/workflows/test.yaml` & `scmallet-0.1.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/src/scmallet/binarize.py` & `scmallet-0.1.0/src/scmallet/binarize.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     Yen, J.C., Chang, F.J. and Chang, S., 1995. A new criterion for automatic multilevel thresholding. IEEE Transactions on
     Image Processing, 4(3), pp.370-378.
     Li, C.H. and Lee, C.K., 1993. Minimum cross entropy thresholding. Pattern recognition, 26(4), pp.617-625.
     Van de Sande, B., Flerin, C., Davie, K., De Waegeneer, M., Hulselmans, G., Aibar, S., Seurinck, R., Saelens, W., Cannoodt, R.,
     Rouchon, Q. and Verbeiren, T., 2020. A scalable SCENIC workflow for single-cell gene regulatory network analysis. Nature Protocols,
     15(7), pp.2247-2276.
     """
+    if isinstance(topic_dist, np.ndarray):
+        topic_dist = pd.DataFrame(topic_dist)
+
     # smooth topics:
     topic_dist = _smooth_topics_f(topic_dist)
 
     binarized_topics = {}
     for i, col in enumerate(topic_dist.columns):
         l = np.asarray(topic_dist.iloc[:, i])
         l_norm = (l - np.min(l)) / np.ptp(l)
```

### Comparing `scmallet-0.0.3/src/scmallet/eval_model.py` & `scmallet-0.1.0/src/scmallet/eval_model.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/src/scmallet/infer.py` & `scmallet-0.1.0/src/scmallet/infer.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/src/scmallet/input.py` & `scmallet-0.1.0/src/scmallet/input.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/src/scmallet/mallet.py` & `scmallet-0.1.0/src/scmallet/mallet.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
         optimize_interval: int = 0,
         optimize_burn_in: int = 200,
         topic_threshold: float = 0.0,
         iterations: int = 300,
         random_seed: int = 555,
         n_cpu: int = 8,
         mem_gb: int = 16,
-    ) -> ray.Task:
+    ) -> ray.ObjectRef:
         """
         Train Mallet LDA.
 
         Parameters
         ----------
         num_topics : int
             The number of topics to use in the model.
@@ -361,16 +361,16 @@
         n_cpu : int, optional
             Number of threads that will be used for training. Default: 8.
         mem_gb : int, optional
             Memory to use in GB. Default: 16.
 
         Returns
         -------
-        ray.Task
-            Ray task to train the model.
+        ray.ObjectRef
+            Ray object reference to the training task.
         """
         flag_path = self._get_train_flag_path(num_topics)
 
         # record number of iterations trained in total
         if flag_path.exists():
             with open(flag_path) as fin:
                 cur_cycle = int(fin.read())
@@ -414,15 +414,15 @@
         @ray.remote(num_cpus=n_cpu)
         def _train_worker(
             cmd: str,
             flag_path: Path,
             iterations: int,
             num_topics: int,
             temp_paths: list[Path],
-        ) -> ray.Task:
+        ) -> ray.ObjectRef:
             print("Running command:", cmd)
             try:
                 subprocess.check_output(args=shlex.split(cmd), shell=False, stderr=subprocess.STDOUT)
             except subprocess.CalledProcessError as e:
                 raise RuntimeError(f"command '{e.cmd}' return with error (code {e.returncode}): {e.output}") from e
 
             # record number of iterations trained in total
```

### Comparing `scmallet-0.0.3/src/scmallet/topic_metrices.py` & `scmallet-0.1.0/src/scmallet/topic_metrices.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/src/scmallet/utils.py` & `scmallet-0.1.0/src/scmallet/utils.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/LICENSE` & `scmallet-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/README.md` & `scmallet-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/pyproject.toml` & `scmallet-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.3/PKG-INFO` & `scmallet-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scmallet
-Version: 0.0.3
+Version: 0.1.0
 Summary: Python wrapper of MALLET for LDA analysis on single-cell data
 Project-URL: Source, https://github.com/lhqing/scmallet
 Project-URL: Home-page, https://github.com/lhqing/scmallet
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanqingliu@fas.harvard.edu>
 License: MIT License
```

