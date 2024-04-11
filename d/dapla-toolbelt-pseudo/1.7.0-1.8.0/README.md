# Comparing `tmp/dapla_toolbelt_pseudo-1.7.0.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.7.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.8.0.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.7.0.tar` & `dapla_toolbelt_pseudo-1.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-04-09 16:03:11.809585 dapla_toolbelt_pseudo-1.7.0/LICENSE
--rw-r--r--   0        0        0    17119 2024-04-09 16:03:11.809585 dapla_toolbelt_pseudo-1.7.0/README.md
--rw-r--r--   0        0        0     4728 2024-04-09 16:03:28.369570 dapla_toolbelt_pseudo-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     1443 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      828 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2115 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     9774 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2974 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6118 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    15039 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    15314 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     9346 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19278 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8330 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5611 2024-04-09 16:03:11.813585 dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    18569 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-10 11:52:43.075945 dapla_toolbelt_pseudo-1.8.0/LICENSE
+-rw-r--r--   0        0        0    17053 2024-04-10 11:52:43.075945 dapla_toolbelt_pseudo-1.8.0/README.md
+-rw-r--r--   0        0        0     4728 2024-04-10 11:52:52.755920 dapla_toolbelt_pseudo-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1443 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      828 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2115 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0     9774 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2974 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6118 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    15341 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    15622 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     9346 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19278 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8330 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4188 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5611 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.0/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.7.0/LICENSE` & `dapla_toolbelt_pseudo-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/README.md` & `dapla_toolbelt_pseudo-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,26 +74,25 @@
 the function `with_stable_id()` to convert the identification number to a stable ID (SID) prior to pseudonymization.
 In that case, the pseudonymization algorithm is FPE (Format Preserving Encryption).
 
 > [!IMPORTANT]
 > FPE requires minimum two bytes/characters to perform encryption and minimum four bytes in case of Unicode.
 
 If a field cannot be converted using the function `with_stable_id()` the default behaviour is to use the original value
-as input to the FPE encryption function. However, this behaviour can be changed by supplying a `failure_strategy` like
-this:
+as input to the FPE encryption function. However, this behaviour can be changed by supplying a `on_map_failure` argument
+like this:
 
 ```python
 from dapla_pseudo import Pseudonymize
-from dapla_pseudo.constants import MapFailureStrategy
 
 # Example: Single field sid mapping and pseudonymization (FPE), unmatching SIDs will return Null
 result_df = (
     Pseudonymize.from_polars(df)
     .on_fields("fnr")
-    .with_stable_id(failure_strategy=MapFailureStrategy.RETURN_NULL)
+    .with_stable_id(on_map_failure="RETURN_NULL")
     .run()
     .to_polars()
 )
 ```
 
 
 ### Reading dataframes
```

### Comparing `dapla_toolbelt_pseudo-1.7.0/pyproject.toml` & `dapla_toolbelt_pseudo-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.7.0"
+version = "1.8.0"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/types.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/api_models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/baseclass.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/baseclass.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/depseudo.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,41 +237,49 @@
             self._fields = fields
             self._existing_rules = [] if rules is None else rules
 
         def with_stable_id(
             self,
             sid_snapshot_date: str | date | None = None,
             custom_key: str | None = None,
-            failure_strategy: MapFailureStrategy | None = None,
+            on_map_failure: MapFailureStrategy | str | None = None,
         ) -> "Depseudonymize._Depseudonymizer":
             """Depseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             1) Decrypt stable-id
             2) Then map decrypted stable-id to fnr and return original fnr.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
-                failure_strategy (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
+                on_map_failure (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
 
             Returns:
                 Self: The object configured to be mapped to fnr
             """
             kwargs = (
                 MapSidKeywordArgs(
                     key_id=custom_key,
                     snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=failure_strategy,
+                    failure_strategy=(
+                        None
+                        if on_map_failure is None
+                        else MapFailureStrategy(on_map_failure)
+                    ),
                 )
                 if custom_key
                 else MapSidKeywordArgs(
                     snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=failure_strategy,
+                    failure_strategy=(
+                        None
+                        if on_map_failure is None
+                        else MapFailureStrategy(on_map_failure)
+                    ),
                 )
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
             )
             return self._rule_constructor(function)
```

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo.py`

 * *Files 4% similar despite different names*

```diff
@@ -244,40 +244,48 @@
             self._fields = fields
             self._existing_rules = [] if rules is None else rules
 
         def with_stable_id(
             self,
             sid_snapshot_date: str | date | None = None,
             custom_key: PredefinedKeys | str | None = None,
-            failure_strategy: MapFailureStrategy | None = None,
+            on_map_failure: MapFailureStrategy | str | None = None,
         ) -> "Pseudonymize._Pseudonymizer":
             """Map the selected fields to Stable ID, then pseudonymize with a PAPIS-compatible encryption.
 
             In other words, this is a compound operation that both: 1) maps FNR to stable ID 2) then encrypts the Stable IDs.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
-                failure_strategy (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
+                on_map_failure (Optional[MapFailureStrategy | str], optional): defines how to handle mapping failures
 
             Returns:
                 Self: The object configured to be mapped to stable ID
             """
             kwargs = (
                 MapSidKeywordArgs(
                     key_id=custom_key,
                     snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=failure_strategy,
+                    failure_strategy=(
+                        None
+                        if on_map_failure is None
+                        else MapFailureStrategy(on_map_failure)
+                    ),
                 )
                 if custom_key
                 else MapSidKeywordArgs(
                     snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=failure_strategy,
+                    failure_strategy=(
+                        None
+                        if on_map_failure is None
+                        else MapFailureStrategy(on_map_failure)
+                    ),
                 )
             )
             function = PseudoFunction(
                 function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
             )
             return self._rule_constructor(function)
```

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/repseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/result.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/validation.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.7.0/PKG-INFO` & `dapla_toolbelt_pseudo-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.7.0
+Version: 1.8.0
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -109,26 +109,25 @@
 the function `with_stable_id()` to convert the identification number to a stable ID (SID) prior to pseudonymization.
 In that case, the pseudonymization algorithm is FPE (Format Preserving Encryption).
 
 > [!IMPORTANT]
 > FPE requires minimum two bytes/characters to perform encryption and minimum four bytes in case of Unicode.
 
 If a field cannot be converted using the function `with_stable_id()` the default behaviour is to use the original value
-as input to the FPE encryption function. However, this behaviour can be changed by supplying a `failure_strategy` like
-this:
+as input to the FPE encryption function. However, this behaviour can be changed by supplying a `on_map_failure` argument
+like this:
 
 ```python
 from dapla_pseudo import Pseudonymize
-from dapla_pseudo.constants import MapFailureStrategy
 
 # Example: Single field sid mapping and pseudonymization (FPE), unmatching SIDs will return Null
 result_df = (
     Pseudonymize.from_polars(df)
     .on_fields("fnr")
-    .with_stable_id(failure_strategy=MapFailureStrategy.RETURN_NULL)
+    .with_stable_id(on_map_failure="RETURN_NULL")
     .run()
     .to_polars()
 )
 ```
 
 
 ### Reading dataframes
```

