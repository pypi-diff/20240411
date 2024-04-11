# Comparing `tmp/hsslms-0.1.2.tar.gz` & `tmp/hsslms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsslms-0.1.2.tar", last modified: Thu Feb 17 19:00:03 2022, max compression
+gzip compressed data, was "hsslms-0.1.3.tar", last modified: Thu Apr 11 12:52:40 2024, max compression
```

## Comparing `hsslms-0.1.2.tar` & `hsslms-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 mvr       (1000) users      (100)        0 2022-02-17 19:00:03.014655 hsslms-0.1.2/
--rw-r--r--   0 mvr       (1000) users      (100)     1061 2022-01-02 18:32:57.000000 hsslms-0.1.2/LICENSE
--rw-r--r--   0 mvr       (1000) users      (100)     5609 2022-02-17 19:00:03.014655 hsslms-0.1.2/PKG-INFO
--rw-r--r--   0 mvr       (1000) users      (100)     4931 2022-02-17 18:28:26.000000 hsslms-0.1.2/README.rst
-drwxr-xr-x   0 mvr       (1000) users      (100)        0 2022-02-17 19:00:03.014655 hsslms-0.1.2/bin/
--rwxr--r--   0 mvr       (1000) users      (100)       40 2022-01-13 07:46:40.000000 hsslms-0.1.2/bin/hsslms
--rw-r--r--   0 mvr       (1000) users      (100)      103 2022-01-02 14:48:37.000000 hsslms-0.1.2/pyproject.toml
--rw-r--r--   0 mvr       (1000) users      (100)      802 2022-02-17 19:00:03.014655 hsslms-0.1.2/setup.cfg
-drwxr-xr-x   0 mvr       (1000) users      (100)        0 2022-02-17 19:00:03.014655 hsslms-0.1.2/src/
-drwxr-xr-x   0 mvr       (1000) users      (100)        0 2022-02-17 19:00:03.014655 hsslms-0.1.2/src/hsslms/
--rw-r--r--   0 mvr       (1000) users      (100)     2629 2022-02-13 19:24:15.000000 hsslms-0.1.2/src/hsslms/__init__.py
--rw-r--r--   0 mvr       (1000) users      (100)     9700 2022-01-23 12:44:07.000000 hsslms-0.1.2/src/hsslms/__main__.py
--rw-r--r--   0 mvr       (1000) users      (100)     5137 2022-01-17 16:19:46.000000 hsslms-0.1.2/src/hsslms/hss.py
--rw-r--r--   0 mvr       (1000) users      (100)     6342 2022-02-14 09:07:27.000000 hsslms-0.1.2/src/hsslms/lmots.py
--rw-r--r--   0 mvr       (1000) users      (100)     8071 2022-02-14 09:07:01.000000 hsslms-0.1.2/src/hsslms/lms.py
--rw-r--r--   0 mvr       (1000) users      (100)     4665 2022-01-19 09:27:19.000000 hsslms-0.1.2/src/hsslms/pershss.py
--rw-r--r--   0 mvr       (1000) users      (100)     1493 2022-01-15 09:50:30.000000 hsslms-0.1.2/src/hsslms/restricted_unpickler.py
--rw-r--r--   0 mvr       (1000) users      (100)     2303 2022-01-30 18:44:09.000000 hsslms-0.1.2/src/hsslms/utils.py
-drwxr-xr-x   0 mvr       (1000) users      (100)        0 2022-02-17 19:00:03.014655 hsslms-0.1.2/src/hsslms.egg-info/
--rw-r--r--   0 mvr       (1000) users      (100)     5609 2022-02-17 19:00:02.000000 hsslms-0.1.2/src/hsslms.egg-info/PKG-INFO
--rw-r--r--   0 mvr       (1000) users      (100)      402 2022-02-17 19:00:03.000000 hsslms-0.1.2/src/hsslms.egg-info/SOURCES.txt
--rw-r--r--   0 mvr       (1000) users      (100)        1 2022-02-17 19:00:02.000000 hsslms-0.1.2/src/hsslms.egg-info/dependency_links.txt
--rw-r--r--   0 mvr       (1000) users      (100)       13 2022-02-17 19:00:02.000000 hsslms-0.1.2/src/hsslms.egg-info/requires.txt
--rw-r--r--   0 mvr       (1000) users      (100)        7 2022-02-17 19:00:02.000000 hsslms-0.1.2/src/hsslms.egg-info/top_level.txt
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.498353 hsslms-0.1.3/
+-rw-r--r--   0 mvr       (1002) users      (100)     1061 2024-04-11 11:49:26.000000 hsslms-0.1.3/LICENSE
+-rw-r--r--   0 mvr       (1002) users      (100)     5600 2024-04-11 12:52:40.498353 hsslms-0.1.3/PKG-INFO
+-rw-r--r--   0 mvr       (1002) users      (100)     4931 2024-04-11 11:49:26.000000 hsslms-0.1.3/README.rst
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.494353 hsslms-0.1.3/bin/
+-rwxr-xr-x   0 mvr       (1002) users      (100)       40 2024-04-11 11:49:26.000000 hsslms-0.1.3/bin/hsslms
+-rw-r--r--   0 mvr       (1002) users      (100)      103 2024-04-11 11:49:26.000000 hsslms-0.1.3/pyproject.toml
+-rw-r--r--   0 mvr       (1002) users      (100)      802 2024-04-11 12:52:40.498353 hsslms-0.1.3/setup.cfg
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.494353 hsslms-0.1.3/src/
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.498353 hsslms-0.1.3/src/hsslms/
+-rw-r--r--   0 mvr       (1002) users      (100)     2670 2024-04-11 12:48:17.000000 hsslms-0.1.3/src/hsslms/__init__.py
+-rw-r--r--   0 mvr       (1002) users      (100)     9700 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/__main__.py
+-rw-r--r--   0 mvr       (1002) users      (100)     5137 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/hss.py
+-rw-r--r--   0 mvr       (1002) users      (100)     6399 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/lmots.py
+-rw-r--r--   0 mvr       (1002) users      (100)     8129 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/lms.py
+-rw-r--r--   0 mvr       (1002) users      (100)     5300 2024-04-11 11:54:16.000000 hsslms-0.1.3/src/hsslms/lmswrapper.py
+-rw-r--r--   0 mvr       (1002) users      (100)     4665 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/pershss.py
+-rw-r--r--   0 mvr       (1002) users      (100)     1493 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/restricted_unpickler.py
+-rw-r--r--   0 mvr       (1002) users      (100)     2809 2024-04-11 11:49:26.000000 hsslms-0.1.3/src/hsslms/utils.py
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.498353 hsslms-0.1.3/src/hsslms.egg-info/
+-rw-r--r--   0 mvr       (1002) users      (100)     5600 2024-04-11 12:52:40.000000 hsslms-0.1.3/src/hsslms.egg-info/PKG-INFO
+-rw-r--r--   0 mvr       (1002) users      (100)      459 2024-04-11 12:52:40.000000 hsslms-0.1.3/src/hsslms.egg-info/SOURCES.txt
+-rw-r--r--   0 mvr       (1002) users      (100)        1 2024-04-11 12:52:40.000000 hsslms-0.1.3/src/hsslms.egg-info/dependency_links.txt
+-rw-r--r--   0 mvr       (1002) users      (100)       13 2024-04-11 12:52:40.000000 hsslms-0.1.3/src/hsslms.egg-info/requires.txt
+-rw-r--r--   0 mvr       (1002) users      (100)        7 2024-04-11 12:52:40.000000 hsslms-0.1.3/src/hsslms.egg-info/top_level.txt
+drwxr-xr-x   0 mvr       (1002) users      (100)        0 2024-04-11 12:52:40.498353 hsslms-0.1.3/tests/
+-rw-r--r--   0 mvr       (1002) users      (100)    19683 2024-04-11 11:49:26.000000 hsslms-0.1.3/tests/test.py
+-rw-r--r--   0 mvr       (1002) users      (100)     5287 2024-04-11 11:49:26.000000 hsslms-0.1.3/tests/test_cli.py
```

### Comparing `hsslms-0.1.2/LICENSE` & `hsslms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hsslms-0.1.2/PKG-INFO` & `hsslms-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: hsslms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Leighton-Micali Hash-Based Signatures
 Home-page: https://github.com/pmvr/python-hsslms
 Author: Matthias Vögeler
 Author-email: matthias.voegeler@hshl.de
-License: UNKNOWN
 Project-URL: Documentation, https://pmvr.github.io/python-hsslms/
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Project-URL: Bug Tracker, https://github.com/pmvr/python-hsslms/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 
 python-hsslms
 =============
 
 This is an implementation of Leighton-Micali Hash-Based Signatures in Python according to `RFC 8554 <https://www.rfc-editor.org/rfc/rfc8554.html>`_. The one time signature keys are generated by using pseudo random generator, which saves a lot of memory to store the private keys in ram and on harddisk.
 
 The implementation is meant as a reference and for educational purposes.
@@ -91,15 +90,15 @@
    vk = sk.gen_pub()
    # verify the signature, if invalid an exception will be raised
    vk.verify(b'abc', signature)
 
 Performance Measurements
 ------------------------
 
-The measurements are done on a Ryzen 5800X, where multiprocessing
+The measurements are done on a Ryzen 5600X, where multiprocessing
 features are used with 6 cores.
 
 Key Generation
 ^^^^^^^^^^^^^^
 
 +----------+-----+-----+-----+-----+-------------+------+------+------+-------+
 | Key-Type | Time[s]               | #Signatures | Size of Signature          |
@@ -144,9 +143,7 @@
 | H15      | 0.001 | 0.001 | 0.001 | 0.004 |
 +----------+-------+-------+-------+-------+
 
 License
 =======
 
 `MIT <https://opensource.org/licenses/MIT>`__
-
-
```

### Comparing `hsslms-0.1.2/README.rst` & `hsslms-0.1.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
    vk = sk.gen_pub()
    # verify the signature, if invalid an exception will be raised
    vk.verify(b'abc', signature)
 
 Performance Measurements
 ------------------------
 
-The measurements are done on a Ryzen 5800X, where multiprocessing
+The measurements are done on a Ryzen 5600X, where multiprocessing
 features are used with 6 cores.
 
 Key Generation
 ^^^^^^^^^^^^^^
 
 +----------+-----+-----+-----+-----+-------------+------+------+------+-------+
 | Key-Type | Time[s]               | #Signatures | Size of Signature          |
```

### Comparing `hsslms-0.1.2/setup.cfg` & `hsslms-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hsslms
-version = 0.1.2
+version = 0.1.3
 author = Matthias Vögeler
 author_email = matthias.voegeler@hshl.de
 description = Leighton-Micali Hash-Based Signatures
 long_description = file: README.rst
 long_description_content_type = text/markdown
 url = https://github.com/pmvr/python-hsslms
 project_urls =
```

### Comparing `hsslms-0.1.2/src/hsslms/__init__.py` & `hsslms-0.1.3/src/hsslms/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         # compute the related public key
         vk = sk.gen_pub()
         # verify the signature, if invalid an exception will be raised
         vk.verify(b'abc', signature)
 """
 
 __all__ = ['INVALID', 'FAILURE', 'LMOTS_ALGORITHM_TYPE', 'LMS_ALGORITHM_TYPE', 'LM_OTS_Pub', 'LM_OTS_Priv', 'LMS_Pub', 'LMS_Priv', 'HSS_Pub', 'HSS_Priv', 'PersHSS_Priv']
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from .utils import INVALID, FAILURE
 from .utils import LMOTS_ALGORITHM_TYPE, LMS_ALGORITHM_TYPE
 from .lmots import LM_OTS_Priv, LM_OTS_Pub
 from .lms import LMS_Priv, LMS_Pub
 from .hss import HSS_Pub, HSS_Priv
 from .pershss import PersHSS_Priv
+from .lmswrapper import LMS_Wrapper_Priv
```

### Comparing `hsslms-0.1.2/src/hsslms/__main__.py` & `hsslms-0.1.3/src/hsslms/__main__.py`

 * *Files identical despite different names*

### Comparing `hsslms-0.1.2/src/hsslms/hss.py` & `hsslms-0.1.3/src/hsslms/hss.py`

 * *Files identical despite different names*

### Comparing `hsslms-0.1.2/src/hsslms/lmots.py` & `hsslms-0.1.3/src/hsslms/lmots.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,24 +54,24 @@
                     if len(buffer) < 1024**2:
                         break
                 message.close()
             except IOError:
                 raise FAILURE("Error. Cannot read message.")
         else:
             raise FAILURE("Invalid message type.")
-        Q = Q.digest()
+        Q = Q.digest()[:n]
         Qa = Q + cksm(Q, w, n, ls)
         Kc = H(self.I + self.q + D_PBLC)
         for i in range(p):
             a = coef(Qa, i, w)
             tmp = signature[4+n+i*n : 4+n+(i+1)*n]  # y[i]
             for j in range(a, 2**w - 1):
-                tmp = H(self.I + self.q + u16str(i) + u8str(j) + tmp).digest()
+                tmp = H(self.I + self.q + u16str(i) + u8str(j) + tmp).digest()[:n]
             Kc.update(tmp)  # z
-        return Kc.digest()  # Kc
+        return Kc.digest()[:n]  # Kc
         
     
     def verify(self, message, signature):
         """Signature Verification of LMOTS
         
         Tries to verify the signature of a message with the public key associated
         with the class.
@@ -106,15 +106,15 @@
     """
     
     def __init__(self, typecode, I, q, SEED):
         self.I = I
         self.q = q
         self.H, self.n, self.w, self.p, self.ls = typecode.H, typecode.n, typecode.w, typecode.p, typecode.ls
         self.typecode = u32str(typecode.value)
-        self.x = [self.H(self.I + u32str(self.q) + u16str(i) + b'\xff' + SEED).digest() for i in range(self.p)]
+        self.x = [self.H(self.I + u32str(self.q) + u16str(i) + b'\xff' + SEED).digest()[:self.n] for i in range(self.p)]
         self.used = False
 
     def sign(self, message):
         """Signature Generation of LMOTS
         
         Signs a message with the private key associated with the class.
         
@@ -143,36 +143,36 @@
                     if len(buffer) < 1024**2:
                         break
                 message.close()
             except IOError:
                 raise FAILURE("Error. Cannot read message.")
         else:
             raise FAILURE("Invalid message type.")
-        Q = Q.digest()
+        Q = Q.digest()[:self.n]
         Qa = Q + cksm(Q, self.w, self.n, self.ls)
         for i in range(self.p):
             a = coef(Qa, i, self.w)
             tmp = self.x[i]
             for j in range(a):
-                tmp = self.H(self.I + u32str(self.q) + u16str(i) + u8str(j) + tmp).digest()
+                tmp = self.H(self.I + u32str(self.q) + u16str(i) + u8str(j) + tmp).digest()[:self.n]
             signature += tmp  # y
         self.used = True
         return signature
 
     def gen_pub_K(self):
         u32str_q = u32str(self.q)
         K = self.H(self.I + u32str_q + D_PBLC)
         u8str_j = [u8str(j) for j in range(2**self.w - 1)]
         for i in range(self.p):
             tmp = self.x[i]
             Iqi = self.I + u32str_q + u16str(i)
             for j in u8str_j:
-                tmp = self.H(Iqi + j + tmp).digest()
+                tmp = self.H(Iqi + j + tmp).digest()[:self.n]
             K.update(tmp)
-        return K.digest()
+        return K.digest()[:self.n]
     
     def gen_pub(self):
         """Computes the public key associated with the private key in this class.
         
         Returns:
             LM_OTS_Pub: The public key belonging to this private key.
         """
```

### Comparing `hsslms-0.1.2/src/hsslms/lms.py` & `hsslms-0.1.3/src/hsslms/lms.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,22 @@
         if self.pubtype != sigtype:
             raise INVALID
         if q >= 2**self.h or len(signature) != 12+n*(p+1)+self.m*self.h:
             raise INVALID
         OTS_PUB = LM_OTS_Pub(lmots_signature[:4] + self.I + u32str(q)  + b'\x00'*n)
         Kc = OTS_PUB._algo4b(message, lmots_signature)
         node_num = 2**self.h + q
-        tmp = self.H(self.I + u32str(node_num) + D_LEAF + Kc).digest()
+        tmp = self.H(self.I + u32str(node_num) + D_LEAF + Kc).digest()[:self.m]
         i = 0
         while node_num > 1:
             path = signature[12+n*(p+1)+i*self.m:12+n*(p+1)+(i+1)*self.m]
             if node_num % 2 == 1:
-                tmp = self.H(self.I + u32str(node_num//2) + D_INTR + path + tmp).digest()
+                tmp = self.H(self.I + u32str(node_num//2) + D_INTR + path + tmp).digest()[:self.m]
             else:
-                tmp = self.H(self.I + u32str(node_num//2) + D_INTR + tmp + path).digest()
+                tmp = self.H(self.I + u32str(node_num//2) + D_INTR + tmp + path).digest()[:self.m]
             node_num >>= 1
             i += 1
         return tmp  # Tc
         
     def verify(self, message, signature):
         """Signature Verification of LMS
 
@@ -152,31 +152,31 @@
     Args:
         typecode (LMS_ALGORITHM_TYPE): Enumeration of Leighton-Micali Signatures (LMS) algorithm types
         otstypecode (LMOTS_ALGORITHM_TYPE): Enumeration of Leighton-Micali One-Time-Signatures (LMOTS) algorithm types
         num_cores (int, None, optional): the number of CPU cores used for key generation, None=all cores
     """
     def _calc_leafs(H, I, r, h, otstypecode, SEED):
         OTS_PRIV = LM_OTS_Priv(otstypecode, I, r-2**h, SEED)
-        return H(I + u32str(r) + D_LEAF + OTS_PRIV.gen_pub_K()).digest()
-    def _calc_knots(H, I, r, Tl, Tr):
-        return H(I + u32str(r) + D_INTR + Tl + Tr).digest()
+        return H(I + u32str(r) + D_LEAF + OTS_PRIV.gen_pub_K()).digest()[:otstypecode.n]
+    def _calc_knots(H, I, r, Tl, Tr, m):
+        return H(I + u32str(r) + D_INTR + Tl + Tr).digest()[:m]
     
     def __init__(self, typecode, otstypecode, num_cores=None):
         if num_cores is None:
             num_cores = cpu_count()
         self.typecode = typecode
         self.otstypecode = otstypecode
         self.H, self.m, self.h = self.typecode.H, self.typecode.m, self.typecode.h
         self.SEED = token_bytes(self.m)
         self.I = token_bytes(16)
         with Pool(num_cores) as p:
             self.T = [None]*(2**(self.h+1))
             self.T[2**self.h : 2**(self.h+1)] = p.starmap(LMS_Priv._calc_leafs, ((self.H, self.I, r, self.h, self.otstypecode, self.SEED) for r in range(2**self.h, 2**(self.h+1))))
             for i in range(self.h-1, -1, -1):
-                self.T[2**i : 2**(i+1)] = p.starmap(LMS_Priv._calc_knots, ((self.H, self.I, r, self.T[2*r], self.T[2*r+1]) for r in range(2**i, 2**(i+1))))
+                self.T[2**i : 2**(i+1)] = p.starmap(LMS_Priv._calc_knots, ((self.H, self.I, r, self.T[2*r], self.T[2*r+1], self.m) for r in range(2**i, 2**(i+1))))
         self.q = 0
         
     def sign(self, message):
         """Signature Generation of LMS
         
         Signs a message with the private key associated with the class.
```

### Comparing `hsslms-0.1.2/src/hsslms/pershss.py` & `hsslms-0.1.3/src/hsslms/pershss.py`

 * *Files identical despite different names*

### Comparing `hsslms-0.1.2/src/hsslms/restricted_unpickler.py` & `hsslms-0.1.3/src/hsslms/restricted_unpickler.py`

 * *Files identical despite different names*

### Comparing `hsslms-0.1.2/src/hsslms/utils.py` & `hsslms-0.1.3/src/hsslms/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,29 +51,38 @@
         p (int): internal dependent parameter
         ls (int): internal dependent parameter
     """
     LMOTS_SHA256_N32_W1  = 1
     LMOTS_SHA256_N32_W2  = 2
     LMOTS_SHA256_N32_W4  = 3
     LMOTS_SHA256_N32_W8  = 4
+    
+    LMOTS_SHA256_N24_W1  = 5
+    LMOTS_SHA256_N24_W2  = 6
+    LMOTS_SHA256_N24_W4  = 7
+    LMOTS_SHA256_N24_W8  = 8
+
     @property
     def H(self):
         return sha256
     @property
     def n(self):
-        return 32
+        if 'N32' in self.name:
+            return 32
+        else:
+            return 24
     @property
     def w(self):
-        return {1:1, 2:2, 3:4, 4:8}[self.value]
+        return {1:1, 2:2, 3:4, 4:8, 5:1, 6:2, 7:4, 8:8}[self.value]
     @property
     def p(self):
-        return {1:265, 2:133, 3:67, 4:34}[self.value]
+        return {1:265, 2:133, 3:67, 4:34, 5:200, 6:101, 7:51, 8:26}[self.value]
     @property
     def ls(self):
-        return {1:7, 2:6, 3:4, 4:0}[self.value]
+        return {1:7, 2:6, 3:4, 4:0, 5:8, 6:6, 7:4, 8:0}[self.value]
 
 
 class LMS_ALGORITHM_TYPE(Enum):
     """Enumeration of Leighton-Micali Signatures (LMS) algorithm types, see rfc8554.
     
     Attributes:
         H: Hashfunction
@@ -81,16 +90,27 @@
         h (int): height of the tree
     """
     LMS_SHA256_M32_H5  = 5
     LMS_SHA256_M32_H10 = 6
     LMS_SHA256_M32_H15 = 7
     LMS_SHA256_M32_H20 = 8
     LMS_SHA256_M32_H25 = 9
+
+    LMS_SHA256_M24_H5 = 10
+    LMS_SHA256_M24_H10 = 11
+    LMS_SHA256_M24_H15 = 12
+    LMS_SHA256_M24_H20 = 13
+    LMS_SHA256_M24_H25 = 14
+
     @property
     def H(self):
         return sha256
+
     @property
     def m(self):
-        return 32
+        if 'M32' in self.name:
+            return 32
+        else:
+            return 24
     @property
     def h(self):
-        return {5:5, 6:10, 7:15, 8:20, 9:25}[self.value]
+        return {5:5, 6:10, 7:15, 8:20, 9:25, 10:5, 11:10, 12:15, 13:20, 14:25}[self.value]
```

### Comparing `hsslms-0.1.2/src/hsslms.egg-info/PKG-INFO` & `hsslms-0.1.3/src/hsslms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: hsslms
-Version: 0.1.2
+Version: 0.1.3
 Summary: Leighton-Micali Hash-Based Signatures
 Home-page: https://github.com/pmvr/python-hsslms
 Author: Matthias Vögeler
 Author-email: matthias.voegeler@hshl.de
-License: UNKNOWN
 Project-URL: Documentation, https://pmvr.github.io/python-hsslms/
 Project-URL: Source, https://github.com/pypa/sampleproject/
 Project-URL: Bug Tracker, https://github.com/pmvr/python-hsslms/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 
 python-hsslms
 =============
 
 This is an implementation of Leighton-Micali Hash-Based Signatures in Python according to `RFC 8554 <https://www.rfc-editor.org/rfc/rfc8554.html>`_. The one time signature keys are generated by using pseudo random generator, which saves a lot of memory to store the private keys in ram and on harddisk.
 
 The implementation is meant as a reference and for educational purposes.
@@ -91,15 +90,15 @@
    vk = sk.gen_pub()
    # verify the signature, if invalid an exception will be raised
    vk.verify(b'abc', signature)
 
 Performance Measurements
 ------------------------
 
-The measurements are done on a Ryzen 5800X, where multiprocessing
+The measurements are done on a Ryzen 5600X, where multiprocessing
 features are used with 6 cores.
 
 Key Generation
 ^^^^^^^^^^^^^^
 
 +----------+-----+-----+-----+-----+-------------+------+------+------+-------+
 | Key-Type | Time[s]               | #Signatures | Size of Signature          |
@@ -144,9 +143,7 @@
 | H15      | 0.001 | 0.001 | 0.001 | 0.004 |
 +----------+-------+-------+-------+-------+
 
 License
 =======
 
 `MIT <https://opensource.org/licenses/MIT>`__
-
-
```

