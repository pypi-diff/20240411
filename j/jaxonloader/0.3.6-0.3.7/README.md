# Comparing `tmp/jaxonloader-0.3.6.tar.gz` & `tmp/jaxonloader-0.3.7.tar.gz`

## Comparing `jaxonloader-0.3.6.tar` & `jaxonloader-0.3.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/config.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/README.md
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/config.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/README.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 jaxonloader-0.3.7/PKG-INFO
```

### Comparing `jaxonloader-0.3.6/.github/workflows/nox.yaml` & `jaxonloader-0.3.7/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/docs/getting-started.md` & `jaxonloader-0.3.7/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/docs/index.md` & `jaxonloader-0.3.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/docs/images/performance.png` & `jaxonloader-0.3.7/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/jaxonloader/config.py` & `jaxonloader-0.3.7/jaxonloader/config.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/jaxonloader/dataloader.py` & `jaxonloader-0.3.7/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/jaxonloader/dataset.py` & `jaxonloader-0.3.7/jaxonloader/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from abc import ABC, abstractmethod
-from typing import Union
 
-from jaxtyping import Int
+from beartype.typing import Union
+from jaxtyping import Array, Int
 from numpy import ndarray as NDArray
 
 
 class JaxonDataset(ABC):
     @abstractmethod
     def __len__(self) -> int:
         raise NotImplementedError()
 
     @abstractmethod
     def __getitem__(
-        self, idx: Int[NDArray, " batch_size"] | slice | int
-    ) -> Union[NDArray, tuple[NDArray, ...]]:
+        self, idx: Int[Array | NDArray, " batch_size"] | slice | int
+    ) -> Union[Array | NDArray, tuple[Array | NDArray, ...]]:
         raise NotImplementedError()
 
     def split(self, ratio: float) -> tuple["JaxonDataset", "JaxonDataset"]:
         raise NotImplementedError()
 
 
 class SingleArrayDataset(JaxonDataset):
-    def __init__(self, data: NDArray):
+    def __init__(self, data: Array | NDArray):
         self.data = data
 
     def __len__(self) -> int:
         return len(self.data)
 
     def __getitem__(self, idx):
         return self.data[idx]
@@ -34,15 +34,15 @@
         split = int(len(self.data) * ratio)
         return SingleArrayDataset(self.data[:split]), SingleArrayDataset(
             self.data[split:]
         )
 
 
 class DataTargetDataset(JaxonDataset):
-    def __init__(self, data: NDArray, target: NDArray):
+    def __init__(self, data: Array | NDArray, target: Array | NDArray):
         self.data = data
         self.target = target
         if len(data) != len(target):
             raise ValueError("data and target must have the same length")
 
     def __len__(self) -> int:
         return len(self.data)
```

### Comparing `jaxonloader-0.3.6/jaxonloader/utils.py` & `jaxonloader-0.3.7/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.3.7/jaxonloader/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/jaxonloader/datasets/download.py` & `jaxonloader-0.3.7/jaxonloader/datasets/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 from jaxonloader.utils import (
     get_data_path,
     jaxonloader_cache,
 )
 
 
 @jaxonloader_cache(dataset_name="mnist")
-def download_mnist(*, target_path: Optional[str]) -> Path:
+def download_mnist(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("mnist", target_path)
 
 
 @jaxonloader_cache(dataset_name="titanic")
-def download_titanic(*, target_path: Optional[str]) -> Path:
+def download_titanic(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("titanic", target_path)
 
 
 @jaxonloader_cache(dataset_name="hms")
-def download_hms(*, target_path: Optional[str]) -> Path:
+def download_hms(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("hms", target_path)
 
 
 @jaxonloader_cache(dataset_name="cifar10")
-def download_cifar10(*, target_path: Optional[str]) -> Path:
+def download_cifar10(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("cifar10", target_path)
 
 
 @jaxonloader_cache(dataset_name="cifar100")
-def download_cifar100(*, target_path: Optional[str]) -> Path:
+def download_cifar100(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("cifar100", target_path)
 
 
 @jaxonloader_cache(dataset_name="tinyshakespeare")
-def download_tinyshakespeare(*, target_path: Optional[str]) -> Path:
+def download_tinyshakespeare(*, target_path: Optional[str] = None) -> Path:
     return get_data_path("tinyshakespeare", target_path)
```

### Comparing `jaxonloader-0.3.6/tests/test_tinyshakespeare.py` & `jaxonloader-0.3.7/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/.gitignore` & `jaxonloader-0.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/LICENSE` & `jaxonloader-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/README.md` & `jaxonloader-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.6/pyproject.toml` & `jaxonloader-0.3.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "jaxonloader"
-version = "0.3.6"
+version = "0.3.7"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
 dependencies=[
-  "tqdm",
   "jaxtyping",
   "progressbar",
   "polars",
   "beartype",
   "typing_extensions",
   "loguru",
-  "kaggle",
   "pyarrow",
   "boto3",
-  "boto3-stubs"
+  "boto3-stubs",
+  "jax",
+  "jaxlib"
 ]
 [project.optional-dependencies]
 dev = [
     "nox",
     "pre-commit",
     "pytest",
     "mkdocs",
```

### Comparing `jaxonloader-0.3.6/PKG-INFO` & `jaxonloader-0.3.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.6
+Version: 0.3.7
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -25,21 +25,21 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: ~=3.10
 Requires-Dist: beartype
 Requires-Dist: boto3
 Requires-Dist: boto3-stubs
+Requires-Dist: jax
+Requires-Dist: jaxlib
 Requires-Dist: jaxtyping
-Requires-Dist: kaggle
 Requires-Dist: loguru
 Requires-Dist: polars
 Requires-Dist: progressbar
 Requires-Dist: pyarrow
-Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Description-Content-Type: text/markdown
```

