# Comparing `tmp/module_qc_data_tools-1.0.8.tar.gz` & `tmp/module_qc_data_tools-1.0.9.tar.gz`

## Comparing `module_qc_data_tools-1.0.8.tar` & `module_qc_data_tools-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/.flake8
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/.gitlab-ci.yml
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/tbump.toml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/src/module_qc_data_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/src/module_qc_data_tools/_version.py
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/src/module_qc_data_tools/qcDataFrame.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/tests/test_package.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/LICENSE
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/README.md
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/.flake8
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/tbump.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/src/module_qc_data_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/src/module_qc_data_tools/_version.py
+-rw-r--r--   0        0        0    14980 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/src/module_qc_data_tools/qcDataFrame.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/tests/test_package.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/README.md
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 module_qc_data_tools-1.0.9/PKG-INFO
```

### Comparing `module_qc_data_tools-1.0.8/.gitlab-ci.yml` & `module_qc_data_tools-1.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.8/.pre-commit-config.yaml` & `module_qc_data_tools-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.8/tbump.toml` & `module_qc_data_tools-1.0.9/tbump.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2231 2e30 2e38 220a 0a23 2045  t = "1.0.8"..# E
+00000010: 7420 3d20 2231 2e30 2e39 220a 0a23 2045  t = "1.0.9"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -15,15 +15,15 @@
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
 00000140: 6d70 2076 6572 7369 6f6e 3a20 312e 302e  mp version: 1.0.
-00000150: 3820 e286 9220 7b6e 6577 5f76 6572 7369  8 ... {new_versi
+00000150: 3920 e286 9220 7b6e 6577 5f76 6572 7369  9 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_data_tools-1.0.8/src/module_qc_data_tools/__init__.py` & `module_qc_data_tools-1.0.9/src/module_qc_data_tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from module_qc_data_tools.qcDataFrame import (
     check_sn_format,
     convert_name_to_serial,
     convert_serial_to_name,
     get_env,
     get_layer_from_sn,
     get_sn_from_connectivity,
+    get_type_from_sn,
     load_json,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
 __all__ = (
@@ -20,8 +21,9 @@
     "get_layer_from_sn",
     "get_sn_from_connectivity",
     "outputDataFrame",
     "save_dict_list",
     "convert_name_to_serial",
     "convert_serial_to_name",
     "check_sn_format",
+    "get_type_from_sn",
 )
```

### Comparing `module_qc_data_tools-1.0.8/src/module_qc_data_tools/qcDataFrame.py` & `module_qc_data_tools-1.0.9/src/module_qc_data_tools/qcDataFrame.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,14 +120,28 @@
         chipName = chipSerial
         print(
             f"Warning: Can't convert chip serial number ({chipSerial}) into name, setting chip name to {chipSerial}"
         )
     return chipName
 
 
+# Returns module type, given module serial number
+def get_type_from_sn(module_sn):
+    if "PI" in module_sn:
+        if "M1" in module_sn:
+            return "quad"
+        return "triplet"
+    if "PG" in module_sn:
+        return "quad"
+    print(
+        f"Unknown module type ({module_sn}) - will not separate inner from outer pixels in disconnected bump analysis"
+    )
+    return "unknown"
+
+
 # requires the connectivity file name to be "<ATLAS_SN>_<layer>_<suffix>.json" as output from the database tool
 def get_sn_from_connectivity(fileName):
     try:
         moduleSN = os.path.basename(fileName).split("_")[0]
         check_sn_format(moduleSN)
     except Exception as e:
         print(f"Error: Cannot extract module serial number from path ({fileName}): {e}")
@@ -202,31 +216,33 @@
 
     def add_column(self, column, unit=False, x=False, data=None):
         data = data or []
         if column in self._data:
             print(f"Warning: column {column} already exists! Will overwrite.")
         self._data[column] = {"X": x, "Unit": unit, "Values": list(data)}
 
-    def add_property(self, key, value, precision=11):
+    def add_property(self, key, value, precision=-1):
         if self._property.get(key):
             print(f"Warning: property {key} already exists! Will overwrite.")
-        try:
-            value = self._round(key, value, precision)
-        except Exception:
-            pass
+        if precision != -1:
+            try:
+                value = self._round(key, value, precision)
+            except Exception:
+                pass
         self._property[key] = value
 
-    def add_parameter(self, key, value, precision=11):
+    def add_parameter(self, key, value, precision=-1):
         if self._parameter.get(key):
             print(f"Warning: parameter {key} already exists! Will overwrite.")
-        if type(value) == dict:
-            for k, v in value.items():
-                value[k] = self._round(k, v, precision)
-        else:
-            value = self._round(key, value, precision)
+        if precision != -1:
+            if type(value) == dict:
+                for k, v in value.items():
+                    value[k] = self._round(k, v, precision)
+            else:
+                value = self._round(key, value, precision)
         self._parameter[key] = value
 
     def _round(self, key, value, precision):
         try:
             if type(value) == list:
                 value = np.around(value, precision).tolist()
             else:
```

### Comparing `module_qc_data_tools-1.0.8/.gitignore` & `module_qc_data_tools-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.8/LICENSE` & `module_qc_data_tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.8/README.md` & `module_qc_data_tools-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module QC data tools v1.0.8
+# module QC data tools v1.0.9
 
 This project contains the modules needed to write/read the data files used in
 the module QC flow. This project is to be added as a submodule in other
 projects.
 
 ## Installation
 
@@ -28,15 +28,15 @@
 ```
 
 ### via pip
 
 ```
 python -m venv venv
 source venv/bin/activate
-python -m pip install -U pip module-qc-data-tools==1.0.8
+python -m pip install -U pip module-qc-data-tools==1.0.9
 ```
 
 ## Developer
 
 ### versioning
 
 In case you need to tag the version of the code, you need to have either `hatch`
```

### Comparing `module_qc_data_tools-1.0.8/pyproject.toml` & `module_qc_data_tools-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_data_tools-1.0.8/PKG-INFO` & `module_qc_data_tools-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_qc_data_tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Module qc data tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-data-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 The Python Packaging Authority
@@ -32,15 +32,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: jsonschema
 Requires-Dist: numpy
 Requires-Dist: tabulate
 Description-Content-Type: text/markdown
 
-# module QC data tools v1.0.8
+# module QC data tools v1.0.9
 
 This project contains the modules needed to write/read the data files used in
 the module QC flow. This project is to be added as a submodule in other
 projects.
 
 ## Installation
 
@@ -66,15 +66,15 @@
 ```
 
 ### via pip
 
 ```
 python -m venv venv
 source venv/bin/activate
-python -m pip install -U pip module-qc-data-tools==1.0.8
+python -m pip install -U pip module-qc-data-tools==1.0.9
 ```
 
 ## Developer
 
 ### versioning
 
 In case you need to tag the version of the code, you need to have either `hatch`
```

