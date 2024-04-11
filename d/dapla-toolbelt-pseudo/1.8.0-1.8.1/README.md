# Comparing `tmp/dapla_toolbelt_pseudo-1.8.0.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.8.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.8.1.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.8.0.tar` & `dapla_toolbelt_pseudo-1.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-04-10 11:52:43.075945 dapla_toolbelt_pseudo-1.8.0/LICENSE
--rw-r--r--   0        0        0    17053 2024-04-10 11:52:43.075945 dapla_toolbelt_pseudo-1.8.0/README.md
--rw-r--r--   0        0        0     4728 2024-04-10 11:52:52.755920 dapla_toolbelt_pseudo-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1443 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      828 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2115 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0     9774 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2974 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6118 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    15341 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    15622 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     9346 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19278 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8330 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5611 2024-04-10 11:52:43.079945 dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 09:51:27.674737 dapla_toolbelt_pseudo-1.8.1/LICENSE
+-rw-r--r--   0        0        0    17053 2024-04-11 09:51:27.674737 dapla_toolbelt_pseudo-1.8.1/README.md
+-rw-r--r--   0        0        0     4728 2024-04-11 09:51:38.502742 dapla_toolbelt_pseudo-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1493 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      828 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2115 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    12013 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2974 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6118 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    15341 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    15622 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     9346 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19278 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8330 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4188 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5611 2024-04-11 09:51:27.678737 dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.1/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.8.0/LICENSE` & `dapla_toolbelt_pseudo-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/README.md` & `dapla_toolbelt_pseudo-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/pyproject.toml` & `dapla_toolbelt_pseudo-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.8.0"
+version = "1.8.1"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # Avoid having to define the version multiple places.
 # Ref: https://github.com/python-poetry/poetry/issues/144#issuecomment-1488038660
 __version__ = version("dapla_toolbelt_pseudo")
 
 from dapla_pseudo.v1.api_models import Field
 from dapla_pseudo.v1.api_models import PseudoKeyset
+from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.depseudo import Depseudonymize
 from dapla_pseudo.v1.pseudo import Pseudonymize
 from dapla_pseudo.v1.repseudo import Repseudonymize
 from dapla_pseudo.v1.validation import Validator
 
 __all__ = [
```

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/types.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/baseclass.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/baseclass.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/depseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/pseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/repseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/result.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.8.1/src/dapla_pseudo/v1/validation.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.0/PKG-INFO` & `dapla_toolbelt_pseudo-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.8.0
+Version: 1.8.1
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

