# Comparing `tmp/interpolation-2.2.4.tar.gz` & `tmp/interpolation-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpolation-2.2.4.tar", max compression
+gzip compressed data, was "interpolation-2.2.6.tar", max compression
```

## Comparing `interpolation-2.2.4.tar` & `interpolation-2.2.6.tar`

### file list

```diff
@@ -1,45 +1,48 @@
--rw-r--r--   0        0        0     1345 2022-09-21 14:19:42.954569 interpolation-2.2.4/LICENSE
--rw-r--r--   0        0        0      243 2022-09-21 14:19:42.954569 interpolation-2.2.4/README.md
--rw-r--r--   0        0        0       51 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/__init__.py
--rw-r--r--   0        0        0     2566 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/cartesian.py
--rw-r--r--   0        0        0      437 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/compat.py
--rw-r--r--   0        0        0    19591 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/complete_poly.py
--rw-r--r--   0        0        0        0 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/multilinear/__init__.py
--rw-r--r--   0        0        0     6897 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/multilinear/fungen.py
--rw-r--r--   0        0        0     6632 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/multilinear/mlinterp.py
--rw-r--r--   0        0        0     5044 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/multilinear/tests/test_multilinear.py
--rw-r--r--   0        0        0      106 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/__init__.py
--rw-r--r--   0        0        0    25964 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/grid.py
--rw-r--r--   0        0        0     5203 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/interp.py
--rw-r--r--   0        0        0        0 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/tests/__init__.py
--rw-r--r--   0        0        0     1780 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/tests/test_derivatives.py
--rw-r--r--   0        0        0     3328 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/tests/test_interp.py
--rw-r--r--   0        0        0     1061 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/smolyak/util.py
--rw-r--r--   0        0        0     1099 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/splines/__init__.py
--rw-r--r--   0        0        0      814 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/splines/basis_splines.py
--rw-r--r--   0        0        0    12535 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/splines/codegen.py
--rw-r--r--   0        0        0     5551 2022-09-21 14:19:42.954569 interpolation-2.2.4/interpolation/splines/eval_cubic.py
--rw-r--r--   0        0        0   396689 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/eval_cubic_numba.py
--rw-r--r--   0        0        0     8550 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/eval_splines.py
--rw-r--r--   0        0        0     6232 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/filter_cubic.py
--rw-r--r--   0        0        0     4058 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/hermite.py
--rw-r--r--   0        0        0     5318 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/multilinear.py
--rw-r--r--   0        0        0      641 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/multilinear_numba.py
--rw-r--r--   0        0        0      959 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/option_types.py
--rw-r--r--   0        0        0     9844 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/prefilter_cubic.py
--rw-r--r--   0        0        0     7070 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/splines.py
--rw-r--r--   0        0        0        0 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/__init__.py
--rw-r--r--   0        0        0     2529 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_cubic_splines.py
--rw-r--r--   0        0        0     2834 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_derivatives.py
--rw-r--r--   0        0        0     1677 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_eval_splines.py
--rw-r--r--   0        0        0     1440 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_fortran_order.py
--rw-r--r--   0        0        0      718 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_hermite_splines.py
--rw-r--r--   0        0        0     1675 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_multilinear_extrap.py
--rw-r--r--   0        0        0     2253 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_object_api.py
--rw-r--r--   0        0        0      846 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/splines/tests/test_readonly.py
--rw-r--r--   0        0        0        0 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/tests/__init__.py
--rw-r--r--   0        0        0     2527 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/tests/test_complete.py
--rw-r--r--   0        0        0     5051 2022-09-21 14:19:42.958569 interpolation-2.2.4/interpolation/tests/test_derivs.py
--rw-r--r--   0        0        0      736 2022-09-21 14:19:42.962569 interpolation-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 interpolation-2.2.4/setup.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 interpolation-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1345 2024-04-11 17:44:16.643436 interpolation-2.2.6/LICENSE
+-rw-r--r--   0        0        0      243 2024-04-11 17:44:16.643436 interpolation-2.2.6/README.md
+-rw-r--r--   0        0        0       51 2024-04-11 17:44:16.643436 interpolation-2.2.6/interpolation/__init__.py
+-rw-r--r--   0        0        0     2566 2024-04-11 17:44:16.643436 interpolation-2.2.6/interpolation/cartesian.py
+-rw-r--r--   0        0        0      202 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/compat.py
+-rw-r--r--   0        0        0    19590 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/complete_poly.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/multilinear/__init__.py
+-rw-r--r--   0        0        0     7095 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/multilinear/fungen.py
+-rw-r--r--   0        0        0     6708 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/multilinear/mlinterp.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/multilinear/tests/__init__.py
+-rw-r--r--   0        0        0     5202 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/multilinear/tests/test_multilinear.py
+-rw-r--r--   0        0        0      106 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/__init__.py
+-rw-r--r--   0        0        0    25964 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/grid.py
+-rw-r--r--   0        0        0     5203 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/interp.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/tests/__init__.py
+-rw-r--r--   0        0        0     1779 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/tests/test_derivatives.py
+-rw-r--r--   0        0        0     3326 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/tests/test_interp.py
+-rw-r--r--   0        0        0     1061 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/smolyak/util.py
+-rw-r--r--   0        0        0     1100 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/basis_splines.py
+-rw-r--r--   0        0        0    12523 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/codegen.py
+-rw-r--r--   0        0        0     5692 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/eval_cubic.py
+-rw-r--r--   0        0        0   396657 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/eval_cubic_numba.py
+-rw-r--r--   0        0        0     7876 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/eval_splines.py
+-rw-r--r--   0        0        0     6224 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/filter_cubic.py
+-rw-r--r--   0        0        0     4084 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/hermite.py
+-rw-r--r--   0        0        0     5313 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/multilinear.py
+-rw-r--r--   0        0        0      639 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/multilinear_numba.py
+-rw-r--r--   0        0        0      959 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/option_types.py
+-rw-r--r--   0        0        0     9802 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/prefilter_cubic.py
+-rw-r--r--   0        0        0     7068 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/splines.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/__init__.py
+-rw-r--r--   0        0        0     2524 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_cubic_splines.py
+-rw-r--r--   0        0        0     2713 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_derivatives.py
+-rw-r--r--   0        0        0     1676 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_eval_splines.py
+-rw-r--r--   0        0        0     1438 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_fortran_order.py
+-rw-r--r--   0        0        0      716 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_hermite_splines.py
+-rw-r--r--   0        0        0     1674 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_multilinear_extrap.py
+-rw-r--r--   0        0        0     2248 2024-04-11 17:44:16.647436 interpolation-2.2.6/interpolation/splines/tests/test_object_api.py
+-rw-r--r--   0        0        0      844 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/splines/tests/test_readonly.py
+-rw-r--r--   0        0        0    43479 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tempita/__init__.py
+-rw-r--r--   0        0        0     4120 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tempita/_looper.py
+-rw-r--r--   0        0        0      907 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tempita/compat3.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tests/__init__.py
+-rw-r--r--   0        0        0     2526 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tests/test_complete.py
+-rw-r--r--   0        0        0     5024 2024-04-11 17:44:16.651436 interpolation-2.2.6/interpolation/tests/test_derivs.py
+-rw-r--r--   0        0        0      652 2024-04-11 17:44:16.651436 interpolation-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 interpolation-2.2.6/PKG-INFO
```

### Comparing `interpolation-2.2.4/LICENSE` & `interpolation-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/cartesian.py` & `interpolation-2.2.6/interpolation/cartesian.py`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/complete_poly.py` & `interpolation-2.2.6/interpolation/complete_poly.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,10 +605,9 @@
             self.coefs = (1 - damp) * new_coefs + damp * self.coefs
 
     def der(self, s, der):
         dPhi = complete_polynomial_der(s.T, self.d, der).T
         return np.dot(dPhi, self.coefs)
 
     def __call__(self, s):
-
         Phi = complete_polynomial(s.T, self.d).T
         return np.dot(Phi, self.coefs)
```

### Comparing `interpolation-2.2.4/interpolation/multilinear/fungen.py` & `interpolation-2.2.6/interpolation/multilinear/fungen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numba
 import numpy as np
 from numba import float64, int64
-from numba import generated_jit, njit
+from numba import njit
 import ast
 
 from numba.extending import overload
 from ..compat import Array, Tuple, UniTuple
 from ..compat import overload_options
 
 
@@ -21,16 +21,20 @@
 
 @njit
 def clamp(x, a, b):
     return min(b, max(a, x))
 
 
 # returns the index of a 1d point along a 1d dimension
-@generated_jit(nopython=True)
 def get_index(gc, x):
+    pass
+
+
+@overload(get_index)
+def ol_get_index(gc, x):
     if gc == t_coord:
         # regular coordinate
         def fun(gc, x):
             δ = (gc[1] - gc[0]) / (gc[2] - 1)
             d = x - gc[0]
             ii = d // δ
             i = int(ii)
@@ -49,16 +53,20 @@
             λ = (x - gc[i]) / (gc[i + 1] - gc[i])
             return (i, λ)
 
         return fun
 
 
 # returns number of dimension of a dimension
-@generated_jit(nopython=True)
 def get_size(gc):
+    pass
+
+
+@overload(get_size)
+def ol_get_size(gc):
     if gc == t_coord:
         # regular coordinate
         def fun(gc):
             return gc[2]
 
         return fun
     else:
@@ -89,15 +97,14 @@
 
 def fmap():
     pass
 
 
 @overload(fmap, **overload_options)
 def _map(*args):
-
     if len(args) == 2 and isinstance(args[1], (Tuple, UniTuple)):
         k = len(args[1])
         s = "def __map(f, t): return ({}, )".format(
             str.join(", ", ["f(t[{}])".format(i) for i in range(k)])
         )
     elif len(args) == 3 and isinstance(args[1], (Tuple, UniTuple)):
         k = len(args[1])
@@ -142,16 +149,20 @@
 # @njit
 # def fmap(*args):
 #     return _fmap(*args)
 #
 # funzip(((1,2), (2,3), (4,3))) -> ((1,2,4),(2,3,3))
 
 
-@generated_jit(nopython=True)
 def funzip(t):
+    pass
+
+
+@overload(funzip)
+def ol_funzip(t):
     k = t.count
     assert len(set([e.count for e in t.types])) == 1
     l = t.types[0].count
 
     def print_tuple(t):
         return "({},)".format(str.join(", ", t))
 
@@ -166,16 +177,20 @@
 # array subscribing:
 # when X is a 2d array and I=(i,j) a 2d index, `get_coeffs(X,I)`
 # extracts `X[i:i+1,j:j+1]` but represents it as a tuple of tuple, so that
 # the number of its elements can be inferred by the compiler
 #####
 
 
-@generated_jit(nopython=True)
 def get_coeffs(X, I):
+    pass
+
+
+@overload(get_coeffs)
+def ol_get_coeffs(X, I):
     if X.ndim > len(I):
         print("not implemented yet")
     else:
         from itertools import product
 
         d = len(I)
         mat = np.array(
@@ -197,14 +212,15 @@
         return fun
 
 
 # tensor_reduction(C,l)
 # (in 2d) computes the equivalent of np.einsum('ij,i,j->', C, [1-l[0],l[0]], [1-l[1],l[1]])`
 # but where l is a tuple and C a tuple of tuples.
 
+
 # this one is a temporary implementation (should be merged with old gen_splines* code)
 def gen_tensor_reduction(X, symbs, inds=[]):
     if len(symbs) == 0:
         return "{}[{}]".format(X, str.join("][", [str(e) for e in inds]))
     else:
         h = symbs[0]
         q = symbs[1:]
@@ -214,38 +230,50 @@
                 gen_tensor_reduction(X, q, inds + [i]),
             )
             for i in range(2)
         ]
         return str.join(" + ", exprs)
 
 
-@generated_jit(nopython=True)
 def tensor_reduction(C, l):
+    pass
+
+
+@overload(tensor_reduction)
+def ol_tensor_reduction(C, l):
     d = len(l.types)
     ex = gen_tensor_reduction("C", ["l[{}]".format(i) for i in range(d)])
     dd = dict()
     s = "def tensor_reduction(C,l): return {}".format(ex)
     eval(compile(ast.parse(s), "<string>", "exec"), dd)
     return dd["tensor_reduction"]
 
 
-@generated_jit(nopython=True)
 def extract_row(a, n, tup):
+    pass
+
+
+@overload(extract_row)
+def ol_extract_row(a, n, tup):
     d = len(tup.types)
     dd = {}
     s = "def extract_row(a, n, tup): return ({},)".format(
         str.join(", ", [f"a[n,{i}]" for i in range(d)])
     )
     eval(compile(ast.parse(s), "<string>", "exec"), dd)
     return dd["extract_row"]
 
 
 # find closest point inside the grid domain
-@generated_jit
 def project(grid, point):
+    pass
+
+
+@overload(project)
+def ol_project(grid, point):
     s = "def __project(grid, point):\n"
     d = len(grid.types)
     for i in range(d):
         if isinstance(grid.types[i], Array):
             s += f"    x_{i} = min(max(point[{i}], grid[{i}][0]), grid[{i}][grid[{i}].shape[0]-1])\n"
         else:
             s += f"    x_{i} = min(max(point[{i}], grid[{i}][0]), grid[{i}][1])\n"
```

### Comparing `interpolation-2.2.4/interpolation/multilinear/mlinterp.py` & `interpolation-2.2.6/interpolation/multilinear/mlinterp.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,41 +25,45 @@
     tensor_reduction,
     get_index,
     extract_row,
     project,
 )
 
 from numba import njit
+from numba.extending import overload
 from typing import Tuple
 
 from ..compat import UniTuple, Tuple, Float, Integer, Array
 
 Scalar = (Float, Integer)
 
 import numpy as np
-from numba import generated_jit
 
 # logic of multilinear interpolation
 
 
-@generated_jit
-def mlinterp(grid, c, u):
+def _mlinterp(grid, c, u):
+    pass
+
+
+@overload(_mlinterp)
+def ol_mlinterp(grid, c, u):
     if isinstance(u, UniTuple):
 
-        def mlininterp(grid: Tuple, c: Array, u: Tuple) -> float:
+        def mlininterp(grid, c, u):
             # get indices and barycentric coordinates
             tmp = fmap(get_index, grid, u)
             indices, barycenters = funzip(tmp)
             coeffs = get_coeffs(c, indices)
             v = tensor_reduction(coeffs, barycenters)
             return v
 
     elif isinstance(u, Array) and u.ndim == 2:
 
-        def mlininterp(grid: Tuple, c: Array, u: Array) -> float:
+        def mlininterp(grid, c, u):
             N = u.shape[0]
             res = np.zeros(N)
             for n in range(N):
                 uu = extract_row(u, n, grid)
                 # get indices and barycentric coordinates
                 tmp = fmap(get_index, grid, uu)
                 indices, barycenters = funzip(tmp)
@@ -68,23 +72,27 @@
             return res
 
     else:
         mlininterp = None
     return mlininterp
 
 
+@njit
+def mlinterp(grid, c, u):
+    return _mlinterp(grid, c, u)
+
+
 ### The rest of this file constrcts function `interp`
 
 from collections import namedtuple
 
 itt = namedtuple("InterpType", ["d", "values", "eval"])
 
 
 def detect_types(args):
-
     dims = [e.ndim if isinstance(e, Array) else -1 for e in args]
 
     md = max(dims)
 
     if len(args) == 3:
         d = 1
         i_C = 1
@@ -123,15 +131,14 @@
         else:
             raise Exception("Undetected evaluation type.")
 
     return itt(d, values_type, eval_type)
 
 
 def make_mlinterp(it, funname):
-
     if it.values == "vector":
         return None
 
     if it.eval in ("scalar", "tuple") and it.values == "vector":
         # raise Exception("Non supported. (return type unknown)")
         return None
 
@@ -211,25 +218,28 @@
     return res
 """
         else:
             return None
         return source
 
 
-from numba import generated_jit
-
-
-@generated_jit(nopython=True)
-def interp(*args):
+def _interp(*args):
+    pass
 
-    aa = args[0].types
 
-    it = detect_types(aa)
+@overload(_interp)
+def ol_interp(*args):
+    it = detect_types(args)
     if it.d == 1 and it.eval == "point":
         it = itt(it.d, it.values, "cartesian")
     source = make_mlinterp(it, "__mlinterp")
     import ast
 
     tree = ast.parse(source)
     code = compile(tree, "<string>", "exec")
     eval(code, globals())
     return __mlinterp
+
+
+@njit
+def interp(*args):
+    return _interp(*args)
```

### Comparing `interpolation-2.2.4/interpolation/multilinear/tests/test_multilinear.py` & `interpolation-2.2.6/interpolation/multilinear/tests/test_multilinear.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from numpy import linspace, array
 from numpy.random import random
 from numba import typeof
+from numba import njit
 
 import numpy as np
-from interpolation.multilinear.fungen import get_index
+from ..fungen import get_index
 
 
-def test_barycentric_indexes():
+@njit
+def get_index_njit(gc, x):
+    return get_index(gc, x)
+
 
+def test_barycentric_indexes():
     # irregular grid
     gg = np.array([0.0, 1.0])
-    assert get_index(gg, -0.1) == (0, -0.1)
-    assert get_index(gg, 0.5) == (0, 0.5)
-    assert get_index(gg, 1.1) == (0, 1.1)
+    assert get_index_njit(gg, -0.1) == (0, -0.1)
+    assert get_index_njit(gg, 0.5) == (0, 0.5)
+    assert get_index_njit(gg, 1.1) == (0, 1.1)
 
     # regular grid
     gg = (0.0, 1.0, 2)
-    assert get_index(gg, -0.1) == (0, -0.1)
-    assert get_index(gg, 0.5) == (0, 0.5)
-    assert get_index(gg, 1.1) == (0, 1.1)
+    assert get_index_njit(gg, -0.1) == (0, -0.1)
+    assert get_index_njit(gg, 0.5) == (0, 0.5)
+    assert get_index_njit(gg, 1.1) == (0, 1.1)
 
 
 # 2d-vecev-scalar
 a2 = (linspace(0, 1, 10), random((10)), random((200, 1)))
 # 2d-pointev-scalar
 a3 = (linspace(0, 1, 10), random((10)), array([0.5]))
 # 2d-tupev-scalar
@@ -90,15 +95,14 @@
 tests = [a2, a3, a4, c1, c2, c3, c4]
 tests_failing = [b1, b2, b3, b4, b5, d4, d5, d1, d2, d3, d4, d5]
 
 from interpolation.multilinear.mlinterp import mlinterp, interp
 
 
 def test_mlinterp():
-
     # simple multilinear interpolation api
 
     import numpy as np
     from interpolation import mlinterp
 
     # from interpolation.multilinear.mlinterp import mlininterp, mlininterp_vec
     x1 = np.linspace(0, 1, 10)
@@ -107,27 +111,29 @@
 
     z1 = np.linspace(0, 1, 30)
     z2 = np.linspace(0, 1, 30)
 
     pp = np.random.random((2000, 2))
 
     res0 = mlinterp((x1, x2), y, pp)
+    assert res0 is not None
+
     res0 = mlinterp((x1, x2), y, (0.1, 0.2))
+    assert res0 is not None
 
 
 def test_multilinear():
-
     # flat flexible api
 
     for t in tests:
-
         tt = [typeof(e) for e in t]
-        print(tt)
         rr = interp(*t)
 
+        assert rr is not None
+
         try:
             print(f"{tt}: {rr.shape}")
         except:
             print(f"{tt}: OK")
 
 
 #
```

### Comparing `interpolation-2.2.4/interpolation/smolyak/grid.py` & `interpolation-2.2.6/interpolation/smolyak/grid.py`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/smolyak/interp.py` & `interpolation-2.2.6/interpolation/smolyak/interp.py`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/smolyak/tests/test_derivatives.py` & `interpolation-2.2.6/interpolation/smolyak/tests/test_derivatives.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_derivatives():
-
     from ..interp import SmolyakInterp
     from ..grid import SmolyakGrid
 
     d = 5
     N = 100
     mu = 2
     f = lambda x: (x).sum(axis=1)
```

### Comparing `interpolation-2.2.4/interpolation/smolyak/tests/test_interp.py` & `interpolation-2.2.6/interpolation/smolyak/tests/test_interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,12 @@
 
 
 # functions starting with test_ are
 # discovered and automatically run by nosetests
 
 
 def test_interp_2d():
-
     interp_2d(2, 3, func1)
 
 
 def test_interp_2d1():
-
     interp_2d1(2, 3, func1)
```

### Comparing `interpolation-2.2.4/interpolation/smolyak/util.py` & `interpolation-2.2.6/interpolation/smolyak/util.py`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/splines/__init__.py` & `interpolation-2.2.6/interpolation/splines/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .eval_splines import options, eval_linear, eval_cubic, eval_spline
 from .prefilter_cubic import filter_cubic, prefilter
 from .option_types import options as extrap_options
 
 import numba
 import numpy as np
 
+
 # dummy functions
 def UCGrid(*args):
     tt = numba.typeof((10.0, 1.0, 1))
     for a in args:
         assert numba.typeof(a) == tt
         min, max, n = a
         assert min < max
```

### Comparing `interpolation-2.2.4/interpolation/splines/basis_splines.py` & `interpolation-2.2.6/interpolation/splines/basis_splines.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 def B0(u, i, x):
-
     if u[i] <= x < u[i + 1]:
         return 1.0
     else:
         return 0.0
 
 
 def B(p, u, i, x):
-
     if p == 0:
         return B0(u, i, x)
     else:
         return ((x - u[i]) / (u[i + p] - u[i])) * B(p - 1, u, i, x) + (
             (u[i + p + 1] - x) / (u[i + p + 1] - u[i + 1])
         ) * B(p - 1, u, i + 1, x)
```

### Comparing `interpolation-2.2.4/interpolation/splines/codegen.py` & `interpolation-2.2.6/interpolation/splines/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import tempita
+from .. import tempita
 
 import numpy as np
 from numpy import floor
 from numba import njit
 from typing import Callable
 from math import floor
 
 
 def gen_trex(l, c: Callable, inds=[]):
-
     """Generate expression for tensor reduction"""
     # l = [
     #     ('a_0', 'a_1'),
     #     ('b_0', 'b_1', 'b_2')
     # ]
     # c = lambda i,j: 'C_{}_{}'.format(i,j)
     # gen_tr(l, c)
@@ -26,15 +25,14 @@
         exprs = [
             "{}*({})".format(h[i], gen_trex(q, c, inds=inds + [i])) for i in range(k)
         ]
         return str.join(" + ", exprs)
 
 
 def get_values(d, multispline=False, k=4, i_x="i_x", diffs=None):
-
     if diffs is None:
         diffs = (0,) * d
 
     l = []
     for i, diff in enumerate(diffs):
         if diff == 0:
             tt = tuple(["Φ_{}_{}".format(i, ik) for ik in range(k)])
@@ -98,16 +96,15 @@
 d_Φ_{i}_{1} = 1.0/δ_{i}"""
         else:
             s = f"""
 d_{l}_Φ_{i}_{0} = 0.0
 d_{l}_Φ_{i}_{1} = 0.0"""
 
     elif k == 3:
-
-        import tempita
+        from .. import tempita
 
         if l == 0:
             template_0 = """
 μ_{{i}}_0 = λ_{{i}}*λ_{{i}}*λ_{{i}};  μ_{{i}}_1 = λ_{{i}}*λ_{{i}};  μ_{{i}}_2 = λ_{{i}};  μ_{{i}}_3 = 1.0;
         """
             phi = lambda i, j: "Φ_{}_{}".format(i, j)
         elif l == 1:
@@ -146,15 +143,15 @@
 
 ##############
 # Templates  #
 ##############
 
 
 eval_template = """
-def eval_spline(grid, C, points, out=None, order=1, diff="None", extrap_mode='linear'):
+def eval_spline(grid, C, points, out=None, k=1, diff="None", extrap_mode='linear'):
     "This is my docstring"
 
     {{if vector_valued}}
     n_vals = C.shape[{{d}}]
         {{if allocate}}
             {{if orders is None}}
     out = zeros(n_vals)
@@ -290,15 +287,15 @@
 
     {{endif}}
 
     {{endif}}
 """
 
 eval_template_vectorized = """
-def eval_spline(grid, C, points, out=None, order=1, diff="None", extrap_mode='linear'):
+def eval_spline(grid, C, points, out=None, k=1, diff="None", extrap_mode='linear'):
     "This is my docstring"
 
     N = points.shape[0]
 
     {{if vector_valued}}
     n_vals = C.shape[{{d}}]
     {{endif}}
@@ -414,28 +411,25 @@
         {{endif}}
         
     {{if allocate}}
     return out
     {{endif}}
 """
 
-import tempita
-
 
 def get_code_spline(
     d,
     k=1,
     vector_valued=False,
     vectorized=False,
     allocate=False,
     grid_types=None,
     extrap_mode=None,
     orders=None,
 ):
-
     if orders is None:
         bases_orders = [(0,)] * d
     else:
         bases_orders = [sorted(list(set(e))) for e in zip(*orders)]
 
     if grid_types is None:
         grid_types = ["uniform"] * d
```

### Comparing `interpolation-2.2.4/interpolation/splines/eval_cubic.py` & `interpolation-2.2.6/interpolation/splines/eval_cubic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import numpy
 
+from numba import njit
+from numba.extending import overload
 from .eval_splines import eval_cubic
 
 ## the functions in this file provide backward compatibility calls
 ##
 ## they can optionnally allocate memory for the result
 ## they work for any dimension, except the functions which compute the gradient
 
 #######################
 # Compatibility calls #
 #######################
 
-from numba import generated_jit
 from .codegen import source_to_function
 
 
-@generated_jit
-def get_grid(a, b, n, C):
+def _get_grid(a, b, n, C):
+    pass
+
+
+@overload(_get_grid)
+def ol_get_grid(a, b, n, C):
     d = C.ndim
     s = "({},)".format(str.join(", ", [f"(a[{k}],b[{k}],n[{k}])" for k in range(d)]))
     txt = "def get_grid(a,b,n,C): return {}".format(s)
     f = source_to_function(txt)
     return f
 
 
+@njit
+def get_grid(a, b, n, C):
+    return _get_grid(a, b, n, C)
+
+
 def eval_cubic_spline(a, b, orders, coefs, point):
     """Evaluates a cubic spline at one point
 
     Parameters:
     -----------
     a : array of size d (float)
         Lower bounds of the cartesian grid.
@@ -150,15 +160,14 @@
     vec_eval_cubic_splines_G_2,
     vec_eval_cubic_splines_G_3,
     vec_eval_cubic_splines_G_4,
 )
 
 
 def vec_eval_cubic_splines_G(a, b, orders, mcoefs, points, values=None, dvalues=None):
-
     a = numpy.array(a, dtype=float)
     b = numpy.array(b, dtype=float)
     orders = numpy.array(orders, dtype=int)
 
     d = a.shape[0]
     N = points.shape[0]
     n_sp = mcoefs.shape[-1]
```

### Comparing `interpolation-2.2.4/interpolation/splines/eval_cubic_numba.py` & `interpolation-2.2.6/interpolation/splines/eval_cubic_numba.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 #        values[n] = eval_cubic_spline_4(a, b, orders, coefs, point)
 #
 #
 
 
 @njit(cache=True)
 def eval_cubic_spline_1(a, b, orders, coefs, point):
-
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     x0 = point[0]
     u0 = (x0 - start0) * dinv0
     i0 = int(floor(u0))
     i0 = max(min(i0, M0 - 2), 0)
@@ -134,15 +133,14 @@
         + Phi0_3 * (coefs[i0 + 3])
     )
     return t
 
 
 @njit(cache=True)
 def eval_cubic_spline_2(a, b, orders, coefs, point):
-
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
     x0 = point[0]
@@ -266,15 +264,14 @@
         )
     )
     return t
 
 
 @njit(cache=True)
 def eval_cubic_spline_3(a, b, orders, coefs, point):
-
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
     M2 = orders[2]
@@ -542,15 +539,14 @@
         )
     )
     return t
 
 
 @njit(cache=True)
 def eval_cubic_spline_4(a, b, orders, coefs, point):
-
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
     M2 = orders[2]
@@ -1250,20 +1246,18 @@
         )
     )
     return t
 
 
 @njit(cache=True)
 def vec_eval_cubic_spline_1(a, b, orders, coefs, points, out):
-
     d = a.shape[0]
     N = points.shape[0]
 
     for n in range(N):
-
         x0 = points[n, 0]
         M0 = orders[0]
         start0 = a[0]
         dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
@@ -1326,20 +1320,18 @@
             + Phi0_2 * (coefs[i0 + 2])
             + Phi0_3 * (coefs[i0 + 3])
         )
 
 
 @njit(cache=True)
 def vec_eval_cubic_spline_2(a, b, orders, coefs, points, out):
-
     d = a.shape[0]
     N = points.shape[0]
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         M0 = orders[0]
         start0 = a[0]
         dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
         M1 = orders[1]
         start1 = a[1]
@@ -1486,20 +1478,18 @@
                 + Phi1_3 * (coefs[i0 + 3, i1 + 3])
             )
         )
 
 
 @njit(cache=True)
 def vec_eval_cubic_spline_3(a, b, orders, coefs, points, out):
-
     d = a.shape[0]
     N = points.shape[0]
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         M0 = orders[0]
         start0 = a[0]
         dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
         M1 = orders[1]
@@ -1802,20 +1792,18 @@
                 )
             )
         )
 
 
 @njit(cache=True)
 def vec_eval_cubic_spline_4(a, b, orders, coefs, points, out):
-
     d = a.shape[0]
     N = points.shape[0]
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         x3 = points[n, 3]
         M0 = orders[0]
         start0 = a[0]
         dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
@@ -2562,15 +2550,14 @@
                 )
             )
         )
 
 
 @njit(cache=True)
 def eval_cubic_splines_1(a, b, orders, coefs, point, vals):
-
     n_vals = coefs.shape[1]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     x0 = point[0]
     u0 = (x0 - start0) * dinv0
@@ -2624,15 +2611,14 @@
             + Phi0_2 * (coefs[i0 + 2, k])
             + Phi0_3 * (coefs[i0 + 3, k])
         )
 
 
 @njit(cache=True)
 def eval_cubic_splines_2(a, b, orders, coefs, point, vals):
-
     n_vals = coefs.shape[2]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
@@ -2758,15 +2744,14 @@
                 + Phi1_3 * (coefs[i0 + 3, i1 + 3, k])
             )
         )
 
 
 @njit(cache=True)
 def eval_cubic_splines_3(a, b, orders, coefs, point, vals):
-
     n_vals = coefs.shape[3]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
@@ -3036,15 +3021,14 @@
                 )
             )
         )
 
 
 @njit(cache=True)
 def eval_cubic_splines_4(a, b, orders, coefs, point, vals):
-
     n_vals = coefs.shape[4]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
@@ -3746,24 +3730,22 @@
                 )
             )
         )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_1(a, b, orders, coefs, points, vals):
-
     n_vals = coefs.shape[1]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
 
     for n in range(N):
-
         x0 = points[n, 0]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
         tp0_0 = t0 * t0 * t0
         tp0_1 = t0 * t0
@@ -3824,27 +3806,25 @@
                 + Phi0_2 * (coefs[i0 + 2, k])
                 + Phi0_3 * (coefs[i0 + 3, k])
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_2(a, b, orders, coefs, points, vals):
-
     n_vals = coefs.shape[2]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
         u1 = (x1 - start1) * dinv1
@@ -3986,30 +3966,28 @@
                     + Phi1_3 * (coefs[i0 + 3, i1 + 3, k])
                 )
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_3(a, b, orders, coefs, points, vals):
-
     n_vals = coefs.shape[3]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
     M2 = orders[2]
     start2 = a[2]
     dinv2 = (orders[2] - 1.0) / (b[2] - a[2])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
@@ -4304,15 +4282,14 @@
                     )
                 )
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_4(a, b, orders, coefs, points, vals):
-
     n_vals = coefs.shape[4]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
@@ -4322,15 +4299,14 @@
     start2 = a[2]
     dinv2 = (orders[2] - 1.0) / (b[2] - a[2])
     M3 = orders[3]
     start3 = a[3]
     dinv3 = (orders[3] - 1.0) / (b[3] - a[3])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         x3 = points[n, 3]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
@@ -5066,24 +5042,22 @@
                     )
                 )
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_G_1(a, b, orders, coefs, points, vals, dvals):
-
     n_vals = coefs.shape[1]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
 
     for n in range(N):
-
         x0 = points[n, 0]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
         tp0_0 = t0 * t0 * t0
         tp0_1 = t0 * t0
@@ -5175,27 +5149,25 @@
                 + dPhi0_2 * (coefs[i0 + 2, k])
                 + dPhi0_3 * (coefs[i0 + 3, k])
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_G_2(a, b, orders, coefs, points, vals, dvals):
-
     n_vals = coefs.shape[2]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
         u1 = (x1 - start1) * dinv1
@@ -5445,30 +5417,28 @@
                     + dPhi1_3 * (coefs[i0 + 3, i1 + 3, k])
                 )
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_G_3(a, b, orders, coefs, points, vals, dvals):
-
     n_vals = coefs.shape[3]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
     start1 = a[1]
     dinv1 = (orders[1] - 1.0) / (b[1] - a[1])
     M2 = orders[2]
     start2 = a[2]
     dinv2 = (orders[2] - 1.0) / (b[2] - a[2])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
         t0 = u0 - i0
@@ -6212,15 +6182,14 @@
                     )
                 )
             )
 
 
 @njit(cache=True)
 def vec_eval_cubic_splines_G_4(a, b, orders, coefs, points, vals, dvals):
-
     n_vals = coefs.shape[4]
     N = points.shape[0]
 
     M0 = orders[0]
     start0 = a[0]
     dinv0 = (orders[0] - 1.0) / (b[0] - a[0])
     M1 = orders[1]
@@ -6230,15 +6199,14 @@
     start2 = a[2]
     dinv2 = (orders[2] - 1.0) / (b[2] - a[2])
     M3 = orders[3]
     start3 = a[3]
     dinv3 = (orders[3] - 1.0) / (b[3] - a[3])
 
     for n in range(N):
-
         x0 = points[n, 0]
         x1 = points[n, 1]
         x2 = points[n, 2]
         x3 = points[n, 3]
         u0 = (x0 - start0) * dinv0
         i0 = int(floor(u0))
         i0 = max(min(i0, M0 - 2), 0)
```

### Comparing `interpolation-2.2.4/interpolation/splines/eval_splines.py` & `interpolation-2.2.6/interpolation/splines/eval_splines.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-from numba import jit, generated_jit
 from numpy import zeros
 from numpy import floor
 
 from numba import prange
 from .codegen import get_code_spline, source_to_function
 
 
@@ -15,15 +14,14 @@
 import numba.types
 from numba.core.types.misc import NoneType as none
 from numpy import zeros
 from numpy import floor
 from interpolation.splines.codegen import get_code_spline, source_to_function
 from numba.types import UniTuple, float64, Array
 from interpolation.splines.codegen import source_to_function
-from numba import generated_jit
 
 
 from ..compat import Tuple, UniTuple
 from ..compat import overload_options
 
 #
 
@@ -46,17 +44,20 @@
 t_array_2d = [
     Array(float64, 2, a, readonly=b) for b in [True, False] for a in ["A", "C", "F"]
 ]
 
 ### eval spline (main function)
 
 
-# @generated_jit(inline='always', nopython=True) # doens't work
-@generated_jit(nopython=True)
 def allocate_output(G, C, P, O):
+    pass
+
+
+@overload(allocate_output)
+def ol_allocate_output(G, C, P, O):
     if C.ndim == len(G) + 1:
         # vector valued
         if P.ndim == 2:
             # vectorized call
             if isinstance(O, none):
                 return lambda G, C, P, O: np.zeros((P.shape[0], C.shape[C.ndim - 1]))
             else:
@@ -91,33 +92,16 @@
 
 
 def _eval_spline():
     pass
 
 
 @overload(_eval_spline)
-def __eval_spline(
-    grid, C, points, out=None, order=1, diff="None", extrap_mode="linear"
-):
-
-    if not (
-        isinstance(order, numba.types.Literal)
-        and isinstance(diff, numba.types.Literal)
-        and isinstance(extrap_mode, numba.types.Literal)
-    ):
-
-        def ugly_workaround(
-            grid, C, points, out=None, order=1, diff="None", extrap_mode="linear"
-        ):
-            return (literally(order), literally(diff), literally(extrap_mode))
-
-        # def __eval_spline(grid, C, points, out=None, order=1, diff="None", extrap_mode='linear'):
-        #     return __eval_spline(grid, C, points, out=out, order=literally(order), diff=literally(diff), extrap_mode=literally(extrap_mode))
-
-    kk = (order).literal_value
+def __eval_spline(grid, C, points, out=None, k=1, diff="None", extrap_mode="linear"):
+    kk = (k).literal_value
     diffs = (diff).literal_value
     extrap_ = (extrap_mode).literal_value
     d = len(grid)
 
     vectorized = points in t_array_2d
     allocate = True
     vector_valued = C.ndim == (len(grid) + 1)
@@ -151,82 +135,81 @@
     }
     f = source_to_function(code, context)
 
     return f
 
 
 @njit
-def eval_spline(grid, C, points, out=None, order=1, diff="None", extrap_mode="linear"):
+def eval_spline(grid, C, points, out=None, k=1, diff="None", extrap_mode="linear"):
     """Do I get a docstring ?"""
     dd = numba.literally(diff)
-    k = numba.literally(order)
+    k = numba.literally(k)
     extrap_ = numba.literally(extrap_mode)
-    return _eval_spline(grid, C, points, out=out, order=k, diff=dd, extrap_mode=extrap_)
+    return _eval_spline(grid, C, points, out=out, k=k, diff=dd, extrap_mode=extrap_)
 
 
 ###
 ### Compatibility calls:
 ###
 
 
 def _eval_linear():
     pass
 
 
+# TODO: now that constant propagation in numba works well enough we can remove the option_types
+
 from .option_types import options, t_CONSTANT, t_LINEAR, t_NEAREST
 
 
 @overload(_eval_linear, **overload_options)
 def __eval_linear(grid, C, points):
     # print("We allocate with default extrapolation.")
     return lambda grid, C, points: eval_spline(
-        grid, C, points, order=1, extrap_mode="linear", diff="None"
+        grid, C, points, k=1, extrap_mode="linear", diff="None"
     )
 
 
 @overload(_eval_linear, **overload_options)
 def __eval_linear(grid, C, points, extrap_mode):
-
     # print(f"We are going to extrapolate in {extrap_mode} mode.")
     if extrap_mode == t_NEAREST:
         extrap_ = "nearest"
     elif extrap_mode == t_CONSTANT:
         extrap_ = "constant"
     elif extrap_mode == t_LINEAR:
         extrap_ = "linear"
     else:
         return None
 
     return lambda grid, C, points, extrap_mode: eval_spline(
-        grid, C, points, order=1, diff="None", extrap_mode=extrap_
+        grid, C, points, k=1, diff="None", extrap_mode=extrap_
     )
 
 
 @overload(_eval_linear, **overload_options)
 def __eval_linear(grid, C, points, out, extrap_mode):
-
     # print(f"We are going to do inplace, with {extrap_mode} extrapolation")
     if extrap_mode == t_NEAREST:
         extrap_ = "nearest"
     elif extrap_mode == t_CONSTANT:
         extrap_ = "constant"
     elif extrap_mode == t_LINEAR:
         extrap_ = "linear"
     else:
         return None
     return lambda grid, C, points, out, extrap_mode: eval_spline(
-        grid, C, points, out=out, order=1, diff="None", extrap_mode=extrap_
+        grid, C, points, out=out, k=1, diff="None", extrap_mode=extrap_
     )
 
 
 @overload(_eval_linear, **overload_options)
 def __eval_linear(grid, C, points, out):
-
     return lambda grid, C, points, out: eval_spline(
-        grid, C, points, out=out, order=1, diff="None", extrap_mode="linear"
+        grid, C, points, out=out, k=1, diff="None", extrap_mode="linear"
     )
 
 
 @njit
 def eval_linear(*args):
     """Do I get a docstring ?"""
     return _eval_linear(*args)
@@ -245,72 +228,69 @@
 @overload(_eval_cubic, **overload_options)
 def __eval_cubic(grid, C, points):
     # print("We allocate with default extrapolation.")
     return lambda grid, C, points: eval_spline(
         grid,
         C,
         points,
-        order=literally(3),
+        k=literally(3),
         extrap_mode=literally("linear"),
         diff=literally("None"),
     )
 
 
 @overload(_eval_cubic, **overload_options)
 def __eval_cubic(grid, C, points, extrap_mode):
-
     # print(f"We are going to extrapolate in {extrap_mode} mode.")
     if extrap_mode == t_NEAREST:
         extrap_ = literally("nearest")
     elif extrap_mode == t_CONSTANT:
         extrap_ = literally("constant")
-    elif extrap_mode == t_cubic:
-        extrap_ = literally("cubic")
+    elif extrap_mode == t_LINEAR:
+        extrap_ = literally("linear")
     else:
         return None
 
     return lambda grid, C, points, extrap_mode: eval_spline(
-        grid, C, points, order=literally(3), diff=literally("None"), extrap_mode=extrap_
+        grid, C, points, k=literally(3), diff=literally("None"), extrap_mode=extrap_
     )
 
 
 @overload(_eval_cubic, **overload_options)
 def __eval_cubic(grid, C, points, out, extrap_mode):
-
     if extrap_mode == t_NEAREST:
         extrap_ = literally("nearest")
     elif extrap_mode == t_CONSTANT:
         extrap_ = literally("constant")
-    elif extrap_mode == t_cubic:
-        extrap_ = literally("cubic")
+    elif extrap_mode == t_LINEAR:
+        extrap_ = literally("linear")
     else:
         return None
     return lambda grid, C, points, out, extrap_mode: eval_spline(
         grid,
         C,
         points,
         out=out,
-        order=literally(3),
+        k=literally(3),
         diff=literally("None"),
         extrap_mode=extrap_,
     )
 
 
 from numba import literally
 
 
 @overload(_eval_cubic, **overload_options)
 def __eval_cubic(grid, C, points, out):
-
     return lambda grid, C, points, out: eval_spline(
         grid,
         C,
         points,
         out=out,
-        order=literally(3),
+        k=literally(3),
         diff=literally("None"),
         extrap_mode=literally("linear"),
     )
 
 
 @njit
 def eval_cubic(*args):
```

### Comparing `interpolation-2.2.4/interpolation/splines/filter_cubic.py` & `interpolation-2.2.6/interpolation/splines/filter_cubic.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 # used by njitted routines (frozen)
 basis = np.array([1.0 / 6.0, 2.0 / 3.0, 1.0 / 6.0, 0.0])
 
 
 @njit(cache=True)
 def solve_deriv_interp_1d(bands, coefs):
-
     M = coefs.shape[0] - 2
 
     # Solve interpolating equations
     # First and last rows are different
 
     bands[0, 1] /= bands[0, 0]
     bands[0, 2] /= bands[0, 0]
@@ -52,15 +51,14 @@
 
     # Finish with first row
     coefs[0] = bands[0, 3] - bands[0, 1] * coefs[1] - bands[0, 2] * coefs[2]
 
 
 @njit(cache=True)
 def find_coefs_1d(delta_inv, M, data, coefs):
-
     bands = np.zeros((M + 2, 4))
 
     # Setup boundary conditions
     abcd_left = np.zeros(4)
     abcd_right = np.zeros(4)
 
     # Left boundary
@@ -85,27 +83,25 @@
             bands[i + 1, 3] = data[i]
 
     solve_deriv_interp_1d(bands, coefs)
 
 
 @njit(cache=True)
 def filter_coeffs_1d(dinv, data):
-
     M = data.shape[0]
     N = M + 2
 
     coefs = np.zeros(N)
     find_coefs_1d(dinv[0], M, data, coefs)
 
     return coefs
 
 
 @njit(cache=True)
 def filter_coeffs_2d(dinv, data):
-
     Mx = data.shape[0]
     My = data.shape[1]
 
     Nx = Mx + 2
     Ny = My + 2
 
     coefs = np.zeros((Nx, Ny))
@@ -121,15 +117,14 @@
         find_coefs_1d(dinv[1], My, coefs[ix, :], coefs[ix, :])
 
     return coefs
 
 
 @njit(cache=True)
 def filter_coeffs_3d(dinv, data):
-
     Mx = data.shape[0]
     My = data.shape[1]
     Mz = data.shape[2]
 
     Nx = Mx + 2
     Ny = My + 2
     Nz = Mz + 2
@@ -151,15 +146,14 @@
             find_coefs_1d(dinv[2], Mz, coefs[ix, iy, :], coefs[ix, iy, :])
 
     return coefs
 
 
 @njit(cache=True)
 def filter_coeffs_4d(dinv, data):
-
     Mx = data.shape[0]
     My = data.shape[1]
     Mz = data.shape[2]
     Mz4 = data.shape[3]
 
     Nx = Mx + 2
     Ny = My + 2
@@ -200,15 +194,14 @@
     smax = np.array(smax, dtype=float)
     dinv = (smax - smin) / orders
     data = data.reshape(orders)
     return filter_data(dinv, data)
 
 
 def filter_mcoeffs(smin, smax, orders, data):
-
     order = len(smin)
     n_splines = data.shape[-1]
     coefs = np.zeros(tuple([i + 2 for i in orders]) + (n_splines,))
     for i in range(n_splines):
         coefs[..., i] = filter_coeffs(smin, smax, orders, data[..., i])
     return coefs
 
@@ -224,15 +217,14 @@
         return filter_coeffs_4d(dinv, data)
 
 
 #
 
 
 if __name__ == "__main__":
-
     import numpy
 
     dinv = numpy.ones(3, dtype=float) * 0.5
     coeffs_0 = numpy.random.random([10, 10, 10])
     coeffs_1 = numpy.random.random([100, 100, 100])
 
     print(coeffs_0[:2, :2, :2])
```

### Comparing `interpolation-2.2.4/interpolation/splines/hermite.py` & `interpolation-2.2.6/interpolation/splines/hermite.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         x0 = xvect[i]
         out[i] = HermiteInterpolation(x0, x, y, yp)
     return out
 
 
 from numba import njit, types
 from numba.extending import overload, register_jitable
-from numba import generated_jit
 
 
 def _hermite(x0, x, y, yp, out=None):
     pass
 
 
 @overload(_hermite)
@@ -98,16 +97,20 @@
 
     return _hermite
 
 
 from numba.core.types.misc import NoneType as none
 
 
-@generated_jit
 def hermite(x0, x, y, yp, out=None):
+    pass
+
+
+@overload(hermite)
+def ol_hermite(x0, x, y, yp, out=None):
     try:
         n = x0.ndim
         if n == 1:
             input_type = "vector"
         elif n == 2:
             input_type = "matrix"
         else:
```

### Comparing `interpolation-2.2.4/interpolation/splines/multilinear.py` & `interpolation-2.2.6/interpolation/splines/multilinear.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,26 +78,24 @@
         return self.__grid__
 
     def set_values(self, values):
         values = values.reshape(self.orders)
         self.values = numpy.ascontiguousarray(values, dtype=self.dtype)
 
     def interpolate(self, s):
-
         from .eval_splines import eval_linear
 
         s = numpy.ascontiguousarray(s, dtype=self.dtype)
         grid = tuple(
             (self.smin[i], self.smax[i], self.orders[i]) for i in range(len(self.smin))
         )
         a = eval_linear(grid, self.values, s)
         return a
 
     def __call__(self, s):
-
         if s.ndim == 1:
             res = self.__call__(numpy.atleast_2d(s))
             return res[0]
         return self.interpolate(s)
 
 
 class LinearSplines:
@@ -156,31 +154,28 @@
     @property
     def grid(self):
         if self.__grid__ is None:
             self.__grid__ = mlinspace(self.smin, self.smax, self.orders)
         return self.__grid__
 
     def set_values(self, mvalues):
-
         n_x = mvalues.shape[-1]
         new_orders = list(self.orders) + [n_x]
         mvalues = mvalues.reshape(new_orders)
         self.mvalues = numpy.ascontiguousarray(mvalues, dtype=self.dtype)
 
     def interpolate(self, s):
-
         from .multilinear_numba import eval_linear
 
         grid = tuple(
             (self.smin[i], self.smax[i], self.orders[i]) for i in range(len(self.smin))
         )
         s = numpy.ascontiguousarray(s, dtype=self.dtype)
         a = eval_linear(grid, self.mvalues, s)
         return a
 
     def __call__(self, s):
-
         if s.ndim == 1:
             res = self.__call__(numpy.atleast_2d(s))
             return res.ravel()
 
         return self.interpolate(s)
```

### Comparing `interpolation-2.2.4/interpolation/splines/multilinear_numba.py` & `interpolation-2.2.6/interpolation/splines/multilinear_numba.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import numpy as np
 from numba import njit
 from .eval_splines import eval_linear
 from .eval_cubic import get_grid
 
 
 def vec_multilinear_interpolation(smin, smax, orders, mvalues, s, out=None):
-
     grid = get_grid(smin, smax, orders, mvalues[..., 0])
 
     if out is None:
         return eval_linear(grid, mvalues, s)
     else:
         eval_linear(grid, values, s, out)
 
 
 def multilinear_interpolation(smin, smax, orders, values, s, out=None):
-
     grid = get_grid(smin, smax, orders, values)
 
     if out is None:
         return eval_linear(grid, values, s)
     else:
         eval_linear(grid, values, s, out)
```

### Comparing `interpolation-2.2.4/interpolation/splines/option_types.py` & `interpolation-2.2.6/interpolation/splines/option_types.py`

 * *Files identical despite different names*

### Comparing `interpolation-2.2.4/interpolation/splines/prefilter_cubic.py` & `interpolation-2.2.6/interpolation/splines/prefilter_cubic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import numpy as np
 from numba import jit, njit
-from numba import generated_jit
 from numba.extending import overload
 
 
 from packaging.version import parse
 from numba import __version__
 
 if parse(__version__) >= parse("0.43"):
     overload_options = {"strict": False}
 else:
     overload_options = {}
 
 # used by njitted routines (frozen)
 basis = (1.0 / 6.0, 2.0 / 3.0, 1.0 / 6.0, 0.0)
 
+
 #
 @njit
 def solve_deriv_interp_1d(bands, coefs):
-
     M = coefs.shape[0] - 2
 
     # Solve interpolating equations
     # First and last rows are different
 
     bands[0, 1] /= bands[0, 0]
     bands[0, 2] /= bands[0, 0]
@@ -60,15 +59,14 @@
 
     # Finish with first row
     coefs[0] = bands[0, 3] - bands[0, 1] * coefs[1] - bands[0, 2] * coefs[2]
 
 
 @njit
 def find_coefs_1d(δ, data, coefs, bands):
-
     M = bands.shape[0] - 2
 
     # Setup boundary conditions
 
     # Left boundary
     abcd_left = (1.0 * δ * δ, -2.0 * δ * δ, 1.0 * δ * δ, 0.0)
 
@@ -90,31 +88,28 @@
 def _filter_cubic():
     pass
 
 
 # non allocating version
 @overload(_filter_cubic, **overload_options)
 def __filter_cubic(grid, D, C):
-
     d = len(grid.types)
 
     if D.ndim > d:
 
         def ___filter_cubic(grid, D, C):
-
             n_x = C.shape[-1]
             for i_x in range(n_x):
                 _filter_cubic(grid, D[..., i_x], C[..., i_x])
 
         return ___filter_cubic
 
     if d == 1:
 
         def ___filter_cubic(grid, D, C):
-
             dinv_0 = (grid[0][1] - grid[0][0]) / grid[0][2]
 
             Mx = D.shape[0]
 
             Nx = Mx + 2
 
             # First, solve in the X-direction
@@ -122,15 +117,14 @@
             find_coefs_1d(dinv_0, D, C, bands)
 
         return ___filter_cubic
 
     if d == 2:
 
         def ___filter_cubic(grid, D, C):
-
             dinv_0 = (grid[0][1] - grid[0][0]) / grid[0][2]
             dinv_1 = (grid[1][1] - grid[1][0]) / grid[1][2]
 
             Mx = D.shape[0]
             My = D.shape[1]
 
             Nx = Mx + 2
@@ -147,15 +141,14 @@
                 find_coefs_1d(dinv_0, C[ix, :], C[ix, :], bands)
 
         return ___filter_cubic
 
     if d == 3:
 
         def ___filter_cubic(grid, D, C):
-
             dinv_0 = (grid[0][1] - grid[0][0]) / grid[0][2]
             dinv_1 = (grid[1][1] - grid[1][0]) / grid[1][2]
             dinv_2 = (grid[2][1] - grid[2][0]) / grid[2][2]
 
             Mx = D.shape[0]
             My = D.shape[1]
             Mz = D.shape[2]
@@ -182,15 +175,14 @@
                     find_coefs_1d(dinv_2, C[ix, iy, :], C[ix, iy, :], bands)
 
         return ___filter_cubic
 
     if d == 4:
 
         def ___filter_cubic(grid, D, C):
-
             dinv_0 = (grid[0][1] - grid[0][0]) / grid[0][2]
             dinv_1 = (grid[1][1] - grid[1][0]) / grid[1][2]
             dinv_2 = (grid[2][1] - grid[2][0]) / grid[2][2]
             dinv_3 = (grid[3][1] - grid[3][0]) / grid[3][2]
 
             Mx = D.shape[0]
             My = D.shape[1]
@@ -238,15 +230,14 @@
 
         return ___filter_cubic
 
 
 # allocating version
 @overload(_filter_cubic)
 def __filter_cubic(grid, D):
-
     d = len(grid.types)
     if D.ndim == d:
         if D.ndim == 1:
 
             def ___filter_cubic(grid, D):
                 C = np.zeros(D.shape[0] + 2)
                 _filter_cubic(grid, D, C)
@@ -333,17 +324,15 @@
 import numba
 
 none = numba.typeof(None)
 
 
 @numba.extending.overload(_prefilter)
 def _ov_prefilter(grid, V, k, out=None):
-
     if isinstance(k, numba.types.Literal):
-
         if k.literal_value == 1:
 
             def _impl_prefilter(grid, V, k, out=None):
                 return V  # should we copy it here ?
 
             return _impl_prefilter
```

### Comparing `interpolation-2.2.4/interpolation/splines/splines.py` & `interpolation-2.2.6/interpolation/splines/splines.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
             raise Exception("Spline interpolator evaluated at non-finite points.")
 
         if not with_derivatives:
             if points.ndim == 1:
                 # evaluate only on one point
                 return eval_cubic(grid, self.__coeffs__, points)
             else:
-
                 N, d = points.shape
                 assert d == self.d
                 if values is None:
                     values = np.empty(N, dtype=self.dtype)
                 eval_cubic(grid, self.__coeffs__, points, values)
                 return values
 
@@ -120,15 +119,14 @@
             res = self.__call__(numpy.atleast_2d(s))
             return res[0]
 
         return self.interpolate(s)
 
 
 class CubicSplines:
-
     __grid__ = None
     __values__ = None
     __coeffs__ = None
     __n_splines__ = None
 
     def __init__(self, a, b, orders, values=None):
         """Creates a cubic multi-spline interpolator for many functions on a regular cartesian grid."""
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_cubic_splines.py` & `interpolation-2.2.6/interpolation/splines/tests/test_cubic_splines.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 point = array([0.5, 0.5])
 
 # many points
 points = row_stack([[0.5, 0.5]] * N)
 
 
 def test_cubic_spline():
-
     from interpolation.splines.filter_cubic import filter_coeffs
     from interpolation.splines.eval_cubic import (
         eval_cubic_spline,
         vec_eval_cubic_spline,
     )
 
     cc = filter_coeffs(a, b, orders, vals)
@@ -51,15 +50,14 @@
     iii = vec_eval_cubic_spline(a, b, orders, cc, points)
 
     assert isinstance(ii, float)
     assert iii.ndim == 1
 
 
 def test_cubic_multi_spline():
-
     from interpolation.splines.filter_cubic import filter_mcoeffs
     from interpolation.splines.eval_cubic import (
         eval_cubic_splines,
         vec_eval_cubic_splines,
     )
 
     cc = filter_mcoeffs(a, b, orders, mvals)
@@ -69,41 +67,38 @@
     iii = vec_eval_cubic_splines(a, b, orders, cc, points)
 
     assert ii.ndim == 1
     assert iii.ndim == 2
 
 
 def test_cubic_spline_object():
-
     from interpolation.splines import CubicSpline
 
     cs = CubicSpline(a, b, orders, vals)
     ii = cs(point)
     iii = cs(points)
 
     assert ii.ndim == 0
     assert isscalar(ii)
     assert iii.ndim == 1
     assert tuple(iii.shape) == (N,)
 
 
 def test_cubic_multi_spline_object():
-
     from interpolation.splines import CubicSplines
 
     cs = CubicSplines(a, b, orders, mvals)
     ii = cs(point)
     iii = cs(points)
 
     n_splines = mvals.shape[1]
     assert ii.ndim == 1
     assert tuple(ii.shape) == (n_splines,)
     assert iii.ndim == 2
     assert tuple(iii.shape) == (N, n_splines)
 
 
 if __name__ == "__main__":
-
     test_cubic_spline()
     test_cubic_multi_spline()
     test_cubic_spline_object()
     test_cubic_multi_spline_object()
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_derivatives.py` & `interpolation-2.2.6/interpolation/splines/tests/test_derivatives.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 def test_derivatives():
-
     from interpolation.splines.eval_splines import eval_spline, eval_cubic, eval_linear
 
     import numpy as np
 
     grid = ((0.0, 1.0, 10),)
 
     # grid = ((0.0, 1.0, 0.1),(0.0, 1.0, 0.1))
 
     C = np.linspace(0, 1, 10)
     Cx = np.concatenate([C[:, None], C[:, None] * 2])
     points = np.random.random((10, 1))
 
     eval_spline(
-        grid, C, (-0.1,), out=None, order=1, diff="None", extrap_mode="nearest"
+        grid, C, (-0.1,), out=None, k=1, diff="None", extrap_mode="nearest"
     )  # no alloc
     eval_spline(
-        grid, C, (-0.1,), out=None, order=1, diff="None", extrap_mode="constant"
+        grid, C, (-0.1,), out=None, k=1, diff="None", extrap_mode="constant"
     )  # no alloc
     eval_spline(
-        grid, C, (-0.1,), out=None, order=1, diff="None", extrap_mode="linear"
+        grid, C, (-0.1,), out=None, k=1, diff="None", extrap_mode="linear"
     )  # no alloc
 
     eval_spline(
-        grid, C, (1.1,), out=None, order=1, diff="None", extrap_mode="nearest"
+        grid, C, (1.1,), out=None, k=1, diff="None", extrap_mode="nearest"
     )  # no alloc
     eval_spline(
-        grid, C, (1.1,), out=None, order=1, diff="None", extrap_mode="constant"
+        grid, C, (1.1,), out=None, k=1, diff="None", extrap_mode="constant"
     )  # no alloc
     eval_spline(
-        grid, C, (1.1,), out=None, order=1, diff="None", extrap_mode="linear"
+        grid, C, (1.1,), out=None, k=1, diff="None", extrap_mode="linear"
     )  # no alloc
 
     eval_spline(
-        grid, Cx, points[0, :], out=None, order=1, diff="None", extrap_mode="linear"
+        grid, Cx, points[0, :], out=None, k=1, diff="None", extrap_mode="linear"
     )
 
-    eval_spline(grid, C, points, out=None, order=1, diff="None", extrap_mode="linear")
-    eval_spline(grid, Cx, points, out=None, order=1, diff="None", extrap_mode="linear")
+    eval_spline(grid, C, points, out=None, k=1, diff="None", extrap_mode="linear")
+    eval_spline(grid, Cx, points, out=None, k=1, diff="None", extrap_mode="linear")
 
     orders = str(((0,), (1,)))
 
     eval_spline(
-        grid, C, points[0, :], out=None, order=1, diff=orders, extrap_mode="linear"
+        grid, C, points[0, :], out=None, k=1, diff=orders, extrap_mode="linear"
     )  # no alloc
     eval_spline(
-        grid, Cx, points[0, :], out=None, order=1, diff=orders, extrap_mode="linear"
+        grid, Cx, points[0, :], out=None, k=1, diff=orders, extrap_mode="linear"
     )
-    eval_spline(grid, C, points, out=None, order=1, diff=orders, extrap_mode="linear")
-    eval_spline(grid, Cx, points, out=None, order=1, diff=orders, extrap_mode="linear")
+    eval_spline(grid, C, points, out=None, k=1, diff=orders, extrap_mode="linear")
+    eval_spline(grid, Cx, points, out=None, k=1, diff=orders, extrap_mode="linear")
 
     out = eval_spline(
-        grid, Cx, points, out=None, order=1, diff=orders, extrap_mode="linear"
+        grid, Cx, points, out=None, k=1, diff=orders, extrap_mode="linear"
     )
     out2 = np.zeros_like(out)
-    eval_spline(grid, Cx, points, out=out2, order=1, diff=orders, extrap_mode="linear")
+    eval_spline(grid, Cx, points, out=out2, k=1, diff=orders, extrap_mode="linear")
     print(abs(out - out2).max())
 
     k = 3
 
-    eval_spline(
-        grid, C, points[0, :], out=None, order=3, diff="None", extrap_mode="linear"
-    )
+    eval_spline(grid, C, points[0, :], out=None, k=3, diff="None", extrap_mode="linear")
 
-    eval_spline(grid, C, points, out=None, order=k, diff="None", extrap_mode="linear")
+    eval_spline(grid, C, points, out=None, k=k, diff="None", extrap_mode="linear")
     eval_spline(
-        grid, Cx, points[0, :], out=None, order=k, diff="None", extrap_mode="linear"
+        grid, Cx, points[0, :], out=None, k=k, diff="None", extrap_mode="linear"
     )
-    eval_spline(grid, Cx, points, out=None, order=k, diff="None", extrap_mode="linear")
+    eval_spline(grid, Cx, points, out=None, k=k, diff="None", extrap_mode="linear")
 
     orders = str(((0,), (1,)))
 
+    eval_spline(grid, C, points[0, :], out=None, k=k, diff=orders, extrap_mode="linear")
+    eval_spline(grid, C, points, out=None, k=k, diff=orders, extrap_mode="linear")
     eval_spline(
-        grid, C, points[0, :], out=None, order=k, diff=orders, extrap_mode="linear"
-    )
-    eval_spline(grid, C, points, out=None, order=k, diff=orders, extrap_mode="linear")
-    eval_spline(
-        grid, Cx, points[0, :], out=None, order=k, diff=orders, extrap_mode="linear"
+        grid, Cx, points[0, :], out=None, k=k, diff=orders, extrap_mode="linear"
     )
-    eval_spline(grid, Cx, points, out=None, order=k, diff=orders, extrap_mode="linear")
+    eval_spline(grid, Cx, points, out=None, k=k, diff=orders, extrap_mode="linear")
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_eval_splines.py` & `interpolation-2.2.6/interpolation/splines/tests/test_eval_splines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_eval_splines():
-
     from interpolation.splines.eval_splines import eval_linear, eval_cubic
     from interpolation.multilinear.mlinterp import mlinterp
     import numpy as np
 
     N = 1000
     K = 100
     d = 2
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_fortran_order.py` & `interpolation-2.2.6/interpolation/splines/tests/test_fortran_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_eval_with_fortran_order():
-
     import numpy as np
 
     C_F = np.random.random((50, 50)).T
     C = C_F.copy()
 
     print(C.flags)
     print(C_F.flags)
@@ -22,15 +21,14 @@
 
     assert np.array_equal(out_F_C, out_C_C)
     assert np.array_equal(out_F_C, out_F_F)
     assert np.array_equal(out_F_C, out_C_F)
 
 
 def test_guvectorize_compatilibity():
-
     ### this tests type dispatch when order='A'
 
     import numpy as np
     from numba import guvectorize, f8
 
     from interpolation.splines import eval_linear
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_hermite_splines.py` & `interpolation-2.2.6/interpolation/splines/tests/test_hermite_splines.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_hermite_splines():
-
     from interpolation.splines.hermite import HermiteInterpolationVect
     import numpy as np
 
     N = 10000  # Number of points in the initial dataset
     K = 1000  # Number of new points to interpolate
 
     # Initial dataset
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_multilinear_extrap.py` & `interpolation-2.2.6/interpolation/splines/tests/test_multilinear_extrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_multilinear_extrap():
-
     import numpy as np
 
     N = 100000
     K = 10
     d = 1
     a = np.array([0.0] * d)
     b = np.array([1.0] * d)
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_object_api.py` & `interpolation-2.2.6/interpolation/splines/tests/test_object_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,26 +39,24 @@
 point = array([0.5, 0.5])
 
 # many points
 points = row_stack([[0.5, 0.5]] * N)
 
 
 def ttest_object_api(Obj):
-
     cs = Obj(a, b, orders, vals)
     ii = cs(point)
     iii = cs(points)
     assert ii.ndim == 0
     assert isscalar(ii)
     assert iii.ndim == 1
     assert tuple(iii.shape) == (N,)
 
 
 def ttest_object_vector_api(Obj):
-
     cs = Obj(a, b, orders, mvals)
 
     ii = cs(point)
     iii = cs(points)
     try:
         print(cs.mvalues)
     except:
@@ -70,28 +68,26 @@
     print(n_splines)
     assert tuple(ii.shape) == (n_splines,)
     assert iii.ndim == 2
     assert tuple(iii.shape) == (N, n_splines)
 
 
 def ttest_object_vector_diff_api(Obj):
-
     cs = Obj(a, b, orders, mvals)
 
     # ii = cs(point, diff=True)
     iii, d_iii = cs.interpolate(points, diff=True)
 
     n_splines = mvals.shape[1]
     assert iii.ndim == 2
     assert tuple(iii.shape) == (N, n_splines)
     assert tuple(d_iii.shape) == (N, d, n_splines)
 
 
 def test_objects():
-
     from interpolation.splines import CubicSpline
 
     ttest_object_api(CubicSpline)
     from interpolation.splines import CubicSplines
 
     ttest_object_vector_api(CubicSplines)
     ttest_object_vector_diff_api(CubicSplines)
@@ -101,9 +97,8 @@
     ttest_object_api(LinearSpline)
     from interpolation.splines.multilinear import LinearSplines
 
     ttest_object_vector_api(LinearSplines)
 
 
 if __name__ == "__main__":
-
     test_objects()
```

### Comparing `interpolation-2.2.4/interpolation/splines/tests/test_readonly.py` & `interpolation-2.2.6/interpolation/splines/tests/test_readonly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 def test_readonly_vec():
-
     import numpy as np
     from interpolation.splines.eval_splines import eval_cubic
 
     vals = np.random.random((7, 7, 2))
     grid = ((-0.053333333333333344, 0.053333333333333344, 5), (5.0, 15.0, 5))
 
     # this works
@@ -13,15 +12,14 @@
     #
     pp = points.copy()
     pp.flags.writeable = False
     x = eval_cubic(grid, vals, pp)
 
 
 def test_readonly():
-
     import numpy as np
     from interpolation.splines.eval_splines import eval_cubic
 
     vals = np.random.random((7, 7, 2))
     grid = ((-0.053333333333333344, 0.053333333333333344, 5), (5.0, 15.0, 5))
 
     # this works
```

### Comparing `interpolation-2.2.4/interpolation/tests/test_complete.py` & `interpolation-2.2.6/interpolation/tests/test_complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     assert evals.shape == vals.shape
     assert abs(evals - vals).max() < 1e-10
 
     cp.fit_values(points, vals, damp=0.5)
 
 
 def test_complete_derivative():
-
     # Test derivative vector
     z = np.array([1, 2, 3])
     sol_vec = np.array([0.0, 1.0, 0.0, 0.0, 2.0, 2.0, 3.0, 0.0, 0.0, 0.0])
     out_vec = np.empty(n_complete(3, 2))
     _complete_poly_der_impl_vec(z, 2, 0, out_vec)
     assert abs(out_vec - sol_vec).max() < 1e-10
```

### Comparing `interpolation-2.2.4/interpolation/tests/test_derivs.py` & `interpolation-2.2.6/interpolation/tests/test_derivs.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 
 class Check1DDerivatives(unittest.TestCase):
     """
     Checks derivatives in a 1D interpolator
     """
 
     def setUp(self):
-
         pass
 
     def test_linear(self):
-
         # A linear function on a non-uniform grid
         x = np.exp(np.linspace(0, 2, 6))
         y0 = 2
         slope = 1.0
         y = y0 + slope * x
 
         eval_points = np.array([1.5, 2.5, 3.5, 4.5])
 
         grad = eval_spline(
             CGrid(x),
             y,
             eval_points[..., None],
             out=None,
-            order=1,
+            k=1,
             diff=str(((0,), (1,))),
             extrap_mode="linear",
         )
 
         # 0-order must be the function
         # 1-order must be the slope
         result = np.vstack(
@@ -40,27 +38,26 @@
                 np.ones_like(eval_points) * slope,
             ]
         ).T
 
         self.assertTrue(np.allclose(grad, result))
 
     def test_nonlinear(self):
-
         # A non linear function on uniform grid
         x = np.linspace(-10, 10, 21) * (1 / 2) * np.pi
         y = np.sin(x)
 
         eval_points = np.array([-1, -0.5, 0, 0.5, 1]) * np.pi
 
         grad = eval_spline(
             CGrid(x),
             y,
             eval_points[..., None],
             out=None,
-            order=1,
+            k=1,
             diff=str(((0,), (1,))),
             extrap_mode="linear",
         )
 
         # 0-order must be the function
         # 1-order must be + or - pi/2
         result = np.vstack(
@@ -69,27 +66,26 @@
                 np.array([-1, -1, 1, 1, -1]) * 2 / np.pi,
             ]
         ).T
 
         self.assertTrue(np.allclose(grad, result))
 
     def test_nonlinear_approx(self):
-
         # A non linear function on uniform grid
         x = np.linspace(-10, 10, 10000)
         y = np.power(x, 3)
 
         eval_points = np.linspace(-5, 5, 10)
 
         grad = eval_spline(
             CGrid(x),
             y,
             eval_points[..., None],
             out=None,
-            order=1,
+            k=1,
             diff=str(((0,), (1,))),
             extrap_mode="linear",
         )
 
         # 0-order must be x^3
         # 1-order must be close to 3x^2
         result = np.vstack(
@@ -104,19 +100,17 @@
 
 class Check2DDerivatives(unittest.TestCase):
     """
     Checks derivatives in a 2D interpolator
     """
 
     def setUp(self):
-
         pass
 
     def test_linear(self):
-
         # A linear function on a non-uniform grid
         x = np.exp(np.linspace(0, 2, 6))
         y = np.power(np.linspace(0, 5, 10), 2)
 
         inter = 1
         slope_x = 2
         slope_y = -3
@@ -130,15 +124,15 @@
 
         # Get function and 1st derivatives
         grad = eval_spline(
             CGrid(x, y),
             z,
             eval_points,
             out=None,
-            order=1,
+            k=1,
             diff=str(((0, 0), (1, 0), (0, 1), (1, 1))),
             extrap_mode="linear",
         )
 
         # 0-order must be the function
         # (1,0) must be x slope
         # (0,1) must be y slope
@@ -151,15 +145,14 @@
                 np.zeros((n_eval, 1)),
             ]
         )
 
         self.assertTrue(np.allclose(grad, result))
 
     def test_nonlinear_approx(self):
-
         # A non linear function on uniform grid
         n_grid = 100
         x = np.linspace(1, 5, n_grid)
         y = np.linspace(1, 5, n_grid)
         z = np.sin(x[..., None]) * np.log(y[None, ...])
 
         # Evaluation points
@@ -170,15 +163,15 @@
 
         # Get function and 1st derivatives
         grad = eval_spline(
             CGrid(x, y),
             z,
             eval_points,
             out=None,
-            order=1,
+            k=1,
             diff=str(((0, 0), (1, 0), (0, 1), (1, 1))),
             extrap_mode="linear",
         )
 
         # 0-order must be sin(x)*ln(y)
         # (1,0) must be cos(x) * ln(y)
         # (0,1) must be sin(x) / y
```

### Comparing `interpolation-2.2.4/PKG-INFO` & `interpolation-2.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: interpolation
-Version: 2.2.4
+Version: 2.2.6
 Summary: Interpolation in Python
 License: BSD-2-Clause
 Author: Pablo Winant
 Author-email: pablo.winant@gmail.com
 Maintainer: Pablo Winant
 Maintainer-email: pablo.winant@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: numba (>=0.47)
-Requires-Dist: numpy (>=1.22.2,<2.0.0)
-Requires-Dist: packaging (>=21.3,<22.0)
-Requires-Dist: scipy (>=1.4.1,<2.0.0)
-Requires-Dist: tempita (>=0.5.2,<0.6.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numba (>=0.59.1)
+Requires-Dist: scipy (>=1.10,<2.0)
 Description-Content-Type: text/markdown
 
 ![CI](https://github.com/EconForge/interpolation.py/workflows/CI/badge.svg?branch=master) ![DOC](https://github.com/EconForge/interpolation.py/workflows/DOC/badge.svg?branch=master)
 
 
 See the [doc](https://www.econforge.org/interpolation.py).
```

