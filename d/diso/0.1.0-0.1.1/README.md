# Comparing `tmp/diso-0.1.0.tar.gz` & `tmp/diso-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diso-0.1.0.tar", last modified: Wed Feb 28 02:39:30 2024, max compression
+gzip compressed data, was "diso-0.1.1.tar", last modified: Wed Apr 10 05:22:26 2024, max compression
```

## Comparing `diso-0.1.0.tar` & `diso-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-02-28 02:39:30.712146 diso-0.1.0/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      185 2024-02-23 23:52:16.000000 diso-0.1.0/LICENSE
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       13 2024-02-23 23:52:16.000000 diso-0.1.0/MANIFEST.in
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-02-28 02:39:30.712146 diso-0.1.0/PKG-INFO
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     5121 2024-02-23 23:52:16.000000 diso-0.1.0/README.md
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-02-28 02:39:30.712146 diso-0.1.0/diso/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     6145 2024-02-23 23:52:16.000000 diso-0.1.0/diso/__init__.py
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-02-28 02:39:30.712146 diso-0.1.0/diso.egg-info/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-02-28 02:39:30.000000 diso-0.1.0/diso.egg-info/PKG-INFO
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      290 2024-02-28 02:39:30.000000 diso-0.1.0/diso.egg-info/SOURCES.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-02-28 02:39:30.000000 diso-0.1.0/diso.egg-info/dependency_links.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-02-28 02:36:02.000000 diso-0.1.0/diso.egg-info/not-zip-safe
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        8 2024-02-28 02:39:30.000000 diso-0.1.0/diso.egg-info/requires.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        5 2024-02-28 02:39:30.000000 diso-0.1.0/diso.egg-info/top_level.txt
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       38 2024-02-28 02:39:30.712146 diso-0.1.0/setup.cfg
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     2596 2024-02-28 02:39:15.000000 diso-0.1.0/setup.py
-drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-02-28 02:39:30.712146 diso-0.1.0/src/
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    49634 2024-02-23 23:52:16.000000 diso-0.1.0/src/cudualmc.cu
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4597 2024-02-23 23:52:16.000000 diso-0.1.0/src/cudualmc.h
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    36173 2024-02-23 23:52:16.000000 diso-0.1.0/src/cumc.cu
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4282 2024-02-23 23:52:16.000000 diso-0.1.0/src/cumc.h
--rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    15997 2024-02-23 23:52:16.000000 diso-0.1.0/src/pybind.cpp
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-10 05:22:26.338735 diso-0.1.1/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      185 2024-04-08 20:12:31.000000 diso-0.1.1/LICENSE
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       13 2024-04-08 20:12:31.000000 diso-0.1.1/MANIFEST.in
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-04-10 05:22:26.338735 diso-0.1.1/PKG-INFO
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     5047 2024-04-08 20:12:31.000000 diso-0.1.1/README.md
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-10 05:22:26.338735 diso-0.1.1/diso/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     6365 2024-04-09 18:45:02.000000 diso-0.1.1/diso/__init__.py
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-10 05:22:26.338735 diso-0.1.1/diso.egg-info/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     1027 2024-04-10 05:22:26.000000 diso-0.1.1/diso.egg-info/PKG-INFO
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)      290 2024-04-10 05:22:26.000000 diso-0.1.1/diso.egg-info/SOURCES.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-04-10 05:22:26.000000 diso-0.1.1/diso.egg-info/dependency_links.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        1 2024-04-09 18:45:17.000000 diso-0.1.1/diso.egg-info/not-zip-safe
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        8 2024-04-10 05:22:26.000000 diso-0.1.1/diso.egg-info/requires.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)        5 2024-04-10 05:22:26.000000 diso-0.1.1/diso.egg-info/top_level.txt
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)       38 2024-04-10 05:22:26.338735 diso-0.1.1/setup.cfg
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     2596 2024-04-10 05:21:50.000000 diso-0.1.1/setup.py
+drwxrwxr-x   0 sarahwei  (1000) sarahwei  (1000)        0 2024-04-10 05:22:26.338735 diso-0.1.1/src/
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    49634 2024-04-08 20:12:31.000000 diso-0.1.1/src/cudualmc.cu
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4597 2024-04-08 20:12:31.000000 diso-0.1.1/src/cudualmc.h
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    36173 2024-04-08 20:12:31.000000 diso-0.1.1/src/cumc.cu
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)     4282 2024-04-08 20:12:31.000000 diso-0.1.1/src/cumc.h
+-rw-rw-r--   0 sarahwei  (1000) sarahwei  (1000)    15997 2024-04-08 20:12:31.000000 diso-0.1.1/src/pybind.cpp
```

### Comparing `diso-0.1.0/PKG-INFO` & `diso-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diso
-Version: 0.1.0
+Version: 0.1.1
 Summary: Differentiable Iso-Surface Extraction Package
 Author-email: xiwei@ucsd.edu
 License: CC BY-NC 4.0
 Keywords: differentiable iso-surface extraction
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `diso-0.1.0/README.md` & `diso-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 # Quick Start
 You can effortlessly try the following command, which converts a sphere SDF into triangle mesh using different algorithms. The generated results are saved in `out/`.
 ```
 python test/example.py
 ```
 
 Note:
-* `DiffMC` generates guaranteed watertight manifold meshes w/ or w/o grid deformation.
-* `DiffDMC` generates watertight manifold meshes when grid deformation is disabled. When enabling grid deformation, self-intersection may occur, but the face connectivity remains manifold.
+* `DiffMC` and `DiffDMC` generate watertight manifold meshes when grid deformation is disabled. When enabling grid deformation, self-intersection may occur, but the face connectivity remains manifold.
 * `DiffDMC` can produce a more uniform triangle distribution and smoother surfaces than `DiffMC` and supports generating quad meshes (in the example, the quad is automatically divided into two triangles by `trimesh`).
 
 <p align="center">
   <img src="imgs/example.png" alt="four_examples" width="600" />
 </p>
 
 # Usage
@@ -103,8 +102,8 @@
 # Reference
 [1] We L S. Marching cubes: A high resolution 3d surface construction algorithm[J]. Comput Graph, 1987, 21: 163-169.
 
 [2] Nielson G M. Dual marching cubes[C]//IEEE visualization 2004. IEEE, 2004: 489-496.
 
 [3] Shen T, Gao J, Yin K, et al. Deep marching tetrahedra: a hybrid representation for high-resolution 3d shape synthesis[J]. Advances in Neural Information Processing Systems, 2021, 34: 6087-6101.
 
-[4] Shen T, Munkberg J, Hasselgren J, et al. Flexible isosurface extraction for gradient-based mesh optimization[J]. ACM Transactions on Graphics (TOG), 2023, 42(4): 1-16.
+[4] Shen T, Munkberg J, Hasselgren J, et al. Flexible isosurface extraction for gradient-based mesh optimization[J]. ACM Transactions on Graphics (TOG), 2023, 42(4): 1-16.
```

### Comparing `diso-0.1.0/diso/__init__.py` & `diso-0.1.1/diso/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import torch.nn.functional as F
 from torch.autograd import Function
 
 from . import _C
 
 
 class DiffMC(nn.Module):
-    def __init__(self, dtype=torch.float32):
+    def __init__(self, dtype=torch.float32, device="cuda:0"):
         super().__init__()
         self.dtype = dtype
         if dtype == torch.float32:
             mc = _C.CUMCFloat()
         elif dtype == torch.float64:
             mc = _C.CUMCDouble()
+        torch.cuda.set_device(device)
 
         class DMCFunction(Function):
             @staticmethod
             def forward(ctx, grid, deform, isovalue):
                 if deform is None:
                     verts, tris = mc.forward(grid, isovalue)
                 else:
@@ -40,36 +41,38 @@
                     mc.backward(
                         ctx.grid, ctx.deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
                     )
                     return adj_grid, adj_deform, None, None, None
 
         self.func = DMCFunction
 
-    def forward(self, grid, deform=None, isovalue=0.0):
+    def forward(self, grid, deform=None, isovalue=0.0, device="cuda:0"):
+        torch.cuda.set_device(device)
         if grid.min() >= 0 or grid.max() <= 0:
             return torch.zeros((0, 3), dtype=self.dtype, device=grid.device), torch.zeros((0, 3), dtype=torch.int32, device=grid.device)
         dimX, dimY, dimZ = grid.shape
         grid = F.pad(grid, (1, 1, 1, 1, 1, 1), "constant", 1)
         if deform is not None:
             deform = F.pad(deform, (0, 0, 1, 1, 1, 1, 1, 1), "constant", 0)
         verts, tris = self.func.apply(grid, deform, isovalue)
         verts = verts - 1
         verts = verts / (
             torch.tensor([dimX, dimY, dimZ], dtype=verts.dtype, device=verts.device) - 1
         )
         return verts, tris.long()
 
 class DiffDMC(nn.Module):
-    def __init__(self, dtype=torch.float32):
+    def __init__(self, dtype=torch.float32, device="cuda:0"):
         super().__init__()
         self.dtype = dtype
         if dtype == torch.float32:
             dmc = _C.CUDMCFloat()
         elif dtype == torch.float64:
             dmc = _C.CUDMCDouble()
+        torch.cuda.set_device(device)
 
         class DDMCFunction(Function):
             @staticmethod
             def forward(ctx, grid, deform, isovalue):
                 if deform is None:
                     verts, quads = dmc.forward(grid, isovalue)
                 else:
@@ -92,15 +95,16 @@
                     dmc.backward(
                         ctx.grid, ctx.deform, ctx.isovalue, adj_verts, adj_grid, adj_deform
                     )
                     return adj_grid, adj_deform, None, None, None
 
         self.func = DDMCFunction
 
-    def forward(self, grid, deform=None, isovalue=0.0, return_quads=False):
+    def forward(self, grid, deform=None, isovalue=0.0, return_quads=False, device="cuda:0"):
+        torch.cuda.set_device(device)
         if grid.min() >= 0 or grid.max() <= 0:
             return torch.zeros((0, 3), dtype=self.dtype, device=grid.device), torch.zeros((0, 4), dtype=torch.int32, device=grid.device)
         dimX, dimY, dimZ = grid.shape
         grid = F.pad(grid, (1, 1, 1, 1, 1, 1), "constant", 1)
         if deform is not None:
             deform = F.pad(deform, (0, 0, 1, 1, 1, 1, 1, 1), "constant", 0)
         verts, quads = self.func.apply(grid, deform, isovalue)
```

### Comparing `diso-0.1.0/diso.egg-info/PKG-INFO` & `diso-0.1.1/diso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diso
-Version: 0.1.0
+Version: 0.1.1
 Summary: Differentiable Iso-Surface Extraction Package
 Author-email: xiwei@ucsd.edu
 License: CC BY-NC 4.0
 Keywords: differentiable iso-surface extraction
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
```

### Comparing `diso-0.1.0/setup.py` & `diso-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             extra_compile_args=extra_compile_args,
         )
     ]
     return ext_modules
 
 setup(
     name="diso",
-    version="0.1.0",
+    version="0.1.1",
     author_email="xiwei@ucsd.edu",
     keywords="differentiable iso-surface extraction",
     description="Differentiable Iso-Surface Extraction Package",
     classifiers=[
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Intended Audience :: Developers",
```

### Comparing `diso-0.1.0/src/cudualmc.cu` & `diso-0.1.1/src/cudualmc.cu`

 * *Files identical despite different names*

### Comparing `diso-0.1.0/src/cudualmc.h` & `diso-0.1.1/src/cudualmc.h`

 * *Files identical despite different names*

### Comparing `diso-0.1.0/src/cumc.cu` & `diso-0.1.1/src/cumc.cu`

 * *Files identical despite different names*

### Comparing `diso-0.1.0/src/cumc.h` & `diso-0.1.1/src/cumc.h`

 * *Files identical despite different names*

### Comparing `diso-0.1.0/src/pybind.cpp` & `diso-0.1.1/src/pybind.cpp`

 * *Files identical despite different names*

