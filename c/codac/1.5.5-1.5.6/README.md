# Comparing `tmp/codac-1.5.5-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip` & `tmp/codac-1.5.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,32 +1,26 @@
-Zip file size: 4641991 bytes, number of entries: 30
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 20:40 codac/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 20:40 codac-1.5.5.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 20:40 codac.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 20:40 codac/tests/
--rwxr-xr-x  2.0 unx    69640 b- defN 24-Apr-01 20:40 codac/empty.cpython-39-aarch64-linux-gnu.so
--rwx--x--x  2.0 unx  5730648 b- defN 24-Apr-01 20:40 codac/core.cpython-39-aarch64-linux-gnu.so
--rw-r--r--  2.0 unx     1357 b- defN 24-Apr-01 20:40 codac/__init__.py
--rwx--x--x  2.0 unx   334681 b- defN 24-Apr-01 20:40 codac/codac2.cpython-39-aarch64-linux-gnu.so
--rwx--x--x  2.0 unx   948001 b- defN 24-Apr-01 20:40 codac/unsupported.cpython-39-aarch64-linux-gnu.so
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-01 20:40 codac/version.py
--rw-r--r--  2.0 unx     1469 b- defN 24-Apr-01 20:40 codac/tests/test_numpy.py
--rw-r--r--  2.0 unx     1303 b- defN 24-Apr-01 20:40 codac/tests/test_ctcbox.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 20:40 codac/tests/__init__.py
--rw-r--r--  2.0 unx     1982 b- defN 24-Apr-01 20:40 codac/tests/test_sepbox.py
--rw-r--r--  2.0 unx     1123 b- defN 24-Apr-01 20:40 codac/tests/test_function.py
--rw-r--r--  2.0 unx    15680 b- defN 24-Apr-01 20:40 codac/tests/test_cn.py
--rw-r--r--  2.0 unx     3660 b- defN 24-Apr-01 20:40 codac/tests/test_ctc_constell.py
--rw-r--r--  2.0 unx     1262 b- defN 24-Apr-01 20:40 codac/tests/test_actions.py
--rw-r--r--  2.0 unx     1958 b- defN 24-Apr-01 20:40 codac/tests/test_ctcdelay.py
--rw-r--r--  2.0 unx    44226 b- defN 24-Apr-01 20:40 codac/tests/test_ctceval.py
--rw-r--r--  2.0 unx     3955 b- defN 24-Apr-01 20:40 codac/tests/test_multi_arithmetic.py
--rw-r--r--  2.0 unx     1548 b- defN 24-Apr-01 20:40 codac/tests/test_ctccartprod.py
--rw-r--r--  2.0 unx      905 b- defN 24-Apr-01 20:40 codac/tests/test_ctcstatic.py
--rw-r--r--  2.0 unx    13219 b- defN 24-Apr-01 20:40 codac/tests/test_definition.py
--rw-r--r--  2.0 unx    30842 b- defN 24-Apr-01 20:40 codac/tests/test_arithmetic.py
--rw-r--r--  2.0 unx      615 b- defN 24-Apr-01 20:40 codac-1.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-01 20:40 codac-1.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2265 b- defN 24-Apr-01 20:40 codac-1.5.5.dist-info/RECORD
--rw-r--r--  2.0 unx      150 b- defN 24-Apr-01 20:40 codac-1.5.5.dist-info/WHEEL
--rwx--x--x  2.0 unx  6152905 b- defN 24-Apr-01 20:40 codac.libs/core-a9d1df2d.cpython-39-aarch64-linux-gnu.so
-30 files, 13363419 bytes uncompressed, 4637973 bytes compressed:  65.3%
+Zip file size: 2056143 bytes, number of entries: 24
+-rw-rw-rw-  2.0 fat     1395 b- defN 24-Apr-11 12:15 codac/__init__.py
+-rw-rw-rw-  2.0 fat   343552 b- defN 24-Apr-11 12:19 codac/codac2.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  3726336 b- defN 24-Apr-11 12:19 codac/core.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   890368 b- defN 24-Apr-11 12:19 codac/unsupported.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 24-Apr-11 12:15 codac/version.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 12:15 codac/tests/__init__.py
+-rw-rw-rw-  2.0 fat     1302 b- defN 24-Apr-11 12:15 codac/tests/test_actions.py
+-rw-rw-rw-  2.0 fat    31638 b- defN 24-Apr-11 12:15 codac/tests/test_arithmetic.py
+-rw-rw-rw-  2.0 fat    16259 b- defN 24-Apr-11 12:15 codac/tests/test_cn.py
+-rw-rw-rw-  2.0 fat     3773 b- defN 24-Apr-11 12:15 codac/tests/test_ctc_constell.py
+-rw-rw-rw-  2.0 fat     1362 b- defN 24-Apr-11 12:15 codac/tests/test_ctcbox.py
+-rw-rw-rw-  2.0 fat     1620 b- defN 24-Apr-11 12:15 codac/tests/test_ctccartprod.py
+-rw-rw-rw-  2.0 fat     2023 b- defN 24-Apr-11 12:15 codac/tests/test_ctcdelay.py
+-rw-rw-rw-  2.0 fat    45322 b- defN 24-Apr-11 12:15 codac/tests/test_ctceval.py
+-rw-rw-rw-  2.0 fat      939 b- defN 24-Apr-11 12:15 codac/tests/test_ctcstatic.py
+-rw-rw-rw-  2.0 fat    13567 b- defN 24-Apr-11 12:15 codac/tests/test_definition.py
+-rw-rw-rw-  2.0 fat     1156 b- defN 24-Apr-11 12:15 codac/tests/test_function.py
+-rw-rw-rw-  2.0 fat     4061 b- defN 24-Apr-11 12:15 codac/tests/test_multi_arithmetic.py
+-rw-rw-rw-  2.0 fat     1524 b- defN 24-Apr-11 12:15 codac/tests/test_numpy.py
+-rw-rw-rw-  2.0 fat     2057 b- defN 24-Apr-11 12:15 codac/tests/test_sepbox.py
+-rw-rw-rw-  2.0 fat      630 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1982 b- defN 24-Apr-11 12:19 codac-1.5.6.dist-info/RECORD
+24 files, 5090983 bytes uncompressed, 2052959 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,91 +1,73 @@
-Filename: codac/
-Comment: 
-
-Filename: codac-1.5.5.dist-info/
-Comment: 
-
-Filename: codac.libs/
-Comment: 
-
-Filename: codac/tests/
-Comment: 
-
-Filename: codac/empty.cpython-39-aarch64-linux-gnu.so
-Comment: 
-
-Filename: codac/core.cpython-39-aarch64-linux-gnu.so
-Comment: 
-
 Filename: codac/__init__.py
 Comment: 
 
-Filename: codac/codac2.cpython-39-aarch64-linux-gnu.so
+Filename: codac/codac2.cp39-win_amd64.pyd
 Comment: 
 
-Filename: codac/unsupported.cpython-39-aarch64-linux-gnu.so
+Filename: codac/core.cp39-win_amd64.pyd
 Comment: 
 
-Filename: codac/version.py
+Filename: codac/unsupported.cp39-win_amd64.pyd
 Comment: 
 
-Filename: codac/tests/test_numpy.py
-Comment: 
-
-Filename: codac/tests/test_ctcbox.py
+Filename: codac/version.py
 Comment: 
 
 Filename: codac/tests/__init__.py
 Comment: 
 
-Filename: codac/tests/test_sepbox.py
+Filename: codac/tests/test_actions.py
 Comment: 
 
-Filename: codac/tests/test_function.py
+Filename: codac/tests/test_arithmetic.py
 Comment: 
 
 Filename: codac/tests/test_cn.py
 Comment: 
 
 Filename: codac/tests/test_ctc_constell.py
 Comment: 
 
-Filename: codac/tests/test_actions.py
+Filename: codac/tests/test_ctcbox.py
+Comment: 
+
+Filename: codac/tests/test_ctccartprod.py
 Comment: 
 
 Filename: codac/tests/test_ctcdelay.py
 Comment: 
 
 Filename: codac/tests/test_ctceval.py
 Comment: 
 
-Filename: codac/tests/test_multi_arithmetic.py
+Filename: codac/tests/test_ctcstatic.py
 Comment: 
 
-Filename: codac/tests/test_ctccartprod.py
+Filename: codac/tests/test_definition.py
 Comment: 
 
-Filename: codac/tests/test_ctcstatic.py
+Filename: codac/tests/test_function.py
 Comment: 
 
-Filename: codac/tests/test_definition.py
+Filename: codac/tests/test_multi_arithmetic.py
 Comment: 
 
-Filename: codac/tests/test_arithmetic.py
+Filename: codac/tests/test_numpy.py
 Comment: 
 
-Filename: codac-1.5.5.dist-info/METADATA
+Filename: codac/tests/test_sepbox.py
 Comment: 
 
-Filename: codac-1.5.5.dist-info/top_level.txt
+Filename: codac-1.5.6.dist-info/METADATA
 Comment: 
 
-Filename: codac-1.5.5.dist-info/RECORD
+Filename: codac-1.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: codac-1.5.5.dist-info/WHEEL
+Filename: codac-1.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: codac.libs/core-a9d1df2d.cpython-39-aarch64-linux-gnu.so
+Filename: codac-1.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## codac/__init__.py

 * *Ordering differences only*

```diff
@@ -1,39 +1,39 @@
-# Verifying that the former module pyibex 
-# has not been loaded, which could cause conflicts
-import sys
-if 'pyibex' in sys.modules:
-  print('\nWarning: pyIbex has been merged into Codac, please do not use it anymore.')
-  print('Conflicts may occur between the two libraries.\n')
-
-from codac.core import *
-from .version import __version__
-
-
-# Predefined contractor objects
-
-class ctc:
-
-  delay = CtcDelay()
-  deriv = CtcDeriv()
-  eval = CtcEval()
-  dist = CtcDist()
-  polar = CtcPolar()
-
-
-# Deprecated functions from the former pyIbex library:
-
-def pySIVIA(X0, ops, epsilon, figure_name='', draw_boxes=True, save_result=True, color_maybe='', color_out='', color_in=''):
-  print('\nWarning: pySIVIA(..) is deprecated and has been replaced by SIVIA(..).')
-  print('More information can be found with help(SIVIA).\n')
-  print('Example of use:\n')
-  print('  SIVIA(x0, sep, 0.05, regular_paving=False, display_result=True, fig_name="SIVIA", return_result=True, color_map={SetValue.IN:"k[r]", SetValue.OUT:"k[b]", SetValue.UNKNOWN:"k[y]"})\n')
-
-  cmap = {}
-  if color_in:
-    cmap[SetValue.IN] = color_in
-  if color_out:
-    cmap[SetValue.OUT] = color_out
-  if color_maybe:
-    cmap[SetValue.UNKNOWN] = color_maybe
-
+# Verifying that the former module pyibex 
+# has not been loaded, which could cause conflicts
+import sys
+if 'pyibex' in sys.modules:
+  print('\nWarning: pyIbex has been merged into Codac, please do not use it anymore.')
+  print('Conflicts may occur between the two libraries.\n')
+
+from codac.core import *
+from .version import __version__
+
+
+# Predefined contractor objects
+
+class ctc:
+
+  delay = CtcDelay()
+  deriv = CtcDeriv()
+  eval = CtcEval()
+  dist = CtcDist()
+  polar = CtcPolar()
+
+
+# Deprecated functions from the former pyIbex library:
+
+def pySIVIA(X0, ops, epsilon, figure_name='', draw_boxes=True, save_result=True, color_maybe='', color_out='', color_in=''):
+  print('\nWarning: pySIVIA(..) is deprecated and has been replaced by SIVIA(..).')
+  print('More information can be found with help(SIVIA).\n')
+  print('Example of use:\n')
+  print('  SIVIA(x0, sep, 0.05, regular_paving=False, display_result=True, fig_name="SIVIA", return_result=True, color_map={SetValue.IN:"k[r]", SetValue.OUT:"k[b]", SetValue.UNKNOWN:"k[y]"})\n')
+
+  cmap = {}
+  if color_in:
+    cmap[SetValue.IN] = color_in
+  if color_out:
+    cmap[SetValue.OUT] = color_out
+  if color_maybe:
+    cmap[SetValue.UNKNOWN] = color_maybe
+
   return SIVIA(X0, ops, epsilon, regular_paving=False, display_result=draw_boxes, fig_name=figure_name, return_result=save_result, color_map=cmap)
```

## codac/version.py

```diff
@@ -1 +1 @@
-__version__="1.5.5"
+__version__="1.5.6"
```

## codac/tests/test_numpy.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2023
-# \author    Simon Rohou
-# \copyright Copyright 2023 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-import numpy as np
-from codac import *
-
-class TestNumpyMatrices(unittest.TestCase):
-
-  def test_numpytocodac(self):
-
-    cdA=IntervalMatrix(2,6)
-    cdA[0][0]=Interval(1)
-    cdA[0][1]=Interval(3)
-    cdA[0][2]=Interval(5)
-    cdA[0][3]=Interval(7)
-    cdA[0][4]=Interval(9)
-    cdA[0][5]=Interval(11)
-    cdA[1][0]=Interval(2)
-    cdA[1][1]=Interval(4)
-    cdA[1][2]=Interval(6)
-    cdA[1][3]=Interval(8)
-    cdA[1][4]=Interval(10)
-    cdA[1][5]=Interval(12)
-
-    npA=np.array([[1.,3.,5.,7.,9.,11.],[2.,4.,6.,8.,10.,12.]])
-    self.assertEqual(IntervalMatrix(npA), cdA)
-
-  def test_numpytocodac_withtranspose(self):
-
-    cdA=IntervalMatrix(2,6)
-    cdA[0][0]=Interval(1)
-    cdA[0][1]=Interval(3)
-    cdA[0][2]=Interval(5)
-    cdA[0][3]=Interval(7)
-    cdA[0][4]=Interval(9)
-    cdA[0][5]=Interval(11)
-    cdA[1][0]=Interval(2)
-    cdA[1][1]=Interval(4)
-    cdA[1][2]=Interval(6)
-    cdA[1][3]=Interval(8)
-    cdA[1][4]=Interval(10)
-    cdA[1][5]=Interval(12)
-
-    npA=np.array([[1.,2.],[3.,4.],[5.,6.],[7.,8.],[9.,10.],[11.,12.]]).T
-    self.assertEqual(IntervalMatrix(npA), cdA)
-        
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2023
+# \author    Simon Rohou
+# \copyright Copyright 2023 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+import numpy as np
+from codac import *
+
+class TestNumpyMatrices(unittest.TestCase):
+
+  def test_numpytocodac(self):
+
+    cdA=IntervalMatrix(2,6)
+    cdA[0][0]=Interval(1)
+    cdA[0][1]=Interval(3)
+    cdA[0][2]=Interval(5)
+    cdA[0][3]=Interval(7)
+    cdA[0][4]=Interval(9)
+    cdA[0][5]=Interval(11)
+    cdA[1][0]=Interval(2)
+    cdA[1][1]=Interval(4)
+    cdA[1][2]=Interval(6)
+    cdA[1][3]=Interval(8)
+    cdA[1][4]=Interval(10)
+    cdA[1][5]=Interval(12)
+
+    npA=np.array([[1.,3.,5.,7.,9.,11.],[2.,4.,6.,8.,10.,12.]])
+    self.assertEqual(IntervalMatrix(npA), cdA)
+
+  def test_numpytocodac_withtranspose(self):
+
+    cdA=IntervalMatrix(2,6)
+    cdA[0][0]=Interval(1)
+    cdA[0][1]=Interval(3)
+    cdA[0][2]=Interval(5)
+    cdA[0][3]=Interval(7)
+    cdA[0][4]=Interval(9)
+    cdA[0][5]=Interval(11)
+    cdA[1][0]=Interval(2)
+    cdA[1][1]=Interval(4)
+    cdA[1][2]=Interval(6)
+    cdA[1][3]=Interval(8)
+    cdA[1][4]=Interval(10)
+    cdA[1][5]=Interval(12)
+
+    npA=np.array([[1.,2.],[3.,4.],[5.,6.],[7.,8.],[9.,10.],[11.,12.]]).T
+    self.assertEqual(IntervalMatrix(npA), cdA)
+        
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctcbox.py

 * *Ordering differences only*

```diff
@@ -1,60 +1,60 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Quentin Brateau, Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestCtcBox(unittest.TestCase):
-
-  def test_ctcbox_1d(self):
-
-    # 1D IntervalVector
-    b1 = IntervalVector([[0, 1]])
-
-    # CtcBox
-    c = CtcBox(b1)
-
-    # Contraction test
-    x1 = IntervalVector([[-3, 4]])
-    x2 = IntervalVector([[-1, 0.25]])
-
-    # Testing x1
-    c.contract(x1)
-    self.assertEqual(x1[0], Interval(0, 1))
-
-    # Testing x2
-    c.contract(x2);
-    self.assertEqual(x2[0], Interval(0, 0.25))
-
-  def test_ctcbox_2d(self):
-
-    # 2D IntervalVector
-    b1 = IntervalVector([[1, 2], [3, 4]])
-
-    # CtcBox
-    c = CtcBox(b1)
-
-    # Contraction test
-    x1 = IntervalVector([[-3, 4], [2, 5]])
-    x2 = IntervalVector([[1.5, 3], [2, 3.5]])
-
-    # Testing x1
-    c.contract(x1)
-    self.assertEqual(x1, b1)
-
-    # Testing x2
-    c.contract(x2);
-    self.assertEqual(x2[0], Interval(1.5, 2))
-    self.assertEqual(x2[1], Interval(3, 3.5))
-    
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Quentin Brateau, Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestCtcBox(unittest.TestCase):
+
+  def test_ctcbox_1d(self):
+
+    # 1D IntervalVector
+    b1 = IntervalVector([[0, 1]])
+
+    # CtcBox
+    c = CtcBox(b1)
+
+    # Contraction test
+    x1 = IntervalVector([[-3, 4]])
+    x2 = IntervalVector([[-1, 0.25]])
+
+    # Testing x1
+    c.contract(x1)
+    self.assertEqual(x1[0], Interval(0, 1))
+
+    # Testing x2
+    c.contract(x2);
+    self.assertEqual(x2[0], Interval(0, 0.25))
+
+  def test_ctcbox_2d(self):
+
+    # 2D IntervalVector
+    b1 = IntervalVector([[1, 2], [3, 4]])
+
+    # CtcBox
+    c = CtcBox(b1)
+
+    # Contraction test
+    x1 = IntervalVector([[-3, 4], [2, 5]])
+    x2 = IntervalVector([[1.5, 3], [2, 3.5]])
+
+    # Testing x1
+    c.contract(x1)
+    self.assertEqual(x1, b1)
+
+    # Testing x2
+    c.contract(x2);
+    self.assertEqual(x2[0], Interval(1.5, 2))
+    self.assertEqual(x2[1], Interval(3, 3.5))
+    
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_sepbox.py

 * *Ordering differences only*

```diff
@@ -1,76 +1,76 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Quentin Brateau, Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestSepBox(unittest.TestCase):
-
-  def test_sepbox_1d(self):
-
-    # 1D IntervalVector
-    b1 = IntervalVector([[0, 1]])
-
-    # CtcBox
-    s = SepBox(b1)
-
-    # Contraction test
-    x1 = IntervalVector([[0.5, 1.5]])
-    x2 = IntervalVector([[-1, 2]])
-
-    # Testing x1
-    x1_in = IntervalVector(x1)
-    x1_out = IntervalVector(x1)
-    s.separate(x1_in, x1_out)
-    self.assertEqual(x1_in[0], Interval(1, 1.5))
-    self.assertEqual(x1_out[0], Interval(0.5, 1))
-
-    # Testing x2
-    x2_in = IntervalVector(x2)
-    x2_out = IntervalVector(x2)
-    s.separate(x2_in, x2_out)
-    self.assertEqual(x2_in[0], Interval(-1, 2))
-    self.assertEqual(x2_out[0], Interval(0, 1))
-
-
-  def test_sepbox_2d(self):
-
-    # 2D IntervalVector
-    b1 = IntervalVector([[1, 2], [3, 4]])
-
-    # CtcBox
-    s = SepBox(b1)
-
-    # Contraction test
-    x1 = IntervalVector([[0, 5], [0, 5]])
-    x2 = IntervalVector([[1.25, 1.75], [3.5, 4.5]])
-
-    # Testing x1
-    x1_in = IntervalVector(x1)
-    x1_out = IntervalVector(x1)
-    s.separate(x1_in, x1_out)
-    self.assertEqual(x1_in[0], Interval(0, 5))
-    self.assertEqual(x1_in[1], Interval(0, 5))
-    self.assertEqual(x1_out[0], Interval(1, 2))
-    self.assertEqual(x1_out[1], Interval(3, 4))
-
-    # Testing x2
-    x2_in = IntervalVector(x2)
-    x2_out = IntervalVector(x2)
-    s.separate(x2_in, x2_out)
-    self.assertEqual(x2_in[0], Interval(1.25, 1.75))
-    self.assertEqual(x2_in[1], Interval(4, 4.5))
-    self.assertEqual(x2_out[0], Interval(1.25, 1.75))
-    self.assertEqual(x2_out[1], Interval(3.5, 4))
-    
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Quentin Brateau, Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestSepBox(unittest.TestCase):
+
+  def test_sepbox_1d(self):
+
+    # 1D IntervalVector
+    b1 = IntervalVector([[0, 1]])
+
+    # CtcBox
+    s = SepBox(b1)
+
+    # Contraction test
+    x1 = IntervalVector([[0.5, 1.5]])
+    x2 = IntervalVector([[-1, 2]])
+
+    # Testing x1
+    x1_in = IntervalVector(x1)
+    x1_out = IntervalVector(x1)
+    s.separate(x1_in, x1_out)
+    self.assertEqual(x1_in[0], Interval(1, 1.5))
+    self.assertEqual(x1_out[0], Interval(0.5, 1))
+
+    # Testing x2
+    x2_in = IntervalVector(x2)
+    x2_out = IntervalVector(x2)
+    s.separate(x2_in, x2_out)
+    self.assertEqual(x2_in[0], Interval(-1, 2))
+    self.assertEqual(x2_out[0], Interval(0, 1))
+
+
+  def test_sepbox_2d(self):
+
+    # 2D IntervalVector
+    b1 = IntervalVector([[1, 2], [3, 4]])
+
+    # CtcBox
+    s = SepBox(b1)
+
+    # Contraction test
+    x1 = IntervalVector([[0, 5], [0, 5]])
+    x2 = IntervalVector([[1.25, 1.75], [3.5, 4.5]])
+
+    # Testing x1
+    x1_in = IntervalVector(x1)
+    x1_out = IntervalVector(x1)
+    s.separate(x1_in, x1_out)
+    self.assertEqual(x1_in[0], Interval(0, 5))
+    self.assertEqual(x1_in[1], Interval(0, 5))
+    self.assertEqual(x1_out[0], Interval(1, 2))
+    self.assertEqual(x1_out[1], Interval(3, 4))
+
+    # Testing x2
+    x2_in = IntervalVector(x2)
+    x2_out = IntervalVector(x2)
+    s.separate(x2_in, x2_out)
+    self.assertEqual(x2_in[0], Interval(1.25, 1.75))
+    self.assertEqual(x2_in[1], Interval(4, 4.5))
+    self.assertEqual(x2_out[0], Interval(1.25, 1.75))
+    self.assertEqual(x2_out[1], Interval(3.5, 4))
+    
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_function.py

 * *Ordering differences only*

```diff
@@ -1,34 +1,34 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestFunctionOnTube(unittest.TestCase):
-
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-    def test_Functions_1(self):
-
-        x = TubeVector(Interval(0.,10.), 0.01, TFunction("sin(t)+[-0.01,0.01]"));
-        f = TFunction("x", "t/10.+x");
-        y1 = TubeVector(f.eval_vector(x));
-        y2 = TubeVector(Interval(0.,10.), 0.01, TFunction("t/10.+sin(t)+[-0.01,0.01]"));
-        self.assertAlmostEqual(y1.volume(), y2.volume());
-
-    
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestFunctionOnTube(unittest.TestCase):
+
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+    def test_Functions_1(self):
+
+        x = TubeVector(Interval(0.,10.), 0.01, TFunction("sin(t)+[-0.01,0.01]"));
+        f = TFunction("x", "t/10.+x");
+        y1 = TubeVector(f.eval_vector(x));
+        y2 = TubeVector(Interval(0.,10.), 0.01, TFunction("t/10.+sin(t)+[-0.01,0.01]"));
+        self.assertAlmostEqual(y1.volume(), y2.volume());
+
+    
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_cn.py

 * *Ordering differences only*

```diff
@@ -1,580 +1,580 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestCN(unittest.TestCase):
-
-  def test_CN_simple(self):
-
-    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c"))
-    a = Interval(0,1)
-    b = Interval(-1,1)
-    c = Interval(1.5,2)
-
-    cn = ContractorNetwork()
-    cn.add(ctc_plus, [a, b, c]) 
-    cn.contract()
-
-    self.assertEqual(a, Interval(0.5,1))
-    self.assertEqual(b, Interval(0.5,1))
-    self.assertEqual(c, Interval(1.5,2))
-
-    self.assertEqual(cn.nb_dom(), 3)
-    self.assertEqual(cn.nb_ctc(), 1)
-
-
-  def test_simple_static_case(self):
-
-    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c")) # algebraic constraint a+b=c
-
-    a = IntervalVector(2, [0,1])
-    b = IntervalVector(2, [-1,1])
-    c = IntervalVector(2, [1.5,2])
-
-    cn = ContractorNetwork()
-    cn.add(ctc_plus, [a[0], b[0], c[0]]) 
-    cn.contract()
-
-    self.assertEqual(a[0], Interval(0.5,1))
-    self.assertEqual(b[0], Interval(0.5,1))
-    self.assertEqual(c[0], Interval(1.5,2))
-
-    self.assertEqual(cn.nb_dom(), 3)
-    self.assertEqual(cn.nb_ctc(), 1)
-
-
-  def test_dependencies_on_vector_components(self):
-
-    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c")) # algebraic constraint a+b=c
-
-    a = IntervalVector(2, [0,1])
-    b = IntervalVector(2, [-1,1])
-    c = IntervalVector(2, [1.5,2])
-    d = IntervalVector(2, [0.,0.])
-    e = IntervalVectore(2)
-
-    cn = ContractorNetwork()
-    # Contractors are added to the graph, 
-    # the first one contracts the vector sets, the second one then contracts the components intervals,
-    # and so it should trigger again the first one since components have changed.
-    cn.add(ctc_plus, [b, d, e])
-    cn.add(ctc_plus, [b, d, e])
-    cn.add(ctc_plus, [b, d, e])
-    cn.add(ctc_plus, [a[0], b[0], c[0]])
-    cn.add(ctc_plus, [a[0], b[0], c[0]])
-    cn.add(ctc_plus, [a[0], b[0], c[0]])
-    cn.add(ctc_plus, [a[0], b[0], c[0]])
-    cn.contract()
-
-    self.assertEqual(a[0], Interval(0.5,1))
-    self.assertEqual(b[0], Interval(0.5,1))
-    self.assertEqual(c[0], Interval(1.5,2))
-    self.assertEqual(d[0], Interval(0))
-    self.assertEqual(e[0], Interval(0.5,1))
-
-    # Before setting names (some vectors not added entirely):
-    self.assertEqual(cn.nb_dom(), 3*3+2)
-    # vector items contractors + ctc_plus in array mode + ctc_plus on scalar values
-    self.assertEqual(cn.nb_ctc(), 3+2+1)
-
-    cn.set_name(a, "a")
-    cn.set_name(b, "b")
-    cn.set_name(c, "c")
-    cn.set_name(d, "d")
-    cn.set_name(e, "e")
-    cn.set_name(ctc_plus, "+")
-    cn.print_dot_graph("cn_vector_dependencies")
-
-    self.assertEqual(cn.nb_dom(), 3*5)
-    # vector items contractors + ctc_plus in array mode + ctc_plus on scalar values
-    self.assertEqual(cn.nb_ctc(), 5+2+1)
-
-
-  def test_dependencies_on_vector_components(self):
-
-    dt = 5
-    domain = Interval(0.,20.)
-    x = Tube(domain, dt, Interval(-10.,10.))
-    v = Tube(domain, dt, Interval(0.))
-
-    ctc_deriv = CtcDeriv()
-
-    cn = ContractorNetwork()
-    cn.add(ctc_deriv, [x, v])
-    cn.add(ctc_deriv, [x, v]) # redundant contractor that should not be added
-    cn.contract()
-    cn.contract()
-
-    self.assertEqual(v.codomain(), Interval(0.))
-    self.assertEqual(x.codomain(), Interval(-10.,10.))
-    self.assertEqual(x.nb_slices(), 4)
-    self.assertEqual(v.nb_slices(), 4)
-    self.assertEqual(cn.nb_ctc(), 12)
-    self.assertEqual(cn.nb_dom(), 10)
-
-    ctc_eval = CtcEval()
-    t1 = Interval(5.)
-    z = Interval(2.)
-
-    cn.add(ctc_eval, [t1, z, x, v])
-    cn.add(ctc_eval, [t1, z, x, v])
-    cn.add(ctc_eval, [t1, z, x, v])
-    cn.add(ctc_eval, [t1, z, x, v]) # redundant contractor that should not be added
-    cn.contract()
-
-    cn.set_name(t1, "t_1")
-    cn.set_name(z, "z")
-    cn.set_name(x, "x")
-    cn.set_name(v, "v")
-    cn.print_dot_graph("cn_observation")
-
-    self.assertEqual(v.codomain(), Interval(0.))
-    self.assertEqual(x.codomain(), Interval(2.))
-    self.assertEqual(cn.nb_ctc(), 13)
-    self.assertEqual(cn.nb_dom(), 12)
-
-
-  def test_dependencies_on_vector_components(self):
-
-    dt = 5.
-    domain = Interval(0.,20.)
-    x = Tube(domain, dt, Interval(-10.,10.))
-    v = Tube(domain, dt, Interval(0.))
-
-    ctc_deriv = CtcDeriv()
-    ctc_f = CtcFunction(Function("x", "xdot", "xdot+sin(x)"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_deriv, [x, v])
-    cn.add(ctc_f, [x, v])
-
-    self.assertEqual(v.codomain(), Interval(0.))
-    self.assertEqual(x.codomain(), Interval(-10.,10.))
-    self.assertEqual(x.nb_slices(), 4)
-    self.assertEqual(v.nb_slices(), 4)
-    self.assertEqual(cn.nb_ctc(), 16)
-    self.assertEqual(cn.nb_dom(), 10)
-
-    cn.set_fixedpoint_ratio(0.8)
-    cn.contract()
-
-
-  def test_dependencies_on_vector_components_1(self):
-
-    x = Interval(0,1)
-    y = Interval(-2,3)
-    a = Interval(1,20)
-    vx = IntervalVector(2,x)
-    vy = IntervalVector(2,y)
-    va = IntervalVector(2,a)
-    vec = [4,0.5]
-    
-    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
-    ctc_cos = CtcFunction(Function("b", "c", "a", "b+c-a"))
-    ctc_minus = CtcFunction(Function("b", "c", "b-c-0"))
-
-    cn = ContractorNetwork()
-
-    cn.add(ctc_add, [x,y,a])
-    cn.add(ctc_add, [x,y,a])
-    cn.contract()
-
-    self.assertEqual(x, Interval(0,1))
-    self.assertEqual(y, Interval(0,3))
-    self.assertEqual(a, Interval(1,4))
-    self.assertEqual(cn.nb_dom(), 3)
-    self.assertEqual(cn.nb_ctc(), 1)
-
-
-  def test_dependencies_on_vector_components_2(self):
-
-    x = Interval(0,1)
-    y = Interval(-2,3)
-    a = Interval(1,20)
-    vx = IntervalVector(2,x)
-    vy = IntervalVector(2,y)
-    va = IntervalVector(2,a)
-    vec = [4,0.5]
-    
-    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
-    ctc_cos = CtcFunction(Function("b", "c", "a", "b+c-a"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [vx,vy,va])
-    cn.add(ctc_add, [vx[0],vy[0],va[0]])
-    cn.contract()
-
-    self.assertEqual(vx, IntervalVector(2,[0,1]))
-    self.assertEqual(vy, IntervalVector(2,[0,3]))
-    self.assertEqual(va, IntervalVector(2,[1,4]))
-
-    self.assertEqual(cn.nb_dom(), 3*3)
-    self.assertEqual(cn.nb_ctc(), 3+2)
-
-    cn.set_name(va, "a")
-    cn.set_name(vx, "x")
-    cn.set_name(vy, "y")
-    cn.print_dot_graph("cn_function")
-
-
-  def test_CtcFunction_on_heterogeneous_variables(self):
-
-    x = IntervalVector([[0,1],[-2,3]])
-    a = Interval(1,20)
-    
-    ctc_add = CtcFunction(Function("b[2]", "a", "b[0]+b[1]-a"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a])
-    cn.contract()
-
-    self.assertEqual(x[0], Interval(0,1))
-    self.assertEqual(x[1], Interval(0,3))
-    self.assertEqual(a, Interval(1,4))
-
-
-  def test_subvector(self):
-
-    x = IntervalVector([[0,1],[-2,3],[1,20]])
-
-    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
-
-    cn = ContractorNetwork()
-    sub_x = cn.subvector(x,1,2)
-
-    self.assertEqual(sub_x[0], Interval(-2,3))
-    self.assertEqual(sub_x[1], Interval(1,20))
-
-    cn.add(ctc_add, [x[0],x[1],x[2]])
-    cn.contract()
-
-    self.assertEqual(x[0], Interval(0,1))
-    self.assertEqual(x[1], Interval(0,3))
-    self.assertEqual(x[2], Interval(1,4))
-
-    self.assertEqual(sub_x[0], Interval(0,3))
-    self.assertEqual(sub_x[1], Interval(1,4))
-
-    sub_x[0] = Interval(1,2)
-    cn.trigger_all_contractors()
-    cn.contract()
-    self.assertEqual(x[1], Interval(1,2))
-
-
-  def test_singleton_variables_double_or_Vector_1(self):
-
-    x = Interval(0,1)
-    y = Interval(-2,3)
-    a = Interval(1,20)
-
-    double_y = 1.
-    vector_y = [2, 1.]
-    ivx = IntervalVector(2,x)
-    ivy = IntervalVector(2,y)
-    iva = IntervalVector(2,a)
-    
-    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
-
-    cn = ContractorNetwork()
-
-    cn.add(ctc_add, [x,double_y,a])
-    cn.add(ctc_add, [x,double_y,a]) # redundant adding
-    cn.add(ctc_add, [x,double_y,a]) # redundant adding
-    cn.contract()
-
-    self.assertEqual(x, Interval(0,1))
-    self.assertEqual(double_y, 1.)
-    self.assertEqual(a, Interval(1,2))
-    #self.assertEqual(cn.nb_dom(), 3) # todo: not able to get reference from a py::float_
-    #self.assertEqual(cn.nb_ctc(), 1) # todo: not able to get reference from a py::float_: adds several contractors
-
-
-  def test_singleton_variables_double_or_Vector_2(self):
-
-    x = Interval(0,1)
-    y = Interval(-2,3)
-    a = Interval(1,20)
-
-    vector_y = [2, 1.]
-    ivx = IntervalVector(2,x)
-    iva = IntervalVector(2,a)
-    
-    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
-
-    cn = ContractorNetwork()
-
-    cn.add(ctc_add, [ivx,vector_y,iva])
-    cn.add(ctc_add, [ivx,vector_y,iva]) # redundant adding
-    cn.add(ctc_add, [ivx,vector_y,iva]) # redundant adding
-    cn.contract()
-
-    self.assertEqual(ivx, IntervalVector(2,[0,1]))
-    self.assertEqual(vector_y, [2,1.])
-    self.assertEqual(iva, IntervalVector([[2,3],[1,2]]))
-    #self.assertEqual(cn.nb_dom(), 3*3) # todo: not able to get reference from a py::list
-    #self.assertEqual(cn.nb_ctc(), 3+2) # todo: not able to get reference from a py::list
-
-    cn.set_name(vector_y, "y")
-    cn.set_name(ivx, "x")
-    cn.set_name(iva, "a")
-    cn.set_name(ctc_add, "+")
-    cn.print_dot_graph("cn_singleton")
-
-
-  def test_heterogeneous_variables_with_CtcFunction_1(self):
-
-    dt = 0.1
-    tdomain = Interval(0.,10.)
-
-    x = Interval(2,3)
-    a = Tube(tdomain, dt, Interval(4.,5.))
-    b = Tube(tdomain, dt, Interval(5.,9.))
-
-    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a,b])
-    cn.contract()
-
-    self.assertEqual(x, Interval(2.,3.))
-    self.assertEqual(a.codomain(), Interval(4.,5.))
-    self.assertEqual(b.codomain(), Interval(6.,8.))
-
-
-  def test_heterogeneous_variables_with_CtcFunction_2(self):
-
-    dt = 0.1
-    tdomain = Interval(0.,10.)
-
-    x = Interval(-1.,3.)
-    a = Tube(tdomain, dt, Interval(6.,7.))
-    b = Tube(tdomain, dt, Interval(7.))
-
-    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a,b])
-    cn.contract()
-
-    cn.set_name(x, "x")
-    cn.set_name(a, "a")
-    cn.set_name(b, "b")
-
-    self.assertEqual(x, Interval(0.,1.))
-    self.assertEqual(a.codomain(), Interval(6.,7.))
-    self.assertEqual(b.codomain(), Interval(7.))
-
-
-  def test_heterogeneous_variables_with_CtcFunction_3(self):
-
-    dt = 0.1
-    tdomain = Interval(0.,10.)
-
-    x = Interval(2.,2.5)
-    a = Tube(tdomain, dt, Interval(0.,10.))
-    b = Tube(tdomain, dt, Interval(7.))
-
-    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a,b])
-    cn.contract()
-
-    self.assertEqual(x, Interval(2.,2.5))
-    self.assertEqual(a.codomain(), Interval(4.5,5.))
-    self.assertEqual(b.codomain(), Interval(7.))
-
-
-  def test_heterogeneous_variables_with_CtcFunction_4(self):
-
-    dt = 0.1
-    tdomain = Interval(0.,10.)
-
-    x = Interval(2.,2.5)
-    a = Tube(tdomain, dt, TFunction("cos(t)"))
-    b = Tube(tdomain, dt)
-
-    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a,b])
-    cn.contract()
-    
-    result = Tube(tdomain, dt, TFunction("cos(t)"))
-    result += x
-
-    self.assertEqual(x, Interval(2.,2.5))
-    self.assertEqual(b, result)
-
-
-  def test_adding_continuous_data(self):
-
-    dt = 1.
-    tdomain = Interval(0.,5.)
-
-    x = Tube(tdomain, dt)
-    v = Tube(tdomain, dt)
-    x.set(Interval(0.), 0.) # todo: allow to write x.set(0., 0.) ?
-
-    ctc_deriv = CtcDeriv()
-    cn = ContractorNetwork()
-    cn.add(ctc_deriv, [x,v])
-
-    cn.set_name(x, "x")
-    cn.set_name(v, "v")
-    cn.print_dot_graph("cn_adddata")
-
-    cn.contract()
-
-    self.assertTrue((x.codomain() == Interval.ALL_REALS \
-      or x.codomain(), Interval(-99999, 99999))) # todo: remove this
-    self.assertTrue((v.codomain() == Interval.ALL_REALS \
-      or x.codomain(), Interval(-99999, 99999))) # todo: remove this
-    self.assertEqual(cn.nb_ctc_in_stack(), 0)
-
-    # Adding data
-    cn.add_data(v, 0., Interval(0.))
-    self.assertEqual(cn.nb_ctc_in_stack(), 0)
-    cn.add_data(v, 0.3, Interval(0.))
-    self.assertEqual(cn.nb_ctc_in_stack(), 0)
-    cn.add_data(v, 0.4, Interval(0.))
-    cn.add_data(v, 0.5, Interval(0.))
-    # cn.add_data(x, 0.5, Interval(0.5))) # should fail
-    self.assertEqual(cn.nb_ctc_in_stack(), 0)
-    cn.add_data(v, 0.99, Interval(0.))
-    self.assertEqual(cn.nb_ctc_in_stack(), 0)
-    cn.add_data(v, 1.3, Interval(0.))
-    self.assertEqual(cn.nb_ctc_in_stack(), 3)
-    cn.add_data(v, 1.5, Interval(0.))
-    self.assertEqual(cn.nb_ctc_in_stack(), 3)
-    cn.add_data(v, 4.5, Interval(-3.)) # accross two slices
-    self.assertEqual(cn.nb_ctc_in_stack(), 9)
-    cn.add_data(v, 5.5, Interval(1.)) # after tf
-    self.assertEqual(cn.nb_ctc_in_stack(), 10)
-
-    self.assertEqual(v(0), Interval(0.))
-    self.assertEqual(v(1), Interval(-0.5,0.))
-    self.assertEqual(v(2), Interval(-1.5,-0.5))
-    self.assertEqual(v(3), Interval(-2.5,-1.5))
-    self.assertEqual(v(4), Interval(-3.,-1.))
-
-
-  def test_create_interm_var_tube(self):
-
-    dt = 0.1
-    tdomain = Interval(0.,10.)
-    x = Tube(tdomain, dt)
-    x.set(Interval(0.), 0.)
-
-    self.assertEqual(x.codomain(), Interval())
-
-    cn = ContractorNetwork()
-    ctc_deriv = CtcDeriv()
-
-    v_local = Tube(tdomain, dt, TFunction("0"))
-    #v_inside = cn.create_interm_var(v_local)
-    #cn.add(ctc_deriv, [x,v_inside])
-
-    #cn.contract()
-    #self.assertEqual(x.codomain(), Interval(0))
-
-  
-  def test_cn_variables(self):
-
-    cn = ContractorNetwork()
-    a = IntervalVar()
-
-    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c"))
-    a1 = Interval(0,1)
-    b1 = Interval(-1,1)
-    a2 = Interval(-1,1)
-    b2 = Interval(0,1)
-    c = Interval(1.5,2);
-
-    cn.add(ctc_plus, [a, b1, c])
-
-    cn.contract({
-      a: a1
-    })
-
-    self.assertEqual(a1, Interval(0.5,1))
-    self.assertEqual(b1, Interval(0.5,1))
-    self.assertEqual(c, Interval(1.5,2))
-
-    a1 |= Interval(0,1)
-    b1 |= Interval(-1,1)
-
-    cn.contract({
-      a: a1
-    })
-
-    self.assertEqual(a1, Interval(0.5,1))
-    self.assertEqual(b1, Interval(0.5,1))
-    self.assertEqual(c, Interval(1.5,2))
-
-    cn.contract({
-      a: a2,
-      b1: b2
-    })
-
-    self.assertEqual(a1, Interval(0.5,1))
-    self.assertEqual(b1, Interval(0.5,1))
-    self.assertEqual(a2, Interval(0.5,1))
-    self.assertEqual(b2, Interval(0.5,1))
-    self.assertEqual(c, Interval(1.5,2))
-
-    self.assertEqual(cn.nb_dom(), 3)
-    self.assertEqual(cn.nb_ctc(), 1)
-
-  def test_cn_heterogeneous_variables(self):
-
-    a = IntervalVar()
-    x = IntervalVectorVar(2)
-    
-    ctc_add = CtcFunction(Function("b[2]", "c", "b[0]+b[1]-c"))
-
-    cn = ContractorNetwork()
-    cn.add(ctc_add, [x,a])
-
-    x1 = IntervalVector([[0,1],[-2,3]])
-    a1 = Interval(1,20)
-    cn.contract({
-      a: a1,
-      x: x1
-    })
-
-    self.assertEqual(x1[0], Interval(0,1))
-    self.assertEqual(x1[1], Interval(0,3))
-    self.assertEqual(a1, Interval(1,4))
-
-    x2 = IntervalVector([[10,10.5],[22,99]])
-
-    a2 = Interval(32,33)
-    cn.contract({
-      x: x2,
-      a: a2
-    })
-
-    #self.assertEqual(a, Interval())
-    #self.assertEqual(x, IntervalVector(2))
-
-    self.assertEqual(x1[0], Interval(0,1)) # remain unchanged
-    self.assertEqual(x1[1], Interval(0,3)) # remain unchanged
-    self.assertEqual(a1, Interval(1,4))    # remain unchanged
-    self.assertEqual(x2[0], Interval(10,10.5))
-    self.assertEqual(x2[1], Interval(22,23))
-    self.assertEqual(a2, Interval(32,33))
-
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestCN(unittest.TestCase):
+
+  def test_CN_simple(self):
+
+    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c"))
+    a = Interval(0,1)
+    b = Interval(-1,1)
+    c = Interval(1.5,2)
+
+    cn = ContractorNetwork()
+    cn.add(ctc_plus, [a, b, c]) 
+    cn.contract()
+
+    self.assertEqual(a, Interval(0.5,1))
+    self.assertEqual(b, Interval(0.5,1))
+    self.assertEqual(c, Interval(1.5,2))
+
+    self.assertEqual(cn.nb_dom(), 3)
+    self.assertEqual(cn.nb_ctc(), 1)
+
+
+  def test_simple_static_case(self):
+
+    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c")) # algebraic constraint a+b=c
+
+    a = IntervalVector(2, [0,1])
+    b = IntervalVector(2, [-1,1])
+    c = IntervalVector(2, [1.5,2])
+
+    cn = ContractorNetwork()
+    cn.add(ctc_plus, [a[0], b[0], c[0]]) 
+    cn.contract()
+
+    self.assertEqual(a[0], Interval(0.5,1))
+    self.assertEqual(b[0], Interval(0.5,1))
+    self.assertEqual(c[0], Interval(1.5,2))
+
+    self.assertEqual(cn.nb_dom(), 3)
+    self.assertEqual(cn.nb_ctc(), 1)
+
+
+  def test_dependencies_on_vector_components(self):
+
+    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c")) # algebraic constraint a+b=c
+
+    a = IntervalVector(2, [0,1])
+    b = IntervalVector(2, [-1,1])
+    c = IntervalVector(2, [1.5,2])
+    d = IntervalVector(2, [0.,0.])
+    e = IntervalVectore(2)
+
+    cn = ContractorNetwork()
+    # Contractors are added to the graph, 
+    # the first one contracts the vector sets, the second one then contracts the components intervals,
+    # and so it should trigger again the first one since components have changed.
+    cn.add(ctc_plus, [b, d, e])
+    cn.add(ctc_plus, [b, d, e])
+    cn.add(ctc_plus, [b, d, e])
+    cn.add(ctc_plus, [a[0], b[0], c[0]])
+    cn.add(ctc_plus, [a[0], b[0], c[0]])
+    cn.add(ctc_plus, [a[0], b[0], c[0]])
+    cn.add(ctc_plus, [a[0], b[0], c[0]])
+    cn.contract()
+
+    self.assertEqual(a[0], Interval(0.5,1))
+    self.assertEqual(b[0], Interval(0.5,1))
+    self.assertEqual(c[0], Interval(1.5,2))
+    self.assertEqual(d[0], Interval(0))
+    self.assertEqual(e[0], Interval(0.5,1))
+
+    # Before setting names (some vectors not added entirely):
+    self.assertEqual(cn.nb_dom(), 3*3+2)
+    # vector items contractors + ctc_plus in array mode + ctc_plus on scalar values
+    self.assertEqual(cn.nb_ctc(), 3+2+1)
+
+    cn.set_name(a, "a")
+    cn.set_name(b, "b")
+    cn.set_name(c, "c")
+    cn.set_name(d, "d")
+    cn.set_name(e, "e")
+    cn.set_name(ctc_plus, "+")
+    cn.print_dot_graph("cn_vector_dependencies")
+
+    self.assertEqual(cn.nb_dom(), 3*5)
+    # vector items contractors + ctc_plus in array mode + ctc_plus on scalar values
+    self.assertEqual(cn.nb_ctc(), 5+2+1)
+
+
+  def test_dependencies_on_vector_components(self):
+
+    dt = 5
+    domain = Interval(0.,20.)
+    x = Tube(domain, dt, Interval(-10.,10.))
+    v = Tube(domain, dt, Interval(0.))
+
+    ctc_deriv = CtcDeriv()
+
+    cn = ContractorNetwork()
+    cn.add(ctc_deriv, [x, v])
+    cn.add(ctc_deriv, [x, v]) # redundant contractor that should not be added
+    cn.contract()
+    cn.contract()
+
+    self.assertEqual(v.codomain(), Interval(0.))
+    self.assertEqual(x.codomain(), Interval(-10.,10.))
+    self.assertEqual(x.nb_slices(), 4)
+    self.assertEqual(v.nb_slices(), 4)
+    self.assertEqual(cn.nb_ctc(), 12)
+    self.assertEqual(cn.nb_dom(), 10)
+
+    ctc_eval = CtcEval()
+    t1 = Interval(5.)
+    z = Interval(2.)
+
+    cn.add(ctc_eval, [t1, z, x, v])
+    cn.add(ctc_eval, [t1, z, x, v])
+    cn.add(ctc_eval, [t1, z, x, v])
+    cn.add(ctc_eval, [t1, z, x, v]) # redundant contractor that should not be added
+    cn.contract()
+
+    cn.set_name(t1, "t_1")
+    cn.set_name(z, "z")
+    cn.set_name(x, "x")
+    cn.set_name(v, "v")
+    cn.print_dot_graph("cn_observation")
+
+    self.assertEqual(v.codomain(), Interval(0.))
+    self.assertEqual(x.codomain(), Interval(2.))
+    self.assertEqual(cn.nb_ctc(), 13)
+    self.assertEqual(cn.nb_dom(), 12)
+
+
+  def test_dependencies_on_vector_components(self):
+
+    dt = 5.
+    domain = Interval(0.,20.)
+    x = Tube(domain, dt, Interval(-10.,10.))
+    v = Tube(domain, dt, Interval(0.))
+
+    ctc_deriv = CtcDeriv()
+    ctc_f = CtcFunction(Function("x", "xdot", "xdot+sin(x)"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_deriv, [x, v])
+    cn.add(ctc_f, [x, v])
+
+    self.assertEqual(v.codomain(), Interval(0.))
+    self.assertEqual(x.codomain(), Interval(-10.,10.))
+    self.assertEqual(x.nb_slices(), 4)
+    self.assertEqual(v.nb_slices(), 4)
+    self.assertEqual(cn.nb_ctc(), 16)
+    self.assertEqual(cn.nb_dom(), 10)
+
+    cn.set_fixedpoint_ratio(0.8)
+    cn.contract()
+
+
+  def test_dependencies_on_vector_components_1(self):
+
+    x = Interval(0,1)
+    y = Interval(-2,3)
+    a = Interval(1,20)
+    vx = IntervalVector(2,x)
+    vy = IntervalVector(2,y)
+    va = IntervalVector(2,a)
+    vec = [4,0.5]
+    
+    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
+    ctc_cos = CtcFunction(Function("b", "c", "a", "b+c-a"))
+    ctc_minus = CtcFunction(Function("b", "c", "b-c-0"))
+
+    cn = ContractorNetwork()
+
+    cn.add(ctc_add, [x,y,a])
+    cn.add(ctc_add, [x,y,a])
+    cn.contract()
+
+    self.assertEqual(x, Interval(0,1))
+    self.assertEqual(y, Interval(0,3))
+    self.assertEqual(a, Interval(1,4))
+    self.assertEqual(cn.nb_dom(), 3)
+    self.assertEqual(cn.nb_ctc(), 1)
+
+
+  def test_dependencies_on_vector_components_2(self):
+
+    x = Interval(0,1)
+    y = Interval(-2,3)
+    a = Interval(1,20)
+    vx = IntervalVector(2,x)
+    vy = IntervalVector(2,y)
+    va = IntervalVector(2,a)
+    vec = [4,0.5]
+    
+    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
+    ctc_cos = CtcFunction(Function("b", "c", "a", "b+c-a"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [vx,vy,va])
+    cn.add(ctc_add, [vx[0],vy[0],va[0]])
+    cn.contract()
+
+    self.assertEqual(vx, IntervalVector(2,[0,1]))
+    self.assertEqual(vy, IntervalVector(2,[0,3]))
+    self.assertEqual(va, IntervalVector(2,[1,4]))
+
+    self.assertEqual(cn.nb_dom(), 3*3)
+    self.assertEqual(cn.nb_ctc(), 3+2)
+
+    cn.set_name(va, "a")
+    cn.set_name(vx, "x")
+    cn.set_name(vy, "y")
+    cn.print_dot_graph("cn_function")
+
+
+  def test_CtcFunction_on_heterogeneous_variables(self):
+
+    x = IntervalVector([[0,1],[-2,3]])
+    a = Interval(1,20)
+    
+    ctc_add = CtcFunction(Function("b[2]", "a", "b[0]+b[1]-a"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a])
+    cn.contract()
+
+    self.assertEqual(x[0], Interval(0,1))
+    self.assertEqual(x[1], Interval(0,3))
+    self.assertEqual(a, Interval(1,4))
+
+
+  def test_subvector(self):
+
+    x = IntervalVector([[0,1],[-2,3],[1,20]])
+
+    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
+
+    cn = ContractorNetwork()
+    sub_x = cn.subvector(x,1,2)
+
+    self.assertEqual(sub_x[0], Interval(-2,3))
+    self.assertEqual(sub_x[1], Interval(1,20))
+
+    cn.add(ctc_add, [x[0],x[1],x[2]])
+    cn.contract()
+
+    self.assertEqual(x[0], Interval(0,1))
+    self.assertEqual(x[1], Interval(0,3))
+    self.assertEqual(x[2], Interval(1,4))
+
+    self.assertEqual(sub_x[0], Interval(0,3))
+    self.assertEqual(sub_x[1], Interval(1,4))
+
+    sub_x[0] = Interval(1,2)
+    cn.trigger_all_contractors()
+    cn.contract()
+    self.assertEqual(x[1], Interval(1,2))
+
+
+  def test_singleton_variables_double_or_Vector_1(self):
+
+    x = Interval(0,1)
+    y = Interval(-2,3)
+    a = Interval(1,20)
+
+    double_y = 1.
+    vector_y = [2, 1.]
+    ivx = IntervalVector(2,x)
+    ivy = IntervalVector(2,y)
+    iva = IntervalVector(2,a)
+    
+    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
+
+    cn = ContractorNetwork()
+
+    cn.add(ctc_add, [x,double_y,a])
+    cn.add(ctc_add, [x,double_y,a]) # redundant adding
+    cn.add(ctc_add, [x,double_y,a]) # redundant adding
+    cn.contract()
+
+    self.assertEqual(x, Interval(0,1))
+    self.assertEqual(double_y, 1.)
+    self.assertEqual(a, Interval(1,2))
+    #self.assertEqual(cn.nb_dom(), 3) # todo: not able to get reference from a py::float_
+    #self.assertEqual(cn.nb_ctc(), 1) # todo: not able to get reference from a py::float_: adds several contractors
+
+
+  def test_singleton_variables_double_or_Vector_2(self):
+
+    x = Interval(0,1)
+    y = Interval(-2,3)
+    a = Interval(1,20)
+
+    vector_y = [2, 1.]
+    ivx = IntervalVector(2,x)
+    iva = IntervalVector(2,a)
+    
+    ctc_add = CtcFunction(Function("b", "c", "a", "b+c-a"))
+
+    cn = ContractorNetwork()
+
+    cn.add(ctc_add, [ivx,vector_y,iva])
+    cn.add(ctc_add, [ivx,vector_y,iva]) # redundant adding
+    cn.add(ctc_add, [ivx,vector_y,iva]) # redundant adding
+    cn.contract()
+
+    self.assertEqual(ivx, IntervalVector(2,[0,1]))
+    self.assertEqual(vector_y, [2,1.])
+    self.assertEqual(iva, IntervalVector([[2,3],[1,2]]))
+    #self.assertEqual(cn.nb_dom(), 3*3) # todo: not able to get reference from a py::list
+    #self.assertEqual(cn.nb_ctc(), 3+2) # todo: not able to get reference from a py::list
+
+    cn.set_name(vector_y, "y")
+    cn.set_name(ivx, "x")
+    cn.set_name(iva, "a")
+    cn.set_name(ctc_add, "+")
+    cn.print_dot_graph("cn_singleton")
+
+
+  def test_heterogeneous_variables_with_CtcFunction_1(self):
+
+    dt = 0.1
+    tdomain = Interval(0.,10.)
+
+    x = Interval(2,3)
+    a = Tube(tdomain, dt, Interval(4.,5.))
+    b = Tube(tdomain, dt, Interval(5.,9.))
+
+    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a,b])
+    cn.contract()
+
+    self.assertEqual(x, Interval(2.,3.))
+    self.assertEqual(a.codomain(), Interval(4.,5.))
+    self.assertEqual(b.codomain(), Interval(6.,8.))
+
+
+  def test_heterogeneous_variables_with_CtcFunction_2(self):
+
+    dt = 0.1
+    tdomain = Interval(0.,10.)
+
+    x = Interval(-1.,3.)
+    a = Tube(tdomain, dt, Interval(6.,7.))
+    b = Tube(tdomain, dt, Interval(7.))
+
+    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a,b])
+    cn.contract()
+
+    cn.set_name(x, "x")
+    cn.set_name(a, "a")
+    cn.set_name(b, "b")
+
+    self.assertEqual(x, Interval(0.,1.))
+    self.assertEqual(a.codomain(), Interval(6.,7.))
+    self.assertEqual(b.codomain(), Interval(7.))
+
+
+  def test_heterogeneous_variables_with_CtcFunction_3(self):
+
+    dt = 0.1
+    tdomain = Interval(0.,10.)
+
+    x = Interval(2.,2.5)
+    a = Tube(tdomain, dt, Interval(0.,10.))
+    b = Tube(tdomain, dt, Interval(7.))
+
+    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a,b])
+    cn.contract()
+
+    self.assertEqual(x, Interval(2.,2.5))
+    self.assertEqual(a.codomain(), Interval(4.5,5.))
+    self.assertEqual(b.codomain(), Interval(7.))
+
+
+  def test_heterogeneous_variables_with_CtcFunction_4(self):
+
+    dt = 0.1
+    tdomain = Interval(0.,10.)
+
+    x = Interval(2.,2.5)
+    a = Tube(tdomain, dt, TFunction("cos(t)"))
+    b = Tube(tdomain, dt)
+
+    ctc_add = CtcFunction(Function("x", "a", "b", "x+a-b"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a,b])
+    cn.contract()
+    
+    result = Tube(tdomain, dt, TFunction("cos(t)"))
+    result += x
+
+    self.assertEqual(x, Interval(2.,2.5))
+    self.assertEqual(b, result)
+
+
+  def test_adding_continuous_data(self):
+
+    dt = 1.
+    tdomain = Interval(0.,5.)
+
+    x = Tube(tdomain, dt)
+    v = Tube(tdomain, dt)
+    x.set(Interval(0.), 0.) # todo: allow to write x.set(0., 0.) ?
+
+    ctc_deriv = CtcDeriv()
+    cn = ContractorNetwork()
+    cn.add(ctc_deriv, [x,v])
+
+    cn.set_name(x, "x")
+    cn.set_name(v, "v")
+    cn.print_dot_graph("cn_adddata")
+
+    cn.contract()
+
+    self.assertTrue((x.codomain() == Interval.ALL_REALS \
+      or x.codomain(), Interval(-99999, 99999))) # todo: remove this
+    self.assertTrue((v.codomain() == Interval.ALL_REALS \
+      or x.codomain(), Interval(-99999, 99999))) # todo: remove this
+    self.assertEqual(cn.nb_ctc_in_stack(), 0)
+
+    # Adding data
+    cn.add_data(v, 0., Interval(0.))
+    self.assertEqual(cn.nb_ctc_in_stack(), 0)
+    cn.add_data(v, 0.3, Interval(0.))
+    self.assertEqual(cn.nb_ctc_in_stack(), 0)
+    cn.add_data(v, 0.4, Interval(0.))
+    cn.add_data(v, 0.5, Interval(0.))
+    # cn.add_data(x, 0.5, Interval(0.5))) # should fail
+    self.assertEqual(cn.nb_ctc_in_stack(), 0)
+    cn.add_data(v, 0.99, Interval(0.))
+    self.assertEqual(cn.nb_ctc_in_stack(), 0)
+    cn.add_data(v, 1.3, Interval(0.))
+    self.assertEqual(cn.nb_ctc_in_stack(), 3)
+    cn.add_data(v, 1.5, Interval(0.))
+    self.assertEqual(cn.nb_ctc_in_stack(), 3)
+    cn.add_data(v, 4.5, Interval(-3.)) # accross two slices
+    self.assertEqual(cn.nb_ctc_in_stack(), 9)
+    cn.add_data(v, 5.5, Interval(1.)) # after tf
+    self.assertEqual(cn.nb_ctc_in_stack(), 10)
+
+    self.assertEqual(v(0), Interval(0.))
+    self.assertEqual(v(1), Interval(-0.5,0.))
+    self.assertEqual(v(2), Interval(-1.5,-0.5))
+    self.assertEqual(v(3), Interval(-2.5,-1.5))
+    self.assertEqual(v(4), Interval(-3.,-1.))
+
+
+  def test_create_interm_var_tube(self):
+
+    dt = 0.1
+    tdomain = Interval(0.,10.)
+    x = Tube(tdomain, dt)
+    x.set(Interval(0.), 0.)
+
+    self.assertEqual(x.codomain(), Interval())
+
+    cn = ContractorNetwork()
+    ctc_deriv = CtcDeriv()
+
+    v_local = Tube(tdomain, dt, TFunction("0"))
+    #v_inside = cn.create_interm_var(v_local)
+    #cn.add(ctc_deriv, [x,v_inside])
+
+    #cn.contract()
+    #self.assertEqual(x.codomain(), Interval(0))
+
+  
+  def test_cn_variables(self):
+
+    cn = ContractorNetwork()
+    a = IntervalVar()
+
+    ctc_plus = CtcFunction(Function("a", "b", "c", "a+b-c"))
+    a1 = Interval(0,1)
+    b1 = Interval(-1,1)
+    a2 = Interval(-1,1)
+    b2 = Interval(0,1)
+    c = Interval(1.5,2);
+
+    cn.add(ctc_plus, [a, b1, c])
+
+    cn.contract({
+      a: a1
+    })
+
+    self.assertEqual(a1, Interval(0.5,1))
+    self.assertEqual(b1, Interval(0.5,1))
+    self.assertEqual(c, Interval(1.5,2))
+
+    a1 |= Interval(0,1)
+    b1 |= Interval(-1,1)
+
+    cn.contract({
+      a: a1
+    })
+
+    self.assertEqual(a1, Interval(0.5,1))
+    self.assertEqual(b1, Interval(0.5,1))
+    self.assertEqual(c, Interval(1.5,2))
+
+    cn.contract({
+      a: a2,
+      b1: b2
+    })
+
+    self.assertEqual(a1, Interval(0.5,1))
+    self.assertEqual(b1, Interval(0.5,1))
+    self.assertEqual(a2, Interval(0.5,1))
+    self.assertEqual(b2, Interval(0.5,1))
+    self.assertEqual(c, Interval(1.5,2))
+
+    self.assertEqual(cn.nb_dom(), 3)
+    self.assertEqual(cn.nb_ctc(), 1)
+
+  def test_cn_heterogeneous_variables(self):
+
+    a = IntervalVar()
+    x = IntervalVectorVar(2)
+    
+    ctc_add = CtcFunction(Function("b[2]", "c", "b[0]+b[1]-c"))
+
+    cn = ContractorNetwork()
+    cn.add(ctc_add, [x,a])
+
+    x1 = IntervalVector([[0,1],[-2,3]])
+    a1 = Interval(1,20)
+    cn.contract({
+      a: a1,
+      x: x1
+    })
+
+    self.assertEqual(x1[0], Interval(0,1))
+    self.assertEqual(x1[1], Interval(0,3))
+    self.assertEqual(a1, Interval(1,4))
+
+    x2 = IntervalVector([[10,10.5],[22,99]])
+
+    a2 = Interval(32,33)
+    cn.contract({
+      x: x2,
+      a: a2
+    })
+
+    #self.assertEqual(a, Interval())
+    #self.assertEqual(x, IntervalVector(2))
+
+    self.assertEqual(x1[0], Interval(0,1)) # remain unchanged
+    self.assertEqual(x1[1], Interval(0,3)) # remain unchanged
+    self.assertEqual(a1, Interval(1,4))    # remain unchanged
+    self.assertEqual(x2[0], Interval(10,10.5))
+    self.assertEqual(x2[1], Interval(22,23))
+    self.assertEqual(a2, Interval(32,33))
+
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctc_constell.py

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestCtcConstell(unittest.TestCase):
-
-  def test_raw(self):
-
-    v_map = [IntervalVector(2)] * 4
-    v_map[0] = IntervalVector([1.5,2.5])
-    v_map[1] = IntervalVector([2.5,1.5])
-    v_map[2] = IntervalVector([4.,2.])
-    v_map[3] = IntervalVector([1.,0.5])
-
-    ctc_constell = CtcConstell(v_map)
-
-    x1 = IntervalVector([[0.5,6],[0,3.5]])
-    x2 = IntervalVector([[3.5,5.5],[0.5,2.5]])
-    x3 = IntervalVector([[2,5],[1,3]])
-    x4 = IntervalVector([[1,3],[1,2]])
-    x5 = IntervalVector([[1.5,2],[2.5,3]])
-    x6 = IntervalVector([[6.5,7.5],[2.5,3.5]])
-
-    ctc_constell.contract(x1)
-    ctc_constell.contract(x2)
-    ctc_constell.contract(x3)
-    ctc_constell.contract(x4)
-    ctc_constell.contract(x5)
-    ctc_constell.contract(x6)
-
-    self.assertEqual(x1, IntervalVector([[1,4],[0.5,2.5]]))
-    self.assertEqual(x2, IntervalVector([4,2]))
-    self.assertEqual(x3, IntervalVector([[2.5,4],[1.5,2]]))
-    self.assertEqual(x4, IntervalVector([2.5,1.5]))
-    self.assertEqual(x5, IntervalVector([1.5,2.5]))
-    self.assertEqual(x6, IntervalVector.empty(2))
-
-  def test_in_CN(self):
-
-    v_map = [IntervalVector(2)] * 4
-    v_map[0] = IntervalVector([1.5,2.5])
-    v_map[1] = IntervalVector([2.5,1.5])
-    v_map[2] = IntervalVector([4.,2.])
-    v_map[3] = IntervalVector([1.,0.5])
-
-    ctc_constell = CtcConstell(v_map)
-
-    x1 = IntervalVector([[0.5,6],[0,3.5]])
-    x2 = IntervalVector([[3.5,5.5],[0.5,2.5]])
-    x3 = IntervalVector([[2,5],[1,3]])
-    x4 = IntervalVector([[1,3],[1,2]])
-    x5 = IntervalVector([[1.5,2],[2.5,3]])
-    x6 = IntervalVector([[6.5,7.5],[2.5,3.5]])
-
-    cn = ContractorNetwork()
-    cn.add(ctc_constell, [x1])
-    cn.add(ctc_constell, [x2])
-    cn.add(ctc_constell, [x3])
-    cn.add(ctc_constell, [x4])
-    cn.add(ctc_constell, [x5])
-    cn.add(ctc_constell, [x6])
-    self.assertEqual(cn.nb_dom(), 18)
-    cn.contract()
-
-    self.assertEqual(x1, IntervalVector([[1,4],[0.5,2.5]]))
-    self.assertEqual(x2, IntervalVector([4,2]))
-    self.assertEqual(x3, IntervalVector([[2.5,4],[1.5,2]]))
-    self.assertEqual(x4, IntervalVector([2.5,1.5]))
-    self.assertEqual(x5, IntervalVector([1.5,2.5]))
-    self.assertEqual(x6, IntervalVector.empty(2))
-
-  def test_in_CN_with_list(self):
-
-    v_map = [IntervalVector(2)] * 4
-    v_map[0] = IntervalVector([1.5,2.5])
-    v_map[1] = IntervalVector([2.5,1.5])
-    v_map[2] = IntervalVector([4.,2.])
-    v_map[3] = IntervalVector([1.,0.5])
-
-    ctc_constell = CtcConstell(v_map)
-
-    n = 6
-    x = [IntervalVector(2)] * n
-    x[1-1] = IntervalVector([[0.5,6],[0,3.5]])
-    x[2-1] = IntervalVector([[3.5,5.5],[0.5,2.5]])
-    x[3-1] = IntervalVector([[2,5],[1,3]])
-    x[4-1] = IntervalVector([[1,3],[1,2]])
-    x[5-1] = IntervalVector([[1.5,2],[2.5,3]])
-    x[6-1] = IntervalVector([[6.5,7.5],[2.5,3.5]])
-
-    cn = ContractorNetwork()
-    for i in range(0,len(x)):
-      cn.add(ctc_constell, [x[i]])
-    cn.contract()
-
-    self.assertEqual(x[1-1], IntervalVector([[1,4],[0.5,2.5]]))
-    self.assertEqual(x[2-1], IntervalVector([4,2]))
-    self.assertEqual(x[3-1], IntervalVector([[2.5,4],[1.5,2]]))
-    self.assertEqual(x[4-1], IntervalVector([2.5,1.5]))
-    self.assertEqual(x[5-1], IntervalVector([1.5,2.5]))
-    self.assertEqual(x[6-1], IntervalVector.empty(2))
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestCtcConstell(unittest.TestCase):
+
+  def test_raw(self):
+
+    v_map = [IntervalVector(2)] * 4
+    v_map[0] = IntervalVector([1.5,2.5])
+    v_map[1] = IntervalVector([2.5,1.5])
+    v_map[2] = IntervalVector([4.,2.])
+    v_map[3] = IntervalVector([1.,0.5])
+
+    ctc_constell = CtcConstell(v_map)
+
+    x1 = IntervalVector([[0.5,6],[0,3.5]])
+    x2 = IntervalVector([[3.5,5.5],[0.5,2.5]])
+    x3 = IntervalVector([[2,5],[1,3]])
+    x4 = IntervalVector([[1,3],[1,2]])
+    x5 = IntervalVector([[1.5,2],[2.5,3]])
+    x6 = IntervalVector([[6.5,7.5],[2.5,3.5]])
+
+    ctc_constell.contract(x1)
+    ctc_constell.contract(x2)
+    ctc_constell.contract(x3)
+    ctc_constell.contract(x4)
+    ctc_constell.contract(x5)
+    ctc_constell.contract(x6)
+
+    self.assertEqual(x1, IntervalVector([[1,4],[0.5,2.5]]))
+    self.assertEqual(x2, IntervalVector([4,2]))
+    self.assertEqual(x3, IntervalVector([[2.5,4],[1.5,2]]))
+    self.assertEqual(x4, IntervalVector([2.5,1.5]))
+    self.assertEqual(x5, IntervalVector([1.5,2.5]))
+    self.assertEqual(x6, IntervalVector.empty(2))
+
+  def test_in_CN(self):
+
+    v_map = [IntervalVector(2)] * 4
+    v_map[0] = IntervalVector([1.5,2.5])
+    v_map[1] = IntervalVector([2.5,1.5])
+    v_map[2] = IntervalVector([4.,2.])
+    v_map[3] = IntervalVector([1.,0.5])
+
+    ctc_constell = CtcConstell(v_map)
+
+    x1 = IntervalVector([[0.5,6],[0,3.5]])
+    x2 = IntervalVector([[3.5,5.5],[0.5,2.5]])
+    x3 = IntervalVector([[2,5],[1,3]])
+    x4 = IntervalVector([[1,3],[1,2]])
+    x5 = IntervalVector([[1.5,2],[2.5,3]])
+    x6 = IntervalVector([[6.5,7.5],[2.5,3.5]])
+
+    cn = ContractorNetwork()
+    cn.add(ctc_constell, [x1])
+    cn.add(ctc_constell, [x2])
+    cn.add(ctc_constell, [x3])
+    cn.add(ctc_constell, [x4])
+    cn.add(ctc_constell, [x5])
+    cn.add(ctc_constell, [x6])
+    self.assertEqual(cn.nb_dom(), 18)
+    cn.contract()
+
+    self.assertEqual(x1, IntervalVector([[1,4],[0.5,2.5]]))
+    self.assertEqual(x2, IntervalVector([4,2]))
+    self.assertEqual(x3, IntervalVector([[2.5,4],[1.5,2]]))
+    self.assertEqual(x4, IntervalVector([2.5,1.5]))
+    self.assertEqual(x5, IntervalVector([1.5,2.5]))
+    self.assertEqual(x6, IntervalVector.empty(2))
+
+  def test_in_CN_with_list(self):
+
+    v_map = [IntervalVector(2)] * 4
+    v_map[0] = IntervalVector([1.5,2.5])
+    v_map[1] = IntervalVector([2.5,1.5])
+    v_map[2] = IntervalVector([4.,2.])
+    v_map[3] = IntervalVector([1.,0.5])
+
+    ctc_constell = CtcConstell(v_map)
+
+    n = 6
+    x = [IntervalVector(2)] * n
+    x[1-1] = IntervalVector([[0.5,6],[0,3.5]])
+    x[2-1] = IntervalVector([[3.5,5.5],[0.5,2.5]])
+    x[3-1] = IntervalVector([[2,5],[1,3]])
+    x[4-1] = IntervalVector([[1,3],[1,2]])
+    x[5-1] = IntervalVector([[1.5,2],[2.5,3]])
+    x[6-1] = IntervalVector([[6.5,7.5],[2.5,3.5]])
+
+    cn = ContractorNetwork()
+    for i in range(0,len(x)):
+      cn.add(ctc_constell, [x[i]])
+    cn.contract()
+
+    self.assertEqual(x[1-1], IntervalVector([[1,4],[0.5,2.5]]))
+    self.assertEqual(x[2-1], IntervalVector([4,2]))
+    self.assertEqual(x[3-1], IntervalVector([[2.5,4],[1.5,2]]))
+    self.assertEqual(x[4-1], IntervalVector([2.5,1.5]))
+    self.assertEqual(x[5-1], IntervalVector([1.5,2.5]))
+    self.assertEqual(x[6-1], IntervalVector.empty(2))
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_actions.py

 * *Ordering differences only*

```diff
@@ -1,41 +1,41 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2023
-# \author    Simon Rohou
-# \copyright Copyright 2023 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-try:
-  import numpy as np
-except:
-  print("NUMPY UNAVAILABLE")
-from codac import *
-from codac.codac2 import *
-
-class TestActions(unittest.TestCase):
-
-    def tests_action(self):
-
-        x = IntervalVector([[-1,0],[5,6]])
-        a = OctaSym([2,-1])
-
-        print(x)                 # Result: ([-1, 0] ; [5, 6])
-        print(a(x))              # Result: ([5, 6] ; [-0, 1])
-        print(a.invert()(a(x)))  # Result: ([-1, 0] ; [5, 6])
-
-        print(a)                 # Result: (2 -1)
-        print(a.invert())        # Result: (-2 1)
-        print(a*a)               # Result: (-1 -2)
-
-        self.assertEqual(a(x), IntervalVector([[5,6],[-0,1]]))
-        self.assertEqual(a.invert()(a(x)), IntervalVector([[-1,0],[5,6]]))
-        self.assertEqual(a, OctaSym([2,-1]))
-        self.assertEqual(a.invert(), OctaSym([-2,1]))
-        self.assertEqual(a*a, OctaSym([-1,-2]))
-        
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2023
+# \author    Simon Rohou
+# \copyright Copyright 2023 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+try:
+  import numpy as np
+except:
+  print("NUMPY UNAVAILABLE")
+from codac import *
+from codac.codac2 import *
+
+class TestActions(unittest.TestCase):
+
+    def tests_action(self):
+
+        x = IntervalVector([[-1,0],[5,6]])
+        a = OctaSym([2,-1])
+
+        print(x)                 # Result: ([-1, 0] ; [5, 6])
+        print(a(x))              # Result: ([5, 6] ; [-0, 1])
+        print(a.invert()(a(x)))  # Result: ([-1, 0] ; [5, 6])
+
+        print(a)                 # Result: (2 -1)
+        print(a.invert())        # Result: (-2 1)
+        print(a*a)               # Result: (-1 -2)
+
+        self.assertEqual(a(x), IntervalVector([[5,6],[-0,1]]))
+        self.assertEqual(a.invert()(a(x)), IntervalVector([[-1,0],[5,6]]))
+        self.assertEqual(a, OctaSym([2,-1]))
+        self.assertEqual(a.invert(), OctaSym([-2,1]))
+        self.assertEqual(a*a, OctaSym([-1,-2]))
+        
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctcdelay.py

 * *Ordering differences only*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-import math
-from codac import *
-
-class TestCtcDelay(unittest.TestCase):
-
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-
-    def test_ctcdelay_1(self):
-        tdomain = Interval(0.,10.)
-        x = Tube(tdomain, 0.01, TFunction("cos(t)"))
-        y = Tube(tdomain, 0.01)
-
-        pi = Interval.PI
-        ctc_delay = CtcDelay()
-        ctc_delay.contract(pi, x, y)
-
-        beginDrawing()
-        fig_x = VIBesFigTube("delay x", x)
-        fig_x.show()
-        fig_y = VIBesFigTube("delay y", y)
-        fig_y.show()
-        endDrawing()
-
-        self.assertEqual(y(Interval(0.,math.pi)), Interval.ALL_REALS)
-        self.assertApproxIntv(y(Interval(math.pi+0.01,10.)), Interval(-1.,1.))
-        self.assertTrue(y(5.).is_superset(x(5. - math.pi)))
-
-    def test_ctcdelay_2(self):
-        tdomain = Interval(0.,10.)
-        dt = 0.01
-        x = Tube(tdomain, dt, TFunction("cos(t)"))
-        y = Tube(tdomain, dt, TFunction("sin(t)"))
-
-        delay = Interval(0.,2.*math.pi)
-        ctc_delay = CtcDelay()
-        ctc_delay.contract(delay, x, y)
-
-        beginDrawing()
-        fig_x = VIBesFigTube("delay x", x)
-        fig_x.show()
-        fig_y = VIBesFigTube("delay y", y)
-        fig_y.show()
-        endDrawing()
-
-        self.assertTrue(delay.contains(math.pi/2.))
-        self.assertTrue(delay.diam() < 3.*dt)
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+import math
+from codac import *
+
+class TestCtcDelay(unittest.TestCase):
+
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+
+    def test_ctcdelay_1(self):
+        tdomain = Interval(0.,10.)
+        x = Tube(tdomain, 0.01, TFunction("cos(t)"))
+        y = Tube(tdomain, 0.01)
+
+        pi = Interval.PI
+        ctc_delay = CtcDelay()
+        ctc_delay.contract(pi, x, y)
+
+        beginDrawing()
+        fig_x = VIBesFigTube("delay x", x)
+        fig_x.show()
+        fig_y = VIBesFigTube("delay y", y)
+        fig_y.show()
+        endDrawing()
+
+        self.assertEqual(y(Interval(0.,math.pi)), Interval.ALL_REALS)
+        self.assertApproxIntv(y(Interval(math.pi+0.01,10.)), Interval(-1.,1.))
+        self.assertTrue(y(5.).is_superset(x(5. - math.pi)))
+
+    def test_ctcdelay_2(self):
+        tdomain = Interval(0.,10.)
+        dt = 0.01
+        x = Tube(tdomain, dt, TFunction("cos(t)"))
+        y = Tube(tdomain, dt, TFunction("sin(t)"))
+
+        delay = Interval(0.,2.*math.pi)
+        ctc_delay = CtcDelay()
+        ctc_delay.contract(delay, x, y)
+
+        beginDrawing()
+        fig_x = VIBesFigTube("delay x", x)
+        fig_x.show()
+        fig_y = VIBesFigTube("delay y", y)
+        fig_y.show()
+        endDrawing()
+
+        self.assertTrue(delay.contains(math.pi/2.))
+        self.assertTrue(delay.diam() < 3.*dt)
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctceval.py

 * *Ordering differences only*

```diff
@@ -1,1097 +1,1097 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-
-class TestCtcEval(unittest.TestCase):
-
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-
-    def test_ctceval_1(self):
-
-        t = Interval(0.,6.)
-        z = Interval(-1.,1.)
-        x = Tube(Interval(-1.,7.), 2.);
-        v = Tube(x);
-        v.set(Interval(-1.), 0);
-        v.set(Interval(-1.,1.), 1);
-        v.set(Interval(-1.), 2);
-        v.set(Interval(1.), 3);
-
-        self.assertEqual(x.nb_slices(), 4);
-        ctc_eval = CtcEval();
-        ctc_eval.preserve_slicing(False);
-        ctc_eval.enable_time_propag(False);
-        ctc_eval.contract(t, z, x, v);
-        self.assertEqual(x.nb_slices(), 6);
-
-        self.assertEqual(x.codomain(), Interval.ALL_REALS); # only gates should be affected
-        self.assertEqual(x(-1.), Interval.ALL_REALS);
-        self.assertEqual(x(0.), Interval(-2.,6.));
-        self.assertEqual(x(1.), Interval(-3.,5.));
-        self.assertEqual(x(3.), Interval(-4.,3.));
-        self.assertEqual(x(5.), Interval(-6.,1.));
-        self.assertEqual(x(6.), Interval(-5.,2.));
-        self.assertEqual(x(7.), Interval.ALL_REALS);
-
-
-    def test_ctceval_2(self):
-        t, z =  Interval(0.,6.), Interval(-1.,1.);
-        x = Tube(Interval(-1.,7.), 2.);
-        v = Tube(x);
-        v.set(Interval(-1.), 0);
-        v.set(Interval(-1.,1.), 1);
-        v.set(Interval(-1.), 2);
-        v.set(Interval(1.), 3);
-
-        x.set(Interval(0.,1.), 2.);
-        v.sample(2.);
-
-        self.assertEqual(x.nb_slices(), 5);
-
-        ctc_eval = CtcEval();
-        ctc_eval.preserve_slicing(False);
-        ctc_eval.enable_time_propag(False);
-        ctc_eval.contract(t, z, x, v);
-
-        self.assertEqual(x.nb_slices(), 7);
-
-        self.assertEqual(x.codomain(), Interval.ALL_REALS); # only gates should be affected
-        self.assertEqual(x(-1.), Interval.ALL_REALS);
-        self.assertEqual(x(0.), Interval(0.,3.));
-        self.assertEqual(x(1.), Interval(-1.,2.));
-        self.assertEqual(x(2.), Interval(0.,1.));
-        self.assertEqual(x(3.), Interval(-1.,2.));
-        self.assertEqual(x(5.), Interval(-3.,1.));
-        self.assertEqual(x(6.), Interval(-2.,2.));
-        self.assertEqual(x(7.), Interval.ALL_REALS);
-
-        t = Interval(1.75,5.5);
-        z = Interval(1.6);
-
-        ctc_eval.enable_time_propag(True);
-        ctc_eval.contract(t, z, x, v);
-
-
-        box = IntervalVector([Interval(1.75,5.5), Interval(1.6)])
-
-        # if(VIBES_DRAWING) fig_tube->draw_box(box, vibesParams("figure", "ctceval", "red"));
-        ctc_eval.contract(box[0], box[1], x, v);
-        # if(VIBES_DRAWING) fig_tube->draw_box(box, vibesParams("figure", "ctceval", "blue"));
-
-        self.assertApproxIntv(x.interpol(3.4,v), Interval(0.8,1.6));
-        self.assertApproxIntv(box[0], Interval(2.6,3.4));
-        self.assertApproxIntv(box[1], Interval(1.6));
-
-
-class TestCtcEval2(unittest.TestCase):
-
-  def assertApproxIntv(self, first, second):
-    if first.is_empty() is False:
-    # if isinstance(second, Interval):
-        self.assertAlmostEqual(first.lb(), second.lb())
-        self.assertAlmostEqual(first.ub(), second.ub())
-    else:
-        self.assertEqual(first, second)
-
-  def setUp(self):
-    xdot = Tube(Interval(0., 10.), 1.0);
-    xdot.set(Interval(-0.5,1.));
-
-    x = Tube(xdot);
-    x.set(Interval.ALL_REALS);
-    x.set(Interval(-1.5,1.), 4);
-    x.set(Interval(-1.,1.5), 5);
-    self.assertEqual(x.nb_slices(), 10);
-    
-    self.ctc_deriv = CtcDeriv();
-    self.ctc_deriv.contract(x, xdot);
-
-    self.x_raw = Tube(x)
-    self.xdot_raw = Tube(xdot);
-
-    self.ctc_eval_propa = CtcEval()
-    self.ctc_eval_nopropa = CtcEval()
-    self.ctc_eval_propa.preserve_slicing(False);
-    self.ctc_eval_nopropa.preserve_slicing(False);
-    self.ctc_eval_propa.enable_time_propag(True);
-    self.ctc_eval_nopropa.enable_time_propag(False);
-
-  def test_1(self):
-    # Checking the tube...
-    self.assertEqual(self.x_raw(0), Interval(-5.5,3.));
-    self.assertEqual(self.x_raw(1), Interval(-4.5,2.5));
-    self.assertEqual(self.x_raw(2), Interval(-3.5,2.));
-    self.assertEqual(self.x_raw(3), Interval(-2.5,1.5));
-    self.assertEqual(self.x_raw(4), Interval(-1.5,1.));
-    self.assertEqual(self.x_raw(5), Interval(-1.,1.5));
-    self.assertEqual(self.x_raw(6), Interval(-1.5,2.5));
-    self.assertEqual(self.x_raw(7), Interval(-2.,3.5));
-    self.assertEqual(self.x_raw(8), Interval(-2.5,4.5));
-    self.assertEqual(self.x_raw(9), Interval(-3.,5.5));
-
-      # Interval intv_t, intv_y;
-      
-
-  def test_1_no_propa(self):
-    # Test A_no_propa
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 1.;
-    intv_y = Interval(-0.5,1.);
-    self.assertEqual(x(1.), Interval(-4.5,2.5));
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(intv_t, 1.);
-    self.assertEqual(intv_y, Interval(-0.5,1.));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1.), intv_y);
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(7), Interval(-2.,3.5));
-    self.assertEqual(x(8), Interval(-2.5,4.5));
-    self.assertEqual(x(9), Interval(-3.,5.5));
-
-  def  test_A__propa(self): 
-    # Test A_propa
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 1.;
-    intv_y = Interval(-0.5,1.);
-    self.assertEqual(x(1.), Interval(-4.5,2.5));
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(intv_t, 1.);
-    self.assertEqual(intv_y, Interval(-0.5,1.));
-    self.assertEqual(x(0), Interval(-1.5,1.5));
-    self.assertEqual(x(1.), intv_y);
-    self.assertEqual(x(1), Interval(-1.,2.));
-    self.assertEqual(x(2), Interval(-1.5,2.));
-    self.assertApproxIntv(x(3), Interval(-1.5-1./3.,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(7), Interval(-2.,3.5));
-    self.assertEqual(x(8), Interval(-2.5,4.5));
-    self.assertEqual(x(9), Interval(-3.,5.5));
-
-  def test_A_ctc_deriv(self):
-  # def test_A: ctc_deriv should not be effective after ctc_eval(true)(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 1.;
-    intv_y = Interval(-0.5,1.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-  def test_B_ctc_deriv(self):
-    # Test B_no_propa
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(0.5,2.5);
-    intv_y = Interval(-2.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(0.5,2.5));
-    self.assertEqual(intv_y, Interval(-2.));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(0.5), Interval(-4.,-1.));
-    self.assertEqual(x(1), Interval(-5.5,3.));
-    self.assertEqual(x(1.), Interval(-3.5,-1.25));
-    self.assertEqual(x(2), Interval(-4.5,2.5));
-    self.assertEqual(x(2.), Interval(-2.75,-0.5));
-    self.assertEqual(x(3), Interval(-3.5,2.));
-    self.assertEqual(x(2.5), Interval(-3.,-0.));
-    self.assertEqual(x(4), Interval(-3.5,2.));
-    self.assertEqual(x(5), Interval(-2.5,1.5));
-    self.assertEqual(x(6), Interval(-1.5,1.));
-    self.assertEqual(x(7), Interval(-1.,1.5));
-    self.assertEqual(x(8), Interval(-1.5,2.5));
-    self.assertEqual(x(9), Interval(-2.,3.5));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_B_ctc_deriv_propa(self):
-    # Test B_propa
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(0.5,2.5);
-    intv_y = Interval(-2.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(0.5,2.5));
-    self.assertEqual(intv_y, Interval(-2.));
-    self.assertEqual(x(0), Interval(-4.5,-0.75));
-    self.assertEqual(x(0.5), Interval(-4.,-1.));
-    self.assertEqual(x(1), Interval(-4.,-1.));
-    self.assertEqual(x(1.), Interval(-3.5,-1.25));
-    self.assertEqual(x.slice(0.6).tdomain(), Interval(0.5,1.));
-    self.assertEqual(x.slice(0.6).input_gate(), Interval(-4.,-1.));
-    self.assertEqual(x.slice(0.6).output_gate(), Interval(-3.5,-1.25));
-    self.assertEqual(xdot(2), Interval(-0.5,1.));
-    #self.assertEqual(x(2), Interval(-3.5,-0.5)); # todo: optimal implementation?
-    self.assertEqual(x(2.), Interval(-2.75,-0.5));
-    self.assertEqual(x(3), Interval(-3.,0.));
-    self.assertEqual(x(2.5), Interval(-3.,-0.));
-    self.assertEqual(x(4), Interval(-3.,0.5));
-    self.assertApproxIntv(x(5), Interval(-2.5,1.+1./6.));
-    self.assertEqual(x(6), Interval(-1.5,1.));
-    self.assertEqual(x(7), Interval(-1.,1.5));
-    self.assertEqual(x(8), Interval(-1.5,2.5));
-    self.assertEqual(x(9), Interval(-2.,3.5));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-
-  def test_C_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(0.5,3.5);
-    intv_y = Interval(-4.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(0.5,1.5));
-    self.assertEqual(intv_y, Interval(-4.));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(0.5), Interval(-5.,-3.5));
-    self.assertEqual(x(1), Interval(-5.5,3.));
-    self.assertEqual(x(1.), Interval(-4.5,-3.5));
-    self.assertEqual(x(2), Interval(-4.5,2.5));
-    self.assertEqual(x(1.5), Interval(-4.,-3.));
-    self.assertEqual(x(3), Interval(-4.5,2.5));
-    self.assertEqual(x(4), Interval(-3.5,2.));
-    self.assertEqual(x(5), Interval(-2.5,1.5));
-    self.assertEqual(x(6), Interval(-1.5,1.));
-    self.assertEqual(x(7), Interval(-1.,1.5));
-    self.assertEqual(x(8), Interval(-1.5,2.5));
-    self.assertEqual(x(9), Interval(-2.,3.5));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_C_propas(self):
-      x = Tube(self.x_raw);
-      xdot = Tube(self.xdot_raw);
-      intv_t = Interval(0.5,3.5);
-      intv_y = Interval(-4.);
-      self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-      self.assertEqual(x.nb_slices(), 12);
-      self.assertEqual(intv_t, Interval(0.5,1.5));
-      self.assertEqual(intv_y, Interval(-4.));
-      self.assertEqual(x(0), Interval(-5.5,-3.25));
-      self.assertEqual(x(0.5), Interval(-5.,-3.5));
-      # //self.assertEqual(x(1), Interval(-5.,-3.5)); // optimality
-      self.assertEqual(x(1.), Interval(-4.5,-3.5));
-      self.assertEqual(x(2), Interval(-4.5,-3.));
-      self.assertEqual(x(1.5), Interval(-4.,-3.));
-      self.assertEqual(x(3), Interval(-4.,-2.5));
-      self.assertEqual(x(4), Interval(-3.5,-1.5));
-      self.assertEqual(x(5), Interval(-2.5,-0.5));
-      self.assertEqual(x(6), Interval(-1.5,0.5));
-      self.assertEqual(x(7), Interval(-1.,1.5));
-      self.assertEqual(x(8), Interval(-1.5,2.5));
-      self.assertEqual(x(9), Interval(-2.,3.5));
-      self.assertEqual(x(10), Interval(-2.5,4.5));
-      self.assertEqual(x(11), Interval(-3.,5.5));
-
-#     if(false & VIBES_DRAWING) // drawing results
-#     {
-#       //x = x_raw;
-#       //xdot = xdot_raw;
-#       //IntervalVector box(2);
-#       //box[0] = Interval(0.5,3.5);
-#       //box[1] = Interval(-4.);
-#       //vibes::beginDrawing();
-#       //VIBesFigTube fig_tube("ctceval", &x);
-#       //fig_tube.set_properties(100, 100, 500, 500);
-#       //fig_tube.set_tube_derivative(&x, &xdot);
-#       //fig_tube.show(true);
-#       //contraction = ctc_eval_propa.contract(box[0], box[1], x, xdot);
-#       //fig_tube.show(true);
-#       //vibes::drawBox(box, vibesParams("figure", "ctceval", "blue"));
-#       //vibes::endDrawing();
-#     }
-
-  def test_D_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 3.5;
-    intv_y = Interval(-3.5,-0.5);
-    self.assertEqual(x.nb_slices(), 10);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(intv_t, 3.5);
-    self.assertEqual(intv_y, Interval(-2.,-0.5));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(3.5), Interval(-2.,-0.5));
-    self.assertEqual(x(4), Interval(-2.5,1.5));
-    self.assertEqual(x(5), Interval(-1.5,1.));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_D_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 3.5;
-    intv_y = Interval(-3.5,-0.5);
-    self.assertEqual(x.nb_slices(), 10);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(intv_t, 3.5);
-    self.assertEqual(intv_y, Interval(-2.,-0.5));
-    self.assertEqual(x(0), Interval(-5.5,1.25));
-    self.assertEqual(x(1), Interval(-4.5,0.75));
-    self.assertEqual(x(2), Interval(-3.5,0.25));
-    self.assertEqual(x(3), Interval(-2.5,-0.25));
-    self.assertEqual(x(3.5), Interval(-2.,-0.5));
-    self.assertEqual(x(4), Interval(-2.,0.));
-    self.assertEqual(x(5), Interval(-1.5,1.));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_E_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(6.5, 8.5);
-    intv_y = Interval(-4.5, -1.75);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(7.5, 8.5));
-    self.assertEqual(intv_y, Interval(-2.25, -1.75));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(7), Interval(-2.,3.5));
-    self.assertEqual(x(7.5), Interval(-1.75,-1.25));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(8.), Interval(-2.,-1.25));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_E_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(6.5, 8.5);
-    intv_y = Interval(-4.5, -1.75);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(7.5, 8.5));
-    self.assertEqual(intv_y, Interval(-2.25, -1.75));
-    self.assertEqual(x(0), Interval(-5.5,2.5));
-    self.assertEqual(x(1), Interval(-4.5,2.));
-    self.assertEqual(x(2), Interval(-3.5,1.5));
-    self.assertEqual(x(3), Interval(-2.5,1.));
-    self.assertEqual(x(4), Interval(-1.5,0.5));
-    self.assertEqual(x(5), Interval(-1.,0.));
-    self.assertEqual(x(6), Interval(-1.5,-0.5));
-    self.assertEqual(x(7), Interval(-1.75,-1.));
-    self.assertEqual(x(7.5), Interval(-1.75,-1.25));
-#     //CHECK(x(8), Interval(-2.,-1.25)); // optimality
-    self.assertEqual(x(8.), Interval(-2.,-1.25));
-    self.assertEqual(x(9), Interval(-2.25,-0.75));
-    self.assertEqual(x(10), Interval(-2.5,-0.25));
-    self.assertEqual(x(11), Interval(-3.,0.75));
-
-  def test_F_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(8.5,9.5);
-    intv_y = Interval(-0.5,2.5);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(8.5,9.5));
-    self.assertEqual(intv_y, Interval(-0.5,2.5));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(7), Interval(-2.,3.5));
-    self.assertEqual(x(8), Interval(-2.5,4.5));
-    self.assertEqual(x(8.5), Interval(-1.5,3.));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-    self.assertEqual(x(9.5), Interval(-1.,3.5));
-    self.assertEqual(x(11), Interval(-3,5.5));
-
-  def test_F_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(8.5,9.5);
-    intv_y = Interval(-0.5,2.5);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(intv_t, Interval(8.5,9.5));
-    self.assertEqual(intv_y, Interval(-0.5,2.5));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertApproxIntv(x(7), Interval(-2.,3.+1./3.));
-    self.assertEqual(x(8), Interval(-2.,3.25));
-    self.assertEqual(x(8.5), Interval(-1.5,3.));
-#     //CHECK(x(9), Interval(-1.5,3.)); // optimality
-#     //CHECK(x(10), Interval(-1.,3.5)); // optimality
-    self.assertEqual(x(9.5), Interval(-1.,3.5));
-    self.assertEqual(x(11), Interval(-1.25,4.));
-
-  def test_G_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(6.5,7.5);
-    intv_y = Interval(3.,4.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(7.5));
-    self.assertEqual(intv_y, Interval(3.));
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(7), Interval(-2.,3.5));
-    self.assertEqual(x(7.5), Interval(3.));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_G_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(6.5,7.5);
-    intv_y = Interval(3.,4.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(7.5));
-    self.assertEqual(intv_y, Interval(3.));
-    self.assertEqual(x(0), Interval(-4.5,3.));
-    self.assertEqual(x(1), Interval(-3.5,2.5));
-    self.assertEqual(x(2), Interval(-2.5,2.));
-    self.assertEqual(x(3), Interval(-1.5,1.5));
-    self.assertEqual(x(4), Interval(-0.5,1.));
-    self.assertEqual(x(5), Interval(0.5,1.5));
-    self.assertEqual(x(6), Interval(1.5,2.5));
-    self.assertEqual(x(7), Interval(2.5,3.));
-    self.assertEqual(x(7.5), Interval(3.));
-    self.assertEqual(x(8), Interval(2.75,3.5));
-    self.assertEqual(x(9), Interval(2.25,4.5));
-    self.assertEqual(x(10), Interval(1.75,5.5));
-
-  def test_H_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(7.,8.25);
-    intv_y = Interval(4.25,5.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval.EMPTY_SET);
-    self.assertEqual(intv_y, Interval.EMPTY_SET);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(x(0), Interval.EMPTY_SET);
-    self.assertEqual(x(1), Interval.EMPTY_SET);
-    self.assertEqual(x(2), Interval.EMPTY_SET);
-    self.assertEqual(x(3), Interval.EMPTY_SET);
-    self.assertEqual(x(4), Interval.EMPTY_SET);
-    self.assertEqual(x(5), Interval.EMPTY_SET);
-    self.assertEqual(x(6), Interval.EMPTY_SET);
-    self.assertEqual(x(7), Interval.EMPTY_SET);
-    self.assertEqual(x(8), Interval.EMPTY_SET);
-    self.assertEqual(x(9), Interval.EMPTY_SET);
-    self.assertTrue(x.is_empty());
-
-  def test_H_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(7.,8.25);
-    intv_y = Interval(4.25,5.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval.EMPTY_SET);
-    self.assertEqual(intv_y, Interval.EMPTY_SET);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(x(0), Interval.EMPTY_SET);
-    self.assertEqual(x(1), Interval.EMPTY_SET);
-    self.assertEqual(x(2), Interval.EMPTY_SET);
-    self.assertEqual(x(3), Interval.EMPTY_SET);
-    self.assertEqual(x(4), Interval.EMPTY_SET);
-    self.assertEqual(x(5), Interval.EMPTY_SET);
-    self.assertEqual(x(6), Interval.EMPTY_SET);
-    self.assertEqual(x(7), Interval.EMPTY_SET);
-    self.assertEqual(x(8), Interval.EMPTY_SET);
-    self.assertEqual(x(9), Interval.EMPTY_SET);
-    self.assertTrue(x.is_empty());
-
-  def test_I_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(2.5);
-    intv_y = Interval(0.5);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(2.5));
-    self.assertEqual(intv_y, Interval(0.5));
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(2.5), Interval(0.5));
-    self.assertEqual(x(3), Interval(-3.5,2.));
-    self.assertEqual(x(4), Interval(-2.5,1.5));
-    self.assertEqual(x(5), Interval(-1.5,1.));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_I_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(2.5);
-    intv_y = Interval(0.5);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(2.5));
-    self.assertEqual(intv_y, Interval(0.5));
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(x(0), Interval(-2.,1.75));
-    self.assertEqual(x(1), Interval(-1.,1.25));
-    self.assertEqual(x(2), Interval(-0.,0.75));
-    self.assertEqual(x(2.5), Interval(0.5));
-    self.assertEqual(x(3), Interval(0.25,1.));
-    self.assertApproxIntv(x(4), Interval(-0.25,1.+1./3.));
-    self.assertEqual(x(5), Interval(-0.75,1.));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_J_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 6.25;
-    intv_y = Interval(0.5,1.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, 6.25);
-    self.assertEqual(intv_y, Interval(0.5,1.));
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(6.25), Interval(0.5,1.));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-
-  def test_J_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = 6.25;
-    intv_y = Interval(0.5,1.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, 6.25);
-    self.assertEqual(intv_y, Interval(0.5,1.));
-    self.assertEqual(x.nb_slices(), 11);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5.), Interval(-0.75,1.));
-    self.assertApproxIntv(x(5), Interval(-0.75,1.4+1./60.));
-    self.assertEqual(x(6), Interval(0.25,1.125));
-    self.assertEqual(x(7), Interval(0.125,1.75));
-    self.assertEqual(x(8), Interval(0.125-0.5,2.75));
-    self.assertEqual(x(9), Interval(0.125-1.,3.75));
-    self.assertEqual(x(10), Interval(0.125-1.5,4.75));
-
-  def test_K_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(5.25, 8.25);
-    intv_y = Interval(-0.5, 0.);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(5.25, 8.25));
-    self.assertEqual(intv_y, Interval(-0.5, 0.));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(5.25), Interval(-1.,1.25));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(8.25), Interval(-2.,3.));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_K_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(5.25, 8.25);
-    intv_y = Interval(-0.5, 0.);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(5.25, 8.25));
-    self.assertEqual(intv_y, Interval(-0.5, 0.));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.25));
-    self.assertEqual(x(5.25), Interval(-1.,1.25));
-    self.assertApproxIntv(x(6), Interval(-1.,1.4+1./60.));
-    self.assertEqual(x(7), Interval(-1.5,1.875));
-    self.assertApproxIntv(x(8), Interval(-1.625-1./3.,2.75));
-    self.assertEqual(x(9), Interval(-2.,3.));
-    self.assertEqual(x(8.25), Interval(-2.,3.));
-    self.assertEqual(x(10), Interval(-2.375,3.75));
-    self.assertEqual(x(11), Interval(-2.875,4.75));
-
-  def test_L_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(1.5,4.5);
-    intv_y = Interval(1.75,2.75);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(1.5,2.5));
-    self.assertEqual(intv_y, Interval(1.75,2.25));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(1.5), Interval(0.75,2.25));
-    self.assertEqual(x(2), Interval(-4.5,2.5));
-    self.assertEqual(x(3), Interval(-3.5,2.));
-    self.assertEqual(x(2.5), Interval(1.25,1.75));
-    self.assertEqual(x(4), Interval(-3.5,2.));
-    self.assertEqual(x(5), Interval(-2.5,1.5));
-    self.assertEqual(x(6), Interval(-1.5,1.));
-    self.assertEqual(x(7), Interval(-1.,1.5));
-    self.assertEqual(x(8), Interval(-1.5,2.5));
-    self.assertEqual(x(9), Interval(-2.,3.5));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_L_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(1.5,2.5);
-    intv_y = Interval(1.75,2.75);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(1.5,2.5));
-    self.assertEqual(intv_y, Interval(1.75,2.25));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-0.75,3.));
-    self.assertEqual(x(1), Interval(0.25,2.5));
-    self.assertEqual(x(1.5), Interval(0.75,2.25));
-    self.assertEqual(x(2), Interval(0.75,2.25));
-#     //CHECK(x(3), Interval(1.25,2.)); // optimality
-    self.assertEqual(x(2.5), Interval(1.25,1.75));
-    self.assertEqual(x(4), Interval(1.,1.75));
-    self.assertEqual(x(5), Interval(0.5,1.5));
-    self.assertEqual(x(6), Interval(0.,1.));
-    self.assertEqual(x(7), Interval(-0.5,1.5));
-    self.assertEqual(x(8), Interval(-1.,2.5));
-    self.assertEqual(x(9), Interval(-1.5,3.5));
-    self.assertEqual(x(10), Interval(-2.,4.5));
-    self.assertEqual(x(11), Interval(-2.5,5.5));
-
-  def test_M_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(0.75,1.25);
-    intv_y = Interval(-5.75,-5.25);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval.EMPTY_SET);
-    self.assertEqual(intv_y, Interval.EMPTY_SET);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(x(0), Interval.EMPTY_SET);
-    self.assertEqual(x(1), Interval.EMPTY_SET);
-    self.assertEqual(x(2), Interval.EMPTY_SET);
-    self.assertEqual(x(3), Interval.EMPTY_SET);
-    self.assertEqual(x(4), Interval.EMPTY_SET);
-    self.assertEqual(x(5), Interval.EMPTY_SET);
-    self.assertEqual(x(6), Interval.EMPTY_SET);
-    self.assertEqual(x(7), Interval.EMPTY_SET);
-    self.assertEqual(x(8), Interval.EMPTY_SET);
-    self.assertEqual(x(9), Interval.EMPTY_SET);
-    self.assertTrue(x.is_empty());
-
-  def test_M_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(0.75,1.25);
-    intv_y = Interval(-5.75,-5.25);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval.EMPTY_SET);
-    self.assertEqual(intv_y, Interval.EMPTY_SET);
-    self.assertEqual(x.nb_slices(), 10);
-    self.assertEqual(x(0), Interval.EMPTY_SET);
-    self.assertEqual(x(1), Interval.EMPTY_SET);
-    self.assertEqual(x(2), Interval.EMPTY_SET);
-    self.assertEqual(x(3), Interval.EMPTY_SET);
-    self.assertEqual(x(4), Interval.EMPTY_SET);
-    self.assertEqual(x(5), Interval.EMPTY_SET);
-    self.assertEqual(x(6), Interval.EMPTY_SET);
-    self.assertEqual(x(7), Interval.EMPTY_SET);
-    self.assertEqual(x(8), Interval.EMPTY_SET);
-    self.assertEqual(x(9), Interval.EMPTY_SET);
-    self.assertTrue(x.is_empty());
-
-  def test_N_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(5.5,8.5);
-    intv_y = Interval(2.,5.5);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(6.5,8.5));
-    self.assertEqual(intv_y, Interval(2.,4.));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-1.5,2.5));
-    self.assertEqual(x(6.5), Interval(0.,2.));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(8.5), Interval(1.,4.));
-    self.assertEqual(x(10), Interval(-2.5,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_N_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(5.5,8.5);
-    intv_y = Interval(2.,5.5);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(6.5,8.5));
-    self.assertEqual(intv_y, Interval(2.,4.));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(3), Interval(-2.5,1.5));
-    self.assertEqual(x(4), Interval(-1.5,1.));
-    self.assertEqual(x(5), Interval(-1.,1.5));
-    self.assertEqual(x(6), Interval(-0.5,2.));
-    self.assertEqual(x(6.5), Interval(0.,2.));
-    self.assertEqual(x(7), Interval(0.,2.5));
-#     //CHECK(x(8), Interval(xxx)); // optimality
-    self.assertEqual(x(9), Interval(1.,4.));
-    self.assertEqual(x(8.5), Interval(1.,4.));
-    self.assertEqual(x(10), Interval(0.75,4.5));
-    self.assertEqual(x(11), Interval(0.25,5.5));
-
-  def test_0_no_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(2.5,9.5);
-    intv_y = Interval(-5.,-2.5);
-    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(2.5,9.5));
-    self.assertEqual(intv_y, Interval(-3.,-2.5));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,3.));
-    self.assertEqual(x(1), Interval(-4.5,2.5));
-    self.assertEqual(x(2), Interval(-3.5,2.));
-    self.assertEqual(x(2.5), Interval(-3.,1.));
-    self.assertEqual(x(3), Interval(-3.5,2.));
-    self.assertEqual(x(4), Interval(-2.5,1.5));
-    self.assertEqual(x(5), Interval(-1.5,1.));
-    self.assertEqual(x(6), Interval(-1.,1.5));
-    self.assertEqual(x(7), Interval(-1.5,2.5));
-    self.assertEqual(x(8), Interval(-2.,3.5));
-    self.assertEqual(x(9), Interval(-2.5,4.5));
-    self.assertEqual(x(10), Interval(-3.,5.5));
-    self.assertEqual(x(9.5), Interval(-2.75,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.5));
-
-  def test_0_propa(self):
-    x = Tube(self.x_raw);
-    xdot = Tube(self.xdot_raw);
-    intv_t = Interval(2.5,9.5);
-    intv_y = Interval(-5.,-2.5);
-    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
-    self.assertEqual(intv_t, Interval(2.5,9.5));
-    self.assertEqual(intv_y, Interval(-3.,-2.5));
-    self.assertEqual(x.nb_slices(), 12);
-    self.assertEqual(x(0), Interval(-5.5,2.25));
-    self.assertEqual(x(1), Interval(-4.5,1.75));
-    self.assertEqual(x(2), Interval(-3.5,1.25));
-    self.assertEqual(x(2.5), Interval(-3.,1.));
-    self.assertEqual(x(3), Interval(-3.,1.));
-    self.assertEqual(x(4), Interval(-2.5,0.75));
-#     //CHECK(x(5), Interval(xxx)); // optimality
-    self.assertEqual(x(6), Interval(-1.,1.));
-    self.assertEqual(x(7), Interval(-1.5,2.));
-    self.assertEqual(x(8), Interval(-2.,3.));
-    self.assertEqual(x(9), Interval(-2.5,4.));
-    self.assertEqual(x(10), Interval(-2.75,4.5));
-    self.assertEqual(x(9.5), Interval(-2.75,4.5));
-    self.assertEqual(x(11), Interval(-3.,5.));
-#   }
-
-  def Test_CtcEval_multi_eval(self):
-
-    x = Tube(Interval(0.,20.), 0.1, TFunction("cos(t)+t*[-0.1,0.2]"));
-    v = Tube(Interval(0.,20.), 0.1, TFunction("-sin(t)+[-0.1,0.2]"));
-    
-    ctc_deriv = CtcDeriv();
-    ctc_deriv.contract(x, v);
-
-    box = IntervalVector(2);
-    ctc_eval = CtcEval();
-    ctc_eval.enable_time_propag(True);
-    x_c = Tube(x); 
-    v_c = Tube(v);
-
-    box[0] = Interval(11.98);
-    box[1] = Interval(1.);
-    ctc_eval.contract(box[0], box[1], x_c, v_c);
-
-    box[0] = Interval(6.5);
-    box[1] = Interval(1.);
-    ctc_eval.contract(box[0], box[1], x_c, v_c);
-
-#     if(VIBES_DRAWING) // drawing results
-#     {
-#       //vibes::beginDrawing();
-#       //VIBesFigTube fig_tube("ctceval", &x);
-#       //fig_tube.set_properties(100, 100, 800, 400);
-#       //fig_tube.set_tube_derivative(&x, &v);
-#       //fig_tube.show(true);
-#       //x = x_c;
-#       //v = v_c;
-#       //fig_tube.show(true);
-#       //vibes::drawBox(box, vibesParams("figure", "ctceval", "red"));
-#     }
-#   }
-  def  Test_CtcEval_non_zero_derivative_negative_case(self):
-#   SECTION("Test CtcEval, non-zero derivative (negative case)")
-
-    x = Tube(Interval(0.,11.), 1.);
-    v = Tube(x);
-    v.set(Interval(-1.5,-1.));
-    x.set(Interval(6.,8.), 0);
-
-    ctc_eval = CtcEval;
-    ctc_deriv = CtcDeriv;
-    ctc_deriv.contract(x, v);
-
-    self.assertEqual(x(0), Interval(6.,8.)); 
-    self.assertEqual(x(1), Interval(4.5,7.));
-    self.assertEqual(x(2), Interval(3.,6.));
-    self.assertEqual(x(3), Interval(1.5,5.));
-    self.assertEqual(x(4), Interval(-0.,4.));
-    self.assertEqual(x(5), Interval(-1.5,3.));
-    self.assertEqual(x(6), Interval(-3.,2.));
-    self.assertEqual(x(7), Interval(-4.5,1.));
-    self.assertEqual(x(8), Interval(-6.,0.));
-    self.assertEqual(x(9), Interval(-7.5,-1.));
-    self.assertEqual(x(10), Interval(-9.,-2.));
-
-    # Interval t, y;
-    # x_raw = Tube(x);
-    # v_raw = Tube(v);
-
-    # x = Tube(x_raw);
-    # v = Tube(v_raw);
-    # t = Interval(3.5,6.);
-    # y = Interval(3.5,6.);
-    # ctc_eval.contract(t, y, x, v);
-  #   /*CHECK(t, Interval(3.5,5.));
-  #     self.assertEqual(y, Interval(3.5,4.5));
-  #     self.assertEqual(x(0), Interval(6.,8.));
-  #     self.assertEqual(x(1), Interval(4.5,7.));
-  #     self.assertEqual(x(2), Interval(4.,6.));
-  #     self.assertEqual(x(3), Interval(2.75,5.));
-  #     self.assertEqual(x(4), Interval(1.25,4.));
-  #     self.assertEqual(x(5), Interval(-0.25,3.));
-  #     self.assertEqual(x(6), Interval(-3.,2.));
-  #     self.assertEqual(x(7), Interval(-4.5,1.));
-  #     self.assertEqual(x(8), Interval(-6.,0.));
-  #     self.assertEqual(x(9), Interval(-7.5,-1.));
-  #     self.assertEqual(x(10), Interval(-9.,-2.));
-
-  #   x = x_raw;
-  #   v = v_raw;
-  #   t = Interval(3.,8.5);
-  #   y = Interval(-7.,-2.5);
-  #   ctc_eval.contract(t, y, x, v);
-  #     self.assertEqual(t, Interval(6.,8.5));
-  #     self.assertEqual(y, Interval(-5.25,-2.5));
-  #     self.assertEqual(x(0), Interval(6.,8.)); 
-  #     self.assertEqual(x(1), Interval(4.5,7.));
-  #     self.assertEqual(x(2), Interval(3.,6.));
-  #     self.assertEqual(x(3), Interval(1.5,5.));
-  #     self.assertEqual(x(4), Interval(-0.,4.));
-  #     self.assertEqual(x(5), Interval(-1.5,2.75));
-  #     self.assertEqual(x(6), Interval(-3.,1.25));
-  #     self.assertEqual(x(7), Interval(-4.5,-0.25));
-  #     self.assertEqual(x(8), Interval(-6.,-1.75));
-  #     self.assertEqual(x(9), Interval(-7.5,-3.));
-  #     self.assertEqual(x(10), Interval(-9.,-2.));
-
-  #   x = x_raw;
-  #   v = v_raw;
-  #   t = Interval(7.,8.);
-  #   y = Interval(-2.,-1.);
-  #   ctc_eval.contract(t, y, x, v);
-  #     self.assertEqual(t, Interval(7.,8.));
-  #     self.assertEqual(y, Interval(-2.,-1.));
-  #     self.assertEqual(x(0), Interval(6.,8.)); 
-  #     self.assertEqual(x(1), Interval(4.5,7.));
-  #     self.assertEqual(x(2), Interval(3.,6.));
-  #     self.assertEqual(x(3), Interval(1.5,5.));
-  #     self.assertEqual(x(4), Interval(-0.,4.));
-  #     self.assertEqual(x(5), Interval(-1.,3.));
-  #     self.assertEqual(x(6), Interval(-2.,2.));
-  #     self.assertEqual(x(7), Interval(-3.5,0.5));
-  #     self.assertEqual(x(8), Interval(-5.,-1.));
-  #     self.assertEqual(x(9), Interval(-6.5,-2.));
-  #     self.assertEqual(x(10), Interval(-9.,-2.));
-
-  #   x = x_raw;
-  #   v = v_raw;
-  #   t = Interval(0.);
-  #   y = Interval(6.,8.);
-  #   ctc_eval.contract(t, y, x, v);
-  #     self.assertEqual(t, Interval(0.));
-  #     self.assertEqual(y, Interval(7.,8.));
-  #     self.assertEqual(x(0), Interval(6.,8.)); 
-  #     self.assertEqual(x(1), Interval(4.5,7.));
-  #     self.assertEqual(x(2), Interval(3.,6.));
-  #     self.assertEqual(x(3), Interval(1.5,5.));
-  #     self.assertEqual(x(4), Interval(-0.,4.));
-  #     self.assertEqual(x(5), Interval(-1.5,3.));
-  #     self.assertEqual(x(6), Interval(-3.,2.));
-  #     self.assertEqual(x(7), Interval(-4.5,1.));
-  #     self.assertEqual(x(8), Interval(-6.,0.));
-  #     self.assertEqual(x(9), Interval(-7.5,-1.));
-  #     self.assertEqual(x(10), Interval(-9.,-2.));/*
-  # }
-
-#   SECTION("Test CtcEval, non-zero derivative (positive case)")
-#   {
-#     Tube tube(Interval(0.,20.), 1.);
-#     Tube derivative(tube);
-#     derivative.set(Interval(1.,1.5));
-#     tube.set(Interval(-8.,-6.), 0);
-#     tube.ctc_deriv(derivative);
-
-      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
-      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
-      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
-      # self.assertEqual(tube(3), Interval(-5.,-1.5)); 
-      # self.assertEqual(tube(4), Interval(-4.,0.)); 
-      # self.assertEqual(tube(5), Interval(-3.,1.5)); 
-      # self.assertEqual(tube(6), Interval(-2.,3.)); 
-      # self.assertEqual(tube(7), Interval(-1.,4.5)); 
-      # self.assertEqual(tube(8), Interval(-0.,6.)); 
-      # self.assertEqual(tube(9), Interval(1.,7.5)); 
-      # self.assertEqual(tube(10), Interval(2.,9.)); 
-
-#     Interval intv_t, intv_y;
-#     Tube tube_raw(tube);
-
-      # intv_t = Interval(5.,10.);
-      # intv_y = Interval(-3.,-1.);
-#     tube.ctc_eval(intv_t, intv_y, derivative, false);
-      # self.assertEqual(intv_t, Interval(5.,8.));
-      # self.assertEqual(intv_y, Interval(-3.,-1.));
-      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
-      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
-      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
-      # self.assertEqual(tube(3), Interval(-5.,-2.)); 
-      # self.assertEqual(tube(4), Interval(-4.,-1.)); 
-      # self.assertEqual(tube(5), Interval(-3.,0.5)); 
-      # self.assertEqual(tube(6), Interval(-2.,2.)); 
-      # self.assertEqual(tube(7), Interval(-1.,3.5)); 
-      # self.assertEqual(tube(8), Interval(0.,5.)); 
-      # self.assertEqual(tube(9), Interval(1.,7.5)); 
-      # self.assertEqual(tube(10), Interval(2.,9.)); 
-
-#     tube = tube_raw;
-      # intv_t = Interval(2.,5.5);
-      # intv_y = Interval(-0.5,3.);
-#     tube.ctc_eval(intv_t, intv_y, derivative, false);
-      # self.assertEqual(intv_t, Interval(4.,5.5));
-      # self.assertEqual(intv_y, Interval(-0.5,0.75));
-      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
-      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
-      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
-      # self.assertEqual(tube(3), Interval(-4.25,-1.5)); 
-      # self.assertEqual(tube(4), Interval(-2.75,0.)); 
-      # self.assertEqual(tube(5), Interval(-1.25,1.5)); 
-      # self.assertEqual(tube(6), Interval(0.,3.)); 
-      # self.assertEqual(tube(7), Interval(-1.,4.5)); 
-      # self.assertEqual(tube(8), Interval(0.,6.));
-      # self.assertEqual(tube(9), Interval(1.,7.5)); 
-      # self.assertEqual(tube(10), Interval(2.,9.)); 
-
-#     tube = tube_raw;
-      # intv_t = Interval(3.5,7.);
-      # intv_y = Interval(-5.2,-4.8);
-#     tube.ctc_eval(intv_t, intv_y, derivative, false);
-#       self.assertEqual(intv_t, Interval.EMPTY_SET);
-#       self.assertEqual(intv_y, Interval.EMPTY_SET);
-#       self.assertEqual(tube(0), Interval(-8.,-6.)); 
-#       self.assertEqual(tube(1), Interval(-7.,-4.5)); 
-#       self.assertEqual(tube(2), Interval.EMPTY_SET); 
-#       self.assertEqual(tube(3), Interval.EMPTY_SET); 
-#       self.assertEqual(tube(4), Interval.EMPTY_SET); 
-#       self.assertEqual(tube(5), Interval(-3.,1.5)); 
-#       self.assertEqual(tube(6), Interval(-2.,3.)); 
-#       self.assertEqual(tube(7), Interval(-1.,4.5)); 
-#       self.assertEqual(tube(8), Interval(-0.,6.)); 
-#       self.assertEqual(tube(9), Interval(1.,7.5)); 
-#       self.assertEqual(tube(10, Interval(2.,9.));*/
-# #   }
-# }
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+
+class TestCtcEval(unittest.TestCase):
+
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+
+    def test_ctceval_1(self):
+
+        t = Interval(0.,6.)
+        z = Interval(-1.,1.)
+        x = Tube(Interval(-1.,7.), 2.);
+        v = Tube(x);
+        v.set(Interval(-1.), 0);
+        v.set(Interval(-1.,1.), 1);
+        v.set(Interval(-1.), 2);
+        v.set(Interval(1.), 3);
+
+        self.assertEqual(x.nb_slices(), 4);
+        ctc_eval = CtcEval();
+        ctc_eval.preserve_slicing(False);
+        ctc_eval.enable_time_propag(False);
+        ctc_eval.contract(t, z, x, v);
+        self.assertEqual(x.nb_slices(), 6);
+
+        self.assertEqual(x.codomain(), Interval.ALL_REALS); # only gates should be affected
+        self.assertEqual(x(-1.), Interval.ALL_REALS);
+        self.assertEqual(x(0.), Interval(-2.,6.));
+        self.assertEqual(x(1.), Interval(-3.,5.));
+        self.assertEqual(x(3.), Interval(-4.,3.));
+        self.assertEqual(x(5.), Interval(-6.,1.));
+        self.assertEqual(x(6.), Interval(-5.,2.));
+        self.assertEqual(x(7.), Interval.ALL_REALS);
+
+
+    def test_ctceval_2(self):
+        t, z =  Interval(0.,6.), Interval(-1.,1.);
+        x = Tube(Interval(-1.,7.), 2.);
+        v = Tube(x);
+        v.set(Interval(-1.), 0);
+        v.set(Interval(-1.,1.), 1);
+        v.set(Interval(-1.), 2);
+        v.set(Interval(1.), 3);
+
+        x.set(Interval(0.,1.), 2.);
+        v.sample(2.);
+
+        self.assertEqual(x.nb_slices(), 5);
+
+        ctc_eval = CtcEval();
+        ctc_eval.preserve_slicing(False);
+        ctc_eval.enable_time_propag(False);
+        ctc_eval.contract(t, z, x, v);
+
+        self.assertEqual(x.nb_slices(), 7);
+
+        self.assertEqual(x.codomain(), Interval.ALL_REALS); # only gates should be affected
+        self.assertEqual(x(-1.), Interval.ALL_REALS);
+        self.assertEqual(x(0.), Interval(0.,3.));
+        self.assertEqual(x(1.), Interval(-1.,2.));
+        self.assertEqual(x(2.), Interval(0.,1.));
+        self.assertEqual(x(3.), Interval(-1.,2.));
+        self.assertEqual(x(5.), Interval(-3.,1.));
+        self.assertEqual(x(6.), Interval(-2.,2.));
+        self.assertEqual(x(7.), Interval.ALL_REALS);
+
+        t = Interval(1.75,5.5);
+        z = Interval(1.6);
+
+        ctc_eval.enable_time_propag(True);
+        ctc_eval.contract(t, z, x, v);
+
+
+        box = IntervalVector([Interval(1.75,5.5), Interval(1.6)])
+
+        # if(VIBES_DRAWING) fig_tube->draw_box(box, vibesParams("figure", "ctceval", "red"));
+        ctc_eval.contract(box[0], box[1], x, v);
+        # if(VIBES_DRAWING) fig_tube->draw_box(box, vibesParams("figure", "ctceval", "blue"));
+
+        self.assertApproxIntv(x.interpol(3.4,v), Interval(0.8,1.6));
+        self.assertApproxIntv(box[0], Interval(2.6,3.4));
+        self.assertApproxIntv(box[1], Interval(1.6));
+
+
+class TestCtcEval2(unittest.TestCase):
+
+  def assertApproxIntv(self, first, second):
+    if first.is_empty() is False:
+    # if isinstance(second, Interval):
+        self.assertAlmostEqual(first.lb(), second.lb())
+        self.assertAlmostEqual(first.ub(), second.ub())
+    else:
+        self.assertEqual(first, second)
+
+  def setUp(self):
+    xdot = Tube(Interval(0., 10.), 1.0);
+    xdot.set(Interval(-0.5,1.));
+
+    x = Tube(xdot);
+    x.set(Interval.ALL_REALS);
+    x.set(Interval(-1.5,1.), 4);
+    x.set(Interval(-1.,1.5), 5);
+    self.assertEqual(x.nb_slices(), 10);
+    
+    self.ctc_deriv = CtcDeriv();
+    self.ctc_deriv.contract(x, xdot);
+
+    self.x_raw = Tube(x)
+    self.xdot_raw = Tube(xdot);
+
+    self.ctc_eval_propa = CtcEval()
+    self.ctc_eval_nopropa = CtcEval()
+    self.ctc_eval_propa.preserve_slicing(False);
+    self.ctc_eval_nopropa.preserve_slicing(False);
+    self.ctc_eval_propa.enable_time_propag(True);
+    self.ctc_eval_nopropa.enable_time_propag(False);
+
+  def test_1(self):
+    # Checking the tube...
+    self.assertEqual(self.x_raw(0), Interval(-5.5,3.));
+    self.assertEqual(self.x_raw(1), Interval(-4.5,2.5));
+    self.assertEqual(self.x_raw(2), Interval(-3.5,2.));
+    self.assertEqual(self.x_raw(3), Interval(-2.5,1.5));
+    self.assertEqual(self.x_raw(4), Interval(-1.5,1.));
+    self.assertEqual(self.x_raw(5), Interval(-1.,1.5));
+    self.assertEqual(self.x_raw(6), Interval(-1.5,2.5));
+    self.assertEqual(self.x_raw(7), Interval(-2.,3.5));
+    self.assertEqual(self.x_raw(8), Interval(-2.5,4.5));
+    self.assertEqual(self.x_raw(9), Interval(-3.,5.5));
+
+      # Interval intv_t, intv_y;
+      
+
+  def test_1_no_propa(self):
+    # Test A_no_propa
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 1.;
+    intv_y = Interval(-0.5,1.);
+    self.assertEqual(x(1.), Interval(-4.5,2.5));
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(intv_t, 1.);
+    self.assertEqual(intv_y, Interval(-0.5,1.));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1.), intv_y);
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(7), Interval(-2.,3.5));
+    self.assertEqual(x(8), Interval(-2.5,4.5));
+    self.assertEqual(x(9), Interval(-3.,5.5));
+
+  def  test_A__propa(self): 
+    # Test A_propa
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 1.;
+    intv_y = Interval(-0.5,1.);
+    self.assertEqual(x(1.), Interval(-4.5,2.5));
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(intv_t, 1.);
+    self.assertEqual(intv_y, Interval(-0.5,1.));
+    self.assertEqual(x(0), Interval(-1.5,1.5));
+    self.assertEqual(x(1.), intv_y);
+    self.assertEqual(x(1), Interval(-1.,2.));
+    self.assertEqual(x(2), Interval(-1.5,2.));
+    self.assertApproxIntv(x(3), Interval(-1.5-1./3.,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(7), Interval(-2.,3.5));
+    self.assertEqual(x(8), Interval(-2.5,4.5));
+    self.assertEqual(x(9), Interval(-3.,5.5));
+
+  def test_A_ctc_deriv(self):
+  # def test_A: ctc_deriv should not be effective after ctc_eval(true)(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 1.;
+    intv_y = Interval(-0.5,1.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+  def test_B_ctc_deriv(self):
+    # Test B_no_propa
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(0.5,2.5);
+    intv_y = Interval(-2.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(0.5,2.5));
+    self.assertEqual(intv_y, Interval(-2.));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(0.5), Interval(-4.,-1.));
+    self.assertEqual(x(1), Interval(-5.5,3.));
+    self.assertEqual(x(1.), Interval(-3.5,-1.25));
+    self.assertEqual(x(2), Interval(-4.5,2.5));
+    self.assertEqual(x(2.), Interval(-2.75,-0.5));
+    self.assertEqual(x(3), Interval(-3.5,2.));
+    self.assertEqual(x(2.5), Interval(-3.,-0.));
+    self.assertEqual(x(4), Interval(-3.5,2.));
+    self.assertEqual(x(5), Interval(-2.5,1.5));
+    self.assertEqual(x(6), Interval(-1.5,1.));
+    self.assertEqual(x(7), Interval(-1.,1.5));
+    self.assertEqual(x(8), Interval(-1.5,2.5));
+    self.assertEqual(x(9), Interval(-2.,3.5));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_B_ctc_deriv_propa(self):
+    # Test B_propa
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(0.5,2.5);
+    intv_y = Interval(-2.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(0.5,2.5));
+    self.assertEqual(intv_y, Interval(-2.));
+    self.assertEqual(x(0), Interval(-4.5,-0.75));
+    self.assertEqual(x(0.5), Interval(-4.,-1.));
+    self.assertEqual(x(1), Interval(-4.,-1.));
+    self.assertEqual(x(1.), Interval(-3.5,-1.25));
+    self.assertEqual(x.slice(0.6).tdomain(), Interval(0.5,1.));
+    self.assertEqual(x.slice(0.6).input_gate(), Interval(-4.,-1.));
+    self.assertEqual(x.slice(0.6).output_gate(), Interval(-3.5,-1.25));
+    self.assertEqual(xdot(2), Interval(-0.5,1.));
+    #self.assertEqual(x(2), Interval(-3.5,-0.5)); # todo: optimal implementation?
+    self.assertEqual(x(2.), Interval(-2.75,-0.5));
+    self.assertEqual(x(3), Interval(-3.,0.));
+    self.assertEqual(x(2.5), Interval(-3.,-0.));
+    self.assertEqual(x(4), Interval(-3.,0.5));
+    self.assertApproxIntv(x(5), Interval(-2.5,1.+1./6.));
+    self.assertEqual(x(6), Interval(-1.5,1.));
+    self.assertEqual(x(7), Interval(-1.,1.5));
+    self.assertEqual(x(8), Interval(-1.5,2.5));
+    self.assertEqual(x(9), Interval(-2.,3.5));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+
+  def test_C_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(0.5,3.5);
+    intv_y = Interval(-4.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(0.5,1.5));
+    self.assertEqual(intv_y, Interval(-4.));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(0.5), Interval(-5.,-3.5));
+    self.assertEqual(x(1), Interval(-5.5,3.));
+    self.assertEqual(x(1.), Interval(-4.5,-3.5));
+    self.assertEqual(x(2), Interval(-4.5,2.5));
+    self.assertEqual(x(1.5), Interval(-4.,-3.));
+    self.assertEqual(x(3), Interval(-4.5,2.5));
+    self.assertEqual(x(4), Interval(-3.5,2.));
+    self.assertEqual(x(5), Interval(-2.5,1.5));
+    self.assertEqual(x(6), Interval(-1.5,1.));
+    self.assertEqual(x(7), Interval(-1.,1.5));
+    self.assertEqual(x(8), Interval(-1.5,2.5));
+    self.assertEqual(x(9), Interval(-2.,3.5));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_C_propas(self):
+      x = Tube(self.x_raw);
+      xdot = Tube(self.xdot_raw);
+      intv_t = Interval(0.5,3.5);
+      intv_y = Interval(-4.);
+      self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+      self.assertEqual(x.nb_slices(), 12);
+      self.assertEqual(intv_t, Interval(0.5,1.5));
+      self.assertEqual(intv_y, Interval(-4.));
+      self.assertEqual(x(0), Interval(-5.5,-3.25));
+      self.assertEqual(x(0.5), Interval(-5.,-3.5));
+      # //self.assertEqual(x(1), Interval(-5.,-3.5)); // optimality
+      self.assertEqual(x(1.), Interval(-4.5,-3.5));
+      self.assertEqual(x(2), Interval(-4.5,-3.));
+      self.assertEqual(x(1.5), Interval(-4.,-3.));
+      self.assertEqual(x(3), Interval(-4.,-2.5));
+      self.assertEqual(x(4), Interval(-3.5,-1.5));
+      self.assertEqual(x(5), Interval(-2.5,-0.5));
+      self.assertEqual(x(6), Interval(-1.5,0.5));
+      self.assertEqual(x(7), Interval(-1.,1.5));
+      self.assertEqual(x(8), Interval(-1.5,2.5));
+      self.assertEqual(x(9), Interval(-2.,3.5));
+      self.assertEqual(x(10), Interval(-2.5,4.5));
+      self.assertEqual(x(11), Interval(-3.,5.5));
+
+#     if(false & VIBES_DRAWING) // drawing results
+#     {
+#       //x = x_raw;
+#       //xdot = xdot_raw;
+#       //IntervalVector box(2);
+#       //box[0] = Interval(0.5,3.5);
+#       //box[1] = Interval(-4.);
+#       //vibes::beginDrawing();
+#       //VIBesFigTube fig_tube("ctceval", &x);
+#       //fig_tube.set_properties(100, 100, 500, 500);
+#       //fig_tube.set_tube_derivative(&x, &xdot);
+#       //fig_tube.show(true);
+#       //contraction = ctc_eval_propa.contract(box[0], box[1], x, xdot);
+#       //fig_tube.show(true);
+#       //vibes::drawBox(box, vibesParams("figure", "ctceval", "blue"));
+#       //vibes::endDrawing();
+#     }
+
+  def test_D_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 3.5;
+    intv_y = Interval(-3.5,-0.5);
+    self.assertEqual(x.nb_slices(), 10);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(intv_t, 3.5);
+    self.assertEqual(intv_y, Interval(-2.,-0.5));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(3.5), Interval(-2.,-0.5));
+    self.assertEqual(x(4), Interval(-2.5,1.5));
+    self.assertEqual(x(5), Interval(-1.5,1.));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_D_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 3.5;
+    intv_y = Interval(-3.5,-0.5);
+    self.assertEqual(x.nb_slices(), 10);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(intv_t, 3.5);
+    self.assertEqual(intv_y, Interval(-2.,-0.5));
+    self.assertEqual(x(0), Interval(-5.5,1.25));
+    self.assertEqual(x(1), Interval(-4.5,0.75));
+    self.assertEqual(x(2), Interval(-3.5,0.25));
+    self.assertEqual(x(3), Interval(-2.5,-0.25));
+    self.assertEqual(x(3.5), Interval(-2.,-0.5));
+    self.assertEqual(x(4), Interval(-2.,0.));
+    self.assertEqual(x(5), Interval(-1.5,1.));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_E_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(6.5, 8.5);
+    intv_y = Interval(-4.5, -1.75);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(7.5, 8.5));
+    self.assertEqual(intv_y, Interval(-2.25, -1.75));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(7), Interval(-2.,3.5));
+    self.assertEqual(x(7.5), Interval(-1.75,-1.25));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(8.), Interval(-2.,-1.25));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_E_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(6.5, 8.5);
+    intv_y = Interval(-4.5, -1.75);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(7.5, 8.5));
+    self.assertEqual(intv_y, Interval(-2.25, -1.75));
+    self.assertEqual(x(0), Interval(-5.5,2.5));
+    self.assertEqual(x(1), Interval(-4.5,2.));
+    self.assertEqual(x(2), Interval(-3.5,1.5));
+    self.assertEqual(x(3), Interval(-2.5,1.));
+    self.assertEqual(x(4), Interval(-1.5,0.5));
+    self.assertEqual(x(5), Interval(-1.,0.));
+    self.assertEqual(x(6), Interval(-1.5,-0.5));
+    self.assertEqual(x(7), Interval(-1.75,-1.));
+    self.assertEqual(x(7.5), Interval(-1.75,-1.25));
+#     //CHECK(x(8), Interval(-2.,-1.25)); // optimality
+    self.assertEqual(x(8.), Interval(-2.,-1.25));
+    self.assertEqual(x(9), Interval(-2.25,-0.75));
+    self.assertEqual(x(10), Interval(-2.5,-0.25));
+    self.assertEqual(x(11), Interval(-3.,0.75));
+
+  def test_F_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(8.5,9.5);
+    intv_y = Interval(-0.5,2.5);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(8.5,9.5));
+    self.assertEqual(intv_y, Interval(-0.5,2.5));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(7), Interval(-2.,3.5));
+    self.assertEqual(x(8), Interval(-2.5,4.5));
+    self.assertEqual(x(8.5), Interval(-1.5,3.));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+    self.assertEqual(x(9.5), Interval(-1.,3.5));
+    self.assertEqual(x(11), Interval(-3,5.5));
+
+  def test_F_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(8.5,9.5);
+    intv_y = Interval(-0.5,2.5);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(intv_t, Interval(8.5,9.5));
+    self.assertEqual(intv_y, Interval(-0.5,2.5));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertApproxIntv(x(7), Interval(-2.,3.+1./3.));
+    self.assertEqual(x(8), Interval(-2.,3.25));
+    self.assertEqual(x(8.5), Interval(-1.5,3.));
+#     //CHECK(x(9), Interval(-1.5,3.)); // optimality
+#     //CHECK(x(10), Interval(-1.,3.5)); // optimality
+    self.assertEqual(x(9.5), Interval(-1.,3.5));
+    self.assertEqual(x(11), Interval(-1.25,4.));
+
+  def test_G_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(6.5,7.5);
+    intv_y = Interval(3.,4.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(7.5));
+    self.assertEqual(intv_y, Interval(3.));
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(7), Interval(-2.,3.5));
+    self.assertEqual(x(7.5), Interval(3.));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_G_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(6.5,7.5);
+    intv_y = Interval(3.,4.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(7.5));
+    self.assertEqual(intv_y, Interval(3.));
+    self.assertEqual(x(0), Interval(-4.5,3.));
+    self.assertEqual(x(1), Interval(-3.5,2.5));
+    self.assertEqual(x(2), Interval(-2.5,2.));
+    self.assertEqual(x(3), Interval(-1.5,1.5));
+    self.assertEqual(x(4), Interval(-0.5,1.));
+    self.assertEqual(x(5), Interval(0.5,1.5));
+    self.assertEqual(x(6), Interval(1.5,2.5));
+    self.assertEqual(x(7), Interval(2.5,3.));
+    self.assertEqual(x(7.5), Interval(3.));
+    self.assertEqual(x(8), Interval(2.75,3.5));
+    self.assertEqual(x(9), Interval(2.25,4.5));
+    self.assertEqual(x(10), Interval(1.75,5.5));
+
+  def test_H_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(7.,8.25);
+    intv_y = Interval(4.25,5.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval.EMPTY_SET);
+    self.assertEqual(intv_y, Interval.EMPTY_SET);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(x(0), Interval.EMPTY_SET);
+    self.assertEqual(x(1), Interval.EMPTY_SET);
+    self.assertEqual(x(2), Interval.EMPTY_SET);
+    self.assertEqual(x(3), Interval.EMPTY_SET);
+    self.assertEqual(x(4), Interval.EMPTY_SET);
+    self.assertEqual(x(5), Interval.EMPTY_SET);
+    self.assertEqual(x(6), Interval.EMPTY_SET);
+    self.assertEqual(x(7), Interval.EMPTY_SET);
+    self.assertEqual(x(8), Interval.EMPTY_SET);
+    self.assertEqual(x(9), Interval.EMPTY_SET);
+    self.assertTrue(x.is_empty());
+
+  def test_H_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(7.,8.25);
+    intv_y = Interval(4.25,5.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval.EMPTY_SET);
+    self.assertEqual(intv_y, Interval.EMPTY_SET);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(x(0), Interval.EMPTY_SET);
+    self.assertEqual(x(1), Interval.EMPTY_SET);
+    self.assertEqual(x(2), Interval.EMPTY_SET);
+    self.assertEqual(x(3), Interval.EMPTY_SET);
+    self.assertEqual(x(4), Interval.EMPTY_SET);
+    self.assertEqual(x(5), Interval.EMPTY_SET);
+    self.assertEqual(x(6), Interval.EMPTY_SET);
+    self.assertEqual(x(7), Interval.EMPTY_SET);
+    self.assertEqual(x(8), Interval.EMPTY_SET);
+    self.assertEqual(x(9), Interval.EMPTY_SET);
+    self.assertTrue(x.is_empty());
+
+  def test_I_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(2.5);
+    intv_y = Interval(0.5);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(2.5));
+    self.assertEqual(intv_y, Interval(0.5));
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(2.5), Interval(0.5));
+    self.assertEqual(x(3), Interval(-3.5,2.));
+    self.assertEqual(x(4), Interval(-2.5,1.5));
+    self.assertEqual(x(5), Interval(-1.5,1.));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_I_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(2.5);
+    intv_y = Interval(0.5);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(2.5));
+    self.assertEqual(intv_y, Interval(0.5));
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(x(0), Interval(-2.,1.75));
+    self.assertEqual(x(1), Interval(-1.,1.25));
+    self.assertEqual(x(2), Interval(-0.,0.75));
+    self.assertEqual(x(2.5), Interval(0.5));
+    self.assertEqual(x(3), Interval(0.25,1.));
+    self.assertApproxIntv(x(4), Interval(-0.25,1.+1./3.));
+    self.assertEqual(x(5), Interval(-0.75,1.));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_J_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 6.25;
+    intv_y = Interval(0.5,1.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, 6.25);
+    self.assertEqual(intv_y, Interval(0.5,1.));
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(6.25), Interval(0.5,1.));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+
+  def test_J_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = 6.25;
+    intv_y = Interval(0.5,1.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, 6.25);
+    self.assertEqual(intv_y, Interval(0.5,1.));
+    self.assertEqual(x.nb_slices(), 11);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5.), Interval(-0.75,1.));
+    self.assertApproxIntv(x(5), Interval(-0.75,1.4+1./60.));
+    self.assertEqual(x(6), Interval(0.25,1.125));
+    self.assertEqual(x(7), Interval(0.125,1.75));
+    self.assertEqual(x(8), Interval(0.125-0.5,2.75));
+    self.assertEqual(x(9), Interval(0.125-1.,3.75));
+    self.assertEqual(x(10), Interval(0.125-1.5,4.75));
+
+  def test_K_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(5.25, 8.25);
+    intv_y = Interval(-0.5, 0.);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(5.25, 8.25));
+    self.assertEqual(intv_y, Interval(-0.5, 0.));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(5.25), Interval(-1.,1.25));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(8.25), Interval(-2.,3.));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_K_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(5.25, 8.25);
+    intv_y = Interval(-0.5, 0.);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(5.25, 8.25));
+    self.assertEqual(intv_y, Interval(-0.5, 0.));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.25));
+    self.assertEqual(x(5.25), Interval(-1.,1.25));
+    self.assertApproxIntv(x(6), Interval(-1.,1.4+1./60.));
+    self.assertEqual(x(7), Interval(-1.5,1.875));
+    self.assertApproxIntv(x(8), Interval(-1.625-1./3.,2.75));
+    self.assertEqual(x(9), Interval(-2.,3.));
+    self.assertEqual(x(8.25), Interval(-2.,3.));
+    self.assertEqual(x(10), Interval(-2.375,3.75));
+    self.assertEqual(x(11), Interval(-2.875,4.75));
+
+  def test_L_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(1.5,4.5);
+    intv_y = Interval(1.75,2.75);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(1.5,2.5));
+    self.assertEqual(intv_y, Interval(1.75,2.25));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(1.5), Interval(0.75,2.25));
+    self.assertEqual(x(2), Interval(-4.5,2.5));
+    self.assertEqual(x(3), Interval(-3.5,2.));
+    self.assertEqual(x(2.5), Interval(1.25,1.75));
+    self.assertEqual(x(4), Interval(-3.5,2.));
+    self.assertEqual(x(5), Interval(-2.5,1.5));
+    self.assertEqual(x(6), Interval(-1.5,1.));
+    self.assertEqual(x(7), Interval(-1.,1.5));
+    self.assertEqual(x(8), Interval(-1.5,2.5));
+    self.assertEqual(x(9), Interval(-2.,3.5));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_L_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(1.5,2.5);
+    intv_y = Interval(1.75,2.75);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(1.5,2.5));
+    self.assertEqual(intv_y, Interval(1.75,2.25));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-0.75,3.));
+    self.assertEqual(x(1), Interval(0.25,2.5));
+    self.assertEqual(x(1.5), Interval(0.75,2.25));
+    self.assertEqual(x(2), Interval(0.75,2.25));
+#     //CHECK(x(3), Interval(1.25,2.)); // optimality
+    self.assertEqual(x(2.5), Interval(1.25,1.75));
+    self.assertEqual(x(4), Interval(1.,1.75));
+    self.assertEqual(x(5), Interval(0.5,1.5));
+    self.assertEqual(x(6), Interval(0.,1.));
+    self.assertEqual(x(7), Interval(-0.5,1.5));
+    self.assertEqual(x(8), Interval(-1.,2.5));
+    self.assertEqual(x(9), Interval(-1.5,3.5));
+    self.assertEqual(x(10), Interval(-2.,4.5));
+    self.assertEqual(x(11), Interval(-2.5,5.5));
+
+  def test_M_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(0.75,1.25);
+    intv_y = Interval(-5.75,-5.25);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval.EMPTY_SET);
+    self.assertEqual(intv_y, Interval.EMPTY_SET);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(x(0), Interval.EMPTY_SET);
+    self.assertEqual(x(1), Interval.EMPTY_SET);
+    self.assertEqual(x(2), Interval.EMPTY_SET);
+    self.assertEqual(x(3), Interval.EMPTY_SET);
+    self.assertEqual(x(4), Interval.EMPTY_SET);
+    self.assertEqual(x(5), Interval.EMPTY_SET);
+    self.assertEqual(x(6), Interval.EMPTY_SET);
+    self.assertEqual(x(7), Interval.EMPTY_SET);
+    self.assertEqual(x(8), Interval.EMPTY_SET);
+    self.assertEqual(x(9), Interval.EMPTY_SET);
+    self.assertTrue(x.is_empty());
+
+  def test_M_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(0.75,1.25);
+    intv_y = Interval(-5.75,-5.25);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval.EMPTY_SET);
+    self.assertEqual(intv_y, Interval.EMPTY_SET);
+    self.assertEqual(x.nb_slices(), 10);
+    self.assertEqual(x(0), Interval.EMPTY_SET);
+    self.assertEqual(x(1), Interval.EMPTY_SET);
+    self.assertEqual(x(2), Interval.EMPTY_SET);
+    self.assertEqual(x(3), Interval.EMPTY_SET);
+    self.assertEqual(x(4), Interval.EMPTY_SET);
+    self.assertEqual(x(5), Interval.EMPTY_SET);
+    self.assertEqual(x(6), Interval.EMPTY_SET);
+    self.assertEqual(x(7), Interval.EMPTY_SET);
+    self.assertEqual(x(8), Interval.EMPTY_SET);
+    self.assertEqual(x(9), Interval.EMPTY_SET);
+    self.assertTrue(x.is_empty());
+
+  def test_N_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(5.5,8.5);
+    intv_y = Interval(2.,5.5);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(6.5,8.5));
+    self.assertEqual(intv_y, Interval(2.,4.));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-1.5,2.5));
+    self.assertEqual(x(6.5), Interval(0.,2.));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(8.5), Interval(1.,4.));
+    self.assertEqual(x(10), Interval(-2.5,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_N_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(5.5,8.5);
+    intv_y = Interval(2.,5.5);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(6.5,8.5));
+    self.assertEqual(intv_y, Interval(2.,4.));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(3), Interval(-2.5,1.5));
+    self.assertEqual(x(4), Interval(-1.5,1.));
+    self.assertEqual(x(5), Interval(-1.,1.5));
+    self.assertEqual(x(6), Interval(-0.5,2.));
+    self.assertEqual(x(6.5), Interval(0.,2.));
+    self.assertEqual(x(7), Interval(0.,2.5));
+#     //CHECK(x(8), Interval(xxx)); // optimality
+    self.assertEqual(x(9), Interval(1.,4.));
+    self.assertEqual(x(8.5), Interval(1.,4.));
+    self.assertEqual(x(10), Interval(0.75,4.5));
+    self.assertEqual(x(11), Interval(0.25,5.5));
+
+  def test_0_no_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(2.5,9.5);
+    intv_y = Interval(-5.,-2.5);
+    self.ctc_eval_nopropa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(2.5,9.5));
+    self.assertEqual(intv_y, Interval(-3.,-2.5));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,3.));
+    self.assertEqual(x(1), Interval(-4.5,2.5));
+    self.assertEqual(x(2), Interval(-3.5,2.));
+    self.assertEqual(x(2.5), Interval(-3.,1.));
+    self.assertEqual(x(3), Interval(-3.5,2.));
+    self.assertEqual(x(4), Interval(-2.5,1.5));
+    self.assertEqual(x(5), Interval(-1.5,1.));
+    self.assertEqual(x(6), Interval(-1.,1.5));
+    self.assertEqual(x(7), Interval(-1.5,2.5));
+    self.assertEqual(x(8), Interval(-2.,3.5));
+    self.assertEqual(x(9), Interval(-2.5,4.5));
+    self.assertEqual(x(10), Interval(-3.,5.5));
+    self.assertEqual(x(9.5), Interval(-2.75,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.5));
+
+  def test_0_propa(self):
+    x = Tube(self.x_raw);
+    xdot = Tube(self.xdot_raw);
+    intv_t = Interval(2.5,9.5);
+    intv_y = Interval(-5.,-2.5);
+    self.ctc_eval_propa.contract(intv_t, intv_y, x, xdot);
+    self.assertEqual(intv_t, Interval(2.5,9.5));
+    self.assertEqual(intv_y, Interval(-3.,-2.5));
+    self.assertEqual(x.nb_slices(), 12);
+    self.assertEqual(x(0), Interval(-5.5,2.25));
+    self.assertEqual(x(1), Interval(-4.5,1.75));
+    self.assertEqual(x(2), Interval(-3.5,1.25));
+    self.assertEqual(x(2.5), Interval(-3.,1.));
+    self.assertEqual(x(3), Interval(-3.,1.));
+    self.assertEqual(x(4), Interval(-2.5,0.75));
+#     //CHECK(x(5), Interval(xxx)); // optimality
+    self.assertEqual(x(6), Interval(-1.,1.));
+    self.assertEqual(x(7), Interval(-1.5,2.));
+    self.assertEqual(x(8), Interval(-2.,3.));
+    self.assertEqual(x(9), Interval(-2.5,4.));
+    self.assertEqual(x(10), Interval(-2.75,4.5));
+    self.assertEqual(x(9.5), Interval(-2.75,4.5));
+    self.assertEqual(x(11), Interval(-3.,5.));
+#   }
+
+  def Test_CtcEval_multi_eval(self):
+
+    x = Tube(Interval(0.,20.), 0.1, TFunction("cos(t)+t*[-0.1,0.2]"));
+    v = Tube(Interval(0.,20.), 0.1, TFunction("-sin(t)+[-0.1,0.2]"));
+    
+    ctc_deriv = CtcDeriv();
+    ctc_deriv.contract(x, v);
+
+    box = IntervalVector(2);
+    ctc_eval = CtcEval();
+    ctc_eval.enable_time_propag(True);
+    x_c = Tube(x); 
+    v_c = Tube(v);
+
+    box[0] = Interval(11.98);
+    box[1] = Interval(1.);
+    ctc_eval.contract(box[0], box[1], x_c, v_c);
+
+    box[0] = Interval(6.5);
+    box[1] = Interval(1.);
+    ctc_eval.contract(box[0], box[1], x_c, v_c);
+
+#     if(VIBES_DRAWING) // drawing results
+#     {
+#       //vibes::beginDrawing();
+#       //VIBesFigTube fig_tube("ctceval", &x);
+#       //fig_tube.set_properties(100, 100, 800, 400);
+#       //fig_tube.set_tube_derivative(&x, &v);
+#       //fig_tube.show(true);
+#       //x = x_c;
+#       //v = v_c;
+#       //fig_tube.show(true);
+#       //vibes::drawBox(box, vibesParams("figure", "ctceval", "red"));
+#     }
+#   }
+  def  Test_CtcEval_non_zero_derivative_negative_case(self):
+#   SECTION("Test CtcEval, non-zero derivative (negative case)")
+
+    x = Tube(Interval(0.,11.), 1.);
+    v = Tube(x);
+    v.set(Interval(-1.5,-1.));
+    x.set(Interval(6.,8.), 0);
+
+    ctc_eval = CtcEval;
+    ctc_deriv = CtcDeriv;
+    ctc_deriv.contract(x, v);
+
+    self.assertEqual(x(0), Interval(6.,8.)); 
+    self.assertEqual(x(1), Interval(4.5,7.));
+    self.assertEqual(x(2), Interval(3.,6.));
+    self.assertEqual(x(3), Interval(1.5,5.));
+    self.assertEqual(x(4), Interval(-0.,4.));
+    self.assertEqual(x(5), Interval(-1.5,3.));
+    self.assertEqual(x(6), Interval(-3.,2.));
+    self.assertEqual(x(7), Interval(-4.5,1.));
+    self.assertEqual(x(8), Interval(-6.,0.));
+    self.assertEqual(x(9), Interval(-7.5,-1.));
+    self.assertEqual(x(10), Interval(-9.,-2.));
+
+    # Interval t, y;
+    # x_raw = Tube(x);
+    # v_raw = Tube(v);
+
+    # x = Tube(x_raw);
+    # v = Tube(v_raw);
+    # t = Interval(3.5,6.);
+    # y = Interval(3.5,6.);
+    # ctc_eval.contract(t, y, x, v);
+  #   /*CHECK(t, Interval(3.5,5.));
+  #     self.assertEqual(y, Interval(3.5,4.5));
+  #     self.assertEqual(x(0), Interval(6.,8.));
+  #     self.assertEqual(x(1), Interval(4.5,7.));
+  #     self.assertEqual(x(2), Interval(4.,6.));
+  #     self.assertEqual(x(3), Interval(2.75,5.));
+  #     self.assertEqual(x(4), Interval(1.25,4.));
+  #     self.assertEqual(x(5), Interval(-0.25,3.));
+  #     self.assertEqual(x(6), Interval(-3.,2.));
+  #     self.assertEqual(x(7), Interval(-4.5,1.));
+  #     self.assertEqual(x(8), Interval(-6.,0.));
+  #     self.assertEqual(x(9), Interval(-7.5,-1.));
+  #     self.assertEqual(x(10), Interval(-9.,-2.));
+
+  #   x = x_raw;
+  #   v = v_raw;
+  #   t = Interval(3.,8.5);
+  #   y = Interval(-7.,-2.5);
+  #   ctc_eval.contract(t, y, x, v);
+  #     self.assertEqual(t, Interval(6.,8.5));
+  #     self.assertEqual(y, Interval(-5.25,-2.5));
+  #     self.assertEqual(x(0), Interval(6.,8.)); 
+  #     self.assertEqual(x(1), Interval(4.5,7.));
+  #     self.assertEqual(x(2), Interval(3.,6.));
+  #     self.assertEqual(x(3), Interval(1.5,5.));
+  #     self.assertEqual(x(4), Interval(-0.,4.));
+  #     self.assertEqual(x(5), Interval(-1.5,2.75));
+  #     self.assertEqual(x(6), Interval(-3.,1.25));
+  #     self.assertEqual(x(7), Interval(-4.5,-0.25));
+  #     self.assertEqual(x(8), Interval(-6.,-1.75));
+  #     self.assertEqual(x(9), Interval(-7.5,-3.));
+  #     self.assertEqual(x(10), Interval(-9.,-2.));
+
+  #   x = x_raw;
+  #   v = v_raw;
+  #   t = Interval(7.,8.);
+  #   y = Interval(-2.,-1.);
+  #   ctc_eval.contract(t, y, x, v);
+  #     self.assertEqual(t, Interval(7.,8.));
+  #     self.assertEqual(y, Interval(-2.,-1.));
+  #     self.assertEqual(x(0), Interval(6.,8.)); 
+  #     self.assertEqual(x(1), Interval(4.5,7.));
+  #     self.assertEqual(x(2), Interval(3.,6.));
+  #     self.assertEqual(x(3), Interval(1.5,5.));
+  #     self.assertEqual(x(4), Interval(-0.,4.));
+  #     self.assertEqual(x(5), Interval(-1.,3.));
+  #     self.assertEqual(x(6), Interval(-2.,2.));
+  #     self.assertEqual(x(7), Interval(-3.5,0.5));
+  #     self.assertEqual(x(8), Interval(-5.,-1.));
+  #     self.assertEqual(x(9), Interval(-6.5,-2.));
+  #     self.assertEqual(x(10), Interval(-9.,-2.));
+
+  #   x = x_raw;
+  #   v = v_raw;
+  #   t = Interval(0.);
+  #   y = Interval(6.,8.);
+  #   ctc_eval.contract(t, y, x, v);
+  #     self.assertEqual(t, Interval(0.));
+  #     self.assertEqual(y, Interval(7.,8.));
+  #     self.assertEqual(x(0), Interval(6.,8.)); 
+  #     self.assertEqual(x(1), Interval(4.5,7.));
+  #     self.assertEqual(x(2), Interval(3.,6.));
+  #     self.assertEqual(x(3), Interval(1.5,5.));
+  #     self.assertEqual(x(4), Interval(-0.,4.));
+  #     self.assertEqual(x(5), Interval(-1.5,3.));
+  #     self.assertEqual(x(6), Interval(-3.,2.));
+  #     self.assertEqual(x(7), Interval(-4.5,1.));
+  #     self.assertEqual(x(8), Interval(-6.,0.));
+  #     self.assertEqual(x(9), Interval(-7.5,-1.));
+  #     self.assertEqual(x(10), Interval(-9.,-2.));/*
+  # }
+
+#   SECTION("Test CtcEval, non-zero derivative (positive case)")
+#   {
+#     Tube tube(Interval(0.,20.), 1.);
+#     Tube derivative(tube);
+#     derivative.set(Interval(1.,1.5));
+#     tube.set(Interval(-8.,-6.), 0);
+#     tube.ctc_deriv(derivative);
+
+      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
+      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
+      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
+      # self.assertEqual(tube(3), Interval(-5.,-1.5)); 
+      # self.assertEqual(tube(4), Interval(-4.,0.)); 
+      # self.assertEqual(tube(5), Interval(-3.,1.5)); 
+      # self.assertEqual(tube(6), Interval(-2.,3.)); 
+      # self.assertEqual(tube(7), Interval(-1.,4.5)); 
+      # self.assertEqual(tube(8), Interval(-0.,6.)); 
+      # self.assertEqual(tube(9), Interval(1.,7.5)); 
+      # self.assertEqual(tube(10), Interval(2.,9.)); 
+
+#     Interval intv_t, intv_y;
+#     Tube tube_raw(tube);
+
+      # intv_t = Interval(5.,10.);
+      # intv_y = Interval(-3.,-1.);
+#     tube.ctc_eval(intv_t, intv_y, derivative, false);
+      # self.assertEqual(intv_t, Interval(5.,8.));
+      # self.assertEqual(intv_y, Interval(-3.,-1.));
+      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
+      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
+      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
+      # self.assertEqual(tube(3), Interval(-5.,-2.)); 
+      # self.assertEqual(tube(4), Interval(-4.,-1.)); 
+      # self.assertEqual(tube(5), Interval(-3.,0.5)); 
+      # self.assertEqual(tube(6), Interval(-2.,2.)); 
+      # self.assertEqual(tube(7), Interval(-1.,3.5)); 
+      # self.assertEqual(tube(8), Interval(0.,5.)); 
+      # self.assertEqual(tube(9), Interval(1.,7.5)); 
+      # self.assertEqual(tube(10), Interval(2.,9.)); 
+
+#     tube = tube_raw;
+      # intv_t = Interval(2.,5.5);
+      # intv_y = Interval(-0.5,3.);
+#     tube.ctc_eval(intv_t, intv_y, derivative, false);
+      # self.assertEqual(intv_t, Interval(4.,5.5));
+      # self.assertEqual(intv_y, Interval(-0.5,0.75));
+      # self.assertEqual(tube(0), Interval(-8.,-6.)); 
+      # self.assertEqual(tube(1), Interval(-7.,-4.5)); 
+      # self.assertEqual(tube(2), Interval(-6.,-3.)); 
+      # self.assertEqual(tube(3), Interval(-4.25,-1.5)); 
+      # self.assertEqual(tube(4), Interval(-2.75,0.)); 
+      # self.assertEqual(tube(5), Interval(-1.25,1.5)); 
+      # self.assertEqual(tube(6), Interval(0.,3.)); 
+      # self.assertEqual(tube(7), Interval(-1.,4.5)); 
+      # self.assertEqual(tube(8), Interval(0.,6.));
+      # self.assertEqual(tube(9), Interval(1.,7.5)); 
+      # self.assertEqual(tube(10), Interval(2.,9.)); 
+
+#     tube = tube_raw;
+      # intv_t = Interval(3.5,7.);
+      # intv_y = Interval(-5.2,-4.8);
+#     tube.ctc_eval(intv_t, intv_y, derivative, false);
+#       self.assertEqual(intv_t, Interval.EMPTY_SET);
+#       self.assertEqual(intv_y, Interval.EMPTY_SET);
+#       self.assertEqual(tube(0), Interval(-8.,-6.)); 
+#       self.assertEqual(tube(1), Interval(-7.,-4.5)); 
+#       self.assertEqual(tube(2), Interval.EMPTY_SET); 
+#       self.assertEqual(tube(3), Interval.EMPTY_SET); 
+#       self.assertEqual(tube(4), Interval.EMPTY_SET); 
+#       self.assertEqual(tube(5), Interval(-3.,1.5)); 
+#       self.assertEqual(tube(6), Interval(-2.,3.)); 
+#       self.assertEqual(tube(7), Interval(-1.,4.5)); 
+#       self.assertEqual(tube(8), Interval(-0.,6.)); 
+#       self.assertEqual(tube(9), Interval(1.,7.5)); 
+#       self.assertEqual(tube(10, Interval(2.,9.));*/
+# #   }
+# }
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_multi_arithmetic.py

 * *Ordering differences only*

```diff
@@ -1,107 +1,107 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-
-class TestArithmeticOnTube(unittest.TestCase):
-
-  def assertApproxIntv(self, first, second):
-    if first.is_empty() is False:
-    # if isinstance(second, Interval):
-      self.assertAlmostEqual(first.lb(), second.lb())
-      self.assertAlmostEqual(first.ub(), second.ub())
-    else:
-      self.assertEqual(first, second)
-
-  def test_interval(self):
-
-    a = Interval(1,2)
-    b = Interval(6,7)
-    self.assertEqual(a+b, Interval(7,9))
-
-  def test_cos(self):
-
-    testd = 3.0
-    self.assertAlmostEqual(cos(testd), -0.9899924966004454);
-
-    testintv = Interval(0,oo)
-    self.assertEqual(cos(testintv),Interval(-1,1))
-
-    testtube = Tube(Interval(0,1),0.1)
-    self.assertEqual(cos(testtube).codomain(),Interval(-1,1))
-
-    testtraj = Trajectory(Interval(0,1), TFunction("sin(t)"), 0.1)
-    self.assertApproxIntv(cos(testtraj).codomain(),Interval(0.6663667453928805, 1))
-
-  def test_sqr(self):
-
-    testd = 3.0
-    self.assertAlmostEqual(sqr(testd), 9);
-
-    testintv = Interval(1,2)
-    self.assertEqual(sqr(testintv),Interval(1,4))
-
-    testtube = Tube(Interval(0,1),0.1,Interval(3,4))
-    self.assertEqual(sqr(testtube).codomain(),Interval(9,16))
-
-    testtraj = Trajectory(Interval(3,4), TFunction("t"), 0.1)
-    self.assertAlmostEqual(sqr(testtraj).codomain().lb(),9)
-    self.assertAlmostEqual(sqr(testtraj).codomain().ub(),16)
-
-  def test_pow(self):
-
-    testdx = 3.0
-    testdy = 4.0
-    self.assertAlmostEqual(pow(testdx,testdy), 81);
-
-    testintvx = Interval(3)
-    testintvy = Interval(4)
-    self.assertEqual(pow(testintvx,testdy), Interval(81.));
-    self.assertEqual(pow(testdx,testintvy), Interval(81.));
-    self.assertEqual(pow(testintvx,testintvy),Interval(81.))
-
-    testcodac = Tube(Interval(0,1),0.1,Interval(3))
-    testtubey = Tube(Interval(0,1),0.1,Interval(4))
-    self.assertApproxIntv(pow(testcodac,testdy).codomain(),Interval(81.))
-    self.assertApproxIntv(pow(testcodac,testintvy).codomain(),Interval(81.))
-
-    testtrajx = Trajectory(Interval(3,4), TFunction("3"), 0.1)
-    testtrajy = Trajectory(Interval(3,4), TFunction("4"), 0.1)
-    self.assertApproxIntv(pow(testtrajx,testdy).codomain(),Interval(81.))
-
-  def test_atan2(self):
-
-    testdx = 3.0
-    testdy = 4.0
-    self.assertAlmostEqual(atan2(testdy,testdx), 0.9272952180016122);
-
-    testintvx = Interval(3)
-    testintvy = Interval(4)
-    self.assertApproxIntv(atan2(testintvy,testdx), Interval(0.9272952180016122));
-    self.assertApproxIntv(atan2(testdy,testintvx), Interval(0.9272952180016122));
-    self.assertApproxIntv(atan2(testintvy,testintvx),Interval(0.9272952180016122))
-
-    testcodac = Tube(Interval(0,1),0.1,Interval(3))
-    testtubey = Tube(Interval(0,1),0.1,Interval(4))
-    self.assertApproxIntv(atan2(testtubey,testcodac).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testtubey,testdx).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testdy,testcodac).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testtubey,testintvx).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testintvy,testcodac).codomain(),Interval(0.9272952180016122))
-
-    testtrajx = Trajectory(Interval(3,4), TFunction("3"), 0.1)
-    testtrajy = Trajectory(Interval(3,4), TFunction("4"), 0.1)
-    self.assertApproxIntv(atan2(testtrajy,testtrajx).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testtrajy,testdx).codomain(),Interval(0.9272952180016122))
-    self.assertApproxIntv(atan2(testdy,testtrajx).codomain(),Interval(0.9272952180016122))
-        
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+
+class TestArithmeticOnTube(unittest.TestCase):
+
+  def assertApproxIntv(self, first, second):
+    if first.is_empty() is False:
+    # if isinstance(second, Interval):
+      self.assertAlmostEqual(first.lb(), second.lb())
+      self.assertAlmostEqual(first.ub(), second.ub())
+    else:
+      self.assertEqual(first, second)
+
+  def test_interval(self):
+
+    a = Interval(1,2)
+    b = Interval(6,7)
+    self.assertEqual(a+b, Interval(7,9))
+
+  def test_cos(self):
+
+    testd = 3.0
+    self.assertAlmostEqual(cos(testd), -0.9899924966004454);
+
+    testintv = Interval(0,oo)
+    self.assertEqual(cos(testintv),Interval(-1,1))
+
+    testtube = Tube(Interval(0,1),0.1)
+    self.assertEqual(cos(testtube).codomain(),Interval(-1,1))
+
+    testtraj = Trajectory(Interval(0,1), TFunction("sin(t)"), 0.1)
+    self.assertApproxIntv(cos(testtraj).codomain(),Interval(0.6663667453928805, 1))
+
+  def test_sqr(self):
+
+    testd = 3.0
+    self.assertAlmostEqual(sqr(testd), 9);
+
+    testintv = Interval(1,2)
+    self.assertEqual(sqr(testintv),Interval(1,4))
+
+    testtube = Tube(Interval(0,1),0.1,Interval(3,4))
+    self.assertEqual(sqr(testtube).codomain(),Interval(9,16))
+
+    testtraj = Trajectory(Interval(3,4), TFunction("t"), 0.1)
+    self.assertAlmostEqual(sqr(testtraj).codomain().lb(),9)
+    self.assertAlmostEqual(sqr(testtraj).codomain().ub(),16)
+
+  def test_pow(self):
+
+    testdx = 3.0
+    testdy = 4.0
+    self.assertAlmostEqual(pow(testdx,testdy), 81);
+
+    testintvx = Interval(3)
+    testintvy = Interval(4)
+    self.assertEqual(pow(testintvx,testdy), Interval(81.));
+    self.assertEqual(pow(testdx,testintvy), Interval(81.));
+    self.assertEqual(pow(testintvx,testintvy),Interval(81.))
+
+    testcodac = Tube(Interval(0,1),0.1,Interval(3))
+    testtubey = Tube(Interval(0,1),0.1,Interval(4))
+    self.assertApproxIntv(pow(testcodac,testdy).codomain(),Interval(81.))
+    self.assertApproxIntv(pow(testcodac,testintvy).codomain(),Interval(81.))
+
+    testtrajx = Trajectory(Interval(3,4), TFunction("3"), 0.1)
+    testtrajy = Trajectory(Interval(3,4), TFunction("4"), 0.1)
+    self.assertApproxIntv(pow(testtrajx,testdy).codomain(),Interval(81.))
+
+  def test_atan2(self):
+
+    testdx = 3.0
+    testdy = 4.0
+    self.assertAlmostEqual(atan2(testdy,testdx), 0.9272952180016122);
+
+    testintvx = Interval(3)
+    testintvy = Interval(4)
+    self.assertApproxIntv(atan2(testintvy,testdx), Interval(0.9272952180016122));
+    self.assertApproxIntv(atan2(testdy,testintvx), Interval(0.9272952180016122));
+    self.assertApproxIntv(atan2(testintvy,testintvx),Interval(0.9272952180016122))
+
+    testcodac = Tube(Interval(0,1),0.1,Interval(3))
+    testtubey = Tube(Interval(0,1),0.1,Interval(4))
+    self.assertApproxIntv(atan2(testtubey,testcodac).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testtubey,testdx).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testdy,testcodac).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testtubey,testintvx).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testintvy,testcodac).codomain(),Interval(0.9272952180016122))
+
+    testtrajx = Trajectory(Interval(3,4), TFunction("3"), 0.1)
+    testtrajy = Trajectory(Interval(3,4), TFunction("4"), 0.1)
+    self.assertApproxIntv(atan2(testtrajy,testtrajx).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testtrajy,testdx).codomain(),Interval(0.9272952180016122))
+    self.assertApproxIntv(atan2(testdy,testtrajx).codomain(),Interval(0.9272952180016122))
+        
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctccartprod.py

 * *Ordering differences only*

```diff
@@ -1,73 +1,73 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Quentin Brateau, Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-import codac as codac
-
-class TestCtcCartProd(unittest.TestCase):
-
-  def test_ctc(self):
-
-    # C1
-    y1 = Interval(0, 1)
-    f1 = Function("x", "sin(x)")
-    C1 = CtcFunction(f1, y1)
-
-    # C2
-    y2 = Interval(0, 1)
-    f2 = Function("x", "sqr(x)")
-    C2 = CtcFunction(f2, y2)
-
-    # CtcCartProd
-    C = CtcCartProd([C1, C2])
-
-    # Expected
-    e1 = IntervalVector([[-5, 1]])
-    e2 = IntervalVector([[-3, 6]])
-    C1.contract(e1)
-    C2.contract(e2)
-
-    # Testing
-    x = IntervalVector([[-5, 1],[-3, 6]])
-    C.contract(x)
-
-    self.assertEqual(x[0], e1[0])
-    self.assertEqual(x[1], e2[0])
-  
-
-  def test_fn_cart_prod(self):
-  
-    # C1
-    y1 = Interval(0, 1)
-    f1 = Function("x", "sin(x)")
-    C1 = CtcFunction(f1, y1)
-
-    # C2
-    y2 = Interval(0, 1)
-    f2 = Function("x", "sqr(x)")
-    C2 = CtcFunction(f2, y2)
-
-    # CtcCartProd 1
-    Cx1 = CtcCartProd([C1, C2])
-    x1 = IntervalVector([[-5, 1],[-3, 6]])
-    Cx1.contract(x1)
-
-    # CtcCartProd 2
-    Cx2 = cart_prod([C1, C2])
-    x2 = IntervalVector([[-5, 1],[-3, 6]])
-    Cx2.contract(x2)
-
-    self.assertEqual(x1[0], x2[0])
-    self.assertEqual(x1[1], x2[1])
-
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Quentin Brateau, Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+import codac as codac
+
+class TestCtcCartProd(unittest.TestCase):
+
+  def test_ctc(self):
+
+    # C1
+    y1 = Interval(0, 1)
+    f1 = Function("x", "sin(x)")
+    C1 = CtcFunction(f1, y1)
+
+    # C2
+    y2 = Interval(0, 1)
+    f2 = Function("x", "sqr(x)")
+    C2 = CtcFunction(f2, y2)
+
+    # CtcCartProd
+    C = CtcCartProd([C1, C2])
+
+    # Expected
+    e1 = IntervalVector([[-5, 1]])
+    e2 = IntervalVector([[-3, 6]])
+    C1.contract(e1)
+    C2.contract(e2)
+
+    # Testing
+    x = IntervalVector([[-5, 1],[-3, 6]])
+    C.contract(x)
+
+    self.assertEqual(x[0], e1[0])
+    self.assertEqual(x[1], e2[0])
+  
+
+  def test_fn_cart_prod(self):
+  
+    # C1
+    y1 = Interval(0, 1)
+    f1 = Function("x", "sin(x)")
+    C1 = CtcFunction(f1, y1)
+
+    # C2
+    y2 = Interval(0, 1)
+    f2 = Function("x", "sqr(x)")
+    C2 = CtcFunction(f2, y2)
+
+    # CtcCartProd 1
+    Cx1 = CtcCartProd([C1, C2])
+    x1 = IntervalVector([[-5, 1],[-3, 6]])
+    Cx1.contract(x1)
+
+    # CtcCartProd 2
+    Cx2 = cart_prod([C1, C2])
+    x2 = IntervalVector([[-5, 1],[-3, 6]])
+    Cx2.contract(x2)
+
+    self.assertEqual(x1[0], x2[0])
+    self.assertEqual(x1[1], x2[1])
+
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_ctcstatic.py

 * *Ordering differences only*

```diff
@@ -1,35 +1,35 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-
-class TestCtcStatic(unittest.TestCase):
-
-    def test_ctcstatic_1(self):
-
-        dt = 0.1
-        tdomain = Interval(0.,10.)
-
-        ctc_f = CtcFunction(Function("t", "x[2]", "(x[0]-t;x[1]-t)"))
-        ctc_static = CtcStatic(ctc_f, True)
-
-        x = TubeVector(tdomain, dt, 2)
-
-        cn = ContractorNetwork()
-        cn.add(ctc_static, [x])
-        cn.contract()
-
-        expected = Tube(tdomain, dt, TFunction("t"))
-        self.assertEqual(x[0], expected)
-        self.assertEqual(x[1], expected)
-
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+
+class TestCtcStatic(unittest.TestCase):
+
+    def test_ctcstatic_1(self):
+
+        dt = 0.1
+        tdomain = Interval(0.,10.)
+
+        ctc_f = CtcFunction(Function("t", "x[2]", "(x[0]-t;x[1]-t)"))
+        ctc_static = CtcStatic(ctc_f, True)
+
+        x = TubeVector(tdomain, dt, 2)
+
+        cn = ContractorNetwork()
+        cn.add(ctc_static, [x])
+        cn.contract()
+
+        expected = Tube(tdomain, dt, TFunction("t"))
+        self.assertEqual(x[0], expected)
+        self.assertEqual(x[1], expected)
+
+if __name__ ==  '__main__':
   unittest.main()
```

## codac/tests/test_definition.py

 * *Ordering differences only*

```diff
@@ -1,349 +1,349 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import os
-from tempfile import gettempdir
-import unittest
-from codac import *
-import codac as codac
-
-class TestSlice(unittest.TestCase):
-
-  def setUp(self):
-    tube = Tube(Interval(0.,46.), 0.1, Interval(10.,11.));
-    self.tube = tube
-
-  def test_Init(self):
-    self.assertTrue(self.tube.volume() == 46)
-    #print(cos(self.tube).codomain())
-    #self.assertTrue(cos(self.tube).codomain() == cos(Interval(10.,11.)))
-
-  def test_Serialize(self):
-    self.tube.serialize(os.path.join(gettempdir(), "x.tube"))
-    
-  def test_Slice_class(self):
-  
-    tubeslice = Slice(Interval(0.,1.), Interval(-1.,1.));
-    self.assertEqual(tubeslice.tdomain(), Interval(0.,1.));
-    self.assertEqual(tubeslice.codomain(), Interval(-1.,1.));
-
-    # tubeslice_copy1 = tubeslice;
-    # self.assertEqual(tubeslice_copy1.tdomain(), Interval(0.,1.));
-    # self.assertEqual(tubeslice_copy1.codomain(), Interval(-1.,1.));
-    # self.assertEqual(tubeslice_copy1, tubeslice);
-
-    # Slice tubeslice_copy2(tubeslice);
-    # self.assertEqual(tubeslice_copy2.tdomain(), Interval(0.,1.));
-    # self.assertEqual(tubeslice_copy2.codomain(), Interval(-1.,1.));
-    # self.assertEqual(tubeslice_copy2, tubeslice);
-
-    # todo: find a way to catch assert abort: CHECK_THROWS(Slice(Interval::ALL_REALS));
-    # todo: find a way to catch assert abort: CHECK_THROWS(Slice(Interval::EMPTY_SET));
-class TestTube(unittest.TestCase):
-
-  def assertApproxIntv(self, first, second):
-    if isinstance(second, Interval):
-      self.assertAlmostEqual(first.lb(), second.lb())
-      self.assertAlmostEqual(first.ub(), second.ub())
-
-  def test_Slice_class(self):
-    tube = Tube (Interval(0.,1.), Interval(-1.,1.));
-    self.assertEqual(tube.tdomain() , Interval(0.,1.));
-    self.assertEqual(tube.codomain() , Interval(-1.,1.));
-
-    tube_copy1 = tube;
-    self.assertEqual(tube_copy1.tdomain() , Interval(0.,1.));
-    self.assertEqual(tube_copy1.codomain() , Interval(-1.,1.));
-    self.assertEqual(tube_copy1 , tube);
-
-  def test_Tube_fct(self):
-    tube_a = Tube(Interval(0.,12.), 1.);
-    self.assertEqual(tube_a.nb_slices(), 12);
-    self.assertEqual(tube_a.tdomain(), Interval(0.,12.));
-
-    tube_b = Tube(Interval(0.,12.), 0.5, Interval(-3.,-2.));
-    self.assertEqual(tube_b.nb_slices(), 24);
-    self.assertEqual(tube_b.tdomain(), Interval(0.,12.));
-    self.assertEqual(tube_b(3), Interval(-3.,-2.));
-    self.assertEqual(tube_b.codomain(), Interval(-3.,-2.));
-
-  def test_Tube_nb_slices(self):
-    tube_a = Tube(Interval(0.,12.), 1.);
-    self.assertEqual(tube_a.nb_slices(), 12);
-    self.assertEqual(tube_a.tdomain(), Interval(0.,12.));
-
-  def test_Tube_nb_slices2(self):
-    tube_b = Tube(Interval(0.,12.), 0.5, Interval(-3.,-2.));
-    self.assertEqual(tube_b.nb_slices(), 24);
-    self.assertEqual(tube_b.tdomain(), Interval(0.,12.));
-    self.assertEqual(tube_b(3), Interval(-3.,-2.));
-    self.assertEqual(tube_b.codomain(), Interval(-3.,-2.));
-
-  def test_Tube_nbslices3(self):
-    tube_c = Tube(Interval(0.,4.), 1.1);
-    self.assertEqual(tube_c.nb_slices(), 4);
-    
-    self.assertApproxIntv(tube_c.slice(0).tdomain(), Interval(0.,1.1));
-    self.assertApproxIntv(tube_c.slice(1).tdomain(), Interval(1.1,2.2));
-    self.assertApproxIntv(tube_c.slice(2).tdomain(), Interval(2.2,3.3));
-    self.assertApproxIntv(tube_c.slice(3).tdomain(), Interval(3.3,4.));
-
-#     Tube tube_d(tube_c);
-#     CHECK(tube_d == tube_c);
-#     CHECK(tube_d.codomain() == tube_c.codomain());
-#     CHECK(tube_d.nb_slices() == tube_c.nb_slices());
-#     //CHECK(tube_d.slice(0)->tube_reference() == &tube_d);
-#     //CHECK(tube_d.slice(0)->tube_reference() == tube_d.slice(1)->tube_reference());
-#     //CHECK(tube_d.slice(1)->tube_reference() == &tube_d);
-#     //CHECK(tube_d.slice(2)->tube_reference() == &tube_d);
-#     //CHECK(tube_d.slice(3)->tube_reference() == &tube_d);
-
-#     Tube tube_e(tube_c, Interval(1.,2.));
-#     //CHECK(tube_e.slice(0)->tube_reference() == &tube_e);
-#     //CHECK(tube_e.slice(1)->tube_reference() == &tube_e);
-#     //CHECK(tube_e.slice(2)->tube_reference() == &tube_e);
-#     //CHECK(tube_e.slice(3)->tube_reference() == &tube_e);
-#     CHECK(tube_e.codomain() == Interval(1.,2.));
-#     CHECK(tube_e.nb_slices() == tube_c.nb_slices());
-#     CHECK(tube_e.slice(0)->codomain() == Interval(1.,2.));
-#     CHECK(tube_e.slice(1)->codomain() == Interval(1.,2.));
-#     CHECK(tube_e.slice(2)->codomain() == Interval(1.,2.));
-#     CHECK(tube_e.slice(3)->codomain() == Interval(1.,2.));
-
-#     // todo: find a way to catch assert abort: CHECK_THROWS(Tube tube_f(Interval(0.,12.), -1.););
-
-#     Tube tube_f(Interval(0.,12.), 0.);
-#     CHECK(tube_f.tdomain() == Interval(0.,12.));
-#     CHECK(tube_f.nb_slices() == 1);
-    
-class TestTubeVector(unittest.TestCase):
-
-  def test_TubeVector(self):
-    # modif Interval -> IntervalVector
-    tube = TubeVector(Interval(0.,1.), IntervalVector(1, [-1.,1.]));
-    self.assertEqual(tube.tdomain(), Interval(0.,1.));
-    self.assertEqual(tube.codomain(), IntervalVector(1, [-1.,1.]));
-
-    tube_copy1 = tube;
-    self.assertEqual(tube_copy1.tdomain(), Interval(0.,1.));
-    self.assertEqual(tube_copy1.codomain(), IntervalVector(1, [-1.,1.]));
-    self.assertEqual(tube_copy1, tube);
-
-
-class TestTubeClassFunction(unittest.TestCase):
-
-  def assertApproxIntv(self, first, second):
-      if first.is_empty() is False:
-      # if isinstance(second, Interval):
-          self.assertAlmostEqual(first.lb(), second.lb())
-          self.assertAlmostEqual(first.ub(), second.ub())
-      else:
-          self.assertEqual(first, second)
-         
-  # def test_1(self):
-  #   f = TFunction("t^2")
-  #   f2 = TFunction("t^2")
-  #   tube1 = Tube(Interval(-1.,10.), 0.01, f);
-  #   f3 = TFunction("t^2+2")
-  #   f4 = TFunction(f2)
-  #   traj1_inside = Trajectory(Interval(-1.,10.), f2);
-  #   print(f4.eval(Interval(-1.,10.)))
-
-  #   traj1_outside = Trajectory(Interval(-1.,10.), f3);
-
-  #   self.assertEqual(tube1.contains(traj1_inside), codac.YES);
-  #   self.assertEqual(tube1.contains(traj1_outside), codac.NO);
-
-  def test_2(self):
-    tube2 = Tube(Interval(-1.,10.), 0.01, TFunction("t^2+[-1,1]"));
-    traj3_lb = Trajectory(Interval(-1.,10.), TFunction("(t^2)-1"));
-    traj3_ub = Trajectory(Interval(-1.,10.), TFunction("(t^2)+1"));
-    tube3 = Tube(traj3_lb, traj3_ub, 0.01);
-    self.assertEqual(tube2.nb_slices(), tube3.nb_slices());
-    self.assertEqual(tube2.tdomain(), tube3.tdomain());
-    self.assertEqual(tube2.codomain(), tube3.codomain());
-    self.assertEqual(tube2.volume(), tube3.volume());
-    for i in range(tube2.nb_slices()):
-      self.assertEqual(tube2(i), tube3(i)); 
-      
-
-  def test_TubeVector_subvector(self):
-    
-    tdomain = Interval(-10, 10)
-    vtube = TubeVector(Interval(-10, 10), 0.1, TFunction("(t+[-1,1]; t^2+[-1,1]; t^3+[-1,1])"))
-    vtube2 = TubeVector(Interval(-10, 10), 0.1, TFunction("(t+[-1,1]; t^2+[-1,1])"))
-    
-    self.assertEqual(vtube[:].size(), 3)
-    self.assertEqual(vtube[:1].size(), 1)
-    self.assertEqual(vtube[:2].size(), 2)
-    self.assertTrue(vtube[:2] == vtube2)    
-
-# class TestTubeClassFunction_thick_slices(unittest.TestCase):
-#   SECTION("Tube class - Function (thick slices)")
-    # def test_3(self):
-    #   tube = Tube(Interval(-1.,1.), 0.667, TFunction("t^2"));
-    #   self.assertEqual(tube.nb_slices(), 3);
-    #   self.assertEqual(ApproxIntv(tube(0)), Interval(pow(-1. + 0.667, 2), 1.));
-    #   self.assertEqual(tube(-1.), Interval(1.));
-    #   self.assertEqual(tube(1.), Interval(1.));
-    #   self.assertEqual(tube(-0.9), tube(0));
-    #   self.assertEqual(ApproxIntv(tube(1)), Interval(0., pow(tube.slice(1).tdomain().ub(), 2)));
-
-#   SECTION("Tube class - 2 Trajectory")
-#   {
-#     Trajectory traj_lb(Interval(-1.,10.), TFunction("t^2"));
-#     Trajectory traj_ub(Interval(-1.,10.), TFunction("t^2-2"));
-    
-#     Tube tube_1slice(traj_lb, traj_ub, traj_lb.tdomain().diam());
-#     CHECK(tube_1slice.nb_slices() == 1);
-#     CHECK(tube_1slice.tdomain() == Interval(-1.,10.));
-#     CHECK(tube_1slice.codomain() == Interval(-2.,100.));
-#     CHECK(Interval(28.25,30.25).is_subset(tube_1slice(5.5)));
-#     CHECK(tube_1slice.max_diam() > 2.);
-    
-#     Tube tube_100slices(traj_lb, traj_ub, traj_ub.tdomain().diam() / 100.);
-#     CHECK(tube_100slices.nb_slices() == 100);
-#     CHECK(tube_100slices.tdomain() == Interval(-1.,10.));
-#     CHECK(tube_100slices.codomain() == Interval(-2.,100.));
-#     CHECK(Interval(28.25,30.25).is_subset(tube_100slices(5.5)));
-#     CHECK(tube_100slices(5.5).is_subset(Interval(28.,32.)));
-#     CHECK(tube_100slices.max_diam() > 2.);
-#   }
-
-
-  def test_TubeClasss(self):
- 
-    box1 = IntervalVector(2) 
-    box2 = IntervalVector(2) 
-    box3 = IntervalVector(2)
-    box4 = IntervalVector(2)
-
-    box1[0] = Interval(-1.,10.);
-    box1[1] = Interval(3.,4.);
-
-    box2[0] = Interval(10.,10.5);
-    box2[1] = Interval(2.,7.);
-
-    box3[0] = Interval(10.5,12.);
-    box3[1] = Interval(5.,6.);
-
-    box4[0] = Interval(12.,14.);
-    box4[1] = Interval(5.5);
-
-    v_tdomains = [box1[0], box2[0], box3[0], box4[0]]
-    v_codomains = [box1[1], box2[1], box3[1], box4[1]]
-    tube_from_boxes = Tube(v_tdomains, v_codomains);
-
-    self.assertEqual(tube_from_boxes.tdomain(), Interval(-1.,14.));
-    self.assertEqual(tube_from_boxes.codomain(), Interval(2.,7.));
-    self.assertEqual(tube_from_boxes.nb_slices(), 4);
-
-    self.assertEqual(tube_from_boxes(0), Interval(3.,4.));
-    self.assertEqual(tube_from_boxes(1), Interval(2.,7.));
-    self.assertEqual(tube_from_boxes(2), Interval(5.,6.));
-    self.assertEqual(tube_from_boxes(3), Interval(5.5));
-
-    self.assertEqual(tube_from_boxes.slice(0).tdomain(), Interval(-1.,10.));
-    self.assertEqual(tube_from_boxes.slice(1).tdomain(), Interval(10.,10.5));
-    self.assertEqual(tube_from_boxes.slice(2).tdomain(), Interval(10.5,12.));
-    self.assertEqual(tube_from_boxes.slice(3).tdomain(), Interval(12.,14.));
-
-
-  def test_Tube_class_vector_of_boxes_n_dim_case(self):
-    box1 = IntervalVector([ 
-        Interval(-1.,10.), 
-        Interval(3.,4.), 
-        Interval(0.,2.) 
-    ])
-    box2 = IntervalVector([
-      Interval(10.,10.5),
-      Interval(2.,7.),
-      Interval(1.,3.)
-    ])
-
-    box3 = IntervalVector([
-      Interval(10.5,12.),
-      Interval(5.,6.),
-      Interval(2.,4.)
-    ])
-
-    box4 = IntervalVector([
-        Interval(12.,14.),
-        Interval(5.5),
-        Interval(3.,5.)
-    ])
-
-    v_tdomains = [ box1[0], box2[0], box3[0], box4[0]]
-    v_codomains = [
-      box1.subvector(1,2), 
-      box2.subvector(1,2), 
-      box3.subvector(1,2), 
-      box4.subvector(1,2)
-    ]
-
-    tube_from_boxes  = TubeVector(v_tdomains, v_codomains)
-
-    self.assertEqual(tube_from_boxes.size(), 2);
-    self.assertEqual(tube_from_boxes.tdomain(), Interval(-1.,14.));
-    self.assertEqual(tube_from_boxes.codomain()[0], Interval(2.,7.));
-    self.assertEqual(tube_from_boxes.codomain()[1], Interval(0.,5.));
-    self.assertEqual(tube_from_boxes.nb_slices(), 4);
-
-    self.assertEqual(tube_from_boxes[0](0), Interval(3.,4.));
-    self.assertEqual(tube_from_boxes[0](1), Interval(2.,7.));
-    self.assertEqual(tube_from_boxes[0](2), Interval(5.,6.));
-    self.assertEqual(tube_from_boxes[0](3), Interval(5.5));
-
-    self.assertEqual(tube_from_boxes[0].slice(0).tdomain(), Interval(-1.,10.));
-    self.assertEqual(tube_from_boxes[0].slice(1).tdomain(), Interval(10.,10.5));
-    self.assertEqual(tube_from_boxes[0].slice(2).tdomain(), Interval(10.5,12.));
-    self.assertEqual(tube_from_boxes[0].slice(3).tdomain(), Interval(12.,14.));
-
-    self.assertEqual(tube_from_boxes[1](0), Interval(0.,2.));
-    self.assertEqual(tube_from_boxes[1](1), Interval(1.,3.));
-    self.assertEqual(tube_from_boxes[1](2), Interval(2.,4.));
-    self.assertEqual(tube_from_boxes[1](3), Interval(3.,5.));
-
-    self.assertEqual(tube_from_boxes[1].slice(0).tdomain(), Interval(-1.,10.));
-    self.assertEqual(tube_from_boxes[1].slice(1).tdomain(), Interval(10.,10.5));
-    self.assertEqual(tube_from_boxes[1].slice(2).tdomain(), Interval(10.5,12.));
-    self.assertEqual(tube_from_boxes[1].slice(3).tdomain(), Interval(12.,14.));
-
-
-  def test_invert_tube(self):
-
-    tdomain = Interval(-5,20)
-    x = Tube(tdomain, 0.05, TFunction("cos(t+1.5)+(t-8)*[-0.10,0.10]"))
-
-    beginDrawing()
-    fig_x = VIBesFigTube("x")
-    fig_x.set_properties(100, 100, 600, 300)
-    fig_x.add_tube(x, "x")
-    fig_x.show(True);
-
-    v_t = []
-    z = Interval(-oo,-0.6)
-    x.invert(z,v_t,tdomain)
-    for ti in v_t:
-      fig_x.draw_box(IntervalVector([ti,x(ti)&z]), "red")
-      print(ti)
-
-    endDrawing()
-
-    self.assertEqual(len(v_t), 5)
-    self.assertApproxIntv(v_t[0], Interval(-5, -2.55))
-    self.assertApproxIntv(v_t[1], Interval(-0.2, 3.15))
-    self.assertApproxIntv(v_t[2], Interval(6.85,9.))
-    self.assertApproxIntv(v_t[3], Interval(12.75, 16))
-    self.assertApproxIntv(v_t[4], Interval(18.45, 20))
-
-if __name__ == '__main__':
-
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import os
+from tempfile import gettempdir
+import unittest
+from codac import *
+import codac as codac
+
+class TestSlice(unittest.TestCase):
+
+  def setUp(self):
+    tube = Tube(Interval(0.,46.), 0.1, Interval(10.,11.));
+    self.tube = tube
+
+  def test_Init(self):
+    self.assertTrue(self.tube.volume() == 46)
+    #print(cos(self.tube).codomain())
+    #self.assertTrue(cos(self.tube).codomain() == cos(Interval(10.,11.)))
+
+  def test_Serialize(self):
+    self.tube.serialize(os.path.join(gettempdir(), "x.tube"))
+    
+  def test_Slice_class(self):
+  
+    tubeslice = Slice(Interval(0.,1.), Interval(-1.,1.));
+    self.assertEqual(tubeslice.tdomain(), Interval(0.,1.));
+    self.assertEqual(tubeslice.codomain(), Interval(-1.,1.));
+
+    # tubeslice_copy1 = tubeslice;
+    # self.assertEqual(tubeslice_copy1.tdomain(), Interval(0.,1.));
+    # self.assertEqual(tubeslice_copy1.codomain(), Interval(-1.,1.));
+    # self.assertEqual(tubeslice_copy1, tubeslice);
+
+    # Slice tubeslice_copy2(tubeslice);
+    # self.assertEqual(tubeslice_copy2.tdomain(), Interval(0.,1.));
+    # self.assertEqual(tubeslice_copy2.codomain(), Interval(-1.,1.));
+    # self.assertEqual(tubeslice_copy2, tubeslice);
+
+    # todo: find a way to catch assert abort: CHECK_THROWS(Slice(Interval::ALL_REALS));
+    # todo: find a way to catch assert abort: CHECK_THROWS(Slice(Interval::EMPTY_SET));
+class TestTube(unittest.TestCase):
+
+  def assertApproxIntv(self, first, second):
+    if isinstance(second, Interval):
+      self.assertAlmostEqual(first.lb(), second.lb())
+      self.assertAlmostEqual(first.ub(), second.ub())
+
+  def test_Slice_class(self):
+    tube = Tube (Interval(0.,1.), Interval(-1.,1.));
+    self.assertEqual(tube.tdomain() , Interval(0.,1.));
+    self.assertEqual(tube.codomain() , Interval(-1.,1.));
+
+    tube_copy1 = tube;
+    self.assertEqual(tube_copy1.tdomain() , Interval(0.,1.));
+    self.assertEqual(tube_copy1.codomain() , Interval(-1.,1.));
+    self.assertEqual(tube_copy1 , tube);
+
+  def test_Tube_fct(self):
+    tube_a = Tube(Interval(0.,12.), 1.);
+    self.assertEqual(tube_a.nb_slices(), 12);
+    self.assertEqual(tube_a.tdomain(), Interval(0.,12.));
+
+    tube_b = Tube(Interval(0.,12.), 0.5, Interval(-3.,-2.));
+    self.assertEqual(tube_b.nb_slices(), 24);
+    self.assertEqual(tube_b.tdomain(), Interval(0.,12.));
+    self.assertEqual(tube_b(3), Interval(-3.,-2.));
+    self.assertEqual(tube_b.codomain(), Interval(-3.,-2.));
+
+  def test_Tube_nb_slices(self):
+    tube_a = Tube(Interval(0.,12.), 1.);
+    self.assertEqual(tube_a.nb_slices(), 12);
+    self.assertEqual(tube_a.tdomain(), Interval(0.,12.));
+
+  def test_Tube_nb_slices2(self):
+    tube_b = Tube(Interval(0.,12.), 0.5, Interval(-3.,-2.));
+    self.assertEqual(tube_b.nb_slices(), 24);
+    self.assertEqual(tube_b.tdomain(), Interval(0.,12.));
+    self.assertEqual(tube_b(3), Interval(-3.,-2.));
+    self.assertEqual(tube_b.codomain(), Interval(-3.,-2.));
+
+  def test_Tube_nbslices3(self):
+    tube_c = Tube(Interval(0.,4.), 1.1);
+    self.assertEqual(tube_c.nb_slices(), 4);
+    
+    self.assertApproxIntv(tube_c.slice(0).tdomain(), Interval(0.,1.1));
+    self.assertApproxIntv(tube_c.slice(1).tdomain(), Interval(1.1,2.2));
+    self.assertApproxIntv(tube_c.slice(2).tdomain(), Interval(2.2,3.3));
+    self.assertApproxIntv(tube_c.slice(3).tdomain(), Interval(3.3,4.));
+
+#     Tube tube_d(tube_c);
+#     CHECK(tube_d == tube_c);
+#     CHECK(tube_d.codomain() == tube_c.codomain());
+#     CHECK(tube_d.nb_slices() == tube_c.nb_slices());
+#     //CHECK(tube_d.slice(0)->tube_reference() == &tube_d);
+#     //CHECK(tube_d.slice(0)->tube_reference() == tube_d.slice(1)->tube_reference());
+#     //CHECK(tube_d.slice(1)->tube_reference() == &tube_d);
+#     //CHECK(tube_d.slice(2)->tube_reference() == &tube_d);
+#     //CHECK(tube_d.slice(3)->tube_reference() == &tube_d);
+
+#     Tube tube_e(tube_c, Interval(1.,2.));
+#     //CHECK(tube_e.slice(0)->tube_reference() == &tube_e);
+#     //CHECK(tube_e.slice(1)->tube_reference() == &tube_e);
+#     //CHECK(tube_e.slice(2)->tube_reference() == &tube_e);
+#     //CHECK(tube_e.slice(3)->tube_reference() == &tube_e);
+#     CHECK(tube_e.codomain() == Interval(1.,2.));
+#     CHECK(tube_e.nb_slices() == tube_c.nb_slices());
+#     CHECK(tube_e.slice(0)->codomain() == Interval(1.,2.));
+#     CHECK(tube_e.slice(1)->codomain() == Interval(1.,2.));
+#     CHECK(tube_e.slice(2)->codomain() == Interval(1.,2.));
+#     CHECK(tube_e.slice(3)->codomain() == Interval(1.,2.));
+
+#     // todo: find a way to catch assert abort: CHECK_THROWS(Tube tube_f(Interval(0.,12.), -1.););
+
+#     Tube tube_f(Interval(0.,12.), 0.);
+#     CHECK(tube_f.tdomain() == Interval(0.,12.));
+#     CHECK(tube_f.nb_slices() == 1);
+    
+class TestTubeVector(unittest.TestCase):
+
+  def test_TubeVector(self):
+    # modif Interval -> IntervalVector
+    tube = TubeVector(Interval(0.,1.), IntervalVector(1, [-1.,1.]));
+    self.assertEqual(tube.tdomain(), Interval(0.,1.));
+    self.assertEqual(tube.codomain(), IntervalVector(1, [-1.,1.]));
+
+    tube_copy1 = tube;
+    self.assertEqual(tube_copy1.tdomain(), Interval(0.,1.));
+    self.assertEqual(tube_copy1.codomain(), IntervalVector(1, [-1.,1.]));
+    self.assertEqual(tube_copy1, tube);
+
+
+class TestTubeClassFunction(unittest.TestCase):
+
+  def assertApproxIntv(self, first, second):
+      if first.is_empty() is False:
+      # if isinstance(second, Interval):
+          self.assertAlmostEqual(first.lb(), second.lb())
+          self.assertAlmostEqual(first.ub(), second.ub())
+      else:
+          self.assertEqual(first, second)
+         
+  # def test_1(self):
+  #   f = TFunction("t^2")
+  #   f2 = TFunction("t^2")
+  #   tube1 = Tube(Interval(-1.,10.), 0.01, f);
+  #   f3 = TFunction("t^2+2")
+  #   f4 = TFunction(f2)
+  #   traj1_inside = Trajectory(Interval(-1.,10.), f2);
+  #   print(f4.eval(Interval(-1.,10.)))
+
+  #   traj1_outside = Trajectory(Interval(-1.,10.), f3);
+
+  #   self.assertEqual(tube1.contains(traj1_inside), codac.YES);
+  #   self.assertEqual(tube1.contains(traj1_outside), codac.NO);
+
+  def test_2(self):
+    tube2 = Tube(Interval(-1.,10.), 0.01, TFunction("t^2+[-1,1]"));
+    traj3_lb = Trajectory(Interval(-1.,10.), TFunction("(t^2)-1"));
+    traj3_ub = Trajectory(Interval(-1.,10.), TFunction("(t^2)+1"));
+    tube3 = Tube(traj3_lb, traj3_ub, 0.01);
+    self.assertEqual(tube2.nb_slices(), tube3.nb_slices());
+    self.assertEqual(tube2.tdomain(), tube3.tdomain());
+    self.assertEqual(tube2.codomain(), tube3.codomain());
+    self.assertEqual(tube2.volume(), tube3.volume());
+    for i in range(tube2.nb_slices()):
+      self.assertEqual(tube2(i), tube3(i)); 
+      
+
+  def test_TubeVector_subvector(self):
+    
+    tdomain = Interval(-10, 10)
+    vtube = TubeVector(Interval(-10, 10), 0.1, TFunction("(t+[-1,1]; t^2+[-1,1]; t^3+[-1,1])"))
+    vtube2 = TubeVector(Interval(-10, 10), 0.1, TFunction("(t+[-1,1]; t^2+[-1,1])"))
+    
+    self.assertEqual(vtube[:].size(), 3)
+    self.assertEqual(vtube[:1].size(), 1)
+    self.assertEqual(vtube[:2].size(), 2)
+    self.assertTrue(vtube[:2] == vtube2)    
+
+# class TestTubeClassFunction_thick_slices(unittest.TestCase):
+#   SECTION("Tube class - Function (thick slices)")
+    # def test_3(self):
+    #   tube = Tube(Interval(-1.,1.), 0.667, TFunction("t^2"));
+    #   self.assertEqual(tube.nb_slices(), 3);
+    #   self.assertEqual(ApproxIntv(tube(0)), Interval(pow(-1. + 0.667, 2), 1.));
+    #   self.assertEqual(tube(-1.), Interval(1.));
+    #   self.assertEqual(tube(1.), Interval(1.));
+    #   self.assertEqual(tube(-0.9), tube(0));
+    #   self.assertEqual(ApproxIntv(tube(1)), Interval(0., pow(tube.slice(1).tdomain().ub(), 2)));
+
+#   SECTION("Tube class - 2 Trajectory")
+#   {
+#     Trajectory traj_lb(Interval(-1.,10.), TFunction("t^2"));
+#     Trajectory traj_ub(Interval(-1.,10.), TFunction("t^2-2"));
+    
+#     Tube tube_1slice(traj_lb, traj_ub, traj_lb.tdomain().diam());
+#     CHECK(tube_1slice.nb_slices() == 1);
+#     CHECK(tube_1slice.tdomain() == Interval(-1.,10.));
+#     CHECK(tube_1slice.codomain() == Interval(-2.,100.));
+#     CHECK(Interval(28.25,30.25).is_subset(tube_1slice(5.5)));
+#     CHECK(tube_1slice.max_diam() > 2.);
+    
+#     Tube tube_100slices(traj_lb, traj_ub, traj_ub.tdomain().diam() / 100.);
+#     CHECK(tube_100slices.nb_slices() == 100);
+#     CHECK(tube_100slices.tdomain() == Interval(-1.,10.));
+#     CHECK(tube_100slices.codomain() == Interval(-2.,100.));
+#     CHECK(Interval(28.25,30.25).is_subset(tube_100slices(5.5)));
+#     CHECK(tube_100slices(5.5).is_subset(Interval(28.,32.)));
+#     CHECK(tube_100slices.max_diam() > 2.);
+#   }
+
+
+  def test_TubeClasss(self):
+ 
+    box1 = IntervalVector(2) 
+    box2 = IntervalVector(2) 
+    box3 = IntervalVector(2)
+    box4 = IntervalVector(2)
+
+    box1[0] = Interval(-1.,10.);
+    box1[1] = Interval(3.,4.);
+
+    box2[0] = Interval(10.,10.5);
+    box2[1] = Interval(2.,7.);
+
+    box3[0] = Interval(10.5,12.);
+    box3[1] = Interval(5.,6.);
+
+    box4[0] = Interval(12.,14.);
+    box4[1] = Interval(5.5);
+
+    v_tdomains = [box1[0], box2[0], box3[0], box4[0]]
+    v_codomains = [box1[1], box2[1], box3[1], box4[1]]
+    tube_from_boxes = Tube(v_tdomains, v_codomains);
+
+    self.assertEqual(tube_from_boxes.tdomain(), Interval(-1.,14.));
+    self.assertEqual(tube_from_boxes.codomain(), Interval(2.,7.));
+    self.assertEqual(tube_from_boxes.nb_slices(), 4);
+
+    self.assertEqual(tube_from_boxes(0), Interval(3.,4.));
+    self.assertEqual(tube_from_boxes(1), Interval(2.,7.));
+    self.assertEqual(tube_from_boxes(2), Interval(5.,6.));
+    self.assertEqual(tube_from_boxes(3), Interval(5.5));
+
+    self.assertEqual(tube_from_boxes.slice(0).tdomain(), Interval(-1.,10.));
+    self.assertEqual(tube_from_boxes.slice(1).tdomain(), Interval(10.,10.5));
+    self.assertEqual(tube_from_boxes.slice(2).tdomain(), Interval(10.5,12.));
+    self.assertEqual(tube_from_boxes.slice(3).tdomain(), Interval(12.,14.));
+
+
+  def test_Tube_class_vector_of_boxes_n_dim_case(self):
+    box1 = IntervalVector([ 
+        Interval(-1.,10.), 
+        Interval(3.,4.), 
+        Interval(0.,2.) 
+    ])
+    box2 = IntervalVector([
+      Interval(10.,10.5),
+      Interval(2.,7.),
+      Interval(1.,3.)
+    ])
+
+    box3 = IntervalVector([
+      Interval(10.5,12.),
+      Interval(5.,6.),
+      Interval(2.,4.)
+    ])
+
+    box4 = IntervalVector([
+        Interval(12.,14.),
+        Interval(5.5),
+        Interval(3.,5.)
+    ])
+
+    v_tdomains = [ box1[0], box2[0], box3[0], box4[0]]
+    v_codomains = [
+      box1.subvector(1,2), 
+      box2.subvector(1,2), 
+      box3.subvector(1,2), 
+      box4.subvector(1,2)
+    ]
+
+    tube_from_boxes  = TubeVector(v_tdomains, v_codomains)
+
+    self.assertEqual(tube_from_boxes.size(), 2);
+    self.assertEqual(tube_from_boxes.tdomain(), Interval(-1.,14.));
+    self.assertEqual(tube_from_boxes.codomain()[0], Interval(2.,7.));
+    self.assertEqual(tube_from_boxes.codomain()[1], Interval(0.,5.));
+    self.assertEqual(tube_from_boxes.nb_slices(), 4);
+
+    self.assertEqual(tube_from_boxes[0](0), Interval(3.,4.));
+    self.assertEqual(tube_from_boxes[0](1), Interval(2.,7.));
+    self.assertEqual(tube_from_boxes[0](2), Interval(5.,6.));
+    self.assertEqual(tube_from_boxes[0](3), Interval(5.5));
+
+    self.assertEqual(tube_from_boxes[0].slice(0).tdomain(), Interval(-1.,10.));
+    self.assertEqual(tube_from_boxes[0].slice(1).tdomain(), Interval(10.,10.5));
+    self.assertEqual(tube_from_boxes[0].slice(2).tdomain(), Interval(10.5,12.));
+    self.assertEqual(tube_from_boxes[0].slice(3).tdomain(), Interval(12.,14.));
+
+    self.assertEqual(tube_from_boxes[1](0), Interval(0.,2.));
+    self.assertEqual(tube_from_boxes[1](1), Interval(1.,3.));
+    self.assertEqual(tube_from_boxes[1](2), Interval(2.,4.));
+    self.assertEqual(tube_from_boxes[1](3), Interval(3.,5.));
+
+    self.assertEqual(tube_from_boxes[1].slice(0).tdomain(), Interval(-1.,10.));
+    self.assertEqual(tube_from_boxes[1].slice(1).tdomain(), Interval(10.,10.5));
+    self.assertEqual(tube_from_boxes[1].slice(2).tdomain(), Interval(10.5,12.));
+    self.assertEqual(tube_from_boxes[1].slice(3).tdomain(), Interval(12.,14.));
+
+
+  def test_invert_tube(self):
+
+    tdomain = Interval(-5,20)
+    x = Tube(tdomain, 0.05, TFunction("cos(t+1.5)+(t-8)*[-0.10,0.10]"))
+
+    beginDrawing()
+    fig_x = VIBesFigTube("x")
+    fig_x.set_properties(100, 100, 600, 300)
+    fig_x.add_tube(x, "x")
+    fig_x.show(True);
+
+    v_t = []
+    z = Interval(-oo,-0.6)
+    x.invert(z,v_t,tdomain)
+    for ti in v_t:
+      fig_x.draw_box(IntervalVector([ti,x(ti)&z]), "red")
+      print(ti)
+
+    endDrawing()
+
+    self.assertEqual(len(v_t), 5)
+    self.assertApproxIntv(v_t[0], Interval(-5, -2.55))
+    self.assertApproxIntv(v_t[1], Interval(-0.2, 3.15))
+    self.assertApproxIntv(v_t[2], Interval(6.85,9.))
+    self.assertApproxIntv(v_t[3], Interval(12.75, 16))
+    self.assertApproxIntv(v_t[4], Interval(18.45, 20))
+
+if __name__ == '__main__':
+
   unittest.main()
```

## codac/tests/test_arithmetic.py

 * *Ordering differences only*

```diff
@@ -1,797 +1,797 @@
-#!/usr/bin/env python
-
-# Codac tests
-# ---------------------------------------------------------------------------
-# \date      2022
-# \author    Simon Rohou
-# \copyright Copyright 2022 Codac Team
-# \license   This program is distributed under the terms of
-#            the GNU Lesser General Public License (LGPL).
-
-import unittest
-from codac import *
-
-class TestArithmeticOnTube(unittest.TestCase):
-
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-    
-    def tests_scalar_tube(self):
-
-        tdomain = Interval(0.,10.)
-        dt = 0.1
-        a, b = Interval(-0.8), Interval(3.)
-
-        x = Tube(tdomain, dt, Interval(a))
-        y = Tube(x)
-        y.set(Interval(b))
-        self.assertEqual(x.codomain(), Interval(a))
-        self.assertEqual(y.codomain(), Interval(b))
-
-        # const Tube cos(const Tube& x)
-        self.assertApproxIntv(cos(x).codomain(), cos(a))
-
-        # const Tube sin(const Tube& x)
-        self.assertApproxIntv(sin(x).codomain(), sin(a))
-
-        # const Tube abs(const Tube& x)
-        # self.assertApproxIntv(abs(x).codomain(), fabs(a))
-
-        # const Tube sqr(const Tube& x)
-        self.assertApproxIntv(sqr(x).codomain(), a**2)
-
-        # const Tube sqrt(const Tube& x)
-        self.assertApproxIntv(sqrt(x).codomain(), Interval.EMPTY_SET)
-        a = Interval(0.2)
-        x.set(a)
-        self.assertApproxIntv(sqrt(x).codomain(), sqrt(a))
-
-        # const Tube exp(const Tube& x)
-        self.assertApproxIntv(exp(x).codomain(), exp(a))
-
-        # const Tube log(const Tube& x)
-        self.assertApproxIntv(log(x).codomain(), log(a))
-
-        # const Tube tan(const Tube& x)
-        self.assertApproxIntv(tan(x).codomain(), tan(a))
-
-        # const Tube acos(const Tube& x)
-        self.assertApproxIntv(acos(x).codomain(), acos(a))
-
-        # const Tube asin(const Tube& x)
-        self.assertApproxIntv(asin(x).codomain(), asin(a))
-
-        # const Tube atan(const Tube& x)
-        self.assertApproxIntv(atan(x).codomain(), atan(a))
-
-        # const Tube cosh(const Tube& x)
-        self.assertApproxIntv(cosh(x).codomain(), cosh(a))
-
-        # const Tube sinh(const Tube& x)
-        self.assertApproxIntv(sinh(x).codomain(), sinh(a))
-
-        # const Tube tanh(const Tube& x)
-        self.assertApproxIntv(tanh(x).codomain(), tanh(a))
-
-        # const Tube acosh(const Tube& x)
-        self.assertApproxIntv(acosh(x).codomain(), acosh(a))
-
-        # const Tube asinh(const Tube& x)
-        self.assertApproxIntv(asinh(x).codomain(), asinh(a))
-
-        # const Tube atanh(const Tube& x)
-        self.assertApproxIntv(atanh(x).codomain(), atanh(a))
-
-        # const Tube atan2(const Tube& y, const Tube& x)
-        self.assertApproxIntv(atan2(y,x).codomain(), atan2(b,a))
-
-        # const Tube atan2(const Tube& y, const ibex.Interval& x)
-        self.assertApproxIntv(atan2(y,Interval(a)).codomain(), atan2(b,a))
-
-        # const Tube atan2(const ibex.Interval& y, const Tube& x)
-        self.assertApproxIntv(atan2(Interval(b),x).codomain(), atan2(b,a))
-
-        # const Tube pow(const Tube& x, int p)
-        self.assertApproxIntv(pow(x,3).codomain(), a**3)
-
-        # const Tube pow(const Tube& x, double p)
-        self.assertApproxIntv(pow(x,7.2).codomain(), a**7.2) #  todo: not working with GAO
-
-        # const Tube pow(const Tube& x, const ibex.Interval& p)
-        self.assertApproxIntv(pow(x,Interval(4.,5.2)).codomain(), a**Interval(4., 5.2))
-
-        # const Tube root(const Tube& x, int p)
-        self.assertApproxIntv(root(x,6).codomain(), root(a,6))
-
-        # const Tube operator+(const Tube& x)
-        # self.assertEqual(+x, x) # not necessary
-        # self.assertEqual((+x).codomain(),  a)
-
-        # const Tube operator+(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x+y).codomain(), a+b)
-
-        # const Tube operator+(const Tube& x, const ibex.Interval& y)
-        self.assertApproxIntv((x+Interval(b)).codomain(), a+b)
-
-        #     # const Tube operator+(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)+y).codomain(), a+b)
-
-        # Trajectory trajx, trajy
-        # trajx.set(a, tdomain.lb()) trajx.set(a, tdomain.mid()) trajx.set(a, tdomain.ub())
-        # trajy.set(b, tdomain.lb()) trajy.set(b, tdomain.mid()) trajy.set(b, tdomain.ub())
-
-        #     //const Tube operator+(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x+trajy).codomain(), a+b)
-        # self.assertApproxIntv((y+trajx).codomain(), a+b)
-
-        #     //const Tube operator+(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajy+x).codomain(), a+b)
-        # self.assertApproxIntv((trajx+y).codomain(), a+b)
-
-        #     //const Tube operator-(const Tube& x)
-        #     CHECK((-x).codomain(, -a)
-
-        #     //const Tube operator-(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x-y).codomain(), a-b)
-
-        #     //const Tube operator-(const Tube& x, const ibex.Interval& y)
-
-        self.assertApproxIntv((x-Interval(b)).codomain(), a-b)
-
-        #     //const Tube operator-(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)-y).codomain(), a-b)
-
-        #     //const Tube operator-(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x-trajy).codomain(), a-b)
-
-        #     //const Tube operator-(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajx-y).codomain(), a-b)
-        # self.assertApproxIntv((trajy-x).codomain(), b-a)
-
-        #     //const Tube operator*(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x*y).codomain(), a*b)
-
-        #     //const Tube operator*(const Tube& x, const ibex.Interval& y)
-        self.assertApproxIntv((x*Interval(b)).codomain(), a*b)
-
-        #     //const Tube operator*(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)*y).codomain(), a*b)
-
-        #     //const Tube operator*(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x*trajy).codomain(), a*b)
-
-        #     //const Tube operator*(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajx*y).codomain(), a*b)
-
-        #     //const Tube operator/(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x/y).codomain(), a/b)
-
-        #     //const Tube operator/(const Tube& x, const ibex.Interval& y)
-        self.assertApproxIntv((x/Interval(b)).codomain(), a/b)
-
-        #     //const Tube operator/(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)/y).codomain(), a/b)
-
-        #     //const Tube operator/(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x/trajy).codomain(), a/b)
-
-        #     //const Tube operator/(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajx/y).codomain(), a/b)
-
-        #     //const Tube operator|(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x|y).codomain(), (a|b))
-
-        #     //const Tube operator|(const Tube& x, const ibex.Interval& y)
-        self.assertApproxIntv((x|Interval(b)).codomain(), (a|b))
-
-        #     //const Tube operator|(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)|y).codomain(), (a|b))
-
-        #     //const Tube operator|(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x|trajy).codomain(), Interval(a,b))
-
-        #     //const Tube operator|(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajx|y).codomain(), Interval(a,b))
-
-        #     x.set(Interval(-10.,10.))
-
-        #     //const Tube operator&(const Tube& x, const Tube& y)
-        self.assertApproxIntv((x&y).codomain(), a&b)
-
-        #     //const Tube operator&(const Tube& x, const ibex.Interval& y)
-        self.assertApproxIntv((x&Interval(b)).codomain(), a&b)
-
-        #     //const Tube operator&(const ibex.Interval& x, const Tube& y)
-        self.assertApproxIntv((Interval(a)&x).codomain(), a)
-
-        #     //const Tube operator&(const Tube& x, const Trajectory& y)
-        # self.assertApproxIntv((x&trajy).codomain(), b)
-
-        #     //const Tube operator&(const Trajectory& x, const Tube& y)
-        # self.assertApproxIntv((trajx&x).codomain(), a)
-
-        x.set(a)
-
-        # const Tube& operator+=(const ibex.Interval& x)
-        z = Tube(x)
-        z += Interval(b)
-
-        self.assertApproxIntv(z.codomain(), a+b)
-
-        # const Tube& operator+=(const Trajectory& x)
-        # z = x z += trajy
-        # self.assertApproxIntv(z.codomain(), a+b)
-
-        # const Tube& operator+=(const Tube& x)
-        z = Tube(x)
-        z += y
-        self.assertApproxIntv(z.codomain(), a+b)
-
-        # const Tube& operator-=(const ibex.Interval& x)
-        z = Tube(x)
-        z -= Interval(b)
-        self.assertApproxIntv(z.codomain(), a-b)
-
-        # const Tube& operator-=(const Trajectory& x)
-        # z = x z -= trajy
-        # self.assertApproxIntv(z.codomain(), a-b)
-
-        # const Tube& operator-=(const Tube& x)
-        z = Tube(x)
-        z -= y
-        self.assertApproxIntv(z.codomain(), a-b)
-
-        # const Tube& operator*=(const ibex.Interval& x)
-        z = Tube(x)
-        z *= Interval(b)
-        self.assertApproxIntv(z.codomain(), a*b)
-
-        # const Tube& operator*=(const Trajectory& x)
-        # z = Tube(x) z *= trajy
-        # self.assertApproxIntv(z.codomain(), a*b)
-
-        # const Tube& operator*=(const Tube& x)
-        z = Tube(x) 
-        z *= y
-        self.assertApproxIntv(z.codomain(), a*b)
-
-        # const Tube& operator/=(const ibex.Interval& x)
-        z = Tube(x) 
-        z /= Interval(b)
-        self.assertApproxIntv(z.codomain(), a/b)
-
-        # const Tube& operator/=(const Trajectory& x)
-        # z = Tube(x) z /= trajy
-        # self.assertApproxIntv(z.codomain(), a/b)
-
-        # const Tube& operator/=(const Tube& x)
-        z = Tube(x) 
-        z /= y
-        self.assertApproxIntv(z.codomain(), a/b)
-
-        # const Tube& operator|=(const ibex.Interval& x)
-        z = Tube(x) 
-        z |= Interval(b)
-        self.assertApproxIntv(z.codomain(), (a|b))
-
-        # const Tube& operator|=(const Trajectory& x)
-        # z = Tube(x) z |= trajy
-        # self.assertApproxIntv(z.codomain(), Interval(a,b))
-
-        # const Tube& operator|=(const Tube& x)
-        z = Tube(x) 
-        z |= y
-        self.assertApproxIntv(z.codomain(), (a|b))
-
-        # const Tube& operator&=(const ibex.Interval& x)
-        z.set(Interval(-10.,10.))
-        z &= Interval(b)
-        self.assertApproxIntv(z.codomain(), b)
-
-        # const Tube& operator&=(const Trajectory& x)
-        # z.set(Interval(-10.,10.)) z &= trajy
-        # self.assertApproxIntv(z.codomain(), b)
-
-        # const Tube& operator&=(const Tube& x)
-        z.set(Interval(-10.,10.))
-        z &= y
-        self.assertApproxIntv(z.codomain(), b)
-
-class TestArithmeticOnVectorTube(unittest.TestCase):
-    
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-
-    def setUp(self):
-        tdomain = Interval(0.,10.)
-        dt = 0.1
-
-        self.x = TubeVector(tdomain, dt, 3)
-        self.y = TubeVector(self.x)
-        self.z = TubeVector(self.x)
-
-        # TrajectoryVector trajx(3), trajy(3)
-        # IntervalVector ix(3), iy(3)
-        self.a0, self.a1, self.a2 = Interval(1.), Interval(2.), Interval(3.)
-        self.b0, self.b1, self.b2 = Interval(0.), Interval(10.), Interval(20.)
-        self.ix = IntervalVector([self.a0, self.a1, self.a2])
-        self.iy = IntervalVector([self.b0, self.b1, self.b2])
-
-        # ix[0] = a0 ix[1] = a1 ix[2] = a2
-        # iy[0] = b0 iy[1] = b1 iy[2] = b2
-
-        self.x.set(self.ix)
-        self.y.set(self.iy)
-
-    # trajx.set(ix.mid(), tdomain.lb()) trajx.set(ix.mid(), tdomain.mid()) trajx.set(ix.mid(), tdomain.ub())
-    # trajy.set(iy.mid(), tdomain.lb()) trajy.set(iy.mid(), tdomain.mid()) trajy.set(iy.mid(), tdomain.ub())
-    def test_vector_size(self):
-        self.assertEqual(self.x.size(), 3)
-        self.assertEqual(self.y.size(), 3) 
-        self.assertEqual(self.z.size(), 3)
-
-
-    def test_VectorTube_operator_add(self):
-
-        # const TubeVector operator+(const TubeVector& x)
-        # z = +self.x
-        # self.assertEqual(self.z[0].codomain(), self.a0)
-        # # self.assertEqual(self.z[1].codomain(), self.a1)
-        # self.assertEqual(self.z[2].codomain(), self.a2) 
-
-        # const TubeVector operator+(const TubeVector& x, const TubeVector& y)
-        z = self.x + self.y
-        self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
-
-        # const TubeVector operator+(const TubeVector& x, const ibex.IntervalVector& y)
-        z = self.x + self.iy
-        self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
-
-        # const TubeVector operator+(const ibex.IntervalVector& x, const TubeVector& y)
-        z = self.ix + self.y
-    
-        self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
-
-        # const TubeVector operator+(const TubeVector& x, const TrajectoryVector& y)
-        # z = x + trajy
-        # CHECK(z[0].codomain() == a0+b0) CHECK(z[1].codomain() == a1+b1) CHECK(z[2].codomain() == a2+b2) 
-
-        # const TubeVector operator+(const TrajectoryVector& x, const TubeVector& y)
-        # z = trajx + y
-        # CHECK(z[0].codomain() == a0+b0) CHECK(z[1].codomain() == a1+b1) CHECK(z[2].codomain() == a2+b2) 
-
-    def test_VectorTube_operator_sub(self):
-
-        # const TubeVector operator-(const TubeVector& x)
-        z = -self.x
-        self.assertEqual(z[0].codomain(), -self.a0)
-        self.assertEqual(z[1].codomain(), -self.a1)
-        self.assertEqual(z[2].codomain(), -self.a2)
-        
-
-        # const TubeVector operator-(const TubeVector& x, const TubeVector& y)
-        z = self.x - self.y
-        self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        # const TubeVector operator-(const TubeVector& x, const ibex.IntervalVector& y)
-        z = self.x - self.iy
-        self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        # const TubeVector operator-(const ibex.IntervalVector& x, const TubeVector& y)
-        z = self.ix - self.y
-        self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        # const TubeVector operator-(const TubeVector& x, const TrajectoryVector& y)
-        # z = x - trajy
-        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        # const TubeVector operator-(const TrajectoryVector& x, const TubeVector& y)
-        # z = trajx - y
-        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-    def test_VectorTube_operator_mul(self):
-
-        # const TubeVector operator*(const Tube& x, const TubeVector& y)
-        # z =  self.y.__rmul__(self.x[1])
-        z =  self.x[1] * self.y
-        self.assertEqual(z[0].codomain(), self.a1*self.b0)
-        self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        self.assertEqual(z[2].codomain(), self.a1*self.b2)
-        
-        # const TubeVector operator*(const ibex.Interval& x, const TubeVector& y)
-        z = Interval(2) * self.y
-        self.assertEqual(z[0].codomain(), 2*self.b0)
-        self.assertEqual(z[1].codomain(), 2*self.b1)
-        self.assertEqual(z[2].codomain(), 2*self.b2)
-        
-
-        # const TubeVector operator*(const Tube& x, const ibex.IntervalVector& y)
-        z = self.x[1] * self.iy
-        self.assertEqual(z[0].codomain(), self.a1*self.b0)
-        self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        self.assertEqual(z[2].codomain(), self.a1*self.b2)
-        
-
-        # const TubeVector operator*(const Trajectory& x, const TubeVector& y)
-        # z = trajx[1] * y
-        # self.assertEqual(z[0].codomain(), self.a1*self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        # self.assertEqual(z[2].codomain(), self.a1*self.b2)
-        
-    def test_VectorTube_operator_truediv(self):
-        # const TubeVector operator/(const TubeVector& x, const Tube& y)
-        z = self.x / self.y[0]
-        self.assertEqual(z[0].codomain(), self.a0/self.b0)
-        self.assertEqual(z[1].codomain(), self.a1/self.b0)
-        self.assertEqual(z[2].codomain(), self.a2/self.b0)
-        
-
-        # const TubeVector operator/(const TubeVector& x, const ibex.Interval& y)
-        z = self.x / self.iy[0]
-        self.assertEqual(z[0].codomain(), self.a0/self.b0)
-        self.assertEqual(z[1].codomain(), self.a1/self.b0)
-        self.assertEqual(z[2].codomain(), self.a2/self.b0)
-        
-
-        # const TubeVector operator/(const ibex.IntervalVector& x, const Tube& y)
-        z = self.ix / self.y[0]
-        self.assertEqual(z[0].codomain(), self.a0/self.b0)
-        self.assertEqual(z[1].codomain(), self.a1/self.b0)
-        self.assertEqual(z[2].codomain(), self.a2/self.b0)
-        
-
-        # const TubeVector operator/(const TubeVector& x, const Trajectory& y)
-        # z = self.x / trajy[0]
-        # self.assertEqual(z[0].codomain(), self.a0/self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1/self.b0)
-        # self.assertEqual(z[2].codomain(), self.a2/self.b0)
-        
-    def test_VectorTube_operator_or(self):
-
-        # const TubeVector operator|(const TubeVector& x, const TubeVector& y)
-        z = self.x | self.y
-        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
-        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
-        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
-        
-
-        # const TubeVector operator|(const TubeVector& x, const ibex.IntervalVector& y)
-        z = self.x | self.iy
-        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
-        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
-        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
-        
-
-        # const TubeVector operator|(const ibex.IntervalVector& x, const TubeVector& y)
-        z = self.ix | self.y
-        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
-        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
-        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
-        
-
-        # const TubeVector operator|(const TubeVector& x, const TrajectoryVector& y)
-        # z = x | trajy
-        # self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
-        # self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
-        # self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
-        
-
-        # const TubeVector operator|(const TrajectoryVector& x, const TubeVector& y)
-        # z = trajx | y
-        # self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
-        # self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
-        # self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
-        
-
-    def test_VectorTube_operator_and(self):
-    
-        self.iy |= IntervalVector(3, Interval(-1))
-        self.y.set(self.iy)
-
-        # const TubeVector operator&(const TubeVector& x, const TubeVector& y)
-        z = self.x & self.y
-        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
-        self.assertEqual(z[1].codomain(), self.a1)
-        self.assertEqual(z[2].codomain(), self.a2)
-        
-
-        # const TubeVector operator&(const TubeVector& x, const ibex.IntervalVector& y)
-        z = self.x & self.iy
-        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
-        self.assertEqual(z[1].codomain(), self.a1)
-        self.assertEqual(z[2].codomain(), self.a2)
-        
-
-        # const TubeVector operator&(const ibex.IntervalVector& x, const TubeVector& y)
-        z = self.ix & self.y
-        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
-        self.assertEqual(z[1].codomain(), self.a1)
-        self.assertEqual(z[2].codomain(), self.a2)
-        
-
-        # const TubeVector operator&(const TubeVector& x, const TrajectoryVector& y)
-        # z = self.y & trajx
-        # self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
-        # self.assertEqual(z[1].codomain(), self.a1)
-        # self.assertEqual(z[2].codomain(), self.a2)
-        
-
-        # //const TubeVector operator&(const TrajectoryVector& x, const TubeVector& y)
-        # z = trajx & self.y
-        # self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
-        # self.assertEqual(z[1].codomain(), self.a1)
-        # self.assertEqual(z[2].codomain(), self.a2)
-
-class TestArithmeticOnVectorTubeIops(unittest.TestCase):
-  
-    def assertApproxIntv(self, first, second):
-        if first.is_empty() is False:
-        # if isinstance(second, Interval):
-            self.assertAlmostEqual(first.lb(), second.lb())
-            self.assertAlmostEqual(first.ub(), second.ub())
-        else:
-            self.assertEqual(first, second)
-
-    def setUp(self):
-        tdomain = Interval(0.,10.)
-        dt = 0.1
-
-        self.x = TubeVector(tdomain, dt, 3)
-        self.y = TubeVector(self.x)
-        self.z = TubeVector(self.x)
-
-        # TrajectoryVector trajx(3), trajy(3)
-        # IntervalVector ix(3), iy(3)
-        self.a0, self.a1, self.a2 = Interval(1.), Interval(2.), Interval(3.)
-        self.b0, self.b1, self.b2 = Interval(0.), Interval(10.), Interval(20.)
-        self.ix = IntervalVector([self.a0, self.a1, self.a2])
-        self.iy = IntervalVector([self.b0, self.b1, self.b2])
-
-        # ix[0] = a0 ix[1] = a1 ix[2] = a2
-        # iy[0] = b0 iy[1] = b1 iy[2] = b2
-
-        self.x.set(self.ix)
-        self.y.set(self.iy)
-        self.iy[0] = self.b0
-        self.iy[1] = self.b1
-        self.iy[2] = self.b2
-        self.y.set(self.iy)
-
-    def test_VectorTube_operator_iadd(self):
-
-
-        #const TubeVector& operator+=(const ibex.Interval& self.x)
-        z = TubeVector(self.x)
-        z+=self.iy[1]
-        self.assertEqual(z[0].codomain(), self.a0+self.b1)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b1)
-        
-
-        #const TubeVector& operator+=(const Trajectory& self.x)
-        # z = TubeVector(self.x)
-        # z+=trajy[1]
-        # self.assertEqual(z[0].codomain(), self.a0+self.b1)
-        # self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2+self.b1)
-        
-
-        #const TubeVector& operator+=(const Tube& self.x)
-        z = TubeVector(self.x)
-        z+=self.y[1]
-        self.assertEqual(z[0].codomain(), self.a0+self.b1)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b1)
-        
-
-        #const TubeVector& operator+=(const ibex.IntervalVector& self.x)
-        z = TubeVector(self.x)
-        z+=self.iy
-        self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b2)
-        
-
-        #const TubeVector& operator+=(const TrajectoryVector& self.x)
-        # z = TubeVector(self.x)
-        # z+=trajy
-        # self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2+self.b2)
-        
-
-        #const TubeVector& operator+=(const TubeVector& self.x)
-        z = TubeVector(self.x)
-        z+=self.y
-        self.assertEqual(z[0].codomain(), self.a0+self.b0)
-        self.assertEqual(z[1].codomain(), self.a1+self.b1)
-        self.assertEqual(z[2].codomain(), self.a2+self.b2)
-        
-
-    def test_VectorTube_operator_isub(self):
-
-        #const TubeVector& operator-=(const ibex.Interval& self.x)
-        z = TubeVector(self.x)
-        z-=self.iy[1]
-        self.assertEqual(z[0].codomain(), self.a0-self.b1)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b1)
-        
-
-        #const TubeVector& operator-=(const Trajectory& self.x)
-        # z = TubeVector(self.x)
-        # z-=trajy[1]
-        # self.assertEqual(z[0].codomain(), self.a0-self.b1)
-        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2-self.b1)
-        
-
-        #const TubeVector& operator-=(const Tube& self.x)
-        z = TubeVector(self.x)
-        z-=self.y[1]
-        self.assertEqual(z[0].codomain(), self.a0-self.b1)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b1)
-        
-
-        #const TubeVector& operator-=(const ibex.IntervalVector& self.x)
-        z = TubeVector(self.x)
-        z-=self.iy
-        self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        #const TubeVector& operator-=(const TrajectoryVector& self.x)
-        # z = TubeVector(self.x)
-        # z-=trajy
-        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-        #const TubeVector& operator-=(const TubeVector& self.x)
-        z = TubeVector(self.x)
-        z-=self.y
-        self.assertEqual(z[0].codomain(), self.a0-self.b0)
-        self.assertEqual(z[1].codomain(), self.a1-self.b1)
-        self.assertEqual(z[2].codomain(), self.a2-self.b2)
-        
-
-    def test_VectorTube_operator_imul(self):
-
-        #const TubeVector& operator*=(const ibex.Interval& self.x)
-        z = TubeVector(self.x)
-        z*=self.iy[1]
-        self.assertEqual(z[0].codomain(), self.a0*self.b1)
-        self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        self.assertEqual(z[2].codomain(), self.a2*self.b1)
-        
-
-        #const TubeVector& operator*=(const Trajectory& self.x)
-        # z = TubeVector(self.x)
-        # z*=trajy[1]
-        # self.assertEqual(z[0].codomain(), self.a0*self.b1)
-        # self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        # self.assertEqual(z[2].codomain(), self.a2*self.b1)
-        
-
-        #const TubeVector& operator*=(const Tube& self.x)
-        z = TubeVector(self.x)
-        z*=self.y[1]
-        self.assertEqual(z[0].codomain(), self.a0*self.b1)
-        self.assertEqual(z[1].codomain(), self.a1*self.b1)
-        self.assertEqual(z[2].codomain(), self.a2*self.b1)
-        
-
-    def test_VectorTube_operator_itrudiv(self):
-
-        #const TubeVector& operator/=(const ibex.Interval& self.x)
-        z = TubeVector(self.x)
-        z/=self.iy[1]
-        self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
-        self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
-        self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
-        
-
-        #const TubeVector& operator/=(const Trajectory& self.x)
-        # z = TubeVector(self.x)
-        # z/=trajy[1]
-        # self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
-        # self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
-        # self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
-        
-
-        #const TubeVector& operator/=(const Tube& self.x)
-        z = TubeVector(self.x)
-        z/=self.y[1]
-        self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
-        self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
-        self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
-        
-
-    def test_VectorTube_operator_ior(self):
-
-        #const TubeVector& operator|=(const ibex.IntervalVector& self.x)
-        z = TubeVector(self.x)
-        z|=self.iy
-        self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
-        self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
-        self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
-        
-
-        #const TubeVector& operator|=(const TrajectoryVector& self.x)
-        # z = TubeVector(self.x)
-        # z|=trajy
-        # self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
-        # self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
-        # self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
-        
-
-        #const TubeVector& operator|=(const TubeVector& self.x)
-        z = TubeVector(self.x)
-        z|=self.y
-        self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
-        self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
-        self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
-        
-
-    def test_VectorTube_operator_iand(self):
-        self.iy |= IntervalVector(3, Interval(-1))
-        self.y.set(self.iy)
-
-        #const TubeVector& operator&=(const ibex.IntervalVector& self.x)
-        z = TubeVector(self.x)
-        z&=self.iy
-        self.assertApproxIntv(z[0].codomain(), Interval.EMPTY_SET)
-        self.assertApproxIntv(z[1].codomain(), self.a1)
-        self.assertApproxIntv(z[2].codomain(), self.a2)
-        
-
-        #const TubeVector& operator&=(const TrajectoryVector& self.x)
-        # z = TubeVector(self.x)
-        # self.y&=trajx
-        # self.assertApproxIntv(z[0].codomain(), self.a0)
-        # self.assertApproxIntv(z[1].codomain(), self.a1)
-        # self.assertApproxIntv(z[2].codomain(), self.a2)
-        
-
-        #const TubeVector& operator&=(const TubeVector& self.x)
-        z = TubeVector(self.x)
-        z&=self.y
-        self.assertApproxIntv(z[0].codomain(), Interval.EMPTY_SET)
-        self.assertApproxIntv(z[1].codomain(), self.a1)
-        self.assertApproxIntv(z[2].codomain(), self.a2)
-        
-if __name__ ==  '__main__':
+#!/usr/bin/env python
+
+# Codac tests
+# ---------------------------------------------------------------------------
+# \date      2022
+# \author    Simon Rohou
+# \copyright Copyright 2022 Codac Team
+# \license   This program is distributed under the terms of
+#            the GNU Lesser General Public License (LGPL).
+
+import unittest
+from codac import *
+
+class TestArithmeticOnTube(unittest.TestCase):
+
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+    
+    def tests_scalar_tube(self):
+
+        tdomain = Interval(0.,10.)
+        dt = 0.1
+        a, b = Interval(-0.8), Interval(3.)
+
+        x = Tube(tdomain, dt, Interval(a))
+        y = Tube(x)
+        y.set(Interval(b))
+        self.assertEqual(x.codomain(), Interval(a))
+        self.assertEqual(y.codomain(), Interval(b))
+
+        # const Tube cos(const Tube& x)
+        self.assertApproxIntv(cos(x).codomain(), cos(a))
+
+        # const Tube sin(const Tube& x)
+        self.assertApproxIntv(sin(x).codomain(), sin(a))
+
+        # const Tube abs(const Tube& x)
+        # self.assertApproxIntv(abs(x).codomain(), fabs(a))
+
+        # const Tube sqr(const Tube& x)
+        self.assertApproxIntv(sqr(x).codomain(), a**2)
+
+        # const Tube sqrt(const Tube& x)
+        self.assertApproxIntv(sqrt(x).codomain(), Interval.EMPTY_SET)
+        a = Interval(0.2)
+        x.set(a)
+        self.assertApproxIntv(sqrt(x).codomain(), sqrt(a))
+
+        # const Tube exp(const Tube& x)
+        self.assertApproxIntv(exp(x).codomain(), exp(a))
+
+        # const Tube log(const Tube& x)
+        self.assertApproxIntv(log(x).codomain(), log(a))
+
+        # const Tube tan(const Tube& x)
+        self.assertApproxIntv(tan(x).codomain(), tan(a))
+
+        # const Tube acos(const Tube& x)
+        self.assertApproxIntv(acos(x).codomain(), acos(a))
+
+        # const Tube asin(const Tube& x)
+        self.assertApproxIntv(asin(x).codomain(), asin(a))
+
+        # const Tube atan(const Tube& x)
+        self.assertApproxIntv(atan(x).codomain(), atan(a))
+
+        # const Tube cosh(const Tube& x)
+        self.assertApproxIntv(cosh(x).codomain(), cosh(a))
+
+        # const Tube sinh(const Tube& x)
+        self.assertApproxIntv(sinh(x).codomain(), sinh(a))
+
+        # const Tube tanh(const Tube& x)
+        self.assertApproxIntv(tanh(x).codomain(), tanh(a))
+
+        # const Tube acosh(const Tube& x)
+        self.assertApproxIntv(acosh(x).codomain(), acosh(a))
+
+        # const Tube asinh(const Tube& x)
+        self.assertApproxIntv(asinh(x).codomain(), asinh(a))
+
+        # const Tube atanh(const Tube& x)
+        self.assertApproxIntv(atanh(x).codomain(), atanh(a))
+
+        # const Tube atan2(const Tube& y, const Tube& x)
+        self.assertApproxIntv(atan2(y,x).codomain(), atan2(b,a))
+
+        # const Tube atan2(const Tube& y, const ibex.Interval& x)
+        self.assertApproxIntv(atan2(y,Interval(a)).codomain(), atan2(b,a))
+
+        # const Tube atan2(const ibex.Interval& y, const Tube& x)
+        self.assertApproxIntv(atan2(Interval(b),x).codomain(), atan2(b,a))
+
+        # const Tube pow(const Tube& x, int p)
+        self.assertApproxIntv(pow(x,3).codomain(), a**3)
+
+        # const Tube pow(const Tube& x, double p)
+        self.assertApproxIntv(pow(x,7.2).codomain(), a**7.2) #  todo: not working with GAO
+
+        # const Tube pow(const Tube& x, const ibex.Interval& p)
+        self.assertApproxIntv(pow(x,Interval(4.,5.2)).codomain(), a**Interval(4., 5.2))
+
+        # const Tube root(const Tube& x, int p)
+        self.assertApproxIntv(root(x,6).codomain(), root(a,6))
+
+        # const Tube operator+(const Tube& x)
+        # self.assertEqual(+x, x) # not necessary
+        # self.assertEqual((+x).codomain(),  a)
+
+        # const Tube operator+(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x+y).codomain(), a+b)
+
+        # const Tube operator+(const Tube& x, const ibex.Interval& y)
+        self.assertApproxIntv((x+Interval(b)).codomain(), a+b)
+
+        #     # const Tube operator+(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)+y).codomain(), a+b)
+
+        # Trajectory trajx, trajy
+        # trajx.set(a, tdomain.lb()) trajx.set(a, tdomain.mid()) trajx.set(a, tdomain.ub())
+        # trajy.set(b, tdomain.lb()) trajy.set(b, tdomain.mid()) trajy.set(b, tdomain.ub())
+
+        #     //const Tube operator+(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x+trajy).codomain(), a+b)
+        # self.assertApproxIntv((y+trajx).codomain(), a+b)
+
+        #     //const Tube operator+(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajy+x).codomain(), a+b)
+        # self.assertApproxIntv((trajx+y).codomain(), a+b)
+
+        #     //const Tube operator-(const Tube& x)
+        #     CHECK((-x).codomain(, -a)
+
+        #     //const Tube operator-(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x-y).codomain(), a-b)
+
+        #     //const Tube operator-(const Tube& x, const ibex.Interval& y)
+
+        self.assertApproxIntv((x-Interval(b)).codomain(), a-b)
+
+        #     //const Tube operator-(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)-y).codomain(), a-b)
+
+        #     //const Tube operator-(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x-trajy).codomain(), a-b)
+
+        #     //const Tube operator-(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajx-y).codomain(), a-b)
+        # self.assertApproxIntv((trajy-x).codomain(), b-a)
+
+        #     //const Tube operator*(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x*y).codomain(), a*b)
+
+        #     //const Tube operator*(const Tube& x, const ibex.Interval& y)
+        self.assertApproxIntv((x*Interval(b)).codomain(), a*b)
+
+        #     //const Tube operator*(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)*y).codomain(), a*b)
+
+        #     //const Tube operator*(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x*trajy).codomain(), a*b)
+
+        #     //const Tube operator*(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajx*y).codomain(), a*b)
+
+        #     //const Tube operator/(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x/y).codomain(), a/b)
+
+        #     //const Tube operator/(const Tube& x, const ibex.Interval& y)
+        self.assertApproxIntv((x/Interval(b)).codomain(), a/b)
+
+        #     //const Tube operator/(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)/y).codomain(), a/b)
+
+        #     //const Tube operator/(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x/trajy).codomain(), a/b)
+
+        #     //const Tube operator/(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajx/y).codomain(), a/b)
+
+        #     //const Tube operator|(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x|y).codomain(), (a|b))
+
+        #     //const Tube operator|(const Tube& x, const ibex.Interval& y)
+        self.assertApproxIntv((x|Interval(b)).codomain(), (a|b))
+
+        #     //const Tube operator|(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)|y).codomain(), (a|b))
+
+        #     //const Tube operator|(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x|trajy).codomain(), Interval(a,b))
+
+        #     //const Tube operator|(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajx|y).codomain(), Interval(a,b))
+
+        #     x.set(Interval(-10.,10.))
+
+        #     //const Tube operator&(const Tube& x, const Tube& y)
+        self.assertApproxIntv((x&y).codomain(), a&b)
+
+        #     //const Tube operator&(const Tube& x, const ibex.Interval& y)
+        self.assertApproxIntv((x&Interval(b)).codomain(), a&b)
+
+        #     //const Tube operator&(const ibex.Interval& x, const Tube& y)
+        self.assertApproxIntv((Interval(a)&x).codomain(), a)
+
+        #     //const Tube operator&(const Tube& x, const Trajectory& y)
+        # self.assertApproxIntv((x&trajy).codomain(), b)
+
+        #     //const Tube operator&(const Trajectory& x, const Tube& y)
+        # self.assertApproxIntv((trajx&x).codomain(), a)
+
+        x.set(a)
+
+        # const Tube& operator+=(const ibex.Interval& x)
+        z = Tube(x)
+        z += Interval(b)
+
+        self.assertApproxIntv(z.codomain(), a+b)
+
+        # const Tube& operator+=(const Trajectory& x)
+        # z = x z += trajy
+        # self.assertApproxIntv(z.codomain(), a+b)
+
+        # const Tube& operator+=(const Tube& x)
+        z = Tube(x)
+        z += y
+        self.assertApproxIntv(z.codomain(), a+b)
+
+        # const Tube& operator-=(const ibex.Interval& x)
+        z = Tube(x)
+        z -= Interval(b)
+        self.assertApproxIntv(z.codomain(), a-b)
+
+        # const Tube& operator-=(const Trajectory& x)
+        # z = x z -= trajy
+        # self.assertApproxIntv(z.codomain(), a-b)
+
+        # const Tube& operator-=(const Tube& x)
+        z = Tube(x)
+        z -= y
+        self.assertApproxIntv(z.codomain(), a-b)
+
+        # const Tube& operator*=(const ibex.Interval& x)
+        z = Tube(x)
+        z *= Interval(b)
+        self.assertApproxIntv(z.codomain(), a*b)
+
+        # const Tube& operator*=(const Trajectory& x)
+        # z = Tube(x) z *= trajy
+        # self.assertApproxIntv(z.codomain(), a*b)
+
+        # const Tube& operator*=(const Tube& x)
+        z = Tube(x) 
+        z *= y
+        self.assertApproxIntv(z.codomain(), a*b)
+
+        # const Tube& operator/=(const ibex.Interval& x)
+        z = Tube(x) 
+        z /= Interval(b)
+        self.assertApproxIntv(z.codomain(), a/b)
+
+        # const Tube& operator/=(const Trajectory& x)
+        # z = Tube(x) z /= trajy
+        # self.assertApproxIntv(z.codomain(), a/b)
+
+        # const Tube& operator/=(const Tube& x)
+        z = Tube(x) 
+        z /= y
+        self.assertApproxIntv(z.codomain(), a/b)
+
+        # const Tube& operator|=(const ibex.Interval& x)
+        z = Tube(x) 
+        z |= Interval(b)
+        self.assertApproxIntv(z.codomain(), (a|b))
+
+        # const Tube& operator|=(const Trajectory& x)
+        # z = Tube(x) z |= trajy
+        # self.assertApproxIntv(z.codomain(), Interval(a,b))
+
+        # const Tube& operator|=(const Tube& x)
+        z = Tube(x) 
+        z |= y
+        self.assertApproxIntv(z.codomain(), (a|b))
+
+        # const Tube& operator&=(const ibex.Interval& x)
+        z.set(Interval(-10.,10.))
+        z &= Interval(b)
+        self.assertApproxIntv(z.codomain(), b)
+
+        # const Tube& operator&=(const Trajectory& x)
+        # z.set(Interval(-10.,10.)) z &= trajy
+        # self.assertApproxIntv(z.codomain(), b)
+
+        # const Tube& operator&=(const Tube& x)
+        z.set(Interval(-10.,10.))
+        z &= y
+        self.assertApproxIntv(z.codomain(), b)
+
+class TestArithmeticOnVectorTube(unittest.TestCase):
+    
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+
+    def setUp(self):
+        tdomain = Interval(0.,10.)
+        dt = 0.1
+
+        self.x = TubeVector(tdomain, dt, 3)
+        self.y = TubeVector(self.x)
+        self.z = TubeVector(self.x)
+
+        # TrajectoryVector trajx(3), trajy(3)
+        # IntervalVector ix(3), iy(3)
+        self.a0, self.a1, self.a2 = Interval(1.), Interval(2.), Interval(3.)
+        self.b0, self.b1, self.b2 = Interval(0.), Interval(10.), Interval(20.)
+        self.ix = IntervalVector([self.a0, self.a1, self.a2])
+        self.iy = IntervalVector([self.b0, self.b1, self.b2])
+
+        # ix[0] = a0 ix[1] = a1 ix[2] = a2
+        # iy[0] = b0 iy[1] = b1 iy[2] = b2
+
+        self.x.set(self.ix)
+        self.y.set(self.iy)
+
+    # trajx.set(ix.mid(), tdomain.lb()) trajx.set(ix.mid(), tdomain.mid()) trajx.set(ix.mid(), tdomain.ub())
+    # trajy.set(iy.mid(), tdomain.lb()) trajy.set(iy.mid(), tdomain.mid()) trajy.set(iy.mid(), tdomain.ub())
+    def test_vector_size(self):
+        self.assertEqual(self.x.size(), 3)
+        self.assertEqual(self.y.size(), 3) 
+        self.assertEqual(self.z.size(), 3)
+
+
+    def test_VectorTube_operator_add(self):
+
+        # const TubeVector operator+(const TubeVector& x)
+        # z = +self.x
+        # self.assertEqual(self.z[0].codomain(), self.a0)
+        # # self.assertEqual(self.z[1].codomain(), self.a1)
+        # self.assertEqual(self.z[2].codomain(), self.a2) 
+
+        # const TubeVector operator+(const TubeVector& x, const TubeVector& y)
+        z = self.x + self.y
+        self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
+
+        # const TubeVector operator+(const TubeVector& x, const ibex.IntervalVector& y)
+        z = self.x + self.iy
+        self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
+
+        # const TubeVector operator+(const ibex.IntervalVector& x, const TubeVector& y)
+        z = self.ix + self.y
+    
+        self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b2) 
+
+        # const TubeVector operator+(const TubeVector& x, const TrajectoryVector& y)
+        # z = x + trajy
+        # CHECK(z[0].codomain() == a0+b0) CHECK(z[1].codomain() == a1+b1) CHECK(z[2].codomain() == a2+b2) 
+
+        # const TubeVector operator+(const TrajectoryVector& x, const TubeVector& y)
+        # z = trajx + y
+        # CHECK(z[0].codomain() == a0+b0) CHECK(z[1].codomain() == a1+b1) CHECK(z[2].codomain() == a2+b2) 
+
+    def test_VectorTube_operator_sub(self):
+
+        # const TubeVector operator-(const TubeVector& x)
+        z = -self.x
+        self.assertEqual(z[0].codomain(), -self.a0)
+        self.assertEqual(z[1].codomain(), -self.a1)
+        self.assertEqual(z[2].codomain(), -self.a2)
+        
+
+        # const TubeVector operator-(const TubeVector& x, const TubeVector& y)
+        z = self.x - self.y
+        self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        # const TubeVector operator-(const TubeVector& x, const ibex.IntervalVector& y)
+        z = self.x - self.iy
+        self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        # const TubeVector operator-(const ibex.IntervalVector& x, const TubeVector& y)
+        z = self.ix - self.y
+        self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        # const TubeVector operator-(const TubeVector& x, const TrajectoryVector& y)
+        # z = x - trajy
+        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        # const TubeVector operator-(const TrajectoryVector& x, const TubeVector& y)
+        # z = trajx - y
+        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+    def test_VectorTube_operator_mul(self):
+
+        # const TubeVector operator*(const Tube& x, const TubeVector& y)
+        # z =  self.y.__rmul__(self.x[1])
+        z =  self.x[1] * self.y
+        self.assertEqual(z[0].codomain(), self.a1*self.b0)
+        self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        self.assertEqual(z[2].codomain(), self.a1*self.b2)
+        
+        # const TubeVector operator*(const ibex.Interval& x, const TubeVector& y)
+        z = Interval(2) * self.y
+        self.assertEqual(z[0].codomain(), 2*self.b0)
+        self.assertEqual(z[1].codomain(), 2*self.b1)
+        self.assertEqual(z[2].codomain(), 2*self.b2)
+        
+
+        # const TubeVector operator*(const Tube& x, const ibex.IntervalVector& y)
+        z = self.x[1] * self.iy
+        self.assertEqual(z[0].codomain(), self.a1*self.b0)
+        self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        self.assertEqual(z[2].codomain(), self.a1*self.b2)
+        
+
+        # const TubeVector operator*(const Trajectory& x, const TubeVector& y)
+        # z = trajx[1] * y
+        # self.assertEqual(z[0].codomain(), self.a1*self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        # self.assertEqual(z[2].codomain(), self.a1*self.b2)
+        
+    def test_VectorTube_operator_truediv(self):
+        # const TubeVector operator/(const TubeVector& x, const Tube& y)
+        z = self.x / self.y[0]
+        self.assertEqual(z[0].codomain(), self.a0/self.b0)
+        self.assertEqual(z[1].codomain(), self.a1/self.b0)
+        self.assertEqual(z[2].codomain(), self.a2/self.b0)
+        
+
+        # const TubeVector operator/(const TubeVector& x, const ibex.Interval& y)
+        z = self.x / self.iy[0]
+        self.assertEqual(z[0].codomain(), self.a0/self.b0)
+        self.assertEqual(z[1].codomain(), self.a1/self.b0)
+        self.assertEqual(z[2].codomain(), self.a2/self.b0)
+        
+
+        # const TubeVector operator/(const ibex.IntervalVector& x, const Tube& y)
+        z = self.ix / self.y[0]
+        self.assertEqual(z[0].codomain(), self.a0/self.b0)
+        self.assertEqual(z[1].codomain(), self.a1/self.b0)
+        self.assertEqual(z[2].codomain(), self.a2/self.b0)
+        
+
+        # const TubeVector operator/(const TubeVector& x, const Trajectory& y)
+        # z = self.x / trajy[0]
+        # self.assertEqual(z[0].codomain(), self.a0/self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1/self.b0)
+        # self.assertEqual(z[2].codomain(), self.a2/self.b0)
+        
+    def test_VectorTube_operator_or(self):
+
+        # const TubeVector operator|(const TubeVector& x, const TubeVector& y)
+        z = self.x | self.y
+        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
+        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
+        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
+        
+
+        # const TubeVector operator|(const TubeVector& x, const ibex.IntervalVector& y)
+        z = self.x | self.iy
+        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
+        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
+        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
+        
+
+        # const TubeVector operator|(const ibex.IntervalVector& x, const TubeVector& y)
+        z = self.ix | self.y
+        self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
+        self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
+        self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
+        
+
+        # const TubeVector operator|(const TubeVector& x, const TrajectoryVector& y)
+        # z = x | trajy
+        # self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
+        # self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
+        # self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
+        
+
+        # const TubeVector operator|(const TrajectoryVector& x, const TubeVector& y)
+        # z = trajx | y
+        # self.assertEqual(z[0].codomain(), (Interval(self.a0) | self.b0))
+        # self.assertEqual(z[1].codomain(), (Interval(self.a1) | self.b1))
+        # self.assertEqual(z[2].codomain(), (Interval(self.a2) | self.b2))
+        
+
+    def test_VectorTube_operator_and(self):
+    
+        self.iy |= IntervalVector(3, Interval(-1))
+        self.y.set(self.iy)
+
+        # const TubeVector operator&(const TubeVector& x, const TubeVector& y)
+        z = self.x & self.y
+        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
+        self.assertEqual(z[1].codomain(), self.a1)
+        self.assertEqual(z[2].codomain(), self.a2)
+        
+
+        # const TubeVector operator&(const TubeVector& x, const ibex.IntervalVector& y)
+        z = self.x & self.iy
+        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
+        self.assertEqual(z[1].codomain(), self.a1)
+        self.assertEqual(z[2].codomain(), self.a2)
+        
+
+        # const TubeVector operator&(const ibex.IntervalVector& x, const TubeVector& y)
+        z = self.ix & self.y
+        self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
+        self.assertEqual(z[1].codomain(), self.a1)
+        self.assertEqual(z[2].codomain(), self.a2)
+        
+
+        # const TubeVector operator&(const TubeVector& x, const TrajectoryVector& y)
+        # z = self.y & trajx
+        # self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
+        # self.assertEqual(z[1].codomain(), self.a1)
+        # self.assertEqual(z[2].codomain(), self.a2)
+        
+
+        # //const TubeVector operator&(const TrajectoryVector& x, const TubeVector& y)
+        # z = trajx & self.y
+        # self.assertEqual(z[0].codomain(), Interval.EMPTY_SET)
+        # self.assertEqual(z[1].codomain(), self.a1)
+        # self.assertEqual(z[2].codomain(), self.a2)
+
+class TestArithmeticOnVectorTubeIops(unittest.TestCase):
+  
+    def assertApproxIntv(self, first, second):
+        if first.is_empty() is False:
+        # if isinstance(second, Interval):
+            self.assertAlmostEqual(first.lb(), second.lb())
+            self.assertAlmostEqual(first.ub(), second.ub())
+        else:
+            self.assertEqual(first, second)
+
+    def setUp(self):
+        tdomain = Interval(0.,10.)
+        dt = 0.1
+
+        self.x = TubeVector(tdomain, dt, 3)
+        self.y = TubeVector(self.x)
+        self.z = TubeVector(self.x)
+
+        # TrajectoryVector trajx(3), trajy(3)
+        # IntervalVector ix(3), iy(3)
+        self.a0, self.a1, self.a2 = Interval(1.), Interval(2.), Interval(3.)
+        self.b0, self.b1, self.b2 = Interval(0.), Interval(10.), Interval(20.)
+        self.ix = IntervalVector([self.a0, self.a1, self.a2])
+        self.iy = IntervalVector([self.b0, self.b1, self.b2])
+
+        # ix[0] = a0 ix[1] = a1 ix[2] = a2
+        # iy[0] = b0 iy[1] = b1 iy[2] = b2
+
+        self.x.set(self.ix)
+        self.y.set(self.iy)
+        self.iy[0] = self.b0
+        self.iy[1] = self.b1
+        self.iy[2] = self.b2
+        self.y.set(self.iy)
+
+    def test_VectorTube_operator_iadd(self):
+
+
+        #const TubeVector& operator+=(const ibex.Interval& self.x)
+        z = TubeVector(self.x)
+        z+=self.iy[1]
+        self.assertEqual(z[0].codomain(), self.a0+self.b1)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b1)
+        
+
+        #const TubeVector& operator+=(const Trajectory& self.x)
+        # z = TubeVector(self.x)
+        # z+=trajy[1]
+        # self.assertEqual(z[0].codomain(), self.a0+self.b1)
+        # self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2+self.b1)
+        
+
+        #const TubeVector& operator+=(const Tube& self.x)
+        z = TubeVector(self.x)
+        z+=self.y[1]
+        self.assertEqual(z[0].codomain(), self.a0+self.b1)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b1)
+        
+
+        #const TubeVector& operator+=(const ibex.IntervalVector& self.x)
+        z = TubeVector(self.x)
+        z+=self.iy
+        self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b2)
+        
+
+        #const TubeVector& operator+=(const TrajectoryVector& self.x)
+        # z = TubeVector(self.x)
+        # z+=trajy
+        # self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2+self.b2)
+        
+
+        #const TubeVector& operator+=(const TubeVector& self.x)
+        z = TubeVector(self.x)
+        z+=self.y
+        self.assertEqual(z[0].codomain(), self.a0+self.b0)
+        self.assertEqual(z[1].codomain(), self.a1+self.b1)
+        self.assertEqual(z[2].codomain(), self.a2+self.b2)
+        
+
+    def test_VectorTube_operator_isub(self):
+
+        #const TubeVector& operator-=(const ibex.Interval& self.x)
+        z = TubeVector(self.x)
+        z-=self.iy[1]
+        self.assertEqual(z[0].codomain(), self.a0-self.b1)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b1)
+        
+
+        #const TubeVector& operator-=(const Trajectory& self.x)
+        # z = TubeVector(self.x)
+        # z-=trajy[1]
+        # self.assertEqual(z[0].codomain(), self.a0-self.b1)
+        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2-self.b1)
+        
+
+        #const TubeVector& operator-=(const Tube& self.x)
+        z = TubeVector(self.x)
+        z-=self.y[1]
+        self.assertEqual(z[0].codomain(), self.a0-self.b1)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b1)
+        
+
+        #const TubeVector& operator-=(const ibex.IntervalVector& self.x)
+        z = TubeVector(self.x)
+        z-=self.iy
+        self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        #const TubeVector& operator-=(const TrajectoryVector& self.x)
+        # z = TubeVector(self.x)
+        # z-=trajy
+        # self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        # self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+        #const TubeVector& operator-=(const TubeVector& self.x)
+        z = TubeVector(self.x)
+        z-=self.y
+        self.assertEqual(z[0].codomain(), self.a0-self.b0)
+        self.assertEqual(z[1].codomain(), self.a1-self.b1)
+        self.assertEqual(z[2].codomain(), self.a2-self.b2)
+        
+
+    def test_VectorTube_operator_imul(self):
+
+        #const TubeVector& operator*=(const ibex.Interval& self.x)
+        z = TubeVector(self.x)
+        z*=self.iy[1]
+        self.assertEqual(z[0].codomain(), self.a0*self.b1)
+        self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        self.assertEqual(z[2].codomain(), self.a2*self.b1)
+        
+
+        #const TubeVector& operator*=(const Trajectory& self.x)
+        # z = TubeVector(self.x)
+        # z*=trajy[1]
+        # self.assertEqual(z[0].codomain(), self.a0*self.b1)
+        # self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        # self.assertEqual(z[2].codomain(), self.a2*self.b1)
+        
+
+        #const TubeVector& operator*=(const Tube& self.x)
+        z = TubeVector(self.x)
+        z*=self.y[1]
+        self.assertEqual(z[0].codomain(), self.a0*self.b1)
+        self.assertEqual(z[1].codomain(), self.a1*self.b1)
+        self.assertEqual(z[2].codomain(), self.a2*self.b1)
+        
+
+    def test_VectorTube_operator_itrudiv(self):
+
+        #const TubeVector& operator/=(const ibex.Interval& self.x)
+        z = TubeVector(self.x)
+        z/=self.iy[1]
+        self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
+        self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
+        self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
+        
+
+        #const TubeVector& operator/=(const Trajectory& self.x)
+        # z = TubeVector(self.x)
+        # z/=trajy[1]
+        # self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
+        # self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
+        # self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
+        
+
+        #const TubeVector& operator/=(const Tube& self.x)
+        z = TubeVector(self.x)
+        z/=self.y[1]
+        self.assertApproxIntv(z[0].codomain(), self.a0/self.b1)
+        self.assertApproxIntv(z[1].codomain(), self.a1/self.b1)
+        self.assertApproxIntv(z[2].codomain(), self.a2/self.b1)
+        
+
+    def test_VectorTube_operator_ior(self):
+
+        #const TubeVector& operator|=(const ibex.IntervalVector& self.x)
+        z = TubeVector(self.x)
+        z|=self.iy
+        self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
+        self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
+        self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
+        
+
+        #const TubeVector& operator|=(const TrajectoryVector& self.x)
+        # z = TubeVector(self.x)
+        # z|=trajy
+        # self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
+        # self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
+        # self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
+        
+
+        #const TubeVector& operator|=(const TubeVector& self.x)
+        z = TubeVector(self.x)
+        z|=self.y
+        self.assertApproxIntv(z[0].codomain(), (self.a0 | self.b0))
+        self.assertApproxIntv(z[1].codomain(), (self.a1 | self.b1))
+        self.assertApproxIntv(z[2].codomain(), (self.a2 | self.b2))
+        
+
+    def test_VectorTube_operator_iand(self):
+        self.iy |= IntervalVector(3, Interval(-1))
+        self.y.set(self.iy)
+
+        #const TubeVector& operator&=(const ibex.IntervalVector& self.x)
+        z = TubeVector(self.x)
+        z&=self.iy
+        self.assertApproxIntv(z[0].codomain(), Interval.EMPTY_SET)
+        self.assertApproxIntv(z[1].codomain(), self.a1)
+        self.assertApproxIntv(z[2].codomain(), self.a2)
+        
+
+        #const TubeVector& operator&=(const TrajectoryVector& self.x)
+        # z = TubeVector(self.x)
+        # self.y&=trajx
+        # self.assertApproxIntv(z[0].codomain(), self.a0)
+        # self.assertApproxIntv(z[1].codomain(), self.a1)
+        # self.assertApproxIntv(z[2].codomain(), self.a2)
+        
+
+        #const TubeVector& operator&=(const TubeVector& self.x)
+        z = TubeVector(self.x)
+        z&=self.y
+        self.assertApproxIntv(z[0].codomain(), Interval.EMPTY_SET)
+        self.assertApproxIntv(z[1].codomain(), self.a1)
+        self.assertApproxIntv(z[2].codomain(), self.a2)
+        
+if __name__ ==  '__main__':
   unittest.main()
```

## Comparing `codac-1.5.5.dist-info/RECORD` & `codac-1.5.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-codac/empty.cpython-39-aarch64-linux-gnu.so,sha256=zrDVXR83ALpsKLgWavM2zRcyietEnowTZBItcQETtho,69640
-codac/core.cpython-39-aarch64-linux-gnu.so,sha256=qdHfLTqswdAv3D7w0-ZH8nUoK2-hfpG56lHSymWcYb8,5730648
-codac/__init__.py,sha256=gGdR8a3BRf6iDn5V8byHbMglX_1bi4q5RvVuaIhTLB8,1357
-codac/codac2.cpython-39-aarch64-linux-gnu.so,sha256=xYEEreGBgTiPPZyMmXOahqaEZihvjpkLnmqEP0Y9p20,334681
-codac/unsupported.cpython-39-aarch64-linux-gnu.so,sha256=bWz9epm4PTnH1AcHh6al7ZjDDhZ7gNSWyq2PEVSuZ5A,948001
-codac/version.py,sha256=NBmSfS5yKx8pttF9lOwvUSu6T3eg3UrNSyT6IzBkvGQ,19
-codac/tests/test_numpy.py,sha256=_j9W2y09yQ9GeqHb-jHKGWsaQdaa5SYpdZbhbHDTlz8,1469
-codac/tests/test_ctcbox.py,sha256=98qyic6nUO8O3aFoQ4v10dJrtkuINtj1Bt4P9fe2nq0,1303
-codac/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-codac/tests/test_sepbox.py,sha256=aEDHjHE2vELgwkYJh0TEXyE94u5JS60Qmnq6AouR-5A,1982
-codac/tests/test_function.py,sha256=wHj-aAoXFASXNpUpTU-7ypqT1G9No_qcu2UFx9iAwBo,1123
-codac/tests/test_cn.py,sha256=-grkg49m8fB5OqKO_A_L1-iWrGuJgJepAYo1QcV5dvQ,15680
-codac/tests/test_ctc_constell.py,sha256=dcextY7LTz64G_UxKWRaOeltNtBDOgrhfLO0WsgzQto,3660
-codac/tests/test_actions.py,sha256=D7O47J9vRkP7dEDLWxz5XL42arp6C6jXe57VHYRjZRw,1262
-codac/tests/test_ctcdelay.py,sha256=25NTMKbjK-UiWeSqeewM-W6txprZPVQ1fv8a_rBj2P0,1958
-codac/tests/test_ctceval.py,sha256=4teKsdjzUSgTqegkUlJx2AdOFFTWsrJWrsZuZCA5scg,44226
-codac/tests/test_multi_arithmetic.py,sha256=OX5qgWFa8kyuix3p6oyfmizs94xcW6OhRphV76SwQSc,3955
-codac/tests/test_ctccartprod.py,sha256=5BesLneeNSClzzmaq-ROfExVlJOn5jyRxhfLiqkEKi4,1548
-codac/tests/test_ctcstatic.py,sha256=q2wf4We_LPc33ua--uNvcN8TpiqCZoWseEeN0s3_nEQ,905
-codac/tests/test_definition.py,sha256=s6_rJPLn_UDRBFRp-5HptrNqtoc3IZrF_Fh1Gx3BKDg,13219
-codac/tests/test_arithmetic.py,sha256=yiPxEUrvDH3mW9LZBu7LbA1wbwQYiyrUqz6c-ZpHPpI,30842
-codac-1.5.5.dist-info/METADATA,sha256=XD9DFrS9o-yl54hlAFK8C2n1g6AUvPUVGYEQs9HoCAM,615
-codac-1.5.5.dist-info/top_level.txt,sha256=8FIXP4a7FrNu8RyqD7RFUsU7CTUmdd2T6j6EU-DTNYs,6
-codac-1.5.5.dist-info/RECORD,,
-codac-1.5.5.dist-info/WHEEL,sha256=CBycxh3glnwfbPQMOedoey2NiqMJxkbyufq_hPo2rPs,150
-codac.libs/core-a9d1df2d.cpython-39-aarch64-linux-gnu.so,sha256=Nwgs-XNCr7mSSLRfoeEcFtbaL6QHXoWo1q52QsV1f4E,6152905
+codac/__init__.py,sha256=LUOPAUDUfdSeS0Wzcxpg6tClmbb3wjLM5xPqhfjvxfU,1395
+codac/codac2.cp39-win_amd64.pyd,sha256=iwLDSlhO48_-eX3dHj4oZqLAtP-OwgY92wc5ulOK4rQ,343552
+codac/core.cp39-win_amd64.pyd,sha256=3AKv9s5HmCsEz8hiu9o8VQm4KuLcCNOb4vNWiAxAXGs,3726336
+codac/unsupported.cp39-win_amd64.pyd,sha256=IbZLVp3CN4-4hE-Sej6Wq4BDPfZNrVelxtcT6wD7aqc,890368
+codac/version.py,sha256=fsfDu70SofQs0-SEyCBElBIsZdMmuVocuIVUu1kTnD8,19
+codac/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+codac/tests/test_actions.py,sha256=DP2TdwMD5Xis5g9rDQ-M2-jXAIeRXVs0qjTunSRc9Kw,1302
+codac/tests/test_arithmetic.py,sha256=vDj_He6c3GFKWGMkMChdJyXlnkM1ACeZscAJXNJG308,31638
+codac/tests/test_cn.py,sha256=o3rcm33H4I5B4CEbhlySS9RBYhRbJe8AdYdOUhC6qkI,16259
+codac/tests/test_ctc_constell.py,sha256=h1bIudmjmFwCrAHJWJHFAPuIM7iA6qplUfVCq6NQvtY,3773
+codac/tests/test_ctcbox.py,sha256=BobCio0_OP4D_vXtXrP_8LrJIIfikqU3JMnWkWEOEuI,1362
+codac/tests/test_ctccartprod.py,sha256=WZJh_BZwo9B0NEfFy1lfR_wFalVY6rXsQuBGKBSYQpQ,1620
+codac/tests/test_ctcdelay.py,sha256=Eh3pfyv5tCXYNDoiOkOdV80eIgU0h4BGlMTnb-ButBQ,2023
+codac/tests/test_ctceval.py,sha256=GnUwCCDyLS9s8LBlxQXe4Esp4FRaGVa4vGxCSM9y2JA,45322
+codac/tests/test_ctcstatic.py,sha256=bN9H49eWoTaQcydpn-g1AD-IUW10a4q7V2JMC1-1uDA,939
+codac/tests/test_definition.py,sha256=hYAuOLtv9kZ5SfZrO48V4BJgV8kicNmnNDkltyjVZhM,13567
+codac/tests/test_function.py,sha256=8Sx-oxlyVi94eQjhYhKU5OVhOxjkuiQwTQeR6chc8ug,1156
+codac/tests/test_multi_arithmetic.py,sha256=S9rMq2MKU-dFL2AZv-xs1hr2tUeXtyUEHskxN8Ox8YA,4061
+codac/tests/test_numpy.py,sha256=gIPqIcaUe-Sj2clqPhCBuUB4KLqu8iNCXyh17ZtewZQ,1524
+codac/tests/test_sepbox.py,sha256=3LfmqlkRF-6Gj_FmkV12Jjqks2s-5LUh1fqNUwVGe5c,2057
+codac-1.5.6.dist-info/METADATA,sha256=uwrvyND-7F8NfiBlL4wnMRbaEXCiNTBEG1X5Ckb09CA,630
+codac-1.5.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+codac-1.5.6.dist-info/top_level.txt,sha256=8FIXP4a7FrNu8RyqD7RFUsU7CTUmdd2T6j6EU-DTNYs,6
+codac-1.5.6.dist-info/RECORD,,
```

