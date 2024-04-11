# Comparing `tmp/jo3mnist-0.0.4.tar.gz` & `tmp/jo3mnist-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jo3mnist-0.0.4.tar", last modified: Sun Apr  7 08:56:07 2024, max compression
+gzip compressed data, was "jo3mnist-0.0.5.tar", last modified: Thu Apr 11 10:30:45 2024, max compression
```

## Comparing `jo3mnist-0.0.4.tar` & `jo3mnist-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,23 @@
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/
--rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/LICENSE
--rw-r--r--   0 gum       (1001) gum       (1001)     1012 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      391 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/README.md
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.174342 jo3mnist-0.0.4/jo3mnist/
--rw-r--r--   0 gum       (1001) gum       (1001)       86 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/jo3mnist/__main__.py
--rw-r--r--   0 gum       (1001) gum       (1001)      883 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/data.py
--rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/jo3mnist/equinox.py
--rw-r--r--   0 gum       (1001) gum       (1001)     3608 2024-04-07 08:53:42.000000 jo3mnist-0.0.4/jo3mnist/tiny_imagenet.py
--rw-r--r--   0 gum       (1001) gum       (1001)     1211 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/vis.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/jo3mnist.egg-info/
--rw-r--r--   0 gum       (1001) gum       (1001)     1012 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      420 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        1 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1001) gum       (1001)       81 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/requires.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        9 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/top_level.txt
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/mnist/
--rw-r--r--   0 gum       (1001) gum       (1001)       86 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/mnist/__main__.py
--rw-r--r--   0 gum       (1001) gum       (1001)      883 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/data.py
--rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/mnist/equinox.py
--rw-r--r--   0 gum       (1001) gum       (1001)     1211 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/vis.py
--rw-r--r--   0 gum       (1001) gum       (1001)     1025 2024-04-07 08:55:33.000000 jo3mnist-0.0.4/pyproject.toml
--rw-r--r--   0 gum       (1001) gum       (1001)       38 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/setup.cfg
--rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/setup.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/tests/
--rw-r--r--   0 gum       (1001) gum       (1001)      396 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/tests/test_main.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-04-11 10:30:45.466642 jo3mnist-0.0.5/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1069 2023-09-20 11:05:23.000000 jo3mnist-0.0.5/LICENSE
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1036 2024-04-11 10:30:45.466642 jo3mnist-0.0.5/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      391 2023-09-20 11:05:24.000000 jo3mnist-0.0.5/README.md
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-04-11 10:30:45.463308 jo3mnist-0.0.5/jo3mnist/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       86 2023-09-24 10:45:19.000000 jo3mnist-0.0.5/jo3mnist/__init__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     6946 2023-09-20 11:05:54.000000 jo3mnist-0.0.5/jo3mnist/__main__.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      883 2024-01-02 10:24:52.000000 jo3mnist-0.0.5/jo3mnist/data.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     4528 2023-09-23 14:57:44.000000 jo3mnist-0.0.5/jo3mnist/equinox.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1613 2024-04-11 09:31:42.000000 jo3mnist-0.0.5/jo3mnist/imagenet.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     3604 2024-04-11 09:04:34.000000 jo3mnist-0.0.5/jo3mnist/tiny_imagenet.py
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1211 2023-09-24 10:45:58.000000 jo3mnist-0.0.5/jo3mnist/vis.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-04-11 10:30:45.463308 jo3mnist-0.0.5/jo3mnist.egg-info/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1036 2024-04-11 10:30:45.000000 jo3mnist-0.0.5/jo3mnist.egg-info/PKG-INFO
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      361 2024-04-11 10:30:45.000000 jo3mnist-0.0.5/jo3mnist.egg-info/SOURCES.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        1 2024-04-11 10:30:45.000000 jo3mnist-0.0.5/jo3mnist.egg-info/dependency_links.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       90 2024-04-11 10:30:45.000000 jo3mnist-0.0.5/jo3mnist.egg-info/requires.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)        9 2024-04-11 10:30:45.000000 jo3mnist-0.0.5/jo3mnist.egg-info/top_level.txt
+-rw-r--r--   0 jo3       (1000) jo3       (1000)     1041 2024-04-11 10:29:50.000000 jo3mnist-0.0.5/pyproject.toml
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       38 2024-04-11 10:30:45.466642 jo3mnist-0.0.5/setup.cfg
+-rw-r--r--   0 jo3       (1000) jo3       (1000)       61 2023-09-20 11:05:24.000000 jo3mnist-0.0.5/setup.py
+drwxr-xr-x   0 jo3       (1000) jo3       (1000)        0 2024-04-11 10:30:45.463308 jo3mnist-0.0.5/tests/
+-rw-r--r--   0 jo3       (1000) jo3       (1000)      396 2023-09-20 11:05:24.000000 jo3mnist-0.0.5/tests/test_main.py
```

### Comparing `jo3mnist-0.0.4/LICENSE` & `jo3mnist-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.4/PKG-INFO` & `jo3mnist-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: jo3mnist
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/mnist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datasets
 Requires-Dist: equinox
 Requires-Dist: jax
 Requires-Dist: jaxtyping
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: optax
```

### Comparing `jo3mnist-0.0.4/jo3mnist/__main__.py` & `jo3mnist-0.0.5/jo3mnist/__main__.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.4/jo3mnist/data.py` & `jo3mnist-0.0.5/jo3mnist/data.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.4/jo3mnist/equinox.py` & `jo3mnist-0.0.5/jo3mnist/equinox.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.4/jo3mnist/tiny_imagenet.py` & `jo3mnist-0.0.5/jo3mnist/tiny_imagenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,33 +89,31 @@
         else:
             tensor = np.load(tensor_path)
 
         return tensor, label
 
 
 class TinyImageTestNet(Dataset):
-
     def __init__(self, root_dir):
         self.dir = Path(root_dir)
 
         with (self.dir / "val_annotations.txt").open() as f:
             labels = [line.split("\t")[1] for line in f.readlines()]
         label2idx = list(set(labels))
         label2idx.sort()
         label2idx = {l: i for i, l in enumerate(label2idx)}
         self.labels = [label2idx[label] for label in labels]
 
     def __len__(self):
         return len(self.labels)
 
     def __getitem__(self, idx):
-        tensor_path = self.dir / "tensors" / f"test_{idx}.npy"
+        tensor_path = self.dir / "tensors" / f"val_{idx}.npy"
         if not tensor_path.exists():
             tensor_path.parent.mkdir(exist_ok=True)
-            image_path = self.dir / "images" / f"test_{idx}.JPEG"
+            image_path = self.dir / "images" / f"val_{idx}.JPEG"
             tensor = preprocess_image(image_path)
             np.save(tensor_path, tensor, allow_pickle=False)
         else:
             tensor = np.load(tensor_path)
 
         return tensor, self.labels[idx]
-
```

### Comparing `jo3mnist-0.0.4/jo3mnist/vis.py` & `jo3mnist-0.0.5/jo3mnist/vis.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.4/jo3mnist.egg-info/PKG-INFO` & `jo3mnist-0.0.5/jo3mnist.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: jo3mnist
-Version: 0.0.4
+Version: 0.0.5
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/mnist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: datasets
 Requires-Dist: equinox
 Requires-Dist: jax
 Requires-Dist: jaxtyping
 Requires-Dist: numpy
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: optax
```

### Comparing `jo3mnist-0.0.4/pyproject.toml` & `jo3mnist-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 [project]
 name = "jo3mnist"
-version = "0.0.4" # TODO; automatically update versions by looking at git
+version = "0.0.5" # TODO; automatically update versions by looking at git
 description = ""
 dependencies = [
+    "datasets",
     "equinox",
     "jax",
     "jaxtyping",
     "numpy",
     "pillow",
     "opencv-python",
     "optax",
```

