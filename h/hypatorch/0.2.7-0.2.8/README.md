# Comparing `tmp/hypatorch-0.2.7.tar.gz` & `tmp/hypatorch-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypatorch-0.2.7.tar", last modified: Tue Apr  9 09:38:16 2024, max compression
+gzip compressed data, was "hypatorch-0.2.8.tar", last modified: Thu Apr 11 08:48:39 2024, max compression
```

## Comparing `hypatorch-0.2.7.tar` & `hypatorch-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.759660 hypatorch-0.2.7/
--rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.7/LICENSE
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-09 09:38:16.759399 hypatorch-0.2.7/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.7/README.md
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.757785 hypatorch-0.2.7/hypatorch/
--rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-09 09:37:32.000000 hypatorch-0.2.7/hypatorch/__init__.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     4729 2024-03-20 14:26:18.000000 hypatorch-0.2.7/hypatorch/assessments.py
--rw-r--r--   0 paulkrug   (502) staff       (20)    24993 2024-04-09 09:37:24.000000 hypatorch-0.2.7/hypatorch/core.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.7/hypatorch/losses.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     7421 2024-03-27 10:39:37.000000 hypatorch-0.2.7/hypatorch/utils.py
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-09 09:38:16.759104 hypatorch-0.2.7/hypatorch.egg-info/
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/SOURCES.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/dependency_links.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/requires.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-09 09:38:16.000000 hypatorch-0.2.7/hypatorch.egg-info/top_level.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-09 09:38:16.759706 hypatorch-0.2.7/setup.cfg
--rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.7/setup.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.324014 hypatorch-0.2.8/
+-rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.8/LICENSE
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-11 08:48:39.323787 hypatorch-0.2.8/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.8/README.md
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.322178 hypatorch-0.2.8/hypatorch/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-11 08:47:38.000000 hypatorch-0.2.8/hypatorch/__init__.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     4816 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/assessments.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)    25337 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/core.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.8/hypatorch/losses.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     7427 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/utils.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.323524 hypatorch-0.2.8/hypatorch.egg-info/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/requires.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/top_level.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-11 08:48:39.324073 hypatorch-0.2.8/setup.cfg
+-rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.8/setup.py
```

### Comparing `hypatorch-0.2.7/LICENSE` & `hypatorch-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.7/PKG-INFO` & `hypatorch-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.7
+Version: 0.2.8
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.7/hypatorch/assessments.py` & `hypatorch-0.2.8/hypatorch/assessments.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,29 +92,32 @@
                     Dict[ str, Dict ],
                     ],
                 ],
             harmonize_inputs: List[ str ],
             masking: Optional[Dict] = None,
             weight = 1.0,
             apply: Optional[List[str]] = None,
+            harmonizer_kwargs: Dict = {},
             ):
         super().__init__()
         self.apply = apply
         self.weight = weight
         self.name = name
         self.inputs = inputs
         self.harmonize_inputs = harmonize_inputs
         self.masking = masking
         if masking is not None:
             self.assessment = MaskedAssessment(
                 unmasked_assessment=assessment,
                 )
         else:
             self.assessment = assessment
-        self.harmonize_lengths =  LengthHarmonizer()
+        self.harmonize_lengths =  LengthHarmonizer(
+            **harmonizer_kwargs
+            )
         return
 
     def forward(
             self,
             data_dict,
             ):
```

### Comparing `hypatorch-0.2.7/hypatorch/core.py` & `hypatorch-0.2.8/hypatorch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,24 +649,25 @@
             ):
         if assessments:
             assessments_dict = self._compute_assessments(
                 data_dict = data_dict,
                 assessments = assessments[ operation_name ],
                 mode = mode,
                 )
-            for k, v in assessments_dict.items():
-                self.log(
-                    f'{mode}_{k}',
-                    v,
-                    on_epoch=True,
-                    on_step=True,
-                    prog_bar=True,
-                    logger=True,
-                    #sync_dist=False, #TODO: check if this is necessary
-                )
+            if mode != 'predict':
+                for k, v in assessments_dict.items():
+                    self.log(
+                        f'{mode}_{k}',
+                        v,
+                        on_epoch=True,
+                        on_step=True,
+                        prog_bar=True,
+                        logger=True,
+                        #sync_dist=False, #TODO: check if this is necessary
+                    )
         else:
             assessments_dict = None
         return assessments_dict
     
     def _handle_operation_output(
             self,
             x,
@@ -681,18 +682,29 @@
                 Error with output_dict of {operation_name}.
                 Operations are not allowed to overwrite existing keys.
                 However, {operation_name} has the following keys: {x.keys()}
                 and the output_dict has the following keys: {output_dict.keys()}.
                 """
                 )
         return output_dict
-
+    
     def predict_step(self, batch, batch_idx):
+        data_dict = self.test_step(
+            batch = batch,
+            batch_idx = batch_idx,
+            mode = 'predict',
+            )
+        return data_dict
 
-        mode = 'test'
+    def test_step(
+            self,
+            batch,
+            batch_idx,
+            mode = 'test',
+            ):
 
         input_dict = batch
         output_dict = {}
 
         for operation_name in self.operations.keys():
             # Forward Pass
             with torch.no_grad():
```

### Comparing `hypatorch-0.2.7/hypatorch/losses.py` & `hypatorch-0.2.8/hypatorch/losses.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.7/hypatorch/utils.py` & `hypatorch-0.2.8/hypatorch/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,35 +205,35 @@
     S = S.to( x.dtype )
 
     return S
 
 class LengthHarmonizer( torch.nn.Module ):
     def __init__(
             self,
-            mismatch_treshold = 5,
+            mismatch_threshold = 5,
             ):
         super().__init__()
-        self.mismatch_treshold = mismatch_treshold
+        self.mismatch_threshold = mismatch_threshold
         return
     
     def forward(
             self,
             data,
             ):
         # data is a list of tensors
         # find the minimum length
         lengths = [ x.shape[-1] for x in data ]
 
         # check if lengths differ by a threshold, if so raise error
-        if self.mismatch_treshold is not None:
-            if max( lengths ) - min( lengths ) > self.mismatch_treshold:
+        if self.mismatch_threshold is not None:
+            if max( lengths ) - min( lengths ) > self.mismatch_threshold:
                 raise ValueError(
                     f"""
                     losses.LengthHarmonizer: lengths are {lengths}.
-                    Lengths differ by more than {self.mismatch_treshold} samples.
+                    Lengths differ by more than {self.mismatch_threshold} samples.
                     A bug is likely.
                     """
                     )
             
         min_length = min( lengths )
         # truncate all tensors to minimum length
         # NOTE: assumes that last dimension is the length dimension
```

### Comparing `hypatorch-0.2.7/hypatorch.egg-info/PKG-INFO` & `hypatorch-0.2.8/hypatorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.7
+Version: 0.2.8
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.7/setup.py` & `hypatorch-0.2.8/setup.py`

 * *Files identical despite different names*

