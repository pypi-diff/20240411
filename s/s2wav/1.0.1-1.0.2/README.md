# Comparing `tmp/s2wav-1.0.1.tar.gz` & `tmp/s2wav-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2wav-1.0.1.tar", last modified: Tue Apr  9 14:16:09 2024, max compression
+gzip compressed data, was "s2wav-1.0.2.tar", last modified: Thu Apr 11 16:03:33 2024, max compression
```

## Comparing `s2wav-1.0.1.tar` & `s2wav-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 14:16:09.297885 s2wav-1.0.1/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.1/LICENCE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-09 14:16:09.297654 s2wav-1.0.1/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9850 2024-04-09 13:46:46.000000 s2wav-1.0.1/README.md
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 14:16:09.294756 s2wav-1.0.1/s2wav/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      778 2024-04-09 14:10:43.000000 s2wav-1.0.1/s2wav/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24271 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/samples.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 14:16:09.296317 s2wav-1.0.1/s2wav/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/construct.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    14891 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/wavelet.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11659 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/wavelet_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11169 2024-04-09 13:46:46.000000 s2wav-1.0.1/s2wav/transforms/wavelet_precompute_torch.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 14:16:09.297429 s2wav-1.0.1/s2wav.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-09 14:16:09.000000 s2wav-1.0.1/s2wav.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)      555 2024-04-09 14:16:09.000000 s2wav-1.0.1/s2wav.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-09 14:16:09.000000 s2wav-1.0.1/s2wav.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-09 14:16:09.000000 s2wav-1.0.1/s2wav.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-09 14:16:09.000000 s2wav-1.0.1/s2wav.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-09 14:16:09.297928 s2wav-1.0.1/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-09 14:14:42.000000 s2wav-1.0.1/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-09 14:16:09.297234 s2wav-1.0.1/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.1/tests/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.1/tests/conftest.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.1/tests/test_filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4813 2024-04-09 13:46:46.000000 s2wav-1.0.1/tests/test_gradients.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10154 2024-04-09 13:46:46.000000 s2wav-1.0.1/tests/test_wavelets.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.1/tests/test_wavelets_base.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316928 s2wav-1.0.2/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.2/LICENCE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-11 16:03:33.316703 s2wav-1.0.2/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9850 2024-04-09 13:46:46.000000 s2wav-1.0.2/README.md
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.313189 s2wav-1.0.2/s2wav/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      778 2024-04-09 14:10:43.000000 s2wav-1.0.2/s2wav/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24271 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/samples.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.315070 s2wav-1.0.2/s2wav/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/construct.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    14891 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11890 2024-04-11 13:07:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11169 2024-04-09 13:46:46.000000 s2wav-1.0.2/s2wav/transforms/wavelet_precompute_torch.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316463 s2wav-1.0.2/s2wav.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      555 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-11 16:03:33.000000 s2wav-1.0.2/s2wav.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-11 16:03:33.316975 s2wav-1.0.2/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-11 16:02:43.000000 s2wav-1.0.2/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-11 16:03:33.316192 s2wav-1.0.2/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.2/tests/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/conftest.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4813 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_gradients.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10154 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_wavelets.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.2/tests/test_wavelets_base.py
```

### Comparing `s2wav-1.0.1/LICENCE.txt` & `s2wav-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/PKG-INFO` & `s2wav-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.1
+Version: 1.0.2
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `s2wav-1.0.1/README.md` & `s2wav-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/__init__.py` & `s2wav-1.0.2/s2wav/__init__.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/filters.py` & `s2wav-1.0.2/s2wav/filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/samples.py` & `s2wav-1.0.2/s2wav/samples.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/transforms/base.py` & `s2wav-1.0.2/s2wav/transforms/base.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/transforms/construct.py` & `s2wav-1.0.2/s2wav/transforms/construct.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/transforms/wavelet.py` & `s2wav-1.0.2/s2wav/transforms/wavelet.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav/transforms/wavelet_precompute.py` & `s2wav-1.0.2/s2wav/transforms/wavelet_precompute.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,27 +216,28 @@
     else:
         f_scal = spherical.inverse_transform_jax(
             temp, precomps[1], Ls, sampling, reality, spin, nside
         )
     return f_wav, f_scal
 
 
-@partial(jit, static_argnums=(1, 2, 3, 4, 5, 6, 7, 8))
+@partial(jit, static_argnums=(1, 2, 3, 4, 5, 6, 7, 8, 11))
 def flm_to_analysis(
     flm: jnp.ndarray,
     L: int,
     N: int = 1,
     J_min: int = 0,
     J_max: int = None,
     lam: float = 2.0,
     sampling: str = "mw",
     nside: int = None,
     reality: bool = False,
     filters: Tuple[jnp.ndarray] = None,
     precomps: List[List[jnp.ndarray]] = None,
+    _precomp_shift: bool = True,
 ) -> Tuple[jnp.ndarray]:
     r"""Wavelet analysis from pixel space to wavelet space for complex signals.
 
     Args:
         f (jnp.ndarray): Signal :math:`f` on the sphere with shape :math:`[n_{\theta}, n_{\phi}]`.
 
         L (int): Harmonic bandlimit.
@@ -258,14 +259,17 @@
         reality (bool, optional): Whether :math:`f \in \mathbb{R}`, if True exploits
             conjugate symmetry of harmonic coefficients. Defaults to False.
 
         filters (Tuple[jnp.ndarray], optional): Precomputed wavelet filters. Defaults to None.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
+        
+        _precomp_shift (bool, optional): Whether or not the duplicated highest wavelet scale
+            precomputes are provided or not.
 
     Returns:
         f_wav (jnp.ndarray): Array of wavelet pixel-space coefficients
             with shape :math:`[n_{J}, 2N-1, n_{\theta}, n_{\phi}]`.
 
         f_scal (jnp.ndarray): Array of scaling pixel-space coefficients
             with shape :math:`[n_{\theta}, n_{\phi}]`.
@@ -298,18 +302,19 @@
                     flm[L0j:Lj, L - Lj : L - 1 + Lj],
                     wav_lm[j, L0j:Lj, L - Nj : L - 1 + Nj : 2],
                     optimize=True,
                 )
             )
         )
         shift = 0 if j < J else -1
+        shift = shift if _precomp_shift else 0
+
         f_wav[j - J_min] = wigner.inverse_transform_jax(
             f_wav_lmn[j - J_min],
             precomps[2][j - J_min + shift],
             Lj,
             Nj,
             sampling,
             reality,
             nside,
         )
-
     return f_wav
```

### Comparing `s2wav-1.0.1/s2wav/transforms/wavelet_precompute_torch.py` & `s2wav-1.0.2/s2wav/transforms/wavelet_precompute_torch.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/s2wav.egg-info/PKG-INFO` & `s2wav-1.0.2/s2wav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.1
+Version: 1.0.2
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `s2wav-1.0.1/s2wav.egg-info/SOURCES.txt` & `s2wav-1.0.2/s2wav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/setup.py` & `s2wav-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="s2wav",
-    version="1.0.1",
+    version="1.0.2",
     url="https://github.com/astro-informatics/s2wav",
     author="Authors & Contributors",
     license="GNU General Public License v3 (GPLv3)",
     python_requires=">=3.8",
     install_requires=requirements,
     description=("Differentiable and accelerated wavelet transforms with JAX"),
     long_description_content_type="text/x-rst",
```

### Comparing `s2wav-1.0.1/tests/conftest.py` & `s2wav-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/tests/test_filters.py` & `s2wav-1.0.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/tests/test_gradients.py` & `s2wav-1.0.2/tests/test_gradients.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/tests/test_wavelets.py` & `s2wav-1.0.2/tests/test_wavelets.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.1/tests/test_wavelets_base.py` & `s2wav-1.0.2/tests/test_wavelets_base.py`

 * *Files identical despite different names*

