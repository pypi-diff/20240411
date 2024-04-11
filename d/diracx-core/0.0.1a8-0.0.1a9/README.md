# Comparing `tmp/diracx-core-0.0.1a8.tar.gz` & `tmp/diracx-core-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diracx-core-0.0.1a8.tar", last modified: Thu Nov 30 08:40:13 2023, max compression
+gzip compressed data, was "diracx-core-0.0.1a9.tar", last modified: Sun Jan 28 09:12:01 2024, max compression
```

## Comparing `diracx-core-0.0.1a8.tar` & `diracx-core-0.0.1a9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.433400 diracx-core-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-30 08:40:13.433400 diracx-core-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-30 08:40:13.433400 diracx-core-0.0.1a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.425400 diracx-core-0.0.1a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.425400 diracx-core-0.0.1a8/src/diracx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.429400 diracx-core-0.0.1a8/src/diracx/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.429400 diracx-core-0.0.1a8/src/diracx/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/src/diracx/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.429400 diracx-core-0.0.1a8/src/diracx_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-30 08:40:13.000000 diracx-core-0.0.1a8/src/diracx_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 08:40:13.429400 diracx-core-0.0.1a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/tests/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2023-11-30 08:39:21.000000 diracx-core-0.0.1a8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.109041 diracx-core-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.109041 diracx-core-0.0.1a9/src/diracx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.109041 diracx-core-0.0.1a9/src/diracx/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/src/diracx/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/src/diracx/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/src/diracx_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 09:12:01.000000 diracx-core-0.0.1a9/src/diracx_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 09:12:01.113041 diracx-core-0.0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/tests/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-01-28 09:11:11.000000 diracx-core-0.0.1a9/tests/test_utils.py
```

### Comparing `diracx-core-0.0.1a8/PKG-INFO` & `diracx-core-0.0.1a9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-core
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Common code used by all DiracX packages
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-core-0.0.1a8/pyproject.toml` & `diracx-core-0.0.1a9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -54,7 +54,10 @@
 addopts = [
     "-v",
     "--cov=diracx.core", "--cov-report=term-missing",
     "-pdiracx.testing",
     "--import-mode=importlib",
 ]
 asyncio_mode = "auto"
+markers = [
+    "enabled_dependencies: List of dependencies which should be available to the FastAPI test client",
+]
```

### Comparing `diracx-core-0.0.1a8/src/diracx/core/config/__init__.py` & `diracx-core-0.0.1a9/src/diracx/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/config/schema.py` & `diracx-core-0.0.1a9/src/diracx/core/config/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                 if v[field] == "None":
                     v[field] = None
         return v
 
 
 class UserConfig(BaseModel):
     PreferedUsername: str
+    DNs: list[str] = []
     Email: EmailStr | None
     Suspended: list[str] = []
     Quota: int | None = None
     # TODO: These should be LHCbDIRAC specific
     CERNAccountType: str | None = None
     PrimaryCERNAccount: str | None = None
 
@@ -75,14 +76,15 @@
 
 class RegistryConfig(BaseModel):
     IdP: IdpConfig
     Support: SupportInfo = Field(default_factory=SupportInfo)
     DefaultGroup: str
     DefaultStorageQuota: float = 0
     DefaultProxyLifeTime: int = 12 * 60 * 60
+    VOMSName: str | None = None
 
     Users: dict[str, UserConfig]
     Groups: dict[str, GroupConfig]
 
     def sub_from_preferred_username(self, preferred_username: str) -> str:
         """Get the user sub from the preferred username.
```

### Comparing `diracx-core-0.0.1a8/src/diracx/core/exceptions.py` & `diracx-core-0.0.1a9/src/diracx/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/extensions.py` & `diracx-core-0.0.1a9/src/diracx/core/extensions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 __all__ = ("select_from_extension",)
 
 import os
 from collections import defaultdict
 from importlib.metadata import EntryPoint, entry_points
 from importlib.util import find_spec
-from typing import Iterator
 
+from cachetools import LRUCache, cached
 
-def extensions_by_priority() -> Iterator[str]:
+
+@cached(cache=LRUCache(maxsize=1024))
+def extensions_by_priority() -> list[str]:
     """Yield extension module names in order of priority."""
+    results = []
     for module_name in os.environ.get("DIRACX_EXTENSIONS", "diracx").split(","):
         if find_spec(module_name) is None:
             raise RuntimeError(f"Could not find extension module {module_name=}")
-        yield module_name
+        results.append(module_name)
+    return results
 
 
-def select_from_extension(
-    *, group: str, name: str | None = None
-) -> Iterator[EntryPoint]:
+@cached(cache=LRUCache(maxsize=1024))
+def select_from_extension(*, group: str, name: str | None = None) -> list[EntryPoint]:
     """Select entry points by group and name, in order of priority.
 
     Similar to ``importlib.metadata.entry_points.select`` except only modules
     found in ``DIRACX_EXTENSIONS`` are considered and return order is sorted
     from highest to lowest priority.
     """
     selected = entry_points().select(group=group)
@@ -30,9 +33,12 @@
 
     matches = defaultdict(list)
     for entry_point in selected:
         # The parent module of the entry point is the name of the extension
         module_name = entry_point.module.split(".")[0]
         matches[module_name].append(entry_point)
 
-    for module_name in extensions_by_priority():
-        yield from matches.get(module_name, [])
+    return [
+        x
+        for module_name in extensions_by_priority()
+        for x in matches.get(module_name, [])
+    ]
```

### Comparing `diracx-core-0.0.1a8/src/diracx/core/models.py` & `diracx-core-0.0.1a9/src/diracx/core/models.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/preferences.py` & `diracx-core-0.0.1a9/src/diracx/core/preferences.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/properties.py` & `diracx-core-0.0.1a9/src/diracx/core/properties.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/s3.py` & `diracx-core-0.0.1a9/src/diracx/core/s3.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/settings.py` & `diracx-core-0.0.1a9/src/diracx/core/settings.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx/core/utils.py` & `diracx-core-0.0.1a9/src/diracx/core/utils.py`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/src/diracx_core.egg-info/PKG-INFO` & `diracx-core-0.0.1a9/src/diracx_core.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diracx-core
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: Common code used by all DiracX packages
 License: GPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
```

### Comparing `diracx-core-0.0.1a8/src/diracx_core.egg-info/SOURCES.txt` & `diracx-core-0.0.1a9/src/diracx_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diracx-core-0.0.1a8/tests/test_s3.py` & `diracx-core-0.0.1a9/tests/test_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import base64
 import hashlib
+import random
 import secrets
 
 import pytest
 import requests
 from aiobotocore.session import get_session
 
 from diracx.core.s3 import (
@@ -16,17 +17,19 @@
 )
 
 BUCKET_NAME = "test_bucket"
 OTHER_BUCKET_NAME = "other_bucket"
 MISSING_BUCKET_NAME = "missing_bucket"
 INVALID_BUCKET_NAME = ".."
 
+rng = random.Random(1234)
+
 
 def _random_file(size_bytes: int):
-    file_content = secrets.token_bytes(size_bytes)
+    file_content = rng.randbytes(size_bytes)
     checksum = hashlib.sha256(file_content).hexdigest()
     return file_content, checksum
 
 
 def test_b16_to_b64_hardcoded():
     assert b16_to_b64("25") == "JQ==", "%"
     # Make sure we're using the URL-safe variant of base64
```

### Comparing `diracx-core-0.0.1a8/tests/test_secrets.py` & `diracx-core-0.0.1a9/tests/test_secrets.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 def compare_keys(key1, key2):
     """Compare two keys by checking their public numebrs"""
     assert key1.public_key().public_numbers() == key2.public_key().public_numbers()
 
 
 def test_token_signing_key(tmp_path):
-    private_key = rsa.generate_private_key(public_exponent=65537, key_size=4096)
+    private_key = rsa.generate_private_key(
+        public_exponent=65537,
+        # DANGER: 512-bits is a bad idea for prod but makes the test notably faster!
+        key_size=512,
+    )
     private_key_pem = private_key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.PKCS8,
         encryption_algorithm=serialization.NoEncryption(),
     ).decode("ascii")
     key_file = tmp_path / "private_key.pem"
     key_file.write_text(private_key_pem)
```

### Comparing `diracx-core-0.0.1a8/tests/test_utils.py` & `diracx-core-0.0.1a9/tests/test_utils.py`

 * *Files identical despite different names*

