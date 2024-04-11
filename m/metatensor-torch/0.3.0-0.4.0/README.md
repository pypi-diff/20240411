# Comparing `tmp/metatensor-torch-0.3.0.tar.gz` & `tmp/metatensor-torch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metatensor-torch-0.3.0.tar", last modified: Fri Mar  1 16:59:53 2024, max compression
+gzip compressed data, was "metatensor-torch-0.4.0.tar", last modified: Thu Apr 11 12:23:56 2024, max compression
```

## Comparing `metatensor-torch-0.3.0.tar` & `metatensor-torch-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.222359 metatensor-torch-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-01 16:59:53.222359 metatensor-torch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.218359 metatensor-torch-0.3.0/build-backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/build-backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.214359 metatensor-torch-0.3.0/metatensor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.218359 metatensor-torch-0.3.0/metatensor/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/_c_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.218359 metatensor-torch-0.3.0/metatensor/torch/atomistic/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13404 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/ase_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14873 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26666 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/atomistic/systems_to_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    47840 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/metatensor/torch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    55847 2024-03-01 16:58:21.000000 metatensor-torch-0.3.0/metatensor-torch-cxx-0.3.0.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 16:59:53.218359 metatensor-torch-0.3.0/metatensor_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:59:52.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/metatensor_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 16:59:53.000000 metatensor-torch-0.3.0/n_commits_since_last_tag
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 16:59:53.222359 metatensor-torch-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-03-01 16:58:12.000000 metatensor-torch-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/build-backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/build-backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/metatensor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.031126 metatensor-torch-0.4.0/metatensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/_c_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/metatensor/torch/atomistic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/ase_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26835 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/atomistic/systems_to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48268 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/metatensor/torch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59407 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor-torch-cxx-0.4.0.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/metatensor_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:55.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 12:23:56.000000 metatensor-torch-0.4.0/metatensor_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:23:55.000000 metatensor-torch-0.4.0/n_commits_since_last_tag
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:23:56.035126 metatensor-torch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-04-11 12:23:32.000000 metatensor-torch-0.4.0/setup.py
```

### Comparing `metatensor-torch-0.3.0/LICENSE` & `metatensor-torch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.3.0/PKG-INFO` & `metatensor-torch-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.3.0
+Version: 0.4.0
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
@@ -23,14 +23,14 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: torch>=1.11
+Requires-Dist: torch>=1.12
 Requires-Dist: metatensor-core<0.2.0,>=0.1.0
 
 metatensor-torch
 ================
 
 This package contains the TorchScript bindings to the core API of metatensor.
```

### Comparing `metatensor-torch-0.3.0/build-backend/backend.py` & `metatensor-torch-0.4.0/build-backend/backend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-# this is a custom Python build backend wrapping setuptool's to add a build-time
-# dependencies to metatensor-core, using the local version if it exists, and
-# otherwise falling back to the one on PyPI.
+# This is a custom Python build backend wrapping setuptool's to add a build-time
+# dependencies to metatensor-core, using the local version if it exists, and otherwise
+# falling back to the one on PyPI.
+#
+# This also allows to only depend on torch/cmake when building the wheel and not the
+# sdist
 import os
 import uuid
 
 from setuptools import build_meta
 
 
 ROOT = os.path.realpath(os.path.dirname(__file__))
 METATENSOR_CORE = os.path.realpath(os.path.join(ROOT, "..", "..", "metatensor-core"))
 FORCED_METATENSOR_CORE_VERSION = os.environ.get(
-    "METATENSOR_TORCH_BUILD_WITH_METATENSOR_TORCH_VERSION"
+    "METATENSOR_TORCH_BUILD_WITH_METATENSOR_CORE_VERSION"
 )
 
 if FORCED_METATENSOR_CORE_VERSION is not None:
     # force a specific version for metatensor-core, this is used when checking the build
     # from a sdist on a non-released version
     METATENSOR_CORE_DEP = f"metatensor-core =={FORCED_METATENSOR_CORE_VERSION}"
 
@@ -26,18 +29,28 @@
     uuid = uuid.uuid4()
     METATENSOR_CORE_DEP = f"metatensor-core @ file://{METATENSOR_CORE}?{uuid}"
 else:
     # we are building from a sdist
     METATENSOR_CORE_DEP = "metatensor-core >=0.1.0,<0.2.0"
 
 
+FORCED_TORCH_VERSION = os.environ.get("METATENSOR_TORCH_BUILD_WITH_TORCH_VERSION")
+if FORCED_TORCH_VERSION is not None:
+    TORCH_DEP = f"torch =={FORCED_TORCH_VERSION}"
+else:
+    TORCH_DEP = "torch >=1.12"
+
+# ==================================================================================== #
+#                   Build backend functions definition                                 #
+# ==================================================================================== #
+
+# Use the default version of these
 prepare_metadata_for_build_wheel = build_meta.prepare_metadata_for_build_wheel
+get_requires_for_build_sdist = build_meta.get_requires_for_build_sdist
 build_wheel = build_meta.build_wheel
 build_sdist = build_meta.build_sdist
 
 
+# Special dependencies to build the wheels
 def get_requires_for_build_wheel(config_settings=None):
     defaults = build_meta.get_requires_for_build_wheel(config_settings)
-    return defaults + [METATENSOR_CORE_DEP]
-
-
-get_requires_for_build_sdist = build_meta.get_requires_for_build_sdist
+    return defaults + ["cmake", TORCH_DEP, METATENSOR_CORE_DEP]
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/__init__.py` & `metatensor-torch-0.4.0/metatensor/torch/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 from . import utils  # noqa: F401
 
 
 if os.environ.get("METATENSOR_IMPORT_FOR_SPHINX", "0") != "0":
     from .documentation import Labels, LabelsEntry, TensorBlock, TensorMap
     from .documentation import load, load_labels, load_labels_buffer, load_buffer
     from .documentation import save, save_buffer
+    from .documentation import version, dtype_name
 else:
     _load_library()
     Labels = torch.classes.metatensor.Labels
     LabelsEntry = torch.classes.metatensor.LabelsEntry
     TensorBlock = torch.classes.metatensor.TensorBlock
     TensorMap = torch.classes.metatensor.TensorMap
 
+    version = torch.ops.metatensor.version
+    dtype_name = torch.ops.metatensor.dtype_name
+
     load = torch.ops.metatensor.load
     load_buffer = torch.ops.metatensor.load_buffer
     load_labels = torch.ops.metatensor.load_labels
     load_labels_buffer = torch.ops.metatensor.load_labels_buffer
     save = torch.ops.metatensor.save
     save_buffer = torch.ops.metatensor.save_buffer
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/_c_lib.py` & `metatensor-torch-0.4.0/metatensor/torch/_c_lib.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,79 @@
+import glob
 import os
-import re
 import sys
-from collections import namedtuple
 
 import torch
 
 import metatensor
 
-from ._build_versions import BUILD_METATENSOR_CORE_VERSION, BUILD_TORCH_VERSION
+from ._build_versions import BUILD_METATENSOR_CORE_VERSION
+from .utils import parse_version, version_compatible
 from .version import __version__
 
 
-Version = namedtuple("Version", ["major", "minor", "patch"])
-
-
-def parse_version(version):
-    match = re.match(r"(\d+)\.(\d+)\.(\d+).*", version)
-    if match:
-        return Version(*map(int, match.groups()))
-    else:
-        raise ValueError("Invalid version string format")
-
-
-def version_compatible(actual, required):
-    actual = parse_version(actual)
-    required = parse_version(required)
-
-    if actual.major != required.major:
-        return False
-    elif actual.minor != required.minor:
-        return False
-    else:
-        return True
-
-
-if not version_compatible(torch.__version__, BUILD_TORCH_VERSION):
-    raise ImportError(
-        f"Trying to load metatensor-torch with torch v{torch.__version__}, "
-        f"but it was compiled against torch v{BUILD_TORCH_VERSION}, which "
-        "is not ABI compatible"
-    )
-
 if not version_compatible(metatensor.__version__, BUILD_METATENSOR_CORE_VERSION):
     raise ImportError(
         "Trying to load metatensor-torch with metatensor-core "
         f"v{metatensor.__version__}, but it was compiled against "
         f"metatensor-core v{BUILD_METATENSOR_CORE_VERSION}, which "
         "is not ABI compatible"
     )
 
 _HERE = os.path.realpath(os.path.dirname(__file__))
 
 
 def _lib_path():
-    if sys.platform.startswith("darwin"):
-        path = os.path.join(_HERE, "lib", "libmetatensor_torch.dylib")
-        windows = False
-    elif sys.platform.startswith("linux"):
-        path = os.path.join(_HERE, "lib", "libmetatensor_torch.so")
-        windows = False
-    elif sys.platform.startswith("win"):
-        path = os.path.join(_HERE, "bin", "metatensor_torch.dll")
-        windows = True
-    else:
-        raise ImportError("Unknown platform. Please edit this file")
-
-    if os.path.isfile(path):
-        if windows:
-            _check_dll(path)
-        return path
 
-    raise ImportError("Could not find metatensor_torch shared library at " + path)
+    torch_version = parse_version(torch.__version__)
+    expected_prefix = os.path.join(
+        _HERE, f"torch-{torch_version.major}.{torch_version.minor}"
+    )
+    if os.path.exists(expected_prefix):
+        if sys.platform.startswith("darwin"):
+            path = os.path.join(expected_prefix, "lib", "libmetatensor_torch.dylib")
+            windows = False
+        elif sys.platform.startswith("linux"):
+            path = os.path.join(expected_prefix, "lib", "libmetatensor_torch.so")
+            windows = False
+        elif sys.platform.startswith("win"):
+            path = os.path.join(expected_prefix, "bin", "metatensor_torch.dll")
+            windows = True
+        else:
+            raise ImportError("Unknown platform. Please edit this file")
+
+        if os.path.isfile(path):
+            if windows:
+                _check_dll(path)
+            return path
+        else:
+            raise ImportError(
+                "Could not find metatensor_torch shared library at " + path
+            )
+
+    # gather which torch version(s) the current install was built
+    # with to create the error message
+    existing_versions = []
+    for prefix in glob.glob(os.path.join(_HERE, "torch-*")):
+        existing_versions.append(os.path.basename(prefix)[6:])
+
+    if len(existing_versions) == 1:
+        raise ImportError(
+            f"Trying to load metatensor-torch with torch v{torch.__version__}, "
+            f"but it was compiled against torch v{existing_versions[0]}, which "
+            "is not ABI compatible"
+        )
+    else:
+        all_versions = ", ".join(map(lambda version: f"v{version}", existing_versions))
+        raise ImportError(
+            f"Trying to load metatensor-torch with torch v{torch.__version__}, "
+            f"we found builds for torch {all_versions}; which are not ABI compatible.\n"
+            "You can try to re-install from source with "
+            "`pip install metatensor-torch --no-binary=metatensor-torch`"
+        )
 
 
 def _check_dll(path):
     """
     Check if the DLL pointer size matches Python (32-bit or 64-bit)
     """
     import platform
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/__init__.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,30 @@
         ModelEvaluationOptions,
         ModelCapabilities,
         ModelMetadata,
     )
 
     from .documentation import (
         check_atomistic_model,
+        load_model_extensions,
         register_autograd_neighbors,
         unit_conversion_factor,
     )
 
 else:
     System = torch.classes.metatensor.System
     NeighborsListOptions = torch.classes.metatensor.NeighborsListOptions
 
     ModelOutput = torch.classes.metatensor.ModelOutput
     ModelEvaluationOptions = torch.classes.metatensor.ModelEvaluationOptions
     ModelCapabilities = torch.classes.metatensor.ModelCapabilities
     ModelMetadata = torch.classes.metatensor.ModelMetadata
 
+    load_model_extensions = torch.ops.metatensor.load_model_extensions
     check_atomistic_model = torch.ops.metatensor.check_atomistic_model
+
     register_autograd_neighbors = torch.ops.metatensor.register_autograd_neighbors
     unit_conversion_factor = torch.ops.metatensor.unit_conversion_factor
 
 from .model import MetatensorAtomisticModel, ModelInterface  # noqa: F401
+from .model import load_atomistic_model  # noqa: F401
 from .systems_to_torch import systems_to_torch  # noqa: F401
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/ase_calculator.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/ase_calculator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import logging
 import os
 import pathlib
+import warnings
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import torch
 
 from .. import Labels, TensorBlock
 from . import (
     MetatensorAtomisticModel,
     ModelEvaluationOptions,
     ModelMetadata,
     ModelOutput,
     System,
-    check_atomistic_model,
+    load_atomistic_model,
     register_autograd_neighbors,
 )
 
 
 import ase  # isort: skip
 import ase.neighborlist  # isort: skip
 import ase.calculators.calculator  # isort: skip
@@ -29,74 +31,121 @@
 
 if os.environ.get("METATENSOR_IMPORT_FOR_SPHINX", "0") == "0":
     # this can not be imported when building the documentation
     from .. import sum_over_samples  # isort: skip
 
 FilePath = Union[str, bytes, pathlib.PurePath]
 
+LOGGER = logging.getLogger(__name__)
+
+
+STR_TO_DTYPE = {
+    "float32": torch.float32,
+    "float64": torch.float64,
+}
+
 
 class MetatensorCalculator(ase.calculators.calculator.Calculator):
     """
     The :py:class:`MetatensorCalculator` class implements ASE's
     :py:class:`ase.calculators.calculator.Calculator` API using metatensor atomistic
     models to compute energy, forces and any other supported property.
 
     This class can be initialized with any :py:class:`MetatensorAtomisticModel`, and
     used to run simulations using ASE's MD facilities.
     """
 
     def __init__(
         self,
-        model: Union[
-            FilePath,
-            MetatensorAtomisticModel,
-        ],
+        model: Union[FilePath, MetatensorAtomisticModel],
+        *,
+        extensions_directory=None,
         check_consistency=False,
+        device=None,
     ):
         """
         :param model: model to use for the calculation. This can be a file path, a
             Python instance of :py:class:`MetatensorAtomisticModel`, or the output of
             :py:func:`torch.jit.script` on :py:class:`MetatensorAtomisticModel`.
+        :param extensions_directory: if the model uses extensions, we will try to load
+            them from this directory
         :param check_consistency: should we check the model for consistency when
             running, defaults to False.
+        :param device: torch device to use for the calculation. If ``None``, we will try
+            the options in the model's ``supported_device`` in order.
         """
         super().__init__()
 
         self.parameters = {
             "check_consistency": check_consistency,
         }
 
+        # Load the model
         if isinstance(model, (str, bytes, pathlib.PurePath)):
             if not os.path.exists(model):
                 raise InputError(f"given model path '{model}' does not exist")
 
-            check_atomistic_model(model)
-            self._model = torch.jit.load(model)
             self.parameters["model_path"] = str(model)
+
+            model = load_atomistic_model(
+                model, extensions_directory=extensions_directory
+            )
+
         elif isinstance(model, torch.jit.RecursiveScriptModule):
             if model.original_name != "MetatensorAtomisticModel":
                 raise InputError(
                     "torch model must be 'MetatensorAtomisticModel', "
                     f"got '{model.original_name}' instead"
                 )
-            self._model = model
         elif isinstance(model, MetatensorAtomisticModel):
-            self._model = model
+            # nothing to do
+            pass
         else:
             raise TypeError(f"unknown type for model: {type(model)}")
 
-        if check_consistency:
-            capabilities = self._model.capabilities()
-            if "cpu" not in capabilities.supported_devices:
+        self.parameters["device"] = str(device) if device is not None else None
+        # check if the model supports the requested device
+        capabilities = model.capabilities()
+        if device is None:
+            device = _find_best_device(capabilities.supported_devices)
+        else:
+            device = torch.device(device)
+            device_is_supported = False
+
+            for supported in capabilities.supported_devices:
+                try:
+                    supported = torch.device(supported)
+                except RuntimeError as e:
+                    warnings.warn(
+                        "the model contains an invalid device in `supported_devices`: "
+                        f"{e}",
+                        stacklevel=2,
+                    )
+                    continue
+
+                if supported.type == device.type:
+                    device_is_supported = True
+                    break
+
+            if not device_is_supported:
                 raise ValueError(
-                    "ASE calculator only supports CPU device for now, "
-                    "but the model does not"
+                    f"This model does not support the requested device ({device}), "
+                    "the following devices are supported: "
+                    f"{capabilities.supported_devices}"
                 )
 
-            self._model = self._model.to(device="cpu")
+        if capabilities.dtype in STR_TO_DTYPE:
+            self._dtype = STR_TO_DTYPE[capabilities.dtype]
+        else:
+            raise ValueError(
+                f"found unexpected dtype in model capabilities: {capabilities.dtype}"
+            )
+
+        self._device = device
+        self._model = model.to(device=self._device)
 
         # We do our own check to verify if a property is implemented in `calculate()`,
         # so we pretend to be able to compute all properties ASE knows about.
         self.implemented_properties = ALL_ASE_PROPERTIES
 
     def todict(self):
         if "model_path" not in self.parameters:
@@ -106,15 +155,19 @@
                 "to use `todict`"
             )
 
         return self.parameters
 
     @classmethod
     def fromdict(cls, data):
-        return MetatensorCalculator(data["model_path"], data["check_consistency"])
+        return MetatensorCalculator(
+            model=data["model_path"],
+            check_consistency=data["check_consistency"],
+            device=data["device"],
+        )
 
     def metadata(self) -> ModelMetadata:
         """Get the metadata of the underlying model"""
         return self._model.metadata()
 
     def run_model(
         self,
@@ -136,20 +189,24 @@
         All the parameters have the same meaning as the corresponding ones in
         :py:meth:`metatensor.torch.atomistic.ModelInterface.forward`.
 
         :param atoms: system on which to run the model
         :param outputs: outputs of the model that should be predicted
         :param selected_atoms: subset of atoms on which to run the calculation
         """
-        types, positions, cell = _ase_to_torch_data(atoms)
+        types, positions, cell = _ase_to_torch_data(
+            atoms=atoms, dtype=self._dtype, device=self._device
+        )
         system = System(types, positions, cell)
 
         # Compute the neighbors lists requested by the model using ASE NL
         for options in self._model.requested_neighbors_lists():
-            neighbors = _compute_ase_neighbors(atoms, options)
+            neighbors = _compute_ase_neighbors(
+                atoms, options, dtype=self._dtype, device=self._device
+            )
             register_autograd_neighbors(
                 system,
                 neighbors,
                 check_consistency=self.parameters["check_consistency"],
             )
             system.add_neighbors_list(options, neighbors)
 
@@ -189,38 +246,42 @@
         for name in outputs.keys():
             if name not in capabilities.outputs:
                 raise ValueError(
                     f"you asked for the calculation of {name}, but this model does not "
                     "support it"
                 )
 
-        types, positions, cell = _ase_to_torch_data(atoms)
+        types, positions, cell = _ase_to_torch_data(
+            atoms=atoms, dtype=self._dtype, device=self._device
+        )
 
         do_backward = False
         if "forces" in properties:
             do_backward = True
             positions.requires_grad_(True)
 
         if "stress" in properties:
             do_backward = True
 
-            scaling = torch.eye(3, requires_grad=True, dtype=cell.dtype)
+            scaling = torch.eye(3, requires_grad=True, dtype=self._dtype)
 
             positions = positions @ scaling
             positions.retain_grad()
 
             cell = cell @ scaling
 
         if "stresses" in properties:
             raise NotImplementedError("'stresses' are not implemented yet")
 
         # convert from ase.Atoms to metatensor.torch.atomistic.System
         system = System(types, positions, cell)
         for options in self._model.requested_neighbors_lists():
-            neighbors = _compute_ase_neighbors(atoms, options)
+            neighbors = _compute_ase_neighbors(
+                atoms, options, dtype=self._dtype, device=self._device
+            )
             register_autograd_neighbors(
                 system,
                 neighbors,
                 check_consistency=self.parameters["check_consistency"],
             )
             system.add_neighbors_list(options, neighbors)
 
@@ -252,33 +313,78 @@
         assert len(energy.block().gradients_list()) == 0
         energy = energy.block().values
         assert energy.shape == (1, 1)
 
         self.results = {}
 
         if "energies" in properties:
-            self.results["energies"] = (
-                energies.detach().to(device="cpu").numpy().reshape(-1)
-            )
+            energies_values = energies.detach().reshape(-1)
+            energies_values = energies_values.to(device="cpu").to(dtype=torch.float64)
+            self.results["energies"] = energies_values.numpy()
 
         if "energy" in properties:
-            self.results["energy"] = energy.detach().to(device="cpu").numpy()[0, 0]
+            energy_values = energy.detach()
+            energy_values = energy_values.to(device="cpu").to(dtype=torch.float64)
+            self.results["energy"] = energy_values.numpy()[0, 0]
 
         if do_backward:
             energy.backward(-torch.ones_like(energy))
 
         if "forces" in properties:
-            self.results["forces"] = (
-                system.positions.grad.to(device="cpu").numpy().reshape(-1, 3)
-            )
+            forces_values = system.positions.grad.reshape(-1, 3)
+            forces_values = forces_values.to(device="cpu").to(dtype=torch.float64)
+            self.results["forces"] = forces_values.numpy()
 
         if "stress" in properties:
-            volume = atoms.cell.volume
-            scaling_grad = -scaling.grad.to(device="cpu").numpy().reshape(3, 3)
-            self.results["stress"] = _full_3x3_to_voigt_6_stress(scaling_grad / volume)
+            stress_values = -scaling.grad.reshape(3, 3) / atoms.cell.volume
+            stress_values = stress_values.to(device="cpu").to(dtype=torch.float64)
+            self.results["stress"] = _full_3x3_to_voigt_6_stress(stress_values.numpy())
+
+
+def _find_best_device(devices: List[str]) -> torch.device:
+    """
+    Find the best device from the list of ``devices`` that is available to the current
+    PyTorch installation.
+    """
+
+    for device in devices:
+        if device == "cpu":
+            return torch.device("cpu")
+        elif device == "cuda":
+            if torch.cuda.is_available():
+                return torch.device("cuda")
+            else:
+                LOGGER.warning(
+                    "the model suggested to use CUDA devices before CPU, "
+                    "but we are unable to find it"
+                )
+        elif device == "mps":
+            if (
+                hasattr(torch.backends, "mps")
+                and torch.backends.mps.is_built()
+                and torch.backends.mps.is_available()
+            ):
+                return torch.device("mps")
+            else:
+                LOGGER.warning(
+                    "the model suggested to use MPS devices before CPU, "
+                    "but we are unable to find it"
+                )
+        else:
+            warnings.warn(
+                f"unknown device in the model's `supported_devices`: '{device}'",
+                stacklevel=2,
+            )
+
+    warnings.warn(
+        "could not find a valid device in the model's `supported_devices`, "
+        "falling back to CPU",
+        stacklevel=2,
+    )
+    return torch.device("cpu")
 
 
 def _ase_properties_to_metatensor_outputs(properties):
     energy_properties = []
     for p in properties:
         if p in ["energy", "energies", "forces", "stress", "stresses"]:
             energy_properties.append(p)
@@ -300,15 +406,15 @@
 
     if "stresses" in properties:
         output.explicit_gradients = ["cell"]
 
     return {"energy": output}
 
 
-def _compute_ase_neighbors(atoms, options):
+def _compute_ase_neighbors(atoms, options, dtype, device):
     engine_cutoff = options.engine_cutoff(engine_length_unit="angstrom")
     nl = ase.neighborlist.NeighborList(
         cutoffs=[engine_cutoff] * len(atoms),
         skin=0.0,
         sorted=False,
         self_interaction=False,
         bothways=options.full_list,
@@ -329,55 +435,55 @@
 
             distance2 = torch.dot(distance, distance).item()
 
             if distance2 > cutoff2:
                 continue
 
             samples.append((i, j, offset[0], offset[1], offset[2]))
-            distances.append(distance.to(dtype=torch.float64))
+            distances.append(distance.to(dtype=dtype, device=device))
 
     if len(distances) == 0:
-        distances = torch.zeros((0, 3), dtype=positions.dtype)
-        samples = torch.zeros((0, 5))
+        distances = torch.zeros((0, 3), dtype=dtype, device=device)
+        samples = torch.zeros((0, 5), dtype=torch.int32, device=device)
     else:
-        samples = torch.tensor(samples)
+        samples = torch.tensor(samples, device=device)
         distances = torch.vstack(distances)
 
     return TensorBlock(
         values=distances.reshape(-1, 3, 1),
         samples=Labels(
             names=[
                 "first_atom",
                 "second_atom",
                 "cell_shift_a",
                 "cell_shift_b",
                 "cell_shift_c",
             ],
             values=samples,
         ),
-        components=[Labels.range("xyz", 3)],
-        properties=Labels.range("distance", 1),
+        components=[Labels.range("xyz", 3).to(device)],
+        properties=Labels.range("distance", 1).to(device),
     )
 
 
-def _ase_to_torch_data(atoms):
+def _ase_to_torch_data(atoms, dtype, device):
     """Get the positions and cell from ASE atoms as torch tensors"""
 
-    types = torch.from_numpy(atoms.numbers).to(dtype=torch.int32)
-    positions = torch.from_numpy(atoms.positions)
+    types = torch.from_numpy(atoms.numbers).to(dtype=torch.int32, device=device)
+    positions = torch.from_numpy(atoms.positions).to(dtype=dtype, device=device)
 
     if np.all(atoms.pbc):
-        cell = torch.from_numpy(atoms.cell[:])
+        cell = torch.from_numpy(atoms.cell[:]).to(dtype=dtype, device=device)
     elif np.any(atoms.pbc):
         raise ValueError(
             f"partial PBC ({atoms.pbc}) are not currently supported in "
             "metatensor atomistic models"
         )
     else:
-        cell = torch.zeros((3, 3), dtype=torch.float64)
+        cell = torch.zeros((3, 3), dtype=dtype, device=device)
 
     return types, positions, cell
 
 
 def _full_3x3_to_voigt_6_stress(stress):
     ase.stress.full_3x3_to_voigt_6_stress
     """
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/documentation.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/documentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,23 +131,25 @@
         """
 
     def known_neighbors_lists(self) -> List["NeighborsListOptions"]:
         """
         Get all the neighbors lists options registered with this :py:class:`System`
         """
 
-    def add_data(self, name: str, data: TensorBlock):
+    def add_data(self, name: str, data: TensorBlock, override: bool = False):
         """
         Add custom data to this system, stored as :py:class:`TensorBlock`.
 
         This is intended for experimentation with models that need more data as input,
         and moved into a field of ``System`` later.
 
         :param name: name of the custom data
         :param data: values of the custom data
+        :param override: if ``True``, allow this function to override existing data with
+            the same name
         """
 
     def get_data(self, name: str) -> TensorBlock:
         """
         Retrieve custom data stored in this System with the given ``name``, or throw
         an error if no data can be found.
 
@@ -267,27 +269,36 @@
 class ModelCapabilities:
     """Description of a model capabilities, i.e. everything a model can do."""
 
     def __init__(
         self,
         outputs: Dict[str, ModelOutput] = {},  # noqa B006
         atomic_types: List[int] = [],  # noqa B006
-        interaction_range: float = float("inf"),
+        interaction_range: float = -1,
         length_unit: str = "",
         supported_devices: List[str] = [],  # noqa B006
+        dtype: str = "",
     ):
         pass
 
-    outputs: Dict[str, ModelOutput]
-    """
-    All possible outputs from this model and corresponding settings.
+    @property
+    def outputs(self) -> Dict[str, ModelOutput]:
+        """
+        All possible outputs from this model and corresponding settings.
 
-    During a specific run, a model might be asked to only compute a subset of these
-    outputs.
-    """
+        During a specific run, a model might be asked to only compute a subset of these
+        outputs. Some outputs are standardized, and have additional constrains on how
+        the associated metadata should look like, documented in the
+        :ref:`atomistic-models-outputs` section.
+
+        If you want to define a new output for your own usage, it name should looks like
+        ``"<domain>::<output>"``, where ``<domain>`` indicates who defines this new
+        output and ``<output>`` describes the output itself. For example,
+        ``"my-package::foobar"`` for a ``foobar`` output defined in ``my-package``.
+        """
 
     atomic_types: List[int]
     """which atomic types the model can handle"""
 
     interaction_range: float
     """
     How far a given atom needs to know about other atoms, in the length unit of the
@@ -306,14 +317,23 @@
 
         This applies to the ``interaction_range``, any cutoff in neighbors lists, the
         atoms positions and the system cell.
 
         The list of possible units is available :ref:`here <known-quantities-units>`.
         """
 
+    @property
+    def dtype() -> str:
+        """
+        The dtype of this model
+
+        This can be ``"float32"`` or ``"float64"``, and must be used by the engine as
+        the dtype of all inputs and outputs for this model.
+        """
+
     def engine_interaction_range(self, engine_length_unit: str) -> float:
         """
         Same as :py:attr:`interaction_range`, but in the unit of length used by the
         engine.
         """
 
     supported_devices: List[str]
@@ -411,14 +431,33 @@
     This function should be called before :py:func:`torch.jit.load()` when loading an
     existing model.
 
     :param path: path to the exported model file
     """
 
 
+def load_model_extensions(path: str, extensions_directory: Optional[str] = None):
+    """
+    Load the TorchScript extensions (and their dependencies) that the model at ``path``
+    uses.
+
+    If ``extensions_directory`` is provided, we look for the extensions and their
+    dependencies in there first. If this function fails to load some library, it will
+    produce a warning using Torch's warnings infrastructure. Users can set the
+    ``METATENSOR_DEBUG_EXTENSIONS_LOADING`` environment variable to get more
+    informations about a failure in the standard error output.
+
+    :param path: path to the exported model file
+    :param extensions_directory: path to a directory containing the extensions. This
+        directory will typically be created by calling
+        :py:meth:`MetatensorAtomisticModel.export` with
+        ``collect_extensions=extensions_directory``.
+    """
+
+
 def register_autograd_neighbors(
     system: System, neighbors: TensorBlock, check_consistency: bool
 ):
     """
     Register a new autograd node going from (``system.positions``, ``system.cell``) to
     the ``neighbors`` distance vectors.
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/model.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 import datetime
-import hashlib
 import json
+import math
 import os
 import platform
-import shutil
-import site
 import warnings
 from typing import Dict, List, Optional
 
 import torch
 
 from .. import Labels, TensorBlock, TensorMap
 from .. import __version__ as metatensor_version
+from .. import dtype_name
 from . import (
     ModelCapabilities,
     ModelEvaluationOptions,
     ModelMetadata,
     ModelOutput,
     NeighborsListOptions,
     System,
+    check_atomistic_model,
+    load_model_extensions,
     unit_conversion_factor,
 )
+from ._extensions import _collect_extensions
 from .outputs import _check_outputs
 
 
+def load_atomistic_model(path, extensions_directory=None) -> "MetatensorAtomisticModel":
+    """
+    Check and then load the metatensor atomistic model at the given `path`.
+
+    This function calls :py:func:`metatensor.torch.atomistic.check_atomistic_model()`
+    and :py:func:`metatensor.torch.atomistic.load_model_extensions()` before attempting
+    to load the model.
+
+    :param path: path to an exported metatensor model
+    :param extensions_directory: path to a directory containing all extensions required
+        by the exported model
+    """
+    check_atomistic_model(path)
+    load_model_extensions(path, extensions_directory)
+    return torch.jit.load(path)
+
+
 class ModelInterface(torch.nn.Module):
     """
     Interface for models that can be used with :py:class:`MetatensorAtomisticModel`.
 
     There are several requirements that models must satisfy to be usable with
     :py:class:`MetatensorAtomisticModel`. The main one is concerns the
     :py:meth:`forward` function, which must have the signature defined in this
@@ -61,17 +80,21 @@
 
         ``outputs`` will be a subset of the capabilities that where declared when
         exporting the model. For example if a model can compute both an ``"energy"`` and
         a ``"charge"`` output, the simulation engine might only request one them.
 
         The returned dictionary should have the same keys as ``outputs``, and the values
         should contains the corresponding properties of the ``systems``, as computed for
-        the subset of atoms defined in ``selected_atoms``. For some specific outputs,
-        there are additional constrains on how the associated metadata should look like,
-        documented in the :ref:`atomistic-models-outputs` section.
+        the subset of atoms defined in ``selected_atoms``. Some outputs are
+        standardized, and have additional constrains on how the associated metadata
+        should look like, documented in the :ref:`atomistic-models-outputs` section. If
+        you want to define a new output for your own usage, it name should looks like
+        ``"<domain>::<output>"``, where ``<domain>`` indicates who defines this new
+        output and ``<output>`` describes the output itself. For example,
+        ``"my-package::foobar"`` for a ``foobar`` output defined in ``my-package``.
 
         The main use case for ``selected_atoms`` is domain decomposition, where the
         :py:class:`System` given to a model might contain both atoms in the current
         domain and some atoms from other domains; and the calculation should produce
         per-atom output only for the atoms in the domain (but still accounting for atoms
         from the other domains as potential neighbors).
 
@@ -188,14 +211,15 @@
     ...             explicit_gradients=[],
     ...         ),
     ...     },
     ...     atomic_types=[1, 2, 6, 8, 12],
     ...     interaction_range=0.0,
     ...     length_unit="angstrom",
     ...     supported_devices=["cpu"],
+    ...     dtype="float64",
     ... )
     >>> # define metadata about this model
     >>> metadata = ModelMetadata(
     ...     name="model-name",
     ...     authors=["Some Author", "Another One"],
     ...     # references and long description can also be added
     ... )
@@ -252,20 +276,39 @@
         # check that some required capabilities are set
         if capabilities.interaction_range < 0:
             raise ValueError(
                 "`capabilities.interaction_range` was not set, "
                 "but it is required to run simulations"
             )
 
+        if math.isnan(capabilities.interaction_range):
+            raise ValueError(
+                "`capabilities.interaction_range` should be a "
+                "float between 0 and infinity"
+            )
+
         if len(capabilities.supported_devices) == 0:
             raise ValueError(
                 "`capabilities.supported_devices` was not set, "
                 "but it is required to run simulations."
             )
 
+        if capabilities.dtype == "":
+            raise ValueError(
+                "`capabilities.dtype` was not set, "
+                "but it is required to run simulations."
+            )
+
+        if capabilities.dtype == "float32":
+            self._model_dtype = torch.float32
+        elif capabilities.dtype == "float64":
+            self._model_dtype = torch.float64
+        else:
+            raise ValueError(f"unknown dtype in capabilities: {capabilities.dtype}")
+
     def wrapped_module(self) -> torch.nn.Module:
         """Get the module wrapped in this :py:class:`MetatensorAtomisticModel`"""
         return self._module
 
     @torch.jit.export
     def capabilities(self) -> ModelCapabilities:
         """Get the capabilities of the wrapped model"""
@@ -307,18 +350,19 @@
             ``False`` once you are sure everything is running fine.
 
         :return: A dictionary containing all the model outputs
         """
 
         if check_consistency:
             _check_inputs(
-                self._capabilities,
-                self._requested_neighbors_lists,
-                systems,
-                options,
+                capabilities=self._capabilities,
+                requested_neighbors_lists=self._requested_neighbors_lists,
+                systems=systems,
+                options=options,
+                expected_dtype=self._model_dtype,
             )
 
         # convert systems from engine to model units
         if self._capabilities.length_unit != options.length_unit:
             conversion = unit_conversion_factor(
                 quantity="length",
                 from_unit=options.length_unit,
@@ -341,14 +385,15 @@
 
         if check_consistency:
             _check_outputs(
                 systems=systems,
                 requested=options.outputs,
                 selected_atoms=options.selected_atoms,
                 outputs=outputs,
+                expected_dtype=self._model_dtype,
             )
 
         # convert outputs from model to engine units
         for name, output in outputs.items():
             declared = self._capabilities.outputs[name]
             requested = options.outputs[name]
             if declared.quantity == "" or requested.quantity == "":
@@ -393,82 +438,34 @@
             module = torch.jit.script(module)
         except RuntimeError as e:
             raise RuntimeError("could not convert the module to TorchScript") from e
 
         # TODO: can we freeze these?
         # module = torch.jit.freeze(module)
 
-        # record the list of loaded extensions, to check that they are also loaded when
-        # executing the model.
-        if collect_extensions is not None:
-            if os.path.exists(collect_extensions):
-                shutil.rmtree(collect_extensions)
-            os.makedirs(collect_extensions)
-            # TODO: the extensions are currently collected in a separate directory,
-            # should we store the files directly inside the model file? This would makes
-            # the model platform-specific but much more convenient (since the end user
-            # does not have to move a model around)
-
-        extensions = []
-        for library in torch.ops.loaded_libraries:
-            # Remove any site-package prefix
-            path = library
-            for site_packages in site.getsitepackages():
-                if path.startswith(site_packages):
-                    path = os.path.relpath(path, site_packages)
-                    break
-
-            if collect_extensions is not None:
-                collect_path = os.path.join(collect_extensions, path)
-                if os.path.exists(collect_path):
-                    raise RuntimeError(
-                        f"more than one extension would be collected at {collect_path}"
-                    )
-
-                os.makedirs(os.path.dirname(collect_path), exist_ok=True)
-                shutil.copyfile(library, collect_path)
-
-            # get the name of the library, excluding any shared object prefix/suffix
-            name = os.path.basename(library)
-            if name.startswith("lib"):
-                name = name[3:]
-
-            if name.endswith(".so"):
-                name = name[:-3]
-
-            if name.endswith(".dll"):
-                name = name[:-4]
-
-            if name.endswith(".dylib"):
-                name = name[:-6]
-
-            # Collect the hash of the extension shared library. We don't currently use
-            # this, but it would allow for binary-level reproducibility later.
-            with open(library, "rb") as fd:
-                sha256 = hashlib.sha256(fd.read()).hexdigest()
-
-            extensions.append({"path": path, "name": name, "sha256": sha256})
-
         # Metadata about where and when the model was exported
         export_metadata = {
             "date": datetime.datetime.now(datetime.timezone.utc).isoformat(),
             "platform": platform.machine() + "-" + platform.system(),
             # TODO: user/hostname?
         }
 
         if collect_extensions is not None:
             export_metadata["extensions_directory"] = str(collect_extensions)
 
+        extensions, deps = _collect_extensions(extensions_path=collect_extensions)
+
         torch.jit.save(
             module,
             file,
             _extra_files={
                 "torch-version": torch.__version__,
                 "metatensor-version": metatensor_version,
                 "extensions": json.dumps(extensions),
+                "extensions-deps": json.dumps(deps),
                 "metadata": json.dumps(export_metadata),
             },
         )
 
 
 def _get_requested_neighbors_lists(
     module: torch.nn.Module,
@@ -557,21 +554,28 @@
 
 
 def _check_inputs(
     capabilities: ModelCapabilities,
     requested_neighbors_lists: List[NeighborsListOptions],
     systems: List[System],
     options: ModelEvaluationOptions,
+    expected_dtype: torch.dtype,
 ):
     if len(systems) == 0:
         return
 
     global_device = systems[0].device
     global_dtype = systems[0].positions.dtype
 
+    if global_dtype != expected_dtype:
+        raise ValueError(
+            f"wrong dtype for the data: the model wants {dtype_name(expected_dtype)}, "
+            f"we got {dtype_name(global_dtype)}"
+        )
+
     # check that the requested outputs match what the model can do
     for name, requested in options.outputs.items():
         if name not in capabilities.outputs:
             raise ValueError(
                 f"this model can not compute '{name}', the implemented "
                 f"outputs are {capabilities.outputs.keys()}"
             )
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/outputs.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/outputs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 from typing import Dict, List, Optional
 
 import torch
 
-from .. import Labels, TensorMap
+from .. import Labels, TensorMap, dtype_name
 from . import ModelOutput, System
 
 
 def _check_outputs(
     systems: List[System],
     requested: Dict[str, ModelOutput],
     selected_atoms: Optional[Labels],
     outputs: Dict[str, TensorMap],
+    expected_dtype: torch.dtype,
 ):
     """
     Check that the outputs of a model conform to the expected structure for metatensor
     atomistic models.
 
     This function checks conformance with the reference documentation in
     https://lab-cosmo.github.io/metatensor/latest/atomistic/outputs.html
     """
 
-    for name in outputs.keys():
+    for name, output in outputs.items():
         if requested.get(name) is None:
             raise ValueError(
                 f"the model produced an output named '{name}', which was not requested"
             )
 
+        if len(output) != 0:
+            output_dtype = output.block_by_id(0).values.dtype
+            if output_dtype != expected_dtype:
+                raise ValueError(
+                    f"wrong dtype for the {name} output: "
+                    f"the model promised {dtype_name(expected_dtype)}, "
+                    f"we got {dtype_name(output_dtype)}"
+                )
+
     for name, request in requested.items():
         value = outputs.get(name)
         if value is None:
             raise ValueError(
                 f"the model did not produce the '{name}' output, which was requested"
             )
 
         if name == "energy":
             _check_energy(systems, request, selected_atoms, energy=value)
         else:
+            # this is a non-standard output, there is nothing to check
             continue
 
 
 def _check_energy(
     systems: List[System],
     request: ModelOutput,
     selected_atoms: Optional[Labels],
@@ -47,14 +58,15 @@
 ):
     """Check the "energy" output metadata"""
     if energy.keys != Labels("_", torch.tensor([[0]])):
         raise ValueError(
             "invalid keys for 'energy' output: expected `Labels('_', [[0]])`"
         )
 
+    device = energy.device
     energy_block = energy.block_by_id(0)
 
     if request.per_atom:
         expected_samples_names = ["system", "atom"]
     else:
         expected_samples_names = ["system"]
 
@@ -67,26 +79,30 @@
     # check samples values from systems & selected_atoms
     if request.per_atom:
         expected_values: List[List[int]] = []
         for s, system in enumerate(systems):
             for a in range(len(system)):
                 expected_values.append([s, a])
 
-        expected_samples = Labels(["system", "atom"], torch.tensor(expected_values))
+        expected_samples = Labels(
+            ["system", "atom"], torch.tensor(expected_values, device=device)
+        )
         if selected_atoms is not None:
             expected_samples = expected_samples.intersection(selected_atoms)
 
         if len(expected_samples.union(energy_block.samples)) != len(expected_samples):
             raise ValueError(
                 "invalid samples entries for 'energy' output, they do not match the "
                 f"`systems` and `selected_atoms`. Expected samples:\n{expected_samples}"
             )
 
     else:
-        expected_samples = Labels("system", torch.arange(len(systems)).reshape(-1, 1))
+        expected_samples = Labels(
+            "system", torch.arange(len(systems), device=device).reshape(-1, 1)
+        )
         if selected_atoms is not None:
             selected_systems = Labels(
                 "system", torch.unique(selected_atoms.column("system")).reshape(-1, 1)
             )
             expected_samples = expected_samples.intersection(selected_systems)
 
         if len(expected_samples.union(energy_block.samples)) != len(expected_samples):
@@ -96,44 +112,45 @@
             )
 
     if len(energy_block.components) != 0:
         raise ValueError(
             "invalid components for 'energy' output: components should be empty"
         )
 
-    if energy_block.properties != Labels("energy", torch.tensor([[0]])):
+    if energy_block.properties != Labels("energy", torch.tensor([[0]], device=device)):
         raise ValueError(
             "invalid properties for 'energy' output: expected `Labels('energy', [[0]])`"
         )
 
     for parameter, gradient in energy_block.gradients():
         if parameter not in ["strain", "positions"]:
             raise ValueError(f"invalid gradient for 'energy' output: {parameter}")
 
+        xyz = torch.tensor([[0], [1], [2]], device=device)
         # strain gradient checks
         if parameter == "strain":
             if gradient.samples.names != ["sample"]:
                 raise ValueError(
                     "invalid samples for 'energy' output 'strain' gradients: "
                     f"expected the names to be ['sample'], got {gradient.samples.names}"
                 )
 
             if len(gradient.components) != 2:
                 raise ValueError(
                     "invalid components for 'energy' output 'strain' gradients: "
                     "expected two components"
                 )
 
-            if gradient.components[0] != Labels("xyz_1", torch.tensor([[0], [1], [2]])):
+            if gradient.components[0] != Labels("xyz_1", xyz):
                 raise ValueError(
                     "invalid components for 'energy' output 'strain' gradients: "
                     "expected Labels('xyz_1', [[0], [1], [2]]) for the first component"
                 )
 
-            if gradient.components[1] != Labels("xyz_2", torch.tensor([[0], [1], [2]])):
+            if gradient.components[1] != Labels("xyz_2", xyz):
                 raise ValueError(
                     "invalid components for 'energy' output 'strain' gradients: "
                     "expected Labels('xyz_2', [[0], [1], [2]]) for the second component"
                 )
 
         # positions gradient checks
         if parameter == "positions":
@@ -146,12 +163,12 @@
 
             if len(gradient.components) != 1:
                 raise ValueError(
                     "invalid components for 'energy' output 'positions' gradients: "
                     "expected one component"
                 )
 
-            if gradient.components[0] != Labels("xyz", torch.tensor([[0], [1], [2]])):
+            if gradient.components[0] != Labels("xyz", xyz):
                 raise ValueError(
                     "invalid components for 'energy' output 'positions' gradients: "
                     "expected Labels('xyz', [[0], [1], [2]]) for the first component"
                 )
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/atomistic/systems_to_torch.py` & `metatensor-torch-0.4.0/metatensor/torch/atomistic/systems_to_torch.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.3.0/metatensor/torch/documentation.py` & `metatensor-torch-0.4.0/metatensor/torch/documentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,14 +515,18 @@
             42
         )
         """
 
     def to(self, device: Union[str, torch.device]) -> "Labels":
         """move the values for these Labels to the given ``device``"""
 
+    @property
+    def device(self) -> torch.device:
+        """get the current device used for the values of these Labels"""
+
     def position(
         self, entry: Union[LabelsEntry, torch.Tensor, List[int], Tuple[int, ...]]
     ) -> Optional[int]:
         """
         Get the position of the given ``entry`` in this set of
         :py:class:`Labels`, or ``None`` if the entry is not present in the
         labels.
@@ -1237,14 +1241,27 @@
             this is set to ``None``.
         :param arrays: new backend to use for the arrays. This parameter is here for
             compatibility with the pure Python API, can only be set  to ``"torch"`` or
             ``None`` and does nothing.
         """
 
 
+def version() -> str:
+    """Get the version of the underlying metatensor_torch library"""
+
+
+def dtype_name(dtype: torch.dtype) -> str:
+    """
+    Get the name of a dtype.
+
+    This is intended to be used in error message in TorchScript mode, where all dtypes
+    are converted to integers.
+    """
+
+
 def load(path: str) -> TensorMap:
     """
     Load a previously saved :py:class:`TensorMap` from the given path.
 
     :py:class:`TensorMap` are serialized using numpy's ``.npz`` format, i.e. a
     ZIP file without compression (storage method is ``STORED``), where each file
     is stored as a ``.npy`` array. See the C API documentation for more
```

### Comparing `metatensor-torch-0.3.0/metatensor/torch/learn.py` & `metatensor-torch-0.4.0/metatensor/torch/learn.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.3.0/metatensor/torch/operations.py` & `metatensor-torch-0.4.0/metatensor/torch/operations.py`

 * *Files identical despite different names*

### Comparing `metatensor-torch-0.3.0/metatensor_torch.egg-info/PKG-INFO` & `metatensor-torch-0.4.0/metatensor_torch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metatensor-torch
-Version: 0.3.0
+Version: 0.4.0
 Summary: TorchScript bindings for metatensor
 Author: Guillaume Fraux, Davide Tisi, Philip Loche, Joseph W. Abbott, Jigyasa Nigam, Chiheb Ben Mahmoud
 License: BSD-3-Clause
 Project-URL: homepage, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: documentation, https://lab-cosmo.github.io/metatensor/latest/
 Project-URL: repository, https://github.com/lab-cosmo/metatensor
 Project-URL: changelog, https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html
@@ -23,14 +23,14 @@
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: torch>=1.11
+Requires-Dist: torch>=1.12
 Requires-Dist: metatensor-core<0.2.0,>=0.1.0
 
 metatensor-torch
 ================
 
 This package contains the TorchScript bindings to the core API of metatensor.
```

### Comparing `metatensor-torch-0.3.0/metatensor_torch.egg-info/SOURCES.txt` & `metatensor-torch-0.4.0/metatensor_torch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.rst
-metatensor-torch-cxx-0.3.0.tar.gz
+metatensor-torch-cxx-0.4.0.tar.gz
 n_commits_since_last_tag
 pyproject.toml
 setup.py
 build-backend/backend.py
 metatensor/torch/__init__.py
 metatensor/torch/_c_lib.py
 metatensor/torch/documentation.py
 metatensor/torch/learn.py
 metatensor/torch/operations.py
 metatensor/torch/utils.py
 metatensor/torch/version.py
 metatensor/torch/atomistic/__init__.py
+metatensor/torch/atomistic/_extensions.py
 metatensor/torch/atomistic/ase_calculator.py
 metatensor/torch/atomistic/documentation.py
 metatensor/torch/atomistic/model.py
 metatensor/torch/atomistic/outputs.py
 metatensor/torch/atomistic/systems_to_torch.py
 metatensor_torch.egg-info/PKG-INFO
 metatensor_torch.egg-info/SOURCES.txt
```

### Comparing `metatensor-torch-0.3.0/pyproject.toml` & `metatensor-torch-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,20 +32,20 @@
 changelog = "https://lab-cosmo.github.io/metatensor/latest/torch/CHANGELOG.html"
 
 ### ======================================================================== ###
 [build-system]
 requires = [
     "setuptools >=68",
     "packaging >=23",
-    "cmake",
-    "torch >= 1.11",
+    "wheel >=0.41",
 ]
 
-# use a custom build backend to add a dependency on the right version of
-# metatensor-core
+# use a custom build backend to :
+# - add a dependency on the right version of metatensor-core
+# - only depend on torch/cmake when building the wheel and not the sdist
 build-backend = "backend"
 backend-path = ["build-backend"]
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
```

### Comparing `metatensor-torch-0.3.0/setup.py` & `metatensor-torch-0.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,22 +5,36 @@
 import uuid
 
 import packaging.version
 from setuptools import Extension, setup
 from setuptools.command.bdist_egg import bdist_egg
 from setuptools.command.build_ext import build_ext
 from setuptools.command.sdist import sdist
+from wheel.bdist_wheel import bdist_wheel
 
 
 ROOT = os.path.realpath(os.path.dirname(__file__))
 METATENSOR_CORE = os.path.realpath(os.path.join(ROOT, "..", "metatensor-core"))
 
 METATENSOR_TORCH = os.path.join(ROOT, "..", "..", "metatensor-torch")
 
 
+class universal_wheel(bdist_wheel):
+    # When building the wheel, the `wheel` package assumes that if we have a
+    # binary extension then we are linking to `libpython.so`; and thus the wheel
+    # is only usable with a single python version. This is not the case for
+    # here, and the wheel will be compatible with any Python >=3. This is
+    # tracked in https://github.com/pypa/wheel/issues/185, but until then we
+    # manually override the wheel tag.
+    def get_tag(self):
+        tag = bdist_wheel.get_tag(self)
+        # tag[2:] contains the os/arch tags, we want to keep them
+        return ("py3", "none") + tag[2:]
+
+
 class cmake_ext(build_ext):
     """Build the native library using cmake"""
 
     def run(self):
         import torch
 
         import metatensor
@@ -33,17 +47,25 @@
 
         # Tell CMake where to find metatensor & torch
         cmake_prefix_path = [
             metatensor.utils.cmake_prefix_path,
             torch.utils.cmake_prefix_path,
         ]
 
+        # Install the shared library in a prefix matching the torch version used to
+        # compile the code. This allows having multiple version of this shared library
+        # inside the wheel; and dynamically pick the right one.
+        torch_major, torch_minor, *_ = torch.__version__.split(".")
+        cmake_install_prefix = os.path.join(
+            install_dir, f"torch-{torch_major}.{torch_minor}"
+        )
+
         cmake_options = [
             "-DCMAKE_BUILD_TYPE=Release",
-            f"-DCMAKE_INSTALL_PREFIX={install_dir}",
+            f"-DCMAKE_INSTALL_PREFIX={cmake_install_prefix}",
             f"-DCMAKE_PREFIX_PATH={';'.join(cmake_prefix_path)}",
         ]
 
         # ==================================================================== #
         # HACK: Torch cmake build system has a hard time finding CuDNN, so we
         # help it by pointing it to the right files
 
@@ -81,33 +103,28 @@
             check=True,
         )
         subprocess.run(
             [
                 "cmake",
                 "--build",
                 build_dir,
+                "--parallel",
                 "--config",
                 "Release",
                 "--target",
                 "install",
             ],
             check=True,
         )
 
         with open(os.path.join(install_dir, "_build_versions.py"), "w") as fd:
             fd.write("# Autogenerated file, do not edit\n\n\n")
-            # Store the version of torch used to build the extension, to give a
+            # Store the version of metatensor used to build the extension, to give a
             # nice error message to the user when trying to load the extension
-            # with an older torch version installed
-            fd.write(
-                "# version of torch used when compiling this package\n"
-                f"BUILD_TORCH_VERSION = '{torch.__version__}'\n\n"
-            )
-
-            # same for metatensor-core
+            # with an incompatible version
             fd.write(
                 "# version of metatensor-core used when compiling this package\n"
                 f"BUILD_METATENSOR_CORE_VERSION = '{metatensor.__version__}'\n"
             )
 
 
 class bdist_egg_disabled(bdist_egg):
@@ -121,28 +138,65 @@
         sys.exit(
             "Aborting implicit building of eggs.\nUse `pip install .` or "
             "`python -m build --wheel . && pip install dist/metatensor_torch-*.whl` "
             "to install from source."
         )
 
 
-class sdist_git_version(sdist):
+class sdist_generate_data(sdist):
     """
-    Create a sdist with an additional generated file containing the extra
-    version from git.
+    Create a sdist with an additional generated files:
+        - `n_commits_since_last_tag`
+        - `metatensor-torch-cxx-*.tar.gz`
     """
 
     def run(self):
         with open("n_commits_since_last_tag", "w") as fd:
             fd.write(str(n_commits_since_last_tag()))
 
+        generate_cxx_tar()
+
         # run original sdist
         super().run()
 
         os.unlink("n_commits_since_last_tag")
+        for path in glob.glob("metatensor-torch-cxx*.tar.gz"):
+            os.unlink(path)
+
+
+def generate_cxx_tar():
+    script = os.path.join(ROOT, "..", "..", "scripts", "package-torch.sh")
+    assert os.path.exists(script)
+
+    try:
+        output = subprocess.run(
+            ["bash", "--version"],
+            stderr=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            encoding="utf8",
+        )
+    except Exception as e:
+        raise RuntimeError("could not run `bash`, is it installed?") from e
+
+    stderr = ""
+    stdout = ""
+
+    output = subprocess.run(
+        ["bash", script, os.getcwd()],
+        stderr=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        encoding="utf8",
+    )
+    if output.returncode != 0:
+        stderr = output.stderr
+        stdout = output.stdout
+        raise RuntimeError(
+            "failed to collect C++ sources for Python sdist\n"
+            f"stdout:\n {stdout}\n\nstderr:\n {stderr}"
+        )
 
 
 def n_commits_since_last_tag():
     """
     If git is available and we are building from a checkout, get the number of commits
     since the last tag. Otherwise, this always returns 0.
     """
@@ -233,15 +287,15 @@
         authors = fd.read().splitlines()
 
     if authors[0].startswith(".."):
         # handle "raw" symlink files (on Windows or from full repo tarball)
         with open(os.path.join(ROOT, authors[0])) as fd:
             authors = fd.read().splitlines()
 
-    install_requires = ["torch >= 1.11"]
+    install_requires = ["torch >= 1.12"]
 
     # when packaging a sdist for release, we should never use local dependencies
     METATENSOR_NO_LOCAL_DEPS = os.environ.get("METATENSOR_NO_LOCAL_DEPS", "0") == "1"
 
     if not METATENSOR_NO_LOCAL_DEPS and os.path.exists(METATENSOR_CORE):
         # we are building from a git checkout
 
@@ -259,17 +313,18 @@
         install_requires=install_requires,
         ext_modules=[
             Extension(name="metatensor_torch", sources=[]),
         ],
         cmdclass={
             "build_ext": cmake_ext,
             "bdist_egg": bdist_egg if "bdist_egg" in sys.argv else bdist_egg_disabled,
-            "sdist": sdist_git_version,
+            "bdist_wheel": universal_wheel,
+            "sdist": sdist_generate_data,
         },
         package_data={
             "metatensor-torch": [
-                "metatensor/torch/bin/*",
-                "metatensor/torch/lib/*",
-                "metatensor/torch/include/*",
+                "metatensor/torch*/bin/*",
+                "metatensor/torch*/lib/*",
+                "metatensor/torch*/include/*",
             ]
         },
     )
```

