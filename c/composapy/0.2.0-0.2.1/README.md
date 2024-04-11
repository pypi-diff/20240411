# Comparing `tmp/composapy-0.2.0.tar.gz` & `tmp/composapy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composapy-0.2.0.tar", last modified: Wed Dec  8 16:37:45 2021, max compression
+gzip compressed data, was "composapy-0.2.1.tar", last modified: Mon Jan  3 19:12:30 2022, max compression
```

## Comparing `composapy-0.2.0.tar` & `composapy-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.665971 composapy-0.2.0/
--rw-rw-rw-   0        0        0     1098 2021-11-18 14:45:56.000000 composapy-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      658 2021-12-08 16:37:45.665971 composapy-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       50 2021-12-06 15:42:42.000000 composapy-0.2.0/README.md
--rw-rw-rw-   0        0        0      111 2021-11-22 16:47:13.000000 composapy-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      706 2021-12-08 16:37:45.667967 composapy-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.631893 composapy-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.645789 composapy-0.2.0/src/composapy/
--rw-rw-rw-   0        0        0       51 2021-11-19 22:37:55.000000 composapy-0.2.0/src/composapy/__init__.py
--rw-rw-rw-   0        0        0      217 2021-11-22 16:52:02.000000 composapy-0.2.0/src/composapy/api.py
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.663979 composapy-0.2.0/src/composapy/dataflow/
--rw-rw-rw-   0        0        0        0 2021-11-18 16:33:41.000000 composapy-0.2.0/src/composapy/dataflow/__init__.py
--rw-rw-rw-   0        0        0     3856 2021-11-29 20:36:35.000000 composapy-0.2.0/src/composapy/dataflow/api.py
--rw-rw-rw-   0        0        0     9443 2021-12-08 15:11:46.000000 composapy-0.2.0/src/composapy/dataflow/models.py
--rw-rw-rw-   0        0        0     1634 2021-11-30 15:17:58.000000 composapy-0.2.0/src/composapy/loader.py
--rw-rw-rw-   0        0        0     3951 2021-11-23 18:07:37.000000 composapy-0.2.0/src/composapy/mixins.py
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.665014 composapy-0.2.0/src/composapy/queryview/
--rw-rw-rw-   0        0        0        0 2021-11-18 16:33:50.000000 composapy-0.2.0/src/composapy/queryview/__init__.py
--rw-rw-rw-   0        0        0     3530 2021-11-22 16:44:36.000000 composapy-0.2.0/src/composapy/queryview/api.py
--rw-rw-rw-   0        0        0     2450 2021-12-07 21:14:58.000000 composapy-0.2.0/src/composapy/session.py
--rw-rw-rw-   0        0        0      528 2021-11-16 15:37:04.000000 composapy-0.2.0/src/composapy/stream.py
-drwxrwxrwx   0        0        0        0 2021-12-08 16:37:45.661986 composapy-0.2.0/src/composapy.egg-info/
--rw-rw-rw-   0        0        0      658 2021-12-08 16:37:45.000000 composapy-0.2.0/src/composapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2021-12-08 16:37:45.000000 composapy-0.2.0/src/composapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-08 16:37:45.000000 composapy-0.2.0/src/composapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2021-12-08 16:37:45.000000 composapy-0.2.0/src/composapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.688794 composapy-0.2.1/
+-rw-rw-rw-   0        0        0     1098 2021-11-18 14:45:56.000000 composapy-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      658 2022-01-03 19:12:30.689783 composapy-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2021-12-06 15:42:42.000000 composapy-0.2.1/README.md
+-rw-rw-rw-   0        0        0      111 2021-11-22 16:47:13.000000 composapy-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2022-01-03 19:12:30.690787 composapy-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.636082 composapy-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.665996 composapy-0.2.1/src/composapy/
+-rw-rw-rw-   0        0        0       51 2021-11-19 22:37:55.000000 composapy-0.2.1/src/composapy/__init__.py
+-rw-rw-rw-   0        0        0      217 2021-11-22 16:52:02.000000 composapy-0.2.1/src/composapy/api.py
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.687790 composapy-0.2.1/src/composapy/dataflow/
+-rw-rw-rw-   0        0        0        0 2021-11-18 16:33:41.000000 composapy-0.2.1/src/composapy/dataflow/__init__.py
+-rw-rw-rw-   0        0        0     3856 2021-11-29 20:36:35.000000 composapy-0.2.1/src/composapy/dataflow/api.py
+-rw-rw-rw-   0        0        0     9387 2022-01-03 18:43:15.000000 composapy-0.2.1/src/composapy/dataflow/models.py
+-rw-rw-rw-   0        0        0     1629 2022-01-03 18:50:15.000000 composapy-0.2.1/src/composapy/loader.py
+-rw-rw-rw-   0        0        0     3623 2022-01-03 18:37:33.000000 composapy-0.2.1/src/composapy/mixins.py
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.688794 composapy-0.2.1/src/composapy/queryview/
+-rw-rw-rw-   0        0        0        0 2021-11-18 16:33:50.000000 composapy-0.2.1/src/composapy/queryview/__init__.py
+-rw-rw-rw-   0        0        0     3530 2021-11-22 16:44:36.000000 composapy-0.2.1/src/composapy/queryview/api.py
+-rw-rw-rw-   0        0        0     2314 2022-01-03 15:58:23.000000 composapy-0.2.1/src/composapy/session.py
+-rw-rw-rw-   0        0        0      528 2021-11-16 15:37:04.000000 composapy-0.2.1/src/composapy/stream.py
+drwxrwxrwx   0        0        0        0 2022-01-03 19:12:30.684659 composapy-0.2.1/src/composapy.egg-info/
+-rw-rw-rw-   0        0        0      658 2022-01-03 19:12:30.000000 composapy-0.2.1/src/composapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2022-01-03 19:12:30.000000 composapy-0.2.1/src/composapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-03 19:12:30.000000 composapy-0.2.1/src/composapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-01-03 19:12:30.000000 composapy-0.2.1/src/composapy.egg-info/top_level.txt
```

### Comparing `composapy-0.2.0/LICENSE` & `composapy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `composapy-0.2.0/PKG-INFO` & `composapy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composapy
-Version: 0.2.0
+Version: 0.2.1
 Summary: ComposableAnalytics csharp binding for python
 Home-page: https://github.com/ComposableAnalytics/ComposaPy
 Author: michael surdouski
 Author-email: michael.surdouski@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ComposableAnalytics/ComposaPy/issues
 Platform: UNKNOWN
```

### Comparing `composapy-0.2.0/setup.cfg` & `composapy-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6d 706f 7361 7079 0d0a 7665   = composapy..ve
-00000020: 7273 696f 6e20 3d20 302e 322e 300d 0a61  rsion = 0.2.0..a
-00000030: 7574 686f 7220 3d20 6d69 6368 6165 6c20  uthor = michael 
-00000040: 7375 7264 6f75 736b 690d 0a61 7574 686f  surdouski..autho
-00000050: 725f 656d 6169 6c20 3d20 6d69 6368 6165  r_email = michae
-00000060: 6c2e 7375 7264 6f75 736b 6940 676d 6169  l.surdouski@gmai
-00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
-00000080: 6f6e 203d 2043 6f6d 706f 7361 626c 6541  on = ComposableA
-00000090: 6e61 6c79 7469 6373 2063 7368 6172 7020  nalytics csharp 
-000000a0: 6269 6e64 696e 6720 666f 7220 7079 7468  binding for pyth
-000000b0: 6f6e 0d0a 6c6f 6e67 5f64 6573 6372 6970  on..long_descrip
-000000c0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-000000d0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-000000e0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-000000f0: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000100: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000110: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000120: 436f 6d70 6f73 6162 6c65 416e 616c 7974  ComposableAnalyt
-00000130: 6963 732f 436f 6d70 6f73 6150 790d 0a70  ics/ComposaPy..p
-00000140: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000150: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-00000160: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000170: 6d2f 436f 6d70 6f73 6162 6c65 416e 616c  m/ComposableAnal
-00000180: 7974 6963 732f 436f 6d70 6f73 6150 792f  ytics/ComposaPy/
-00000190: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
-000001a0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001c0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-000001d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001e0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001f0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-00000200: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000210: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000220: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
-00000230: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
-00000240: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000250: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-00000260: 6573 203d 203e 3d33 2e37 2e31 0d0a 0d0a  es = >=3.7.1....
-00000270: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000280: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000290: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-000002a0: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-000002b0: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002c0: 0d0a                                     ..
+00000020: 7273 696f 6e20 3d20 302e 322e 3031 0d0a  rsion = 0.2.01..
+00000030: 6175 7468 6f72 203d 206d 6963 6861 656c  author = michael
+00000040: 2073 7572 646f 7573 6b69 0d0a 6175 7468   surdouski..auth
+00000050: 6f72 5f65 6d61 696c 203d 206d 6963 6861  or_email = micha
+00000060: 656c 2e73 7572 646f 7573 6b69 4067 6d61  el.surdouski@gma
+00000070: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
+00000080: 696f 6e20 3d20 436f 6d70 6f73 6162 6c65  ion = Composable
+00000090: 416e 616c 7974 6963 7320 6373 6861 7270  Analytics csharp
+000000a0: 2062 696e 6469 6e67 2066 6f72 2070 7974   binding for pyt
+000000b0: 686f 6e0d 0a6c 6f6e 675f 6465 7363 7269  hon..long_descri
+000000c0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+000000d0: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
+000000e0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+000000f0: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+00000100: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
+00000110: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000120: 2f43 6f6d 706f 7361 626c 6541 6e61 6c79  /ComposableAnaly
+00000130: 7469 6373 2f43 6f6d 706f 7361 5079 0d0a  tics/ComposaPy..
+00000140: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
+00000150: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
+00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000170: 6f6d 2f43 6f6d 706f 7361 626c 6541 6e61  om/ComposableAna
+00000180: 6c79 7469 6373 2f43 6f6d 706f 7361 5079  lytics/ComposaPy
+00000190: 2f69 7373 7565 730d 0a63 6c61 7373 6966  /issues..classif
+000001a0: 6965 7273 203d 200d 0a09 5072 6f67 7261  iers = ...Progra
+000001b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001c0: 3a20 5079 7468 6f6e 203a 3a20 330d 0a09  : Python :: 3...
+000001d0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001e0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001f0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+00000200: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000210: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+00000220: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000230: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000240: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000250: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+00000260: 7265 7320 3d20 3e3d 332e 372e 310d 0a0d  res = >=3.7.1...
+00000270: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000280: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+00000290: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
+000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+000002c0: 0a0d 0a                                  ...
```

### Comparing `composapy-0.2.0/src/composapy/dataflow/api.py` & `composapy-0.2.1/src/composapy/dataflow/api.py`

 * *Files identical despite different names*

### Comparing `composapy-0.2.0/src/composapy/dataflow/models.py` & `composapy-0.2.1/src/composapy/dataflow/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,25 +114,25 @@
         return self.contract.Name
 
     @property
     def inputs(self) -> InputSet:  # Dict[str, Input]:
         """Maps each module input, by name, to a corresponding Input object."""
         return InputSet(
             tuple(
-                Input(self.contract.ModuleInputs.GetItemForKey(name), self.session)
+                Input(self.contract.ModuleInputs[name], self.session)
                 for name in self.contract.ModuleInputs.Indexes.Keys
             )
         )
 
     @property
     def results(self) -> ResultSet:  # Dict[str, Result]:
         """Maps each module result, by name, to a corresponding Result object."""
         return ResultSet(
             tuple(
-                Result(self.contract.ModuleOutputs.GetItemForKey(name), self.session)
+                Result(self.contract.ModuleOutputs[name], self.session)
                 for name in self.contract.ModuleOutputs.Indexes.Keys
             )
         )
 
     @property
     def result(self) -> any:
         """Convenience property that gets the first result.value from results.
@@ -260,13 +260,13 @@
         dataflow_run = DataFlowRun(execution_state, self.session)
         return dataflow_run
 
 
 def _overwrite_module_inputs(
     external_inputs: Dict[str, any], module: Contracts.Module
 ) -> None:
-    module_input = module.ModuleInputs.GetItemForKey("Name")
+    module_input = module.ModuleInputs["Name"]
     if module_input.ValueObj in external_inputs.keys():
-        cache_input = module.ModuleInputs.GetItemForKey("Input")
+        cache_input = module.ModuleInputs["Input"]
         module.ModuleInputs.Remove("Input")
         cache_input.ValueObj = external_inputs[module_input.ValueObj]
         module.ModuleInputs.Add(cache_input)
```

### Comparing `composapy-0.2.0/src/composapy/loader.py` & `composapy-0.2.1/src/composapy/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         clr.AddReference(path)
     except:
         logging.warning(f"Failed to load .dll : {path}.")
 
 
 def load_init(environment_variables: Dict = None) -> None:
-    """Either get environment variable "ROOT_PATH_COMPOSABLE", or attempt to load into
+    """Either get environment variable "DATALAB_DLL_DIR", or attempt to load into
     environment variables using dotenv (for testing or custom load strategy). Afterward, uses root
     path to find and load needed dll's to use a session.
     """
     if environment_variables:
         for key, val in environment_variables.items():
             os.environ[key] = val
```

### Comparing `composapy-0.2.0/src/composapy/mixins.py` & `composapy-0.2.1/src/composapy/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional
 
 import System
 import pandas as pd
 
 from .session import Session
-from CompAnalytics import Contracts
 
 
 class ObjectSetMixin:
     """Used for object model sets which require element navigation tree utilities."""
 
     _target = None
 
@@ -79,16 +78,15 @@
             return
 
         table_results = self.session.table_service.GetResultFromTable(
             table, 0, 0x7FFFFFFF
         )
         headers = table_results.Headers
         results = table_results.Results
-        df = pd.DataFrame(results)
-        df.columns = headers
+        df = pd.DataFrame(results, columns=headers)
 
         dtypes_dict = self._make_pandas_dtypes_dict(table.Columns)
         for key in dtypes_dict.keys():
             if dtypes_dict[key] == "float64":
                 df[key] = df[key].apply(lambda x: System.Decimal.ToDouble(x))
 
         return df.astype(dtypes_dict)
@@ -115,17 +113,7 @@
     """For classes that require a session to function."""
 
     session = None
 
     def __init__(self, session: Session = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.session = session
-
-
-# class ValueObjectMixin:
-#     """Used for interacting with and displaying module inputs and outputs."""
-#
-#     contract: Contracts.ModuleInput | Contracts.ModuleOutput
-#
-#     @property
-#     def value_object(self) -> any:
-#         return self.contract.ValueObj
```

### Comparing `composapy-0.2.0/src/composapy/queryview/api.py` & `composapy-0.2.1/src/composapy/queryview/api.py`

 * *Files identical despite different names*

### Comparing `composapy-0.2.0/src/composapy/session.py` & `composapy-0.2.1/src/composapy/session.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,32 +34,29 @@
         else:
             form_credential = System.Net.NetworkCredential(user_or_token, password)
             self.connection_settings = IServices.Deploy.ConnectionSettings()
             self.connection_settings.Uri = Uri("http://localhost/CompApp/")
             self.connection_settings.AuthMode = IServices.Deploy.AuthMode.Form
             self.connection_settings.FormCredential = form_credential
 
-            self.ResourceManager = IServices.Deploy.ResourceManager(
-                self.connection_settings
-            )
+        self.ResourceManager = IServices.Deploy.ResourceManager(
+            self.connection_settings
+        )
 
-            self.services = self.bind_services_to_auth_channels()
-
-    def bind_services_to_auth_channels(self):
-        services = {}
+        self.services = {}
         for method in self.ResourceManager.AvailableServices():
             method_name = self.get_method_name(method)
             try:
-                services[method_name] = self.ResourceManager.CreateAuthChannel[method](
-                    method_name
-                )
+                self.services[method_name] = self.ResourceManager.CreateAuthChannel[
+                    method
+                ](method_name)
+
             except:
-                services[
+                self.services[
                     method_name
                 ] = self.ResourceManager.CreateAuthChannelNoWebScripting[method](
                     method_name
                 )
-        return services
 
     @staticmethod
     def get_method_name(method):
         return str(method).split(".")[-1][1:]
```

### Comparing `composapy-0.2.0/src/composapy/stream.py` & `composapy-0.2.1/src/composapy/stream.py`

 * *Files identical despite different names*

### Comparing `composapy-0.2.0/src/composapy.egg-info/PKG-INFO` & `composapy-0.2.1/src/composapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composapy
-Version: 0.2.0
+Version: 0.2.1
 Summary: ComposableAnalytics csharp binding for python
 Home-page: https://github.com/ComposableAnalytics/ComposaPy
 Author: michael surdouski
 Author-email: michael.surdouski@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ComposableAnalytics/ComposaPy/issues
 Platform: UNKNOWN
```

