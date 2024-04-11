# Comparing `tmp/klvm-0.9.8-py3-none-any.whl.zip` & `tmp/klvm-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 19894 bytes, number of entries: 19
--rw-r--r--  2.0 unx      132 b- defN 23-Nov-20 02:22 klvm/EvalError.py
--rw-r--r--  2.0 unx      855 b- defN 23-Nov-20 02:22 klvm/KLVMObject.py
--rw-r--r--  2.0 unx     6968 b- defN 23-Nov-20 02:22 klvm/SExp.py
--rw-r--r--  2.0 unx      233 b- defN 23-Nov-20 02:22 klvm/__init__.py
--rw-r--r--  2.0 unx     1089 b- defN 23-Nov-20 02:22 klvm/as_python.py
--rw-r--r--  2.0 unx      627 b- defN 23-Nov-20 02:22 klvm/casts.py
--rw-r--r--  2.0 unx     1738 b- defN 23-Nov-20 02:22 klvm/core_ops.py
--rw-r--r--  2.0 unx     1200 b- defN 23-Nov-20 02:22 klvm/costs.py
--rw-r--r--  2.0 unx    10730 b- defN 23-Nov-20 02:22 klvm/more_ops.py
--rw-r--r--  2.0 unx      427 b- defN 23-Nov-20 02:22 klvm/op_utils.py
--rw-r--r--  2.0 unx     6186 b- defN 23-Nov-20 02:22 klvm/operators.py
--rw-r--r--  2.0 unx     5725 b- defN 23-Nov-20 02:22 klvm/run_program.py
--rw-r--r--  2.0 unx     5193 b- defN 23-Nov-20 02:22 klvm/serialize.py
--rw-r--r--  2.0 unx      212 b- defN 23-Nov-20 02:22 klvm/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Nov-20 02:23 klvm-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1303 b- defN 23-Nov-20 02:23 klvm-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-20 02:23 klvm-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Nov-20 02:23 klvm-0.9.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1386 b- defN 23-Nov-20 02:23 klvm-0.9.8.dist-info/RECORD
-19 files, 55458 bytes uncompressed, 17696 bytes compressed:  68.1%
+Zip file size: 19948 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      132 b- defN 24-Apr-11 14:10 klvm/EvalError.py
+-rw-r--r--  2.0 unx      855 b- defN 24-Apr-11 14:10 klvm/KLVMObject.py
+-rw-r--r--  2.0 unx     6968 b- defN 24-Apr-11 14:10 klvm/SExp.py
+-rw-r--r--  2.0 unx      233 b- defN 24-Apr-11 14:10 klvm/__init__.py
+-rw-r--r--  2.0 unx     1089 b- defN 24-Apr-11 14:10 klvm/as_python.py
+-rw-r--r--  2.0 unx      627 b- defN 24-Apr-11 14:10 klvm/casts.py
+-rw-r--r--  2.0 unx     1738 b- defN 24-Apr-11 14:10 klvm/core_ops.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-Apr-11 14:10 klvm/costs.py
+-rw-r--r--  2.0 unx    10732 b- defN 24-Apr-11 14:10 klvm/more_ops.py
+-rw-r--r--  2.0 unx      550 b- defN 24-Apr-11 14:10 klvm/op_utils.py
+-rw-r--r--  2.0 unx     6186 b- defN 24-Apr-11 14:10 klvm/operators.py
+-rw-r--r--  2.0 unx     5725 b- defN 24-Apr-11 14:10 klvm/run_program.py
+-rw-r--r--  2.0 unx     5183 b- defN 24-Apr-11 14:10 klvm/serialize.py
+-rw-r--r--  2.0 unx      194 b- defN 24-Apr-11 14:10 klvm/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-11 14:10 klvm-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1525 b- defN 24-Apr-11 14:10 klvm-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 14:10 klvm-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-Apr-11 14:10 klvm-0.9.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1386 b- defN 24-Apr-11 14:10 klvm-0.9.9.dist-info/RECORD
+19 files, 55777 bytes uncompressed, 17750 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: klvm/serialize.py
 Comment: 
 
 Filename: klvm/version.py
 Comment: 
 
-Filename: klvm-0.9.8.dist-info/LICENSE
+Filename: klvm-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: klvm-0.9.8.dist-info/METADATA
+Filename: klvm-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: klvm-0.9.8.dist-info/WHEEL
+Filename: klvm-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: klvm-0.9.8.dist-info/top_level.txt
+Filename: klvm-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: klvm-0.9.8.dist-info/RECORD
+Filename: klvm-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## klvm/more_ops.py

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import io
 
-from blspy import G1Element, PrivateKey
+from chik_rs import G1Element, PrivateKey
 
 from .EvalError import EvalError
 from .casts import limbs_for_int
 from .SExp import SExp
 
 from .costs import (
     ARITH_BASE_COST,
```

## klvm/op_utils.py

```diff
@@ -1,12 +1,17 @@
-def operators_for_dict(keyword_to_atom, op_dict, op_name_lookup={}):
+def operators_for_dict(keyword_to_atom, op_dict, op_name_lookup=None):
+    if op_name_lookup is None:
+        op_name_lookup = {}
+
     d = {}
     for op in keyword_to_atom.keys():
         op_name = "op_%s" % op_name_lookup.get(op, op)
         op_f = op_dict.get(op_name)
         if op_f:
             d[keyword_to_atom[op]] = op_f
     return d
 
 
-def operators_for_module(keyword_to_atom, mod, op_name_lookup={}):
+def operators_for_module(keyword_to_atom, mod, op_name_lookup=None):
+    if op_name_lookup is None:
+        op_name_lookup = {}
     return operators_for_dict(keyword_to_atom, mod.__dict__, op_name_lookup)
```

## klvm/serialize.py

```diff
@@ -20,21 +20,21 @@
 CONS_BOX_MARKER = 0xFF
 
 
 def sexp_to_byte_iterator(sexp):
     todo_stack = [sexp]
     while todo_stack:
         sexp = todo_stack.pop()
-        pair = sexp.as_pair()
+        pair = sexp.pair
         if pair:
             yield bytes([CONS_BOX_MARKER])
             todo_stack.append(pair[1])
             todo_stack.append(pair[0])
         else:
-            yield from atom_to_byte_iterator(sexp.as_atom())
+            yield from atom_to_byte_iterator(sexp.atom)
 
 
 def atom_to_byte_iterator(as_atom):
     size = len(as_atom)
     if size == 0:
         yield b"\x80"
         return
```

## klvm/version.py

```diff
@@ -1,7 +1,7 @@
-from pkg_resources import get_distribution, DistributionNotFound
+import importlib_metadata
 
 try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
+    __version__ = importlib_metadata.version(__name__)
+except importlib_metadata.PackageNotFoundError:
     # package is not installed
     __version__ = "unknown"
```

## Comparing `klvm-0.9.8.dist-info/LICENSE` & `klvm-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `klvm-0.9.8.dist-info/METADATA` & `klvm-0.9.9.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: klvm
-Version: 0.9.8
+Version: 0.9.9
 Summary: [Contract Language | Chiklisp] Virtual Machine
 Home-page: https://github.com/Chik-Network/klvm
 Author: Chik Network, Inc.
 Author-email: hello@chiknetwork.com
 License: https://opensource.org/licenses/Apache-2.0
 Project-URL: Bug Reports, https://github.com/Chik-Network/klvm
 Project-URL: Source, https://github.com/Chik-Network/klvm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Security :: Cryptography
+Requires-Python: >=3.8.1, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: blspy >=0.9
+Requires-Dist: chik-rs >=0.2.13
+Requires-Dist: importlib-metadata ~=6.11.0
 Provides-Extra: dev
 Requires-Dist: klvm-tools >=0.4.4 ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
+Requires-Dist: setuptools ; extra == 'dev'
 
 [![Coverage Status](https://coveralls.io/repos/github/Chik-Network/klvm/badge.svg?branch=main)](https://coveralls.io/github/Chik-Network/klvm?branch=main)
 
 This is the in-development version of a LISP-like language for encumbering and releasing funds with smart-contract capabilities.
 
 See docs/klvm.org or https://chiklisp.com/ for more info.
```

## Comparing `klvm-0.9.8.dist-info/RECORD` & `klvm-0.9.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 klvm/KLVMObject.py,sha256=aBd8JmmksW3_jbWcHEGWc_7CbB58geYgxoh66LmJqPM,855
 klvm/SExp.py,sha256=K6qPULZFBhm95ry_IixJEfbV0bDpHpZFphb5f--1zI0,6968
 klvm/__init__.py,sha256=F_MQiGGnobQfAzmlVHKlj5iE9tATixBthNE9eZ0unow,233
 klvm/as_python.py,sha256=IbXuXXDhsSf3FwLQg60fX4lHahZSMqGMRaN_pSu8kyg,1089
 klvm/casts.py,sha256=nv3Bh24oT8cy6Ew18lHu7ey1tMCHGJNZojRlH9Qeais,627
 klvm/core_ops.py,sha256=ohJTxUY73zoUMjluQnp728_ELNru_jSEH-jkoMOjNX4,1738
 klvm/costs.py,sha256=osdTrSCxNg2c7lTtJYm6YUAUp3vltNStyBpzbR8wmPY,1200
-klvm/more_ops.py,sha256=I1rjh_YgTsqOq5iHPmrUf2pRx1y4k_yXJS1HaKnhzUs,10730
-klvm/op_utils.py,sha256=CRXf8epX6bqp2Qaoq6woo1I8Iv_Qk76Br8VZJxS67wg,427
+klvm/more_ops.py,sha256=cL7JtslyQ6rlEWEzC7hGKOouvL4uNqAL-8D1lh44ESE,10732
+klvm/op_utils.py,sha256=jbeexlEo1h1cTIuRyU1sCQ_X9akPPx_ZYrv0uS1dFlw,550
 klvm/operators.py,sha256=dt9T3D8c8hxtwgVZKXE8KiPA6r1oyGTH0B0Aeas0SPk,6186
 klvm/run_program.py,sha256=1G6yTTrtqLhFzw2_XmT8GiA84qel3a7fw3_MJkxccTo,5725
-klvm/serialize.py,sha256=9OyCaKJkZdmcv6XksIiDb3d7ybMHAoeCfvGjOmCCPX0,5193
-klvm/version.py,sha256=phF8Rm7BiuLJWF4-L_sBP5KFtFtgG-s1OAuQJ4O4DGU,212
-klvm-0.9.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-klvm-0.9.8.dist-info/METADATA,sha256=7UxzgIx603MZBSBDlgPfCFlvzEwX7zzq4NZpJLzMhuk,1303
-klvm-0.9.8.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-klvm-0.9.8.dist-info/top_level.txt,sha256=Hnio_LTbhuxjLiW_q1oYzmNRSXB_1_yaVXSdcFG7qVw,5
-klvm-0.9.8.dist-info/RECORD,,
+klvm/serialize.py,sha256=LTR-5XPYVteC9NcXWBxzFMnut--uOx1TYWYzp8xpK5k,5183
+klvm/version.py,sha256=LiRFdralfvZz5N27iK7L-LgcVu2T9fc1u1GC_HZHbQs,194
+klvm-0.9.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+klvm-0.9.9.dist-info/METADATA,sha256=uZi6dQRfjacxhyPEcmflj_X7Q9DIKc-EUoHMEKWqIis,1525
+klvm-0.9.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+klvm-0.9.9.dist-info/top_level.txt,sha256=Hnio_LTbhuxjLiW_q1oYzmNRSXB_1_yaVXSdcFG7qVw,5
+klvm-0.9.9.dist-info/RECORD,,
```

