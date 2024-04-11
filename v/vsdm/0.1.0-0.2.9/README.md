# Comparing `tmp/vsdm-0.1.0.tar.gz` & `tmp/vsdm-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsdm-0.1.0.tar", last modified: Thu Nov  9 02:29:56 2023, max compression
+gzip compressed data, was "vsdm-0.2.9.tar", last modified: Thu Apr 11 07:32:37 2024, max compression
```

## Comparing `vsdm-0.1.0.tar` & `vsdm-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-11-09 02:29:56.609636 vsdm-0.1.0/
--rw-r--r--   0 Ben        (501) staff       (20)     1065 2023-10-02 10:21:17.000000 vsdm-0.1.0/LICENSE
--rw-r--r--   0 Ben        (501) staff       (20)     1492 2023-11-09 02:29:56.609175 vsdm-0.1.0/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)      777 2023-11-09 01:44:47.000000 vsdm-0.1.0/README.md
--rw-r--r--   0 Ben        (501) staff       (20)      956 2023-11-09 02:09:42.000000 vsdm-0.1.0/pyproject.toml
--rw-r--r--   0 Ben        (501) staff       (20)       38 2023-11-09 02:29:56.609725 vsdm-0.1.0/setup.cfg
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-11-09 02:29:56.606638 vsdm-0.1.0/vsdm/
--rw-r--r--   0 Ben        (501) staff       (20)     1343 2023-10-02 09:38:44.000000 vsdm-0.1.0/vsdm/__init__.py
--rw-r--r--   0 Ben        (501) staff       (20)     6788 2023-09-12 06:07:55.000000 vsdm-0.1.0/vsdm/analytic.py
--rw-r--r--   0 Ben        (501) staff       (20)    23732 2023-10-02 09:39:52.000000 vsdm-0.1.0/vsdm/basis.py
--rw-r--r--   0 Ben        (501) staff       (20)     8045 2023-10-02 09:47:34.000000 vsdm-0.1.0/vsdm/gaussians.py
--rw-r--r--   0 Ben        (501) staff       (20)    20249 2023-10-02 09:43:41.000000 vsdm-0.1.0/vsdm/matrixcalc.py
--rw-r--r--   0 Ben        (501) staff       (20)    18115 2023-04-30 06:50:53.000000 vsdm-0.1.0/vsdm/portfolio.py
--rw-r--r--   0 Ben        (501) staff       (20)    26876 2023-10-02 09:43:00.000000 vsdm-0.1.0/vsdm/projection.py
--rw-r--r--   0 Ben        (501) staff       (20)    11441 2023-10-02 09:42:35.000000 vsdm-0.1.0/vsdm/ratecalc.py
--rw-r--r--   0 Ben        (501) staff       (20)     1544 2023-10-02 09:41:08.000000 vsdm-0.1.0/vsdm/units.py
--rw-r--r--   0 Ben        (501) staff       (20)    12795 2023-09-07 22:42:36.000000 vsdm-0.1.0/vsdm/utilities.py
--rw-r--r--   0 Ben        (501) staff       (20)     4056 2023-09-13 23:40:43.000000 vsdm-0.1.0/vsdm/wigner.py
-drwxr-xr-x   0 Ben        (501) staff       (20)        0 2023-11-09 02:29:56.608600 vsdm-0.1.0/vsdm.egg-info/
--rw-r--r--   0 Ben        (501) staff       (20)     1492 2023-11-09 02:29:56.000000 vsdm-0.1.0/vsdm.egg-info/PKG-INFO
--rw-r--r--   0 Ben        (501) staff       (20)      357 2023-11-09 02:29:56.000000 vsdm-0.1.0/vsdm.egg-info/SOURCES.txt
--rw-r--r--   0 Ben        (501) staff       (20)        1 2023-11-09 02:29:56.000000 vsdm-0.1.0/vsdm.egg-info/dependency_links.txt
--rw-r--r--   0 Ben        (501) staff       (20)       40 2023-11-09 02:29:56.000000 vsdm-0.1.0/vsdm.egg-info/requires.txt
--rw-r--r--   0 Ben        (501) staff       (20)        5 2023-11-09 02:29:56.000000 vsdm-0.1.0/vsdm.egg-info/top_level.txt
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2024-04-11 07:32:37.629692 vsdm-0.2.9/
+-rw-r--r--   0 Ben        (501) staff       (20)     1065 2023-10-02 10:21:17.000000 vsdm-0.2.9/LICENSE
+-rw-r--r--   0 Ben        (501) staff       (20)     2342 2024-04-11 07:32:37.629177 vsdm-0.2.9/PKG-INFO
+-rw-r--r--   0 Ben        (501) staff       (20)     1606 2024-04-11 05:15:56.000000 vsdm-0.2.9/README.md
+-rw-r--r--   0 Ben        (501) staff       (20)      892 2024-04-11 04:07:16.000000 vsdm-0.2.9/pyproject.toml
+-rw-r--r--   0 Ben        (501) staff       (20)       38 2024-04-11 07:32:37.629787 vsdm-0.2.9/setup.cfg
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2024-04-11 07:32:37.626155 vsdm-0.2.9/vsdm/
+-rw-r--r--   0 Ben        (501) staff       (20)     1121 2024-04-11 07:30:48.000000 vsdm-0.2.9/vsdm/__init__.py
+-rw-r--r--   0 Ben        (501) staff       (20)    34335 2024-04-11 07:28:50.000000 vsdm-0.2.9/vsdm/adaptive.py
+-rw-r--r--   0 Ben        (501) staff       (20)     6788 2023-09-12 06:07:55.000000 vsdm-0.2.9/vsdm/analytic.py
+-rw-r--r--   0 Ben        (501) staff       (20)    14549 2024-04-11 06:37:36.000000 vsdm-0.2.9/vsdm/basis.py
+-rw-r--r--   0 Ben        (501) staff       (20)     8257 2024-04-11 06:18:46.000000 vsdm-0.2.9/vsdm/gaussians.py
+-rw-r--r--   0 Ben        (501) staff       (20)    35727 2024-04-11 06:37:56.000000 vsdm-0.2.9/vsdm/haar.py
+-rw-r--r--   0 Ben        (501) staff       (20)    20096 2024-04-11 06:38:15.000000 vsdm-0.2.9/vsdm/matrixcalc.py
+-rw-r--r--   0 Ben        (501) staff       (20)    19389 2024-04-11 06:16:35.000000 vsdm-0.2.9/vsdm/portfolio.py
+-rw-r--r--   0 Ben        (501) staff       (20)    28138 2024-04-11 07:07:38.000000 vsdm-0.2.9/vsdm/projection.py
+-rw-r--r--   0 Ben        (501) staff       (20)    11441 2023-10-02 09:42:35.000000 vsdm-0.2.9/vsdm/ratecalc.py
+-rw-r--r--   0 Ben        (501) staff       (20)     1544 2023-10-02 09:41:08.000000 vsdm-0.2.9/vsdm/units.py
+-rw-r--r--   0 Ben        (501) staff       (20)    21330 2024-04-11 06:36:50.000000 vsdm-0.2.9/vsdm/utilities.py
+-rw-r--r--   0 Ben        (501) staff       (20)     4056 2023-09-13 23:40:43.000000 vsdm-0.2.9/vsdm/wigner.py
+drwxr-xr-x   0 Ben        (501) staff       (20)        0 2024-04-11 07:32:37.628659 vsdm-0.2.9/vsdm.egg-info/
+-rw-r--r--   0 Ben        (501) staff       (20)     2342 2024-04-11 07:32:37.000000 vsdm-0.2.9/vsdm.egg-info/PKG-INFO
+-rw-r--r--   0 Ben        (501) staff       (20)      387 2024-04-11 07:32:37.000000 vsdm-0.2.9/vsdm.egg-info/SOURCES.txt
+-rw-r--r--   0 Ben        (501) staff       (20)        1 2024-04-11 07:32:37.000000 vsdm-0.2.9/vsdm.egg-info/dependency_links.txt
+-rw-r--r--   0 Ben        (501) staff       (20)       46 2024-04-11 07:32:37.000000 vsdm-0.2.9/vsdm.egg-info/requires.txt
+-rw-r--r--   0 Ben        (501) staff       (20)        5 2024-04-11 07:32:37.000000 vsdm-0.2.9/vsdm.egg-info/top_level.txt
```

### Comparing `vsdm-0.1.0/LICENSE` & `vsdm-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vsdm-0.1.0/pyproject.toml` & `vsdm-0.2.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.7"
 dependencies = [
+    "numba",
     "scipy",
     "vegas",
     "h5py",
     "spherical",
     "quaternionic",
 ]
 dynamic = ["version"]
@@ -29,15 +30,11 @@
 Homepage = "https://github.com/blillard/vsdm"
 Source = "https://github.com/blillard/vsdm/"
 Documentation = "https://github.com/blillard/vsdm/blob/main/README.md"
 
 [tool.setuptools]
 packages = ["vsdm"]
 
-# [tool.setuptools.packages.find]
-# where = ["vsdm"]
-# exclude = ["tools*"]
-
 [tool.setuptools.dynamic]
 version = {attr = "vsdm.__version__"}
 
 #
```

### Comparing `vsdm-0.1.0/vsdm/analytic.py` & `vsdm-0.2.9/vsdm/analytic.py`

 * *Files identical despite different names*

### Comparing `vsdm-0.1.0/vsdm/basis.py` & `vsdm-0.2.9/vsdm/utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,591 +1,639 @@
-"""VSDM: orthogonal basis functions for class Basis().
+"""Functions for general use: physics functions, GVAR matrix conversions.
 
-Functions and classes:
-    ylm_real: real spherical harmonics. Uses plm_real
-    lag_spherical: spherical Laguerre functions
-    haar_sph: spherical wavelet functions
-    class Basis: defines an orthogonal basis of functions
-        methods for <f|nlm> integration, f(r) = sum_nlm(<nlm|f>|nlm>) summation
-
-Functions here are all dimensionless: no need for .units
+Physics functions:
+    fdm2_n: DM-SM particle scattering form factor, normalized to F(q=q0) = 1.
+        Value of q0 = q0_fdm is defined in units.py in units of qBohr.
+    g_k0: scattering event rate scaling factor with target exposure
+These functions require .units, e.g. for q0 and g_k0().
+
+Mathematics:
+    plm_norm: normalized associated Legendre polynomials
+    ylm_real: real spherical harmonics (m<0 -> sin(m phi), m>0 -> cos(m phi))
+        Using plm_norm for substantially faster evaluation.
+    ylm_cx: complex-valued spherical harmonics (also using plm_norm).
+    sph_to_cart, cart_to_sph: Cartesian/spherical coordinate conversions.
+    NIntegrate: multipurpose numerical integrator. Methods include VEGAS
+        or gaussian quadrature from scipy.
+
+Utilities:
+    makeNLMlist: produces complete list of (nlm) coefficients given
+      values for nMax and ellMax, n=0,1...nMax and ell=0,1,...ellMax
+    splitGVARarray: separates gvar valued matrix into f.mean, f.sdev matrices
+    joinGVARarray: combines f.mean, f.sdev matrices into gvar valued matrix
+
+Interpolation:
+    Interpolator: 1d interpolation object, representing f(x) with a
+        piecewise-defined polynomial function.
+    Interpolator3d: represents a 3d function as a sum of spherical harmonics.
+        Contains a dictionary of 1d Interpolator objects, labeled by (l,m).
 """
 
-__all__ = ['Basis', 'lag_spherical', 'cubic_sph_haar_x',
-           'haar_sph', '_haar_sph_value', '_tophat_value']
-           #'_hindex_LM', '_hindex_n'
+__all__ = ['g_k0', 'fdm2_n', 'mathsinc', 'dV_sph',
+           'plm_real', 'plm_norm', 'ylm_real', 'ylm_cx', 'ylm_scipy',
+           'makeNLMlist',
+           'splitGVARarray', 'joinGVARarray', '_LM_to_x', '_x_to_LM',
+           'sph_to_cart', 'cart_to_sph', 'compare_index_to_shape',
+           '_map_int_to_index', 'gX_to_tgX', 'assign_indices',
+           'getLpower', 'getLMpower', 'getNLMpower', 'NIntegrate',
+           'Interpolator', 'Interpolator3d']
 
 import math
+import numba
 import numpy as np
 import scipy.special as spf
-import vegas # numeric integration
+import scipy.integrate as sint # gaussian quadrature
+import vegas # Monte Carlo integration
 import gvar # gaussian variables; for vegas
-# import time
-# import quaternionic # For rotations
-# import spherical #For Wigner D matrix
-# import csv # file IO for projectFnlm
-# import os.path
-# import h5py # database format
 
-from .utilities import *
+from .units import *
+
 
+### Scaling factor for exposure*sigma0*rhoX
+def g_k0(exp_kgyr=1., mCell_g=1., sigma0_cm2=1e-40,
+         rhoX_GeVcm3=0.4, v0=220.*km_s, q0=qBohr):
+    # 1 year = 365.0 days in 'kgyr'
+    return 3288.95 *( (1.0/mCell_g) * (exp_kgyr/1.) * (sigma0_cm2/1e-40)
+        * (rhoX_GeVcm3/0.4) * (v0/(220.*km_s))**2 * (qBohr/q0) )
+
+### Physics function: squared form factor for DM-SM particle scattering
+def fdm2_n(q, n):
+    """DM-SM scattering form factor, F_DM(q) = (q0/q)**n for integer n."""
+    # F = (q0/q)^n. Normalized to F(q0)=1.
+    #  Default: q0 = alpha*mE.
+    # Function returns F^2, e.g. F^2 = 1 or F^2 = 1/q^4.
+    if n==0:
+        return 1
+    return (q0_fdm/q)**(2*n)
 
 """
-    Spherical Laguerre functions:
+    Mathematics functions: dV_sph integration Jacobian
 """
+### Differing conventions:
+# numpy/scipy sinc functions are normalized with extra factor of pi
+# the incomplete Gamma(s,z) function is implemented as Gamma(s)*spf.gammaincc(s,z)
+
+def mathsinc(z):
+    ## mathsinc = sin(z)/z, whereas numpy.sinc(z) = sin(pi z)/(pi z)
+    return np.sinc(z / np.pi)
+
+def dV_sph(rvec):
+    ## rvec = [r, theta, phi]
+    return rvec[0]**2 * math.sin(rvec[1])
 
-def _lag_half_ln(n, ell, z):
-    return spf.genlaguerre(n, 1/2+ell, monic=False)(z)
-
-def lag_spherical(n, ell, x):
-    """Normalized spherical Laguerre function"""
-    #includes exponential factor! Dimensionless x
-    factor = math.sqrt(math.factorial(n) * 2**(2.5+ell) / spf.gamma(n+1.5+ell))
-    return factor * math.exp(-x**2) * x**ell * _lag_half_ln(n, ell, 2*x**2)
 
 """
-    Spherical wavelet functions:
+    Plm and Ylm functions
 """
 
-#Defining an index for the haar wavelets: n = 2**L + M (n=0 for L=-1)
-def _hindex_n(L, M):
-    if L==-1:
-        return 0
-    else:
-        return 2**L + M
+def plm_real(ell, m, z):
+    """scipy version of associated Legendre polynomials.
 
-def _hindex_LM(n):
-    if n==0:
-        return [-1, 0]
+    Reliable up to ell=150 (m=0,1,...,150), but can produce
+        incorrect results in Ylm when multiplied against sqrt(factorials).
+    Very slow.
+    """
+    ## lpmn calculates P_mn(z) for all m and n less than or equal to the m,n provided.
+    # A more efficient code would vectorize Ylm to take advantage of this
+    return spf.lpmn(math.fabs(m), ell, z)[0][-1][-1]
+
+def ylm_scipy(ell, m, theta, phi):
+    absm = int(math.fabs(m))
+    # math.factorial is faster by 20%, but scipy.gamma allows ell > 100
+    sqrtfact = (-1)**m * (math.sqrt((2*ell+1)/(4*math.pi)
+        # * math.factorial(ell - absm) / math.factorial(ell + absm)))
+        * spf.gamma(ell - absm + 1) / spf.gamma(ell + absm + 1)))
+    Plmpart = plm_real(ell, m,math.cos(theta))
+    if m < 0:
+        return math.sqrt(2) * sqrtfact * Plmpart * math.sin(absm * phi)
+    elif m==0:
+        return sqrtfact * Plmpart
     else:
-        L = int(math.log2(n))
-        M = n - 2**L
-        return [L, M]
+        return math.sqrt(2) * sqrtfact * Plmpart * math.cos(m * phi)
 
-def _haar_sph_value(n):
-    """Returns the value of h_n(x) where it is nonzero."""
-    if n==0:
-        return math.sqrt(3)
-    else:
-        [L,M] = _hindex_LM(n)
-        x1 = 2**(-L) * M
-        x2 = 2**(-L) * (M+0.5)
-        x3 = 2**(-L) * (M+1)
-        y1 = x1**3
-        y2 = x2**3
-        y3 = x3**3
-        A = math.sqrt(3/(y3 - y1) * (y3-y2)/(y2-y1))
-        B = math.sqrt(3/(y3 - y1) * (y2-y1)/(y3-y2))
-        return [A,-B]
 
-def haar_sph(n, x):
-    """Normalized spherical Haar wavelet, n=0,1,2,..."""
-    if n==0:
-        if 0 <= x <= 1:
-            return _haar_sph_value(n)
-        else:
-            return 0
+@numba.jit("double(uint32,uint32,double)", nopython=True,
+           locals={'m_sqrd':numba.double, 'Pk':numba.double,
+                   'Pk_minus2':numba.double,
+                   'Pk_minus1':numba.double,
+                   'x2':numba.double, 'sqrt_1_x2':numba.double})
+def plm_norm(ell, m, x):
+    """The 'normalized' associated Legendre polynomials.
+
+    Defined as: (-1)**m * sqrt[(l-m)! / (l+m)!] * P_lm(x)
+    For m=0, this is identical to the usual P_l(x).
+
+    Method:
+    * Using Bonnet recursion for the m=0 special case (upwards from l=0,1).
+    * For m>0, using 'horizontal' recursion from (m,m) to (l,m),
+        using the 'associated' Bonnet recursion relations.
+
+    Numerically stable for all x in [-1,1], even arbitrarily close to x**2=1.
+    (e.g. x = 1 - 1e-15).
+    Permits the accurate calculation of P_lm(x) up to at least ell=m=1e6.
+    """
+    # poch_plus = 1. # (l+m)!/l!
+    # poch_minus = 1. # l!/(l-m)!
+    if ell==0:
+        return 1
+    x2 = x**2
+    if x2==1:
+        # Evaluate now, to avoid 1/sqrt(1-x**2) division errors.
+        return int(m==0) * (x)**(m%2)
+    sqrt_1_x2 = (1-x2)**0.5
+    if m==0:
+        # Upward recursion along m=0 to (l,0). Bonnet:
+        if ell==1:
+            return x
+        Pk_minus2 = 1
+        Pk_minus1 = x
+        for k in range(2, ell+1):
+            Pk = ((2-1/k)*x*Pk_minus1 - (1-1/k)*Pk_minus2)
+            Pk_minus2 = Pk_minus1
+            Pk_minus1 = Pk
+        return Pk
+        # get the (l,1) term, from the (l-1,0) and (l,0) Legendre polynomials:
+    # else: use horizontal recursion from (m,m) to (ell,m)
+    # modified Bonnet:
+    sqrt_1_x2 = (1-x2)**0.5
+    m_sqrd = 1. # l!/(l-m)! * l!/(l+m)!
+    for i in range(m):
+        # until i=m-1:
+        m_sqrd *= 1 - 0.5/(1+i)
+    Pk_minus2 = sqrt_1_x2**m * m_sqrd**0.5 #l=m
+    if ell==m:
+        return Pk_minus2
+    Pk_minus1 = (2*m+1)**0.5 * x * Pk_minus2 #l=m+1
+    if ell==m+1:
+        return Pk_minus1
+    for k in range(m+2, ell+1):
+        Pk = ((2*k-1)*x*Pk_minus1 - ((k-1)**2-m**2)**0.5*Pk_minus2)/(k**2-m**2)**0.5
+        Pk_minus2 = Pk_minus1
+        Pk_minus1 = Pk
+    return Pk
+
+
+@numba.jit("complex128(uint32,int32,double,double)", nopython=True)
+def ylm_cx(ell, m, theta, phi):
+    "Complex-valued spherical harmonics."
+    phase_phi = np.exp(1j * m * phi)
+    if m < 0:
+        m = -m
     else:
-        [L,M] = _hindex_LM(n)
-        x1 = 2**(-L) * M
-        x2 = 2**(-L) * (M+0.5)
-        x3 = 2**(-L) * (M+1)
-        if x1 <= x < x2:
-            return _haar_sph_value(n)[0]
-        elif x2 < x <= x3:
-            return _haar_sph_value(n)[1]
-        elif x==x2:
-            return 0.5*(_haar_sph_value(n)[0] + _haar_sph_value(n)[1])
-        else:
-            return 0
+        phase_phi *= (-1)**(m%2)
+    return ((2*ell+1)/(4*np.pi))**0.5 * phase_phi * plm_norm(ell, m, np.cos(theta))
 
-def _tophat_value(x1, x2):
-    """Returns the value of the tophat function where it is nonzero.
+@numba.jit("double(uint32,int32,double,double)", nopython=True)
+def ylm_real(ell, m, theta, phi):
+    "Real-valued spherical harmonics."
+    if m==0:
+        return ((2*ell+1)/(4*np.pi))**0.5 * plm_norm(ell, m, np.cos(theta))
+    if m < 0:
+        m = -m
+        return ((2*ell+1)/(2*np.pi))**0.5 * plm_norm(ell, m, np.cos(theta)) * np.sin(m*phi)
+    return ((2*ell+1)/(2*np.pi))**0.5 * plm_norm(ell, m, np.cos(theta)) * np.cos(m*phi)
 
-    i.e. for x1 < x < x2. Assuming x1 != x2, and that both are nonnegative.
-    Normalized for int(x^2 dx * value**2, {x, x1, x2}) = 1.
-    """
-    return math.sqrt(3/(x2**3 - x1**3))
 
 
-def _Hp_sph_n(p, n):
-    "H_p function for spherical wavelet extrapolation"
-    A, mB = _haar_sph_value(n)
-    B = - mB
-    L,M = _hindex_LM(n)
-    # x1 = 2**(-L) * M
-    # x2_Delta = (M+0.5)
-    # x3 = 2**(-L) * (M+1)
-    Delta = 2**(-L)
-    term0 = ((-1)**p*A - B)/(p+3)
-    term1 = -4*(M+0.5) * ((-1)**p*A + B)/(p+2)
-    term2 = 4*(M+0.5)**2 * ((-1)**p*A - B)/(p+1)
-    return Delta**3/8 * (term0 + term1 + term2)
-
-
-def cubic_sph_haar_x(df_123, n):
-    "Predicts <f|n> for radial function f(0<x<1) given df/dx derivatives at x2"
-    # (df1, df2, df3) = df_123
-    L,M = _hindex_LM(n)
-    Delta = 2**(-L)
-    sum = 0.0
-    for p in [1,2,3]:
-        Fp = (0.5*Delta)**p / math.factorial(p) * df_123[p-1]
-        sum += Fp * _Hp_sph_n(p, n)
-    return sum
 
+"""
+    functions for (nlm) lists and gvar/[mean,sdev] conversions:
+"""
 
+def _LM_to_x(ell, m, phi_symmetric=False):
+    # Maps (ell, m) onto an index ix=0,1,2,3...
+    if phi_symmetric:
+        return ell
+    else:
+        return ell*(ell+1) + m
 
-class Basis():
-    """Defines a set of (nlm) basis functions for any type.
+def _x_to_LM(x, phi_symmetric=False):
+    if phi_symmetric:
+        ell = x
+        m = 0
+    else:
+        ell = int(math.floor(math.sqrt(x)))
+        m = x - ell*(ell+1)
+    return ell,m
+
+def makeNLMlist(nMax, lMax, nMin=0, lMin=0,
+                mSymmetry=None, lSymmetry=None, phi_even=False):
+    # For most basis choices, nMin = 0. For tophat, nMin = 1.
+    lList = []
+    if lSymmetry is None or lSymmetry==0 or lSymmetry==False:
+        for l in range(lMin, lMax+1):
+            lList += [l]
+    else:
+        assert (type(lSymmetry) is int), "lSymmetry must be integer-valued or None"
+        for l in range(lMin, lMax+1):
+            if (l%lSymmetry)==0:
+                lList += [l]
+    nlmlist = []
+    if mSymmetry in [None,0,False]:
+        if phi_even:
+            nlmlist = [(n,l,m) for l in lList for m in range(0, l+1)
+                       for n in range(nMin, nMax+1) ]
+        else:
+            nlmlist = [(n,l,m) for l in lList for m in range(-l, l+1)
+                       for n in range(nMin, nMax+1)]
+    elif mSymmetry==True or mSymmetry=='U(1)':
+        nlmlist = [(n,l,0) for n in range(nMin, nMax+1) for l in lList]
+    else:
+        assert (type(mSymmetry) is int), "mSymmetry must be integer-valued, boolean or None"
+        lmList = []
+        for l in lList:
+            if phi_even:
+                for m in range(0, l+1):
+                    if (m%mSymmetry)==0:
+                        lmList += [(l,m)]
+            else:
+                for m in range(-l, l+1):
+                    if (m%mSymmetry)==0:
+                        lmList += [(l,m)]
+        nlmlist = [(n,l,m) for (l,m) in lmList for n in range(nMin, nMax+1)]
+    return nlmlist
+
+def compare_index_to_shape(index, shape):
+    "Returns an array large enough to accommodate new index and original shape."
+    # index: for entry in array. shape: of array
+    # Returns: shape of original array, or one enlarged to include index
+    assert(len(index)==len(shape)), "Error: incompatible objects"
+    dim = len(index) # dimensionality of array
+    larger_shape = shape
+    for i in range(dim):
+        if (index[i] + 1) > larger_shape[i]:
+            larger_shape[i] = index[i] + 1
+    return larger_shape
+
+def _map_int_to_index(ix, shape):
+    """Given array shape, maps integer ix to array index."""
+    # Get multiplicative factors
+    dim = len(shape)
+    ncoeffs = 1
+    for i in range(dim):
+        ncoeffs *= shape[i]
+    if ix >= ncoeffs or ix < 0:
+        return "Error: index out of range."
+    mult_factor = []
+    mfactor = ncoeffs
+    for i in range(dim):
+        mfactor = int(mfactor / shape[i])
+        mult_factor += [mfactor]
+    # mult_factors is done. Ordered to match consecutive for loop style
+    new_x = ix
+    index = []
+    for i in range(dim):
+        index_i = new_x // mult_factor[i]
+        rem_i = new_x % mult_factor[i] # remainder carried to i+= 1
+        i += 1
+        new_x = rem_i
+        index += [index_i]
+    return tuple(index)
+
+def _map_index_to_int(index, shape):
+    """Given array shape, maps array index to integer. Currently unused."""
+    dim = len(shape)
+    if (len(index)!=dim):
+        return "Error: incompatible objects."
+    if shape!=compare_index_to_shape(index, shape):
+        return "Error: index out of range."
+    # Get multiplicative factors
+    ncoeffs = 1
+    for i in range(dim):
+        ncoeffs *= shape[i]
+    mult_factor = []
+    mfactor = ncoeffs
+    for i in range(dim):
+        mfactor = int(mfactor / shape[i])
+        mult_factor += [mfactor]
+    # mult_factors is done. Ordered to match consecutive for loop style
+    out = 0
+    for i in range(dim):
+        out += mult_factor[i] * index[i]
+    # out: a unique integer in 0, 1, 2, ..., ncoeffs-1.
+    return out
+
+def assign_indices(listlength, pn_cpus):
+    """Assigns a list of indices to processor 'p', one of 'n' total."""
+    (p_index, nprocesses) = pn_cpus
+    # this is for the pth process out of a total of n
+    index_list = []
+    index = p_index
+    while index < listlength:
+        index_list += [index]
+        index += nprocesses
+    return index_list
+
+def splitGVARarray(mxgvar):
+    mxshape = np.shape(mxgvar)
+    dim = len(mxshape) # dimensionality of array
+    ncoeffs = 1
+    for i in range(dim):
+        ncoeffs *= mxshape[i]
+    mxMean = np.zeros(mxshape, dtype='float')
+    mxSdev = np.zeros(mxshape, dtype='float')
+    for ix in range(ncoeffs):
+        index = _map_int_to_index(ix, mxshape)
+        mgv = mxgvar[index]
+        if (type(mgv) is float) or (type(mgv) is int):
+            mgv *= gvar.gvar(1., 0)
+        mxMean[index] = mgv.mean
+        mxSdev[index] = mgv.sdev
+    return mxMean, mxSdev
+
+def joinGVARarray(mxmean, mxsdev):
+    mxshape = np.shape(mxmean)
+    dim = len(mxshape) # dimensionality of array
+    ncoeffs = 1
+    for i in range(dim):
+        ncoeffs *= mxshape[i]
+    mxgvar = np.zeros(mxshape, dtype='object')
+    for ix in range(ncoeffs):
+        index = _map_int_to_index(ix, mxshape)
+        m_mean = mxmean[index]
+        if mxsdev is not None:
+            m_sdev = mxsdev[index]
+        else:
+            m_sdev = 0.0
+        mxgvar[index] = gvar.gvar(m_mean, m_sdev)
+    return mxgvar
+
+def sph_to_cart(uSph):
+    """Converts vectors from spherical to Cartesian coordinates."""
+    (u, theta, phi) = uSph
+    ux = u * math.sin(theta) * math.cos(phi)
+    uy = u * math.sin(theta) * math.sin(phi)
+    uz = u * math.cos(theta)
+    return (ux, uy, uz)
+
+def cart_to_sph(uXYZ):
+    """Converts vectors from Cartesian to spherical coordinates."""
+    (ux, uy, uz) = uXYZ
+    u = math.sqrt(ux**2 + uy**2 + uz**2)
+    uxy = math.sqrt(ux**2 + uy**2)
+    # first address uxy=0 and ux=0 special cases...
+    phi = 0 #arbitrary; phi not well defined at theta=0,pi
+    if uxy==0:
+        if uz >= 0:
+            theta = 0
+        else:
+            theta = math.pi
+        return (u, theta, phi)
+    theta = 0.5*math.pi - math.atan(uz/uxy)
+    # ux=0...
+    if ux == 0:
+        if uy > 0:
+            phi = 0.5*math.pi
+        elif uy < 0:
+            phi = 1.5*math.pi
+        return (u, theta, phi)
+    # Now, non-special cases...
+    if ux > 0 and uy > 0:
+        phi = math.atan(uy/ux)
+    elif ux < 0 and uy < 0:
+        phi = math.atan(uy/ux) + math.pi
+    elif ux < 0 and uy > 0:
+        phi = math.atan(uy/ux) + math.pi
+    elif ux > 0 and uy < 0:
+        phi = math.atan(uy/ux) + 2*math.pi
+    return (u, theta, phi)
+
+def gX_to_tgX(gauss, u0):
+    tgauss_vecs = gauss.rescaleGaussianF(u0**3)
+    return vs3dm.GaussianF(tgauss_vecs)
+
+def getNLMpower(f_nlm):
+    #assemble
+    powerNLM = {}
+    for nlm,fnlm in f_nlm.items():
+        powerNLM[nlm] = fnlm**2
+    #sort
+    sortnlm = sorted(powerNLM.items(),
+                    key=lambda z: z[1], reverse=True)
+    powerNLM = {}
+    for key,power in sortnlm:
+        powerNLM[key] = power
+    return powerNLM
+
+def getLMpower(f_nlm):
+    #assemble
+    powerLM = {}
+    for nlm,fnlm in f_nlm.items():
+        (n, l, m) = nlm
+        if (l, m) in powerLM.keys():
+            powerLM[(l, m)] += fnlm**2
+        else:
+            powerLM[(l, m)] = fnlm**2
+    #sort
+    sortlm = sorted(powerLM.items(),
+                    key=lambda z: z[1], reverse=True)
+    powerLM = {}
+    for key,power in sortlm:
+        powerLM[key] = power
+    return powerLM
+
+def getLpower(f_nlm):
+    #assemble
+    powerL = {}
+    for nlm,fnlm in f_nlm.items():
+        (n, l, m) = nlm
+        if l in powerL.keys():
+            powerL[l] += fnlm**2
+        else:
+            powerL[l] = fnlm**2
+    #sort
+    sortl = sorted(powerL.items(),
+                   key=lambda z: z[1], reverse=True)
+    powerL = {}
+    for key,power in sortl:
+        powerL[key] = power
+    return powerL
+
+
+# Numerical integration with gaussian quadrature:
+def intGaussQuad(integrand, volume, quadg_params):
+    """Gaussian quadrature integrals, using quadg_params dictionary.
 
-    Arguments:
-        basis: a dictionary including the following: (mandatory)
-        * type = 'laguerre', 'wavelet', 'tophat'
-        * u0: sets normalization of |nlm>
-            is the scale factor for infinite-domain radial functions
-        conditional/optional items:
-        * uiList: mandatory for 'tophat', the list of u_i to be used
-        * uMax: mandatory for 'laguerre', setting the limit of integration on u.
-            For 'wavelet' and 'tophat', can set uMax=None.
-        * dim = 3,4: if ==4, adds generation of (etype,e0,eiList,eMax)
-            Not strictly mandatory. Defaults to dim=3 if missing.
-    Methods and variables:
-        .basis: dict with (type, u0, uMax, uiList, etc.)
-        radRn(n, ell,u): radial function r^{ell}_n(u), with dimensionful u
-            Passes dimensionless u/u0 to appropriate basis function
-        phiNLM(nlm,uvec): basis function (n,l,m), for uvec=[r, theta, phi]
-            Normalized: integral(d3r/u0**3 * phi(nlm) * phi(nlm)) = 1
-        getFnlm(f, nlm): evaluates <f|nlm> for function f(uvec)
-        get1nlm(nlm): returns <1|nlm>, used in comparisons with L1 normalized gX
-        nlmAssembleFu(f_nlm, uvec): returns an approximation of f(uvec),
-            from sum of <f|nlm> |nlm> over all (nlm)
+    Using VEGAS form of integrand([x1,x2,...]), volume=[[x1a,x1b],[x2a,x2b]...]
+    quadg_params: a dict containing the precision goals
     """
-    # For now, not including spherical bessel functions.
-    # For j_ell, need to initialize list of zeros, alpha_{l,n}
-    def __init__(self, bdict):
-        """Makes self.basis, self.u0, """
-        self.basis = bdict
-        update_dict = self.runBasisCheck(bdict)
-        for lbl,entry in update_dict.items():
-            self.basis[lbl] = entry
-        self.uMax = self.basis['uMax']
-
-    def runBasisCheck(self, bdict):
-        """Ensures mandatory items are included, generates class variables.
-
-        Arguments:
-            bdict: dictionary of basis parameters
-        Returns: dict 'updates' of entries in self.basis that should be updated,
-                e.g. to define 'uMax' from 'u0' if appropriate
-        """
-        updates = {}
-        assert('u0' in bdict), "Missing mandatory parameter: 'u0'."
-        self.u0 = bdict['u0']
-        assert('type' in bdict), "Missing mandatory parameter: 'type'."
-        uType = bdict['type']
-        if uType=="wavelet":
-            assert('uMax' in bdict), "Missing mandatory parameter: 'uMax'."
-            # else:
-            #     assert(self.u0 == bdict['uMax']), "wavelet: require u0=uMax."
-        elif uType=='tophat':
-            assert('uiList' in bdict), "tophat: need uiList."
-            #uiList should be ordered and nonnegative
-            self.uiList = bdict['uiList']
-            assert(all(self.uiList[i] < self.uiList[i+1]
-                       for i in range(len(self.uiList) - 1))), "tophat: uiList must be ordered"
-            assert(self.uiList[0] >= 0), "tophat: all u_i must be nonnegative"
-            if 'uMax' not in bdict:
-                updates['uMax'] = bdict['uiList'][-1]
-            else:
-                assert(bdict['uMax'] == bdict['uiList'][-1]), "tophat: require uMax=uiList[-1]."
-        elif uType=="laguerre":
-            assert('uMax' in bdict), "Missing mandatory parameter: 'uMax'."
-        return updates
-
-    def radRn(self, n, ell, u):
-        """Dimensionless radial function r_n^(ell)(u).
-
-        Normalized: integral(u**2 du/u0**3 radRn**2) = 1,
-            in limit where uMax=infinity
-        ell: specifies type of function for Laguerre, Bessel
-        n: index n=0,1,2,...nMax.
-            For 'tophat', counting starts at n=0,1,2,3,...nMax-1.
-        """
-        x = u/self.u0
-        if self.basis['type']=="wavelet":
-            return haar_sph(n, x)
-        elif self.basis['type']=="laguerre":
-            return lag_spherical(n, ell, x)
-        elif self.basis['type']=="tophat":
-            #x_n = u_n / u0
-            x_n,x_np1 = self.uiList[n]/self.u0, self.uiList[n+1]/self.u0
-            if x_n < x < x_np1:
-                return _tophat_value(x_n, x_np1)
-                # return _tophat_value(x_nm1, x_n)
-            else:
-                return 0
+    if 'rtol' in quadg_params:
+        rtol = quadg_params['rtol']
+    else:
+        rtol = 1e-6
+    if 'atol' in quadg_params:
+        atol = quadg_params['atol']
+    elif 'atol_f' in quadg_params:
+        atol = quadg_params['atol_f']
+    elif 'atol_e' in quadg_params:
+        atol = quadg_params['atol_e']
+    else:
+        atol = 1e-6
+    verbose = False
+    if 'verbose' in quadg_params:
+        verbose = quadg_params['verbose']
+    # complex = False
+    # if 'complex' in quadg_params:
+    #     complex = quadg_params['complex']
+    ndim = len(volume) # dimensionality
+    assert ndim in [1,2,3], "Only using quadrature for 1d, 2d, or 3d integrands"
+    if ndim==1:
+        def sciFunc(x):
+            return integrand([x])
+        result = sint.quad(sciFunc, volume[0][0], volume[0][1],
+                           epsabs=atol, epsrel=rtol)
+    elif ndim==2:
+        def sciFunc(x,y):
+            return integrand([x,y])
+        # note: scipy uses backwards func(y,x) ordering
+        result = sint.dblquad(sciFunc, volume[1][0], volume[1][1],
+                              volume[0][0], volume[0][1],
+                              epsabs=atol, epsrel=rtol)
+    elif ndim==3:
+        def sciFunc(x,y,z):
+            return integrand([x,y,z])
+        # note: scipy uses backwards func(z,y,x) ordering
+        result = sint.tplquad(sciFunc, volume[2][0], volume[2][1],
+                              volume[1][0], volume[1][1],
+                              volume[0][0], volume[0][1],
+                              epsabs=atol, epsrel=rtol)
+    value, error = result
+    resultGVAR = gvar.gvar(value, error)
+    if verbose:
+        print(resultGVAR)
+    return resultGVAR
+
+
+# Numerical integration with VEGAS:
+def intVegas(integrand, volume, vegas_params):
+    "Tool for performing VEGAS integrals using vegas_params dictionary."
+    # Unpack VEGAS parameters
+    nitn_init = vegas_params['nitn_init']
+    nitn = vegas_params['nitn']
+    neval = int(vegas_params['neval'])
+    if 'verbose' in vegas_params:
+        verbose = vegas_params['verbose']
+    else:
+        verbose = False
+    if 'neval_init' in vegas_params:
+        neval_init = int(vegas_params['neval_init'])
+    else:
+        neval_init = neval
+    dim = len(volume) # dimensionality of the integral
+    # Perform the integration:
+    integrator = vegas.Integrator(volume)
+    # adjust integrator to integrand:
+    integrator(integrand, nitn=nitn_init, neval=neval)
+    result = integrator(integrand, nitn=nitn, neval=neval)
+    if verbose:
+        print(result.summary())
+    return result
+
+def NIntegrate(integrand, volume, integ_params, printheader=None):
+    "Numerical integration, using VEGAS or scipy.integrate.quad."
+    if 'method' not in integ_params:
+        integ_params['method'] = 'vegas'
+    if 'verbose' not in integ_params:
+        integ_params['verbose'] = False
+    if integ_params['verbose']==True and printheader is not False:
+        print(printheader)
+    # Numerical Integration:
+    if integ_params['method'] == 'vegas':
+        out = intVegas(integrand, volume, integ_params)
+    elif integ_params['method'] == 'gquad':
+        out = intGaussQuad(integrand, volume, integ_params)
+    return out
 
 
-    def _baseOfSupport_n(self, n, getMidpoint=False):
-        """Returns the range in u for which radRn(u) is nonzero
+class Interpolator():
+    """Interpolated representation of a 1d function f(u).
 
-        For wavelets, also provides the mid-point if (getMidpoint)
-            (Used for analytic MathcalI.)
-        When used to provide integration range for Vegas,
-            keep getMidpoint=False.
-        """
-        if self.basis['type']=='tophat':
-            return [self.uiList[n], self.uiList[n+1]]
-        elif self.basis['type']=='wavelet' and getMidpoint:
-            if n==0:
-                return [0, self.uMax, self.uMax]
-            else:
-                [lam, mu] = _hindex_LM(n)
-                xA = 2**(-lam) * mu
-                xM = 2**(-lam) * (mu+0.5)
-                xB = 2**(-lam) * (mu+1)
-                return [xA*self.u0, xM*self.u0, xB*self.u0]
-        elif self.basis['type']=='wavelet' and not getMidpoint:
-            if n==0:
-                return [0, self.uMax]
-            else:
-                [lam, mu] = _hindex_LM(n)
-                xA = 2**(-lam) * mu
-                xB = 2**(-lam) * (mu+1)
-                return [xA*self.u0, xB*self.u0]
-        else:
-            return [0, self.uMax]
+    Arguments:
+        u_bounds: list of boundaries between interpolation regions, length [n+1]
+        u0_vals: points at which f derivatives are evaluated --> (u-u0)**p
+        f_p_list: derivatives d^(p)f/du^p, for p=0,1,2,3...
+            Note the inclusion of df_p[0] = f(x0).
+    """
 
-    def _volume_fraction_n(self, n, dim=3):
-        """Volume fraction occupied by nth basis function.
+    def __init__(self, u_bounds, u0_vals, f_p_list):
+        self.u_bounds = u_bounds
+        self.u0_vals = u0_vals
+        self.f_p_list = f_p_list
+
+    def __call__(self, u):
+        return self.fU(u)
+
+    def map_u_ix(self, u):
+        assert self.u_bounds[0] <= u <= self.u_bounds[-1], "u out of range"
+        n = 0
+        while u > self.u_bounds[n+1]:
+            n += 1
+        return n
+
+    def fU(self, u):
+        ix = self.map_u_ix(u)
+        u0 = self.u0_vals[ix]
+        df_p_x = self.f_p_list[ix]
+        fu = 0.0
+        for p,f_p in enumerate(df_p_x):
+            fu += f_p/math.factorial(p) * (u-u0)**p
+        return fu
+
+    def df_du_p(self, p, u):
+        "Derivative d^(p)f/du^p"
+        ix = self.map_u_ix(u)
+        df_p_x = self.f_p_list[ix]
+        sum = 0.0
+        for k in range(p, len(df_p_x)):
+            sum += df_p_x[k] * (u-u0)**(k-p) / math.factorial(k-p)
+        return sum
 
-        Used to adjust VEGAS neval points for (dim) dimensional integrals,
-            to sample all basis functions with the same density of points.
-        """
-        [uA, uB] = self._baseOfSupport_n(n, getMidpoint=False)
-        (xA, xB) = (uA/self.uMax, uB/self.uMax)
-        return xB**dim - xA**dim
 
-    def phiNLM(self, nlm, uvec):
-        """Dimensionless basis function |nlm> = r_n(r)*Y_lm(theta,phi).
 
-        Normalized: integral(r**2 dr dOmega / u0**3 * phiNLM**2) = 1.
-        """
-        (n, ell, m) = nlm # index: a 3-tuple
-        [r, theta, phi] = uvec # spherical coordinate: a vector
-        return self.radRn(n, ell, r) * ylm_real(ell, m, theta, phi)
+class Interpolator3d():
+    """Interpolated representation of a 3d function f(u) = sum_lm f_lm(u).
 
+    Arguments:
+        f_lm_dict: list of Interpolator objects, indexed by (lm)
+        complex: whether to use real or complex spherical harmonics
+    """
 
-    def get1nlm(self, n):
-        """Returns <1|nlm> inner product, for L1 integrals."""
-        # vanishes for all l > 0
-        if self.basis['type']=="laguerre":
-            return (-1)**n * (math.sqrt(math.pi * 2**2.5 / math.factorial(n))
-                              * math.sqrt(spf.gamma(n + 1.5)))
-        elif self.basis['type']=="wavelet":
-            if n==0:
-                return math.sqrt(4*math.pi/3)
-            else:
-                return 0
-        elif self.basis['type']=="tophat":
-            x_n,x_np1 = self.uiList[n]/self.u0, self.uiList[n+1]/self.u0
-            return math.sqrt(4*math.pi/3 * (x_np1**3 - x_n**3))
-
-    def doVegas(self, integrand, volume, vegas_params, printheader=None):
-        "Tool for performing VEGAS integrals using vegas_params dictionary."
-        # Unpack VEGAS parameters
-        nitn_init = vegas_params['nitn_init']
-        nitn = vegas_params['nitn']
-        neval = int(vegas_params['neval'])
-        verbose = vegas_params['verbose']
-        if 'neval_init' in vegas_params:
-            neval_init = int(vegas_params['neval_init'])
+    def __init__(self, f_lm_dict, complex=False):
+        self.f_lm = f_lm_dict
+        self.complex = complex
+
+    def __call__(self, uSph):
+        return self.fU(uSph)
+
+    def fU(self, uSph):
+        "Evaluating f(u) at a point uSph=(u,theta,phi)."
+        (u,theta,phi) = uSph
+        fu = 0.
+        if self.complex:
+            for lm,Flm in self.f_lm.items():
+                (ell, m) = lm
+                f_lm_u = Flm(u)
+                fu += ylm_cx(ell, m, theta, phi) * f_lm_u
         else:
-            neval_init = neval
-        # For volume-weighted neval:
-        if 'weight_by_vol' in vegas_params:
-            weight_by_vol = vegas_params['weight_by_vol']
-        else:
-            weight_by_vol = True #default
-        if 'neval_min' in vegas_params:
-            neval_min = vegas_params['neval_min']
-        else:
-            neval_min = 1e3 # lower bound for neval_n in weight_by_vol version
-        # Adjust neval for volume of nth basis function:
-        if type(weight_by_vol) in [int, float]:
-            dim = weight_by_vol
-        else:
-            dim = len(volume) # dimensionality of the integral
-        if weight_by_vol:
-            urange = volume[0] # always in order (u, ang1, ang2...)
-            [u1, u2] = urange
-            volume_fraction = (u2/self.uMax)**dim - (u1/self.uMax)**dim
-            neval_n = neval * volume_fraction
-            neval_init_n = neval_init * volume_fraction
-            if neval_n < neval_min:
-                neval_n = neval_min
-            if neval_init_n < neval_min:
-                neval_init_n = neval_min
-        else:
-            neval_n = neval
-            neval_init_n = neval_init
-        neval_n = int(neval_n)
-        neval_init_n = int(neval_init_n)
-        if verbose and printheader is not None:
-            print(printheader)
-        """Perform the integration:"""
-        integrator = vegas.Integrator(volume)
-        # adjust integrator to integrand:
-        integrator(integrand, nitn=nitn_init, neval=neval_init_n)
-        result = integrator(integrand, nitn=nitn, neval=neval_n)
-        if verbose:
-            print(result.summary())
-        return result
-
-    def getFnlm(self, f_uvec, nlm, vegas_params, saveGnli=True):
-        """Performs <nlm|f> integration for function f of spherical vector uvec.
-
-        f_uvec can have the following attributes:
-        * is_gaussian: (boolean) if f_uvec is a GaussianF instance,
-            defined by a list of (c_i, uSph_i, sigma_i) parameters.
-        * z_even: (boolean) if f_uvec(x,y,z) = f_uvec(x,y,-z)
-            implies <lm|f> = 0 if (l+m) is odd
-        * phi_even: (boolean) if f_uvec(u,theta,phi) = f_uvec(u,theta,-phi)
-            implies <lm|f> = 0 if m is odd
-        * phi_cyclic: (integer) if f_uvec(u,theta,phi) = f_uvec(u,theta,phi + 2*pi/n)
-        * phi_symmetric: (boolean) if f_uvec(u,theta) independent of phi
-
-        If is_gaussian, then f_uvec is a GaussianF instance, defined by
-            a list of (c_i, uSph_i, sigma_i) parameters.
-        In this case, the function f(uvec) is called by f_uvec.gU(uvec).
-            <g|nlm> given by f_uvec.getGnlm(basisU, nlm, vegas_params).
-        Note: f_uvec.getGnlm() only performs numeric integration when the
-            corresponding f_uvec.G[(n,l,i)] have not been evaluated yet.
-        """
-        header = 'Calculating <f|nlm> for nlm: {}'.format(nlm)
-        headerA = 'Calculating <f|nlm(A)> for nlm: {}'.format(nlm)
-        headerB = 'Calculating <f|nlm(B)> for nlm: {}'.format(nlm)
-        # don't let getFnlm modify vegas_params:
-        if hasattr(f_uvec, 'is_gaussian') and f_uvec.is_gaussian==True:
-            fnlm = f_uvec.getGnlm(nlm, vegas_params, saveGnli=saveGnli)
-            return fnlm
-        if not hasattr(f_uvec, 'z_even') or f_uvec.z_even in [0, None]:
-            f_uvec.z_even = False
-        # if z_even, only integrate theta on [0, pi/2]
-        theta_Zn = 1
-        if f_uvec.z_even:
-            theta_Zn = 2
-        theta_region = [0, math.pi/theta_Zn]
-        # else: not is_gaussian. Use main getFnlm method:
-        (n, l, m) = nlm
-        if self.basis['type']=='wavelet' and n!=0:
-            # Split the integral in two for these cases:
-            [umin, umid, umax] = self._baseOfSupport_n(n, getMidpoint=True)
-        else:
-            [umin, umax] = self._baseOfSupport_n(n, getMidpoint=False)
-        # Check for azimuthal symmetry:
-        if hasattr(f_uvec, 'phi_symmetric') and f_uvec.phi_symmetric==True:
-            if m!=0 or (f_uvec.z_even and (l % 2 != 0)):
-                fnlm = gvar.gvar(0,0)
-                return fnlm
-            #else, m==0:  Skip the phi integral.
-            def integrand_m0(u_rth):
-                phi = 0.0 #arbitrary, function is constant wrt phi
-                uvec = (u_rth[0], u_rth[1], phi)
-                return (dV_sph(uvec)/(self.u0**3) * f_uvec(uvec)
-                        * self.phiNLM(nlm, uvec))
-            if self.basis['type']=='wavelet' and n!=0:
-                volume_A = [[umin,umid], theta_region] # 2d
-                volume_B = [[umid,umax], theta_region] # 2d
-                fnlmA = self.doVegas(integrand_m0, volume_A, vegas_params,
-                                     printheader=headerA)
-                fnlmB = self.doVegas(integrand_m0, volume_B, vegas_params,
-                                     printheader=headerB)
-                fnlm = 2*math.pi * theta_Zn * (fnlmA + fnlmB)
-            else:
-                volume_nl = [[umin, umax], theta_region]
-                fnlm = self.doVegas(integrand_m0, volume_nl,
-                                    vegas_params, printheader=header)
-            return 2*math.pi * theta_Zn * fnlm
-        # else: fSph is a function of 3d uvec = (u, theta, phi)
-        if not hasattr(f_uvec, 'phi_cyclic') or f_uvec.phi_cyclic in [0, None]:
-            f_uvec.phi_cyclic = 1
-        if not hasattr(f_uvec, 'phi_even') or f_uvec.phi_even in [0, None]:
-            f_uvec.phi_even = False
-        # check special cases:
-        if (f_uvec.z_even and (l+m) % 2 != 0) or (f_uvec.phi_even and m<0):
-            fnlm = gvar.gvar(0,0)
-            return fnlm
-        # for Z_n symmetric functions, only integrate phi on [0, 2*pi/n]
-        phi_region = [0, 2*math.pi/f_uvec.phi_cyclic]
-        def integrand_fnlm(uvec):
-            return (dV_sph(uvec)/(self.u0**3) * f_uvec(uvec)
-                    * self.phiNLM(nlm, uvec))
-        if self.basis['type']=='wavelet' and n!=0:
-            volume_A = [[umin, umid], theta_region, phi_region]
-            volume_B = [[umid, umax], theta_region, phi_region]
-            fnlmA = self.doVegas(integrand_fnlm, volume_A, vegas_params,
-                                 printheader=headerA)
-            fnlmB = self.doVegas(integrand_fnlm, volume_B, vegas_params,
-                                 printheader=headerB)
-            fnlm = fnlmA + fnlmB
-        else:
-            volume_nlm = [[umin, umax], theta_region, phi_region]
-            fnlm = self.doVegas(integrand_fnlm, volume_nlm, vegas_params,
-                                printheader=header)
-        return fnlm * f_uvec.phi_cyclic * theta_Zn
-
-
-    def nlmAssembleFu(self, f_nlm, uvec, nlmlist=None):
-        """Returns f(uvec) from f = sum_nlm(f_nlm * phi_nlm)."""
-        # here f_nlm is a dictionary of coefficients f_nlm indexed by (nlm)
-        if nlmlist is None:
-            nlmlist = f_nlm.keys()
-        f_uvec = 0.0
-        for nlm in nlmlist:
-            fX = f_nlm[(nlm)] * self.phiNLM(nlm, uvec)
-            f_uvec += fX
-        return f_uvec
-
-    def get_F123_sph_haar(self, f_0mp, n_0):
-        """F_p at center of n_0 wavelet, from coefficients f_0mp.
-
-        F_p = f^{(p)} (Delta/2)^p / p!           for f(x), 0 < x < 1,
-            = (d/du)^p g * (Delta_u/2)^p / p!    for g(u) = f(u/u0).
-        """
-        assert self.basis['type']=='wavelet', "Extrapolation only for wavelets"
-        # (L_minus, M_minus) = (L_0+1, 2*M_0)
-        # (L_plus, M_plus) = (L_0+1, 2*M_0+1)
-        n_m = 2*n_0
-        n_p = 2*n_0 + 1
-        H1_0 = _Hp_sph_n(1, n_0)
-        H2_0 = _Hp_sph_n(2, n_0)
-        H3_0 = _Hp_sph_n(3, n_0)
-        H1_m = _Hp_sph_n(1, n_m)
-        H2_m = _Hp_sph_n(2, n_m)
-        H3_m = _Hp_sph_n(3, n_m)
-        H1_p = _Hp_sph_n(1, n_p)
-        H2_p = _Hp_sph_n(2, n_p)
-        H3_p = _Hp_sph_n(3, n_p)
-        A1_m = 0.5*(H1_m )
-        A1_p = 0.5*(H1_p )
-        A2_m = 0.5*(H2_m - H1_m)
-        A2_p = 0.5*(H2_p + H1_p)
-        A3_m = 0.5*(H3_m - 1.5*H2_m + 0.75*H1_m)
-        A3_p = 0.5*(H3_p + 1.5*H2_p + 0.75*H1_p)
-        # column vectors
-        c1 = [H1_0, A1_m, A1_p]
-        c2 = [H2_0, A2_m, A2_p]
-        c3 = [H3_0, A3_m, A3_p]
-        ff = f_0mp # f_nlm[n_0], f_nlm[n_m], f_nlm[n_p] values
-        mD = np.array([c1, c2, c3]).transpose()
-        m1 = np.array([ff, c2, c3]).transpose()
-        m2 = np.array([c1, ff, c3]).transpose()
-        m3 = np.array([c1, c2, ff]).transpose()
-        dD = np.linalg.det(mD)
-        d1 = np.linalg.det(m1)
-        d2 = np.linalg.det(m2)
-        d3 = np.linalg.det(m3)
-        # fx1 = d1/dD * (2 / Delta) * 1
-        # fx2 = d2/dD * (2 / Delta)**2 * 2
-        # fx3 = d3/dD * (2 / Delta)**3 * 6
-        F1 = d1/dD
-        F2 = d2/dD
-        F3 = d3/dD
-        # These are df/dx derivatives in terms of dimensionless 0 < x < 1.
-        # But, for g(u) = fx(u/u0), Delta^p fx^{(p)} = (Delta u)^p g^{(p)}
-        return (F1, F2, F3)
-
-    def get_df123_sph_haar(self, f_0mp, n_0):
-        "Returns f', f'', f''', with units of f/(u0^p)"
-        [u1,u3] = self._baseOfSupport_n(n_0, getMidpoint=False)
-        Delta_u = u3-u1
-        (F1, F2, F3)  = self.get_F123_sph_haar(f_0mp, n_0)
-        g1 = F1 * math.factorial(1) * (2/Delta_u)**1
-        g2 = F2 * math.factorial(2) * (2/Delta_u)**2
-        g3 = F3 * math.factorial(3) * (2/Delta_u)**3
-        return (g1, g2, g3)
-
-    @staticmethod
-    def _n_list_for_cubic_methods(n_max):
-        "Breaks [0,1] interval into bases of support of the [n] wavelets."
-        assert n_max >= 3, "Must have at least 3 wavelet generations (lambda>=2)"
-        # n_max = 3 would use the n=1,2,3 wavelets to get one set of derivatives
-        # would return n_ordered = [1], i.e. only one cubic interpolation region
-        if n_max % 4 != 3:
-            n_max = n_max - (n_max % 4) - 1
-        # n_max should be 3 mod 4, so n_coeffs = n_max + 1 is zero mod 4
-        n_coeffs = n_max + 1
-        n_start = int(0.25*n_coeffs)
-        n_end = int(0.5*n_coeffs) - 1
-        lambda_start = int(math.log2(n_start))
-        mu_start = n_start - 2**lambda_start
-        Delta_start = 2**(-lambda_start)
-        # Can use partial generations, wrapping around from x=1 back to x=0
-        # the penultimate generation of coefficients determines the x->n map
-        # order the n list by their x values
-        n_start_b = 2**(lambda_start+1) #first element of (lambda_a+1) generation
-        list1 = [n for n in range(n_start_b, n_end+1)] #can have zero length
-        list2 = [n for n in range(n_start, n_start_b)]
-        n_ordered = list1 + list2
-        return n_ordered
-
-    def cubic_extrapolator_lm(self, f_lm_n, n_max):
-        """Cubic extrapolation from 2 generations of wavelets (ending at n_max).
-
-        For calculating larger-n wavelet coefficients from f1, f2, f3 derivates.
-        f_lm_n: ordered list of coefficients n for fixed (lm)
-            Ordered: f_lm_n[n] = f_nlm[(n,l,m)] for n=0,1,...,n_max
-            returns: f_lm(u) interpolation
-        n_max: determines which coefficients to use to find f' derivatives
-            -> (n_max+1)/2, (n_max+1)/2 + 1, ..., n_max - 1, n_max.
-        u: radial coordinate, u = x*uMax.
+            for lm,Flm in self.f_lm.items():
+                (ell, m) = lm
+                f_lm_u = Flm(u)
+                fu += ylm_real(ell, m, theta, phi) * f_lm_u
+        return fu
 
-        Output: an Interpolator object, with f0=0 in each bin.
-            (can be updated later for cubic_interpolation)
-        """
-        n_ordered = self._n_list_for_cubic_methods(n_max)
-        #get x0_vals and x_boundaries
-        u_bounds = [self._baseOfSupport_n(n_ordered[0], getMidpoint=False)[0]]
-        u0_vals = []
-        f0123_vals = []
-        for n in n_ordered:
-            (u1, u2, u3) = self._baseOfSupport_n(n, getMidpoint=True)
-            u0_vals += [u2]
-            u_bounds += [u3]
-            n_m = 2*n
-            n_p = 2*n + 1
-            f_0mp = (f_lm_n[n], f_lm_n[n_m], f_lm_n[n_p])
-            (df1, df2, df3) = self.get_df123_sph_haar(f_0mp, n)
-            f0123 = [0, df1, df2, df3]
-            f0123_vals += [f0123]
-        return Interpolator(u_bounds, u0_vals, f0123_vals)
-
-    def cubic_interpolation(self, f_lm_n, n_max, f0_lm_n):
-        """Uses f0_lm_n values of f(u_2) to interpolate f_lm(x).
-
-        Arguments:
-        f_lm_n: list of coefficients f_lm[n] for n=0,1,2...
-        n_max: determines which coefficients to use for extrapolation
-        f0_lm_n: the value of f_lm at the center of each wavelet n=0,1,2...
+    def flm_grid(self, ulist):
+        """Evaluates all f_lm(u) for all [u in ulist].
 
-        Output:
-        modified cubic_interpolator with f0 values taken from f0_lm_n
+        Output is a 2d numpy array, with rows lm ordered by self.f_lm.keys().
         """
-        n_list = self._n_list_for_cubic_methods(n_max)
-        cubic_interpolator = self.cubic_extrapolator_lm(f_lm_n, n_max)
-        for n in n_list:
-            f0 = f0_lm_n[n]
-            # the nth wavelet maps onto the (ix)th bin of the interpolation
-            (u1,u2,u3) = self._baseOfSupport_n(n, getMidpoint=True)
-            ix = cubic_interpolator.map_u_ix(u2)
-            cubic_interpolator.f0123_vals[ix][0] = f0
-        return cubic_interpolator
-
-
-
+        flmgrid = np.zeros([len(f_lm.keys()), len(ulist)])
+        ix = 0
+        for lm,Flm in self.f_lm.items():
+            f_lm_ug = np.array([Flm(u) for u in ulist])
+            flmgrid[ix] = f_lm_ug
+            ix += 1
+        return flmgrid
 
 
 
 
 #
```

### Comparing `vsdm-0.1.0/vsdm/gaussians.py` & `vsdm-0.2.9/vsdm/gaussians.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 """Analytic results for gaussian functions.
 
 Functions:
     normG_nli_integrand: analytic radial integrand for '\mathcal G'
     GaussianF: a class for functions that are defined as sums of gaussians
-    GaussianFnlm: a Basis class with additional methods for GaussianF functions
+    GBasis: a Basis class with additional methods for GaussianF functions
 """
 
-__all__ = ['GaussianF', 'GaussianFnlm', 'normG_nli_integrand']
+__all__ = ['GaussianF', 'GBasis', 'normG_nli_integrand']
 
 import math
 import numpy as np
 import scipy.special as spf
-import vegas # numeric integration
 import gvar # gaussian variables; for vegas
-# import time
-# import quaternionic # For rotations
-# import spherical #For Wigner D matrix
-# import csv # file IO for projectFnlm
-# import os.path
-# import h5py # database format for mathcalI arrays
 
-# from .units import *
 from .utilities import *
 from .basis import Basis
 
 
 def normG_nli_integrand(radR_nlu, u_i, sigma_i, n, ell, u):
     """For mathcalG_nl(u_i, sigma_i) gaussian and radR_nlu radial function.
 
@@ -85,15 +77,15 @@
         return sum_i
 
     def rescaleGaussianF(self, gFactor):
         "gvec_list for the function gFactor*fU(u)."
         return [(gvec[0]*gFactor, gvec[1], gvec[2]) for gvec in self.gvec_list]
 
 
-class GaussianFnlm(Basis, GaussianF):
+class GBasis(Basis, GaussianF):
     """Tools for projecting GaussianF functions onto an |nlm> basis.
 
     Input:
         bdict: describes the Basis
         gvec_list: specifies the GaussianF function.
             If None or [], this is a 'null gaussian'
     Methods:
@@ -105,88 +97,99 @@
         G_nli_array: formats G_nli_dict into 3d numpy array
     """
     def __init__(self, bdict, gvec_list):
         Basis.__init__(self, bdict)
         GaussianF.__init__(self, gvec_list) # can be None or []
         self.G_nli_dict = {} # format: G_nli_array[n,l,i] = G_nli
 
-
-
-    def Gnl_i(self, n, ell, i, vegas_params, saveGnli=True):
+    def Gnl_i(self, n, ell, i, integ_params, saveGnli=True):
         "Integrates Gnl_i for radRn(n,l) function."
         gvec = self.gvec_list[i]
         (c_i, uSph_i, sigma_i) = gvec
         (u_i, theta_i, phi_i) = uSph_i
+        x_i = u_i/self.u0
+        xsigma_i = sigma_i/self.u0
         header = "\tGnl_i for (n,l,i): {}".format((n, ell, i))
         headerA = "\tGnl_i(A) for (n,l,i): {}".format((n, ell, i))
         headerB = "\tGnl_i(B) for (n,l,i): {}".format((n, ell, i))
-        def integrand_Gnl(u1d):
-            [u] = u1d
-            return normG_nli_integrand(self.radRn, u_i, sigma_i, n, ell, u)
+        def integrand_Gnl(x1d):
+            [x] = x1d
+            return normG_nli_integrand(self.radRn, x_i, xsigma_i, n, ell, x)
         if self.basis['type']=='wavelet' and n!=0:
             # split integrand into two regions...
-            [umin, umid, umax] = self._baseOfSupport_n(n, getMidpoint=True)
+            [xmin, xmid, xmax] = self._baseOfSupport_n(n, getMidpoint=True)
             # Volume here in terms of u, not u/u0!
-            volume_A = [[umin, umid]] # 1d
-            volume_B = [[umid, umax]] # 1d
-            mGnl_A = self.doVegas(integrand_Gnl, volume_A, vegas_params,
-                                  printheader=headerA)
-            mGnl_B = self.doVegas(integrand_Gnl, volume_B, vegas_params,
-                                  printheader=headerB)
+            volume_A = [[xmin, xmid]] # 1d
+            volume_B = [[xmid, xmax]] # 1d
+            mGnl_A = NIntegrate(integrand_Gnl, volume_A, integ_params,
+                                printheader=headerA)
+            mGnl_B = NIntegrate(integrand_Gnl, volume_B, integ_params,
+                                printheader=headerB)
             mathGnl = mGnl_A + mGnl_B
         else:
-            [umin, umax] = self._baseOfSupport_n(n, getMidpoint=False)
-            volume_u = [[umin, umax]] # 1d
-            mathGnl = self.doVegas(integrand_Gnl, volume_u, vegas_params,
-                                   printheader=header)
+            [xmin, xmax] = self._baseOfSupport_n(n, getMidpoint=False)
+            volume_x = [[xmin, xmax]] # 1d
+            mathGnl = NIntegrate(integrand_Gnl, volume_x, integ_params,
+                                 printheader=header)
         if saveGnli:
             self.G_nli_dict[(n,ell,i)] = mathGnl
         return mathGnl
 
-    def getGnlm(self, nlm, vegas_params, saveGnli=True):
+    def getGnlm(self, nlm, integ_params, saveGnli=True):
         "The result <g|nlm>. Reads from G_nli_dict when possible."
         (n, ell, m) = nlm
         # Note: c_i does not affect value of Gnl_i. It appears here in cY_i
         sum_g = 0.0
         for i,gvec in enumerate(self.gvec_list):
             (c_i, uSph_i, sigma_i) = gvec
             (u_i, theta_i, phi_i) = uSph_i
             if (n,ell,i) in self.G_nli_dict.keys():
                 gnli = self.G_nli_dict[(n,ell,i)]
             else:
-                gnli = self.Gnl_i(n, ell, i, vegas_params, saveGnli=saveGnli)
+                gnli = self.Gnl_i(n, ell, i, integ_params, saveGnli=saveGnli)
             cY_i = c_i * ylm_real(ell, m, theta_i, phi_i)
             sum_g += cY_i * gnli
         return sum_g / self.u0**3
 
-    def updateGnlm(self, nlm, vegas_params, saveGnli=True):
+    def updateGnlm(self, nlm, integ_params, saveGnli=True):
         "The result <g|nlm>. Forces numeric evaluation."
         (n, ell, m) = nlm
         # Note: c_i does not affect value of Gnl_i. It appears here in cY_i
         sum_g = 0.0
         for i,gvec in enumerate(self.gvec_list):
             (c_i, uSph_i, sigma_i) = gvec
             (u_i, theta_i, phi_i) = uSph_i
-            gnli = self.Gnl_i(n, ell, i, vegas_params, saveGnli=saveGnli)
+            gnli = self.Gnl_i(n, ell, i, integ_params, saveGnli=saveGnli)
             cY_i = c_i * ylm_real(ell, m, theta_i, phi_i)
             sum_g += cY_i * gnli
         return sum_g  / self.u0**3
 
-    def G_nli_array(self, nMax, ellMax):
+    def G_nli_array(self, nMax, ellMax, use_gvar=False):
         "Creates np.array from G_nli_dict"
-        garray = gvar.gvar(1., 0)*np.zeros([nMax+1, ellMax+1, self.N_gaussians],
-                                           dtype='object')
+        if use_gvar:
+            arraySize = [nMax+1, ellMax+1, self.N_gaussians, 2]
+        else:
+            arraySize = [nMax+1, ellMax+1, self.N_gaussians]
+        g_array = np.zeros(arraySize)
         for nli,value in self.G_nli_dict.items():
             (n,l,i) = nli
             if n <= nMax and l <= ellMax:
-                garray[nli] = value
+                if use_gvar:
+                    if type(value) is gvar._gvarcore.GVar:
+                        garray[nli] = [value.mean, value.sdev]
+                    else:
+                        garray[nli][0] = value.mean
+                elif type(value) is gvar._gvarcore.GVar:
+                    garray[nli] = value.mean
+                else:
+                    garray[nli] = value
         return garray
 
-    def distEnergyG(self):
-        "Total 'energy' int(d^3u g^2)"
+    def norm_energy(self):
+        "Total 'energy' int(d^3x g**2) = int(d^3u/u0**3 g**2)."
         sumE = 0.0
         for i in range(self.N_gaussians):
             gvec_i = self.gvec_list[i]
             (c_i, uSph_i, sigma_i) = gvec_i
             sigma2_i = sigma_i**2
             ui = np.array(sph_to_cart(uSph_i))
             u2i = ui.dot(ui)
@@ -202,24 +205,8 @@
                 exp_ij = np.exp(u2_ij/sigma2_ij - u2i/sigma2_i - u2j/sigma2_j)
                 sumE += c_i*c_j*exp_ij / (np.pi*1.5 * (sigma2_i+sigma2_j)**1.5)
         return sumE / self.u0**3
 
 
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
 #
```

### Comparing `vsdm-0.1.0/vsdm/matrixcalc.py` & `vsdm-0.2.9/vsdm/matrixcalc.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,26 @@
         includes methods for save/read/import with hdf5 files
 """
 
 __all__ = ['McalI', 'MakeMcalI']
 
 import math
 import numpy as np
-import scipy.special as spf
 import vegas # numeric integration
 import gvar # gaussian variables; for vegas
 import time
-# import quaternionic # For rotations
-# import spherical #For Wigner D matrix
-# import csv # file IO for projectFnlm
 import os.path
 import h5py
 
 
 from .utilities import *
 from .portfolio import *
 from .units import *
 from .analytic import *
-from .basis import _haar_sph_value, _tophat_value, Basis
+from .basis import haar_sph_value, tophat_value, Basis
 
 
 #
 
 class McalI():
     """Handles the I(ell) matrices for one choice of DM,SM particle models.
 
@@ -187,15 +183,15 @@
         def integrand(qv):
             [q,v]=qv
             vMinq = DeltaE/q + q/(2*mX)
             if v < vMinq:
                 return 0
             else:
                 partQ = self.Q.radRn(nq, ell, q) * fdm2_n(q, fdm_n)
-                partV = self.V.radRn(nv, ell, v) * legendrePl(ell,vMinq/v)
+                partV = self.V.radRn(nv, ell, v) * plm_norm(ell,0,vMinq/v)
                 return self.kI * q*v/(q0*v0)**2 * partQ * partV
             # Integrand units cancel against units from QV integration area
         integrator = vegas.Integrator(QVrange)
         integrator(integrand, nitn=nitn_init, neval=neval_init) #training
         I_lnvq = integrator(integrand, nitn=nitn, neval=neval) #result
         # self.mcalI[ell, nv, nq] = mcalI
         if verbose:
@@ -238,35 +234,35 @@
             # returns the error type, so one can try again with getI_lvq()
             return AssertionError
         commonFactor = ((q0/v0)**3/(2*mX*muSM**2) * (2*DeltaE/(q0*v0))**2
                         *(q0_fdm/qStar)**(2*fdm_n))
         n_regions = [1,1]
         if v_type=='tophat':
             [v1, v2] = V._baseOfSupport_n(nv, getMidpoint=False)
-            A_v = _tophat_value(v1/v0, v2/v0) #normalize to 0<x<1
+            A_v = tophat_value(v1/v0, v2/v0) #normalize to 0<x<1
             n_regions[0] = 1
         elif v_type=='wavelet':
             [v1, v2, v3] = V._baseOfSupport_n(nv, getMidpoint=True)
             if nv==0:
-                A_v = _haar_sph_value(nv)
+                A_v = haar_sph_value(nv)
                 n_regions[0] = 1
             else:
-                [A_v, B_v] = _haar_sph_value(nv) #already normalized
+                [A_v, B_v] = haar_sph_value(nv) #already normalized
                 n_regions[0] = 2
         if q_type=='tophat':
             [q1, q2] = Q._baseOfSupport_n(nq, getMidpoint=False)
-            A_q = _tophat_value(q1/q0, q2/q0) #normalize to 0<x<1
+            A_q = tophat_value(q1/q0, q2/q0) #normalize to 0<x<1
             n_regions[1] = 1
         elif q_type=='wavelet':
             [q1, q2, q3] = Q._baseOfSupport_n(nq, getMidpoint=True)
             if nq==0:
-                A_q = _haar_sph_value(nq)
+                A_q = haar_sph_value(nq)
                 n_regions[1] = 1
             else:
-                [A_q, B_q] = _haar_sph_value(nq) #already normalized
+                [A_q, B_q] = haar_sph_value(nq) #already normalized
                 n_regions[1] = 2
         # There is always an A_v A_q term:
         v12_star = [v1/vStar, v2/vStar]
         q12_star = [q1/qStar, q2/qStar]
         term_AA = A_v*A_q * mI_star(ell, fdm_n, v12_star, q12_star)
         # There are only B-type contributions if V or Q uses wavelets
         term_AB, term_BA, term_BB = 0, 0, 0
```

### Comparing `vsdm-0.1.0/vsdm/portfolio.py` & `vsdm-0.2.9/vsdm/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Organizes an HDF5 dataset for an analysis combining gX and fs2 models.
 
 """
 
 __all__ = ['Portfolio', 'str_to_bdict', 'str_to_dnames', 'update_namedict',
            'dname_manager', 'DEFAULT_TYPES', 'DNAME_F', 'DNAME_G', 'DNAME_I',
            'DNAME_W', 'TNAME_mcalI', 'TNAME_gX', 'TNAME_fs2', 'TNAME_generic',
-           'TNAME_rotations', 'TNAME_mcalK', '_dset_exists']
+           'TNAME_rotations', 'TNAME_mcalK', 'LM_IX_NAME', '_dset_exists']
 
 
 import numpy as np
-import time
-import csv  
-import os.path
 import h5py
 import gvar
 
 from .utilities import *
 
+"""
+    Global names for hdf5 groups and subgroups (types and databases)
+    DNAME_: database name for saved data (e.g. <f|nlm>, gaussian Gnl, ...)
+    LM_IX_NAME: maps the rows of DNAME_F to the corresponding (l, m).
+"""
 # dataset names for hdf5 files:
 DNAME_F = 'fnlm'
 DNAME_G = 'Gnl'
 DNAME_I = 'Ilvq'
 DNAME_W = 'wG'
+LM_IX_NAME = 'lm_index'
 # _dnames_ = ['DNAME_F', 'DNAME_G', 'DNAME_I', 'DNAME_W']
 # saves gvar matrix to 'NAME_mean' and 'NAME_sdev'.
 # subgroup 'type' names for hdf5 files:
 TNAME_mcalI = 'mcalI'
 TNAME_gX = 'gX'
 TNAME_fs2 = 'fs2'
 TNAME_generic = 'proj'
@@ -86,30 +89,36 @@
         except ValueError:
             #skip anything that doesn't like being turned into an integer
             # in case group.attrs is used to hold unrelated attributes
             continue
         dnames[dname] = dn_index
     return dnames
 
-def dname_manager(dname_dict, dname, sepchar='__'):
+def dname_manager(dname_dict, dname, sepchar='__', delete=False):
     """Reads dataset names from dname_dict, modifies dname or dname_dict.
 
     Format:
         dname: str-valued dictionary key
         dname_dict: int-valued dictionary of name multiplicities
             dname_dict[dname] = # of datasets with 'dname' as name base.
             initialized to 1 upon creation of 'dname'.
         sepchar: appended to 'dname' for dname_dict[dname] > 1 entries.
             default: '__'. Avoid anything already being used in the names.
     Used to label new files as 'dname_2', 'dname_3', etc.
         e.g. as opposed to 'dname_1_1', 'dname_1_1_1', ...
+
+    When called using delete=True, it removes dname from dname_dict.
     """
     dict_out = dname_dict # avoid modifying the input
     if dname in dict_out:
-        # then it needs an integer-valued suffix...
+        # dname can be deleted from the dictionary:
+        if delete:
+            del dict_out[dname]
+            return dict_out, dname
+        # Otherwise, dname needs an integer-valued suffix...
         name_in_dict = True
         while name_in_dict:
             #check if i += 1 is available :
             dict_out[dname] += 1
             dname_new = dname + sepchar + str(dict_out[dname])
             name_in_dict = (dname_new in dict_out)
             if not name_in_dict:
@@ -154,17 +163,22 @@
                 # stop, now name_dict is up to date
     """
     Note 1: this leaves name_dict ready to fill the first open name spot.
     It may appear in the middle of a sequence, _1, _2, _3, _6, _7, ...,
         if items '4' and '5' were deleted.
     dname_manager handles this: before trying to name something _6 it checks
         whether _6 already exists, and moves on to the first available integer.
+
     Note 2: This also adds subgroup names to the name_dict.
         This has little effect: dname_manager does not manage subgroups,
         so any attempt to name a dataset with a group name will lead to error.
+
+    Note 3. Deleting a database from the hdf5 file does not remove its name
+        from the dname_manager. The name entry also needs to be deleted from
+        group.attrs.
     """
     return name_dict
 
 
 def _dset_exists(hdf5file, tname, model, dname):
     """Looks for dataset 'dname' from hdf5, returns True if it exists."""
     with h5py.File(hdf5file,'r') as fhd5:
@@ -334,19 +348,31 @@
         return dname_out
 
     def read_folio(self, tname, model, dname):
         """Reads dataset 'dname' from hdf5. Returns data and dname.attrs."""
         data_attr = {}
         with h5py.File(self.hdf5file,'r') as fhd5:
             mgroup = fhd5[tname + '/' + model]
-            data = mgroup[dname]
-            for lbl,val in data.attrs.items():
+            data = np.array([row for row in mgroup[dname]])
+            for lbl,val in mgroup[dname].attrs.items():
                 data_attr[lbl] = val #import the basis metadata
             return data, data_attr
 
+    def delete_folio(self, tname, model, dname):
+        """Deletes dataset 'dname' from hdf5."""
+        with h5py.File(self.hdf5file,'a') as fhd5:
+            mgroup = fhd5[tname + '/' + model]
+            if dname in mgroup.keys():
+                del mgroup[dname]
+                name_record, dname = dname_manager(group.attrs, dname, delete=True)
+                group.attrs.update(name_record) # save the update to group.attrs
+                print("Deleted dataset '{}' from group '{}'.".format(dname,model))
+            else:
+                print("No dataset '{}' in group '{}'.".format(dname,model))
+
     def update_folio(self, tname, model, dname, newdata={}, attrs={}):
         """Modifies the dataset 'dname' with the provided newdata.
 
         Arguments:
             tname, model, dname: group name and dataset
             newdata: a dict object of form {index: value}, for
                 dname[index] = value
@@ -358,15 +384,15 @@
         with h5py.File(self.hdf5file,'r+') as fhd5:
             mgroup = fhd5[tname + '/' + model]
             dbase = mgroup[dname] # the dataset
             dshape = np.shape(dbase) # initial size of dataset array
             dim = len(dshape) # dimensionality of array
             for index,value in newdata.items():
                 # make sure index is valid
-                if len(index)!=dim:
+                if len(index)>dim:
                     print("Warning: data includes invalid entries.")
                     continue
                 bad_index = False
                 # a correct index length doesn't guarantee its suitability:
                 for i in range(dim):
                     if type(index[i]) is not int:
                         bad_index = True
```

### Comparing `vsdm-0.1.0/vsdm/projection.py` & `vsdm-0.2.9/vsdm/projection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,107 @@
-"""VSDM: ProjectFnlm implements Basis integration for a specific function fSph.
+"""Projects a 3d function onto a basis of orthogonal functions.
 
+ProjectFnlm is one of the primary functions of vsdm. Each class instance
+evaluates and saves the values of <f|nlm> for the specified Basis (|nlm>) and
+function fSph(u,theta,phi), a 3d function in spherical coordinates.
+
+ProjectFnlm contains methods for saving CSV or HDF5 files, or importing
+<f|nlm> coeffients from either type of file.
 """
 
 __all__ = ['ProjectFnlm']
 
 
 import math
 import numpy as np
-import scipy.special as spf
 import vegas # numeric integration
 import gvar # gaussian variables; for vegas
 import time
 import csv # file IO for projectFnlm
 import os.path
 import h5py
 
 from .basis import ylm_real
-from .gaussians import GaussianFnlm
+from .gaussians import GBasis
 from .utilities import *
 from .portfolio import *
 
 
 
-
-
-
-
-class ProjectFnlm(GaussianFnlm):
+class ProjectFnlm(GBasis):
     """Performs projection <fSph|nlm> for one 3d function fSph.
 
     Upon initialization, evaluates <f|nlm> for all nlm in nlmlist. Additional
       values of nlm can be added subsequently using updateFnlm method.
     Like Basis, ProjectFnlm does not require .units.
 
     Arguments:
         fSph: a function of 3d spherical uvec OR a GaussianF object
             Can have attributes: is_gaussian, phi_symmetric, etc
             These become attributes of the ProjectFnlm instance
         bdict: Basis parameters
-        vegas_params: e.g. dict(neval=1e4, nitn=10, nitn_init=5, verbose=False)
+        integ_params: e.g. dict(neval=1e4, nitn=10, nitn_init=5, verbose=False)
         f_type: labels the type of function being projected, e.g. 'gX' or 'fs2'
             default label 'proj' defined in portfolio.py
+        csvsave_name: if not None, then ProjectFnlm saves any new <f|nlm>
+            values to the specified csv file.
 
     Returns:
         f_nlm: dictionary of <f|nlm>, indexed by (n,l,m), with gvar values
         f_lm_n: a single 2d array of coefficients,
             labelled by [x(ell,m), n], for x=0,1,2..., (ellMax+1)**2 - 1.
             See utilities.py.
             phi_symmetric: if so, only adds entries for m=0 coefficients.
                 Length of array is always (ellMax+1)**2!
-            NEW: need not be gvar valued.
-    f_nlm is best for sparse (nlm) lists;
-    f_lm_n is best for saving hdf5 files.
+    f_nlm is best for sparse (nlm) lists; f_lm_n is best for saving hdf5 files.
 
     Methods and variables:
         updateFnlm: adds new f[nlm], or overwrites old value
-            e.g. with better precision
         _makeFarray: makes vectors of <f|nlm> with fixed (lm)
             self.phi_symmetric sets m=0.
             use_gvar=False for float-valued matrix output
-        nlmFu, nlmFu_subset: returns f(uvec) from sums over <f|nlm>
-        errorCalcs: integrates nlmFu(r) and original f(r), and (nlmFu-f)(r)
-        errorTot, errorAbsTot: integrate (nlmFu-f)(r) and np.abs(nlmFu-f)(r)
-        getVSOPbasis: returns a Basis instance of (basisType,u0,uMax)
     Methods for saving/reading/importing...
-    * writeFnlm(hdf5file, nlmlist=None, modelName=''):
-        saves f_nlm to readable CSV file, for all nlm, or nlm in nlmlist
-        row format: ["modelName", "n", "l", "m", "f.mean", "f.sdev"]
-        modelName is optional: can be used to save incompatible
-            <f|nlm> to same file
-    * writeFlmVecs(hdf5file,modelName=''):
-        saves <f(lm)|n> vectors to CSV file
-        row format: ["modelName", "l", "m", "fn.mean", "fn.sdev"],
-            with fn as lists on [n=0,1,...nMax]
-    * writeF_array(hdf5file,modelName):
-        saves <f|(lm)n> array to HDF5 dataset in hdf5file/modelName
-        row format: x = _LM_to_x(l,m) = 0,1,2,...l(l+2).
-        RECOMMEND: modelName = 'gX/(index)' or 'fgs2/(index)' for model index
-    * readFnlm(), readFlmVecs(hdf5file, modelName=None):
-        opens hdf5file, returns data_fnlm dict using all entries
-            (or only those with matching modelName)
-    * importFnlm(), importFlmVecs(csvfile, modelName=None):
-        writes data_fnlm from CSV into self.f_nlm
-        Caution! import() will overwrite any existing f_nlm entries
+    * writeFnlm_csv(hdf5file, nlmlist=None):
+        saves f_nlm to CSV file, for all nlm, or for nlm in nlmlist
+        row format: ["n", "l", "m", "f.mean", "f.sdev"]
+    * writeFnlm(hdf5file,modelName):
+        saves <f|(lm)n> array to HDF5 dataset in hdf5file/modelName/(dataset),
+            usually with the default dataset name DNAME_F = 'fnlm'.
+        The row index 'x' is based on the order of self.lm_index. This mapping
+            is saved to the companion dataset as LM_IX_NAME = 'lm_index'.
+        If either dataset name is already taken, then Portfolio picks a new
+            name (e.g. 'fnlm__2') for the newer data.
+    * importFnlm(hdf5file, model, **kwargs):
+        reads <f|nlm> from an hdf5 file, and saves the results to self.f_nlm.
+        The 'file path' inside the hdf5 file is:
+            hdf5file/type/model/(d_fnlm, lm_ix), where d_fnlm contains <f|nlm>,
+        and lm_ix maps each row to its (l, m) value.
+        The defaults type=self.f_type, d_fnlm=DNAME_F, lm_ix=LM_IX_NAME
+            can be changed using the keyword arguments.
+    * importFnlm_csv(csvfile):
+        writes <f|nlm> data from the csv file into self.f_nlm.
+    Note: the import() functions will overwrite any existing f_nlm[nlm]
+        entries with the new (n, l, m) coeffients.
     """
-    def __init__(self, bdict, fSph, vegas_params, nlmlist=[], f_type=None,
-                 csvsave_name=None, csvsave_model='', use_gvar=True):
+    def __init__(self, bdict, fSph, integ_params, nlmlist=[], f_type=None,
+                 csvsave_name=None, use_gvar=True):
         t0 = time.time()
         self.fSph = fSph # a function fSph(uvec), with uvec=(u,theta,phi)
         self.use_gvar = use_gvar
-        self.vegas_params = vegas_params
+        self.integ_params = integ_params
+        self.csvsave_name = csvsave_name
         self.t_eval = 0.
         # Or, fSph may be a GaussianF instance:
         if hasattr(fSph, 'is_gaussian') and (fSph.is_gaussian):
-            GaussianFnlm.__init__(self, bdict, fSph.gvec_list)
-            # GaussianFnlm contains Basis
+            GBasis.__init__(self, bdict, fSph.gvec_list)
+            # GBasis contains Basis
             # New ProjectFnlm instance does not inherit the G_nli_dict of fSph.
         else:
-            # use GaussianFnlm to import Basis.__init__
-            GaussianFnlm.__init__(self, bdict, None) # self.is_gaussian = False
+            # use GBasis to import Basis.__init__
+            GBasis.__init__(self, bdict, None) # self.is_gaussian = False
         self.z_even = False
         self.phi_symmetric = False
         self.phi_cyclic = 1
         self.phi_even = False
         self.center_Z2 = False
         if hasattr(fSph, 'z_even') and fSph.z_even not in [0, None]:
             # if fSph is Z_2 symmetric in the z direction, only even ell are nonzero
@@ -134,57 +133,52 @@
             self.f_type = TNAME_generic # from portfolio
         else:
             self.f_type = f_type
         self.f_nlm = {} # Primary: <f|nlm> coefficients in gvar format
         # The following are to be updated by update_maxes():
         self.ellMax = 0
         self.nMax = 0
-        # Unpack VEGAS integration parameters:
-        nitn_init = vegas_params['nitn_init']
-        nitn = vegas_params['nitn']
-        neval = int(vegas_params['neval'])
-        verbose = vegas_params['verbose']
-        if 'neval_init' in vegas_params:
-            neval_init = int(vegas_params['neval_init'])
+        self.lm_index = [] # list of (l, m) included in f_nlm.
+        if hasattr(integ_params, 'verbose'):
+            self.verbose = integ_params['verbose']
         else:
-            neval_init = neval
-        # self.vegas_params = vegas_params
+            self.verbose = False
         if self.use_gvar:
             self.f2_energy = gvar.gvar(0,0)
         else:
             self.f2_energy = 0.0
         if nlmlist is not None:
             for nlm in nlmlist:
                 self.update_maxes(nlm)
                 if self.is_gaussian:
-                    # use method from GaussianFnlm:
-                    fnlm = self.getGnlm(nlm, vegas_params, saveGnli=True)
+                    # use method from GBasis:
+                    fnlm = self.getGnlm(nlm, integ_params, saveGnli=True)
                     # save=True ensures that self.G_nli_dict is updated
                 else:
                     # use method from Basis
-                    fnlm = self.getFnlm(fSph, nlm, vegas_params)
+                    fnlm = self.getFnlm(fSph, nlm, integ_params)
                 if self.use_gvar:
                     self.f_nlm[nlm] = fnlm
                 else:
                     self.f_nlm[nlm] = fnlm.mean
                 f2_power = fnlm**2
                 self.f2_energy += f2_power
-                if verbose:
+                if self.verbose:
                     print("Result: <f|{}> = {}".format(nlm, fnlm))
                     print("\ttotal energy: {}".format(self.f2_energy))
                 if csvsave_name is not None:
                     # save as you go:
                     # append this f(nlm) to the CSV file 'csvsave_name',
-                    self.writeFnlm_csv(csvsave_name, nlmlist=[nlm],
-                                       modelName=csvsave_model)
+                    self.writeFnlm_csv(csvsave_name, nlmlist=[nlm])
         self.t_init = time.time() - t0
         self.t_eval = self.t_init
         # Add other metadata to basis dict
-        for lbl in vegas_params:
-            self.basis[lbl] = vegas_params[lbl]
+        for lbl in integ_params:
+            self.basis[lbl] = integ_params[lbl]
+            # This ensures that writeFnlm_csv will save the integ_params.
         self.basis['is_gaussian'] = self.is_gaussian
 
     def getNLMlist(self):
         """Returns all (nlm) that have been added to <f|nlm>."""
         nlmlist = [nlm for nlm in self.f_nlm]
         return nlmlist
 
@@ -262,26 +256,26 @@
         sortl = sorted(powerL.items(),
                        key=lambda z: z[1], reverse=True)
         powerL = {}
         for key,power in sortl:
             powerL[key] = power
         return powerL
 
-    def getDistEnergy(self, vegas_params, integrateG=False):
+    def getDistEnergy(self, integ_params, integrateG=False):
         """Integral of f**2/self.u0**3 (the distributional energy, rescaled by u0).
 
         mSymmetry and lSymmetry restrict integration region to a subregion
             of solid angle.
         For l only expect lSymmetry=2, e.g. z <-> -z.
         m can take larger values than 2 (commonly 4), e.g. polygonal cylindrical symmetry
 
         Saves result to self.basis['distEnergy']
         """
         if self.is_gaussian and not integrateG:
-            energyG = self.distEnergyG()
+            energyG = self.norm_energy()
             energy = gvar.gvar(energyG, 0)
             return energy
         theta_Zn = 1
         if self.center_Z2:
             theta_Zn = 2
         theta_region = [0, math.pi/theta_Zn]
         if self.phi_symmetric:
@@ -292,18 +286,18 @@
                     uvec = (r, theta, 0.0)
                     return dV_sph(uvec) * self.fSph.gU(uvec)**2/self.u0**3
             else:
                 def power_u(u2d):
                     (r, theta) = u2d
                     uvec = (r, theta, 0.0)
                     return dV_sph(uvec) * self.fSph(uvec)**2/self.u0**3
-            # do VEGAS:
-            energy = (self.doVegas(power_u, volume, vegas_params)
+            # integrate:
+            energy = (NIntegrate(power_u, volume, integ_params)
                       * 2*math.pi * theta_Zn)
-            if vegas_params['verbose']==True:
+            if integ_params['verbose']==True:
                 print('energy: {}'.format(energy))
             # include result in self.basis[]
             self.basis['distEnergy'] = energy
             return energy
         #else:
         phi_region = [0, 2*math.pi/self.phi_cyclic]
         volume = [[0, self.uMax], theta_region, phi_region]
@@ -311,87 +305,103 @@
             def power_u(uvec):
                 # energy has units of uMax**3
                 return dV_sph(uvec) * self.fSph.gU(uvec)**2/self.u0**3
         else:
             def power_u(uvec):
                 # energy has units of uMax**3
                 return dV_sph(uvec) * self.fSph(uvec)**2/self.u0**3
-        energy = (self.doVegas(power_u, volume, vegas_params)
+        energy = (NIntegrate(power_u, volume, integ_params)
                   * self.phi_cyclic * theta_Zn)
-        if vegas_params['verbose']==True:
+        if integ_params['verbose']==True:
             print('energy: {}'.format(energy))
+        # include result in self.basis[]
+        self.basis['distEnergy'] = energy
         return energy
 
     def update_maxes(self, nlm):
         """Updates self.Max values to encompass 'nlm'."""
         (n,l,m) = nlm
         assert(int(math.fabs(m)) <= l), "Invalid (nlm): m out of range"
         assert(l >= 0), "Invalid (nlm): l out of range"
         if l > self.ellMax:
             self.ellMax = l
         if n > self.nMax:
             self.nMax = n
+        if (l, m) not in self.lm_index:
+            self.lm_index += [(l, m)]
+
+    def reindex_lm(self):
+        # put lm_index in order of increasing ell and m.
+        out = []
+        for ell in range(self.ellMax+1):
+            for m in range(-ell, ell+1):
+                if (ell,m) in self.lm_index:
+                    out += [(ell, m)]
+        self.lm_index = out
 
-    def updateFnlm(self, nlm, vegas_params, csvsave_name=None, csvsave_model=''):
+    def updateFnlm(self, nlm, integ_params, csvsave_name=None):
         """Calculates <f|nlm> for new (nlm), or overwrites existing <f|nlm>."""
         # Good for adding nlm to the list.
-        # Or, recalculate f_nlm with better precision in vegas_params.
+        # Or, recalculate f_nlm with better precision in integ_params.
         t0 = time.time()
         self.update_maxes(nlm)
-        fnlm = self.getFnlm(self.fSph, nlm, vegas_params, saveGnli=True)
+        fnlm = self.getFnlm(self.fSph, nlm, integ_params, saveGnli=True)
+        if not self.use_gvar:
+            fnlm = fnlm.mean
         self.f_nlm[nlm] = fnlm
         t1 = time.time() - t0
         self.t_eval += t1
-        self.basis['t_eval'] = self.t_eval
-        if vegas_params['verbose']:
+        if integ_params['verbose']:
             print("Result: <f|{}> = {}".format(nlm, fnlm))
         if csvsave_name is not None:
             # save as you go:
             # append this f(nlm) to the CSV file 'csvsave_name',
-            self.writeFnlm_csv(csvsave_name, nlmlist=[nlm],
-                               modelName=csvsave_model)
+            self.writeFnlm_csv(csvsave_name, nlmlist=[nlm])
         return fnlm #in case anyone wants it
 
 
-    def nlmFu(self, uvec, nlmlist=None):
-        """The VSOP reconstruction of f(r), from all <f|nlm>."""
-        return self.nlmAssembleFu(self.f_nlm, uvec, nlmlist=nlmlist)
-
 
     def _makeFarray(self, use_gvar=False):
-        """Creates 'secondary' formats for <f|nlm> from self.f_nlm.
+        """Creates secondary format for saving <f|nlm> for hdf5 output.
 
-        Makes self.f_lm_n, for hdf5 output.
-            rows labeled by (lm) -> x = 0, 1, 2, ... l(l+2).
-            if phi_symmetric: only make rows x = ell, all with m=0.
-                See utilities._LM_to_x() for x(lm) function.
+        Rows are labeled by (lm), in the lm_index order:
+            lm = lm_index[ix_x]  (= (0, 0), (1, -1), (1, 0), ....)
+        If use_gvar, then f_lm_n is a 3d array:
+            f_lm_n[ix_x][n] = [fnlm.mean, fnlm.sdev]
+        Otherwise, f_lm_n is a 2d array, f_lm_n[ix_x][n] = <f|nlm>.
         """
         #make sure self.Max are up to date:
         for nlm in self.getNLMlist():
             self.update_maxes(nlm)
-        if self.phi_symmetric:
-            arraySize = [(self.ellMax+1), (self.nMax+1)]
-        else:
-            arraySize = [(self.ellMax+1)**2, (self.nMax+1)]
+        self.reindex_lm()
+        if use_gvar and not self.use_gvar:
+            use_gvar = False
         if use_gvar:
-            self.f_lm_n = gvar.gvar(1., 0)*np.zeros(arraySize, dtype='object')
+            arraySize = [len(self.lm_index), (self.nMax+1), 2]
         else:
-            self.f_lm_n = np.zeros(arraySize)
+            arraySize = [len(self.lm_index), (self.nMax+1)]
+        self.f_lm_n = np.zeros(arraySize)
         for nlm,f_gvar in self.f_nlm.items():
             (n,l,m) = nlm
             ix_y = n
-            if self.center_Z2 and (l%2 != 0):
+            if (self.center_Z2 or self.z_even) and (l%2 != 0):
                 continue
             if self.phi_symmetric and (m!=0):
                 continue
-            ix_x = _LM_to_x(l,m, phi_symmetric=self.phi_symmetric)
-            if use_gvar:
-                self.f_lm_n[ix_x, ix_y] = f_gvar
-            else:
+            if self.phi_even and m<0:
+                continue
+            if m%self.phi_cyclic != 0:
+                continue
+            ix_x = self.lm_index.index((l,m))
+            if use_gvar and type(f_gvar) is gvar._gvarcore.GVar:
+                self.f_lm_n[ix_x, ix_y] = [f_gvar.mean, f_gvar.sdev]
+            elif type(f_gvar) is gvar._gvarcore.GVar:
                 self.f_lm_n[ix_x, ix_y] = f_gvar.mean
+            else:
+                self.f_lm_n[ix_x, ix_y] = f_gvar
         return self.f_lm_n
 
     @staticmethod
     def addcombine_fnlms(fnlm_list):
         """Adds results from multiple f_nlm objects.
 
         Useful when f is split into f = f_1 + f_2 + ... + f_k,
@@ -413,103 +423,117 @@
                 if nlm in fnlm:
                     gf += fnlm[nlm]
             grand_fnlm[nlm] = gf
         return grand_fnlm
 
 
 
-    def writeFnlm(self, hdf5file, modelName,
-                  writeGnli=False, alt_type=None, use_gvar=False):
+    def writeFnlm(self, hdf5file, modelName, use_gvar=False,
+                  alt_type=None, writeGnli=False):
         """Adds hdf5 dataset to group 'modelName'.
 
         Arguments:
             hdf5file: the hdf5 file to open/write
             modelName: a group name for storing <f|nlm> datasets
         Saves to: hdf5file/typeName/modelName/dataset
             with typeName = self.f_type.
         Database names use the default portfolio.DNAME_F,
             which specifies that this object is an <f|nlm> dataset.
-            Saves gvar .mean and .sdev arrays to _mean and _sdev datasets.
+
+        For gvar-valued data: values are saved as [f.mean, f.sdev].
 
         Using utilities.dname_manager() to avoid name conflicts within
             the group 'modelName' (or 'typeName/modelName').
         Writing multiple versions to the same 'modelName' will save
             the later copies as 'modelName_2', 'modelName_3'...
         """
         if alt_type is not None:
             typeName = alt_type
         else:
             typeName = self.f_type
+        if use_gvar and not self.use_gvar:
+            use_gvar = False
         self._makeFarray(use_gvar=use_gvar)
         # include the following information in .basis and the output:
         self.basis['nMax'] = self.nMax
         self.basis['ellMax'] = self.ellMax
         self.basis['phi_symmetric'] = self.phi_symmetric
+        self.basis['z_even'] = self.z_even
+        self.basis['center_Z2'] = self.center_Z2
+        self.basis['phi_cyclic'] = self.phi_cyclic
+        self.basis['phi_even'] = self.phi_even
         self.basis['t_eval'] = self.t_eval
         folio = Portfolio(hdf5file, extra_types=[typeName])
         dset_attrs = {} # save relevant basis info to hdf5:
         for lbl,value in self.basis.items():
             if value is not None:
                 dset_attrs[lbl] = value
-        dn_mean = DNAME_F + '_mean' # intended dbase name
-        dn_sdev = DNAME_F + '_sdev' # intended dbase name
-        if use_gvar:
-            flm_n_mean, flm_n_sdev = splitGVARarray(self.f_lm_n)
-        else:
-            flm_n_mean = self.f_lm_n
-            flm_n_sdev = np.zeros_like(flm_n_mean)
-        dname_mean = folio.add_folio(typeName, modelName, dn_mean,
-                                     data=flm_n_mean, attrs=dset_attrs)
-        dname_sdev = folio.add_folio(typeName, modelName, dn_sdev,
-                                     data=flm_n_sdev, attrs=dset_attrs)
+        dset_attrs['use_gvar'] = use_gvar
+        dname = folio.add_folio(typeName, modelName, DNAME_F,
+                                data=self.f_lm_n, attrs=dset_attrs)
+        lm_ix = np.array(self.lm_index)
+        folio.add_folio(typeName, modelName, LM_IX_NAME,
+                        data=lm_ix, attrs=dict(dname=dname))
         # add_folio returns the actual dname used
         if writeGnli and (self.is_gaussian): #also save mG_nli_array
-            g_array = self.G_nli_array(self.nMax, self.ellMax)
-            gn_mean = DNAME_G + '_mean'
-            gn_sdev = DNAME_G + '_sdev'
-            gnl_mean, gnl_sdev = splitGVARarray(g_array)
-            gname_mean = folio.add_folio(typeName, modelName, gn_mean,
-                                         data=gnl_mean, attrs=dset_attrs)
-            gname_sdev = folio.add_folio(typeName, modelName, gn_sdev,
-                                         data=gnl_sdev, attrs=dset_attrs)
-        return dname_mean,dname_sdev
+            g_array = self.G_nli_array(self.nMax, self.ellMax, use_gvar=use_gvar)
+            gname = folio.add_folio(typeName, modelName, DNAME_G,
+                                    data=g_array, attrs=dict(dname=dname))
+        return dname
 
-    def write_additional(self, hdf5file, modelName, d_pair, newdata={},
-                         alt_type=None):
+    def add_data(self, hdf5file, modelName, newdata, dname=DNAME_F,
+                 alt_type=None, is_gvar=False):
         """Adds <f|nlm> values to existing hdf5 datasets.
 
         Arguments:
-            hdf5file, modelName, d_pair: specify datasets to use
-                hdf5file/type/modelName/
-                    d_pair[0]: _mean ,   d_pair[1]: _sdev.
+            hdf5file, modelName, dname: specify datasets to use
+                hdf5file/type/modelName/dname
             newdata: a dict of f[(nlm)] coefficients, in style of self.f_nlm.
-        Note: _additional only works for f_nlm, not f_lm_n.
+            is_gvar: whether or not the database dname includes fnlm.sdev.
+                This needs to match dset_attrs['use_gvar'].
+                Otherwise, newdata will have the wrong shape.
+
         """
         if alt_type is not None:
             typeName = alt_type
         else:
             typeName = self.f_type
         folio = Portfolio(hdf5file, extra_types=[typeName])
         data_out = {}
         for nlm,f in newdata.items():
             (n,l,m) = nlm
-            ix_x = _LM_to_x(l,m, phi_symmetric=self.phi_symmetric)
+            ix_x = self.lm_index.index((l,m))
             ix_y = n
-            data_out[(ix_x, ix_y)] = f
-        folio.update_gvar(typeName, modelName, d_pair, newdata=data_out)
+            if is_gvar:
+                if type(f) is gvar._gvarcore.GVar:
+                    data_out[(ix_x, ix_y)] = [f.mean, f.sdev]
+                else:
+                    data_out[(ix_x, ix_y)][0] = f
+            elif type(f) is gvar._gvarcore.GVar:
+                data_out[(ix_x, ix_y)] = f.mean
+            else:
+                data_out[(ix_x, ix_y)] = f
+        folio.update_folio(typeName, modelName, dname, newdata=data_out)
 
 
-    def importFnlm(self, hdf5file, modelName, d_pair, alt_type=None):
+    def importFnlm(self, hdf5file, modelName,
+                   d_fnlm=DNAME_F, lm_ix=LM_IX_NAME, alt_type=None):
         """Imports <f|nlm> from hdf5, adds to f_nlm.
 
         Arguments:
-            d_pair: pair of _mean and _sdev files to merge;
-                or just _mean, if len(dnames)==1.
             hdf5file, modelName, alt_type: sets hdf5file/typeName/modelName
-                with typeName = self.f_type unless an alt_type is provided
+                default typeName = self.f_type, unless an alt_type is provided
+            d_fnlm: database of <f|nlm>, in 2d array f_lm_n
+                Default: value of DNAME_F from portfolio.py.
+            lm_ix: maps the row-number in d_fnlm to (l, m).
+                Default: LM_IX_NAME from portfolio.py.
+        * Note: if self.writeFnlm is applied multiple times with the same
+        modelName, then Portfolio automatically assigns different database
+        names (other than DNAME_F). In this case, imporeFnlm should be run
+        once per database, taking care to match each lm_ix file to its database.
 
         Returns:
             dataFnlm: the f_lm_n gvar array from hdf5file
             bdict_info: contains basis parameters incl. 'phi_symmetric'
                 * recommend checking that this matches self.basis.
 
         Adds or overwrites f_nlm for all (n,l,m) included in the file.
@@ -517,43 +541,56 @@
         """
         t0 = time.time()
         if alt_type is not None:
             typeName = alt_type
         else:
             typeName = self.f_type
         folio = Portfolio(hdf5file, extra_types=[typeName])
-        dataFnlm, attrs = folio.read_gvar(typeName, modelName, d_pair)
+        dataFnlm, attrs = folio.read_folio(typeName, modelName, d_fnlm)
+        lm_index, attrs_lm = folio.read_folio(typeName, modelName, lm_ix)
+        if 'dname' in attrs_lm.keys() and attrs_lm['dname'] != d_fnlm:
+            print("Warning! lm index {} belongs to a different database, {}".format(lm_ix, attrs_lm['dname']))
         bdict_info = str_to_bdict(attrs)
-        # Without 'phi_symmetric', can't make sense of f_lm_n array:
-        assert('phi_symmetric' in bdict_info), "Unspecified mandatory item 'phi_symmetric' for hdf5 dataset."
         for x,row in enumerate(dataFnlm):
-            ell,m = _x_to_LM(x, phi_symmetric=self.basis['phi_symmetric'])
-            for n in len(row):
-                self.f_nlm[(n,l,m)] = row[n]
+            l,m = lm_index[x]
+            for n in range(len(row)):
+                self.update_maxes((n,l,m))
+                data_f = row[n]
+                if type(data_f) in [np.ndarray, list]:
+                    if self.use_gvar:
+                        if len(data_f)>1:
+                            self.f_nlm[(n,l,m)] = gvar.gvar(data_f[0],data_f[1])
+                        else:
+                            self.f_nlm[(n,l,m)] = gvar.gvar(data_f[0], 0)
+                    else:
+                        self.f_nlm[(n,l,m)] = data_f[0]
+                else:
+                # elif type(data_f) is float or int:
+                    if self.use_gvar:
+                        self.f_nlm[(n,l,m)] = gvar.gvar(data_f, 0)
+                    else:
+                        self.f_nlm[(n,l,m)] = data_f
         self.t_eval += time.time() - t0
         return dataFnlm, bdict_info
 
-    def writeFnlm_csv(self, csvfile, nlmlist=None, modelName=''):
+    def writeFnlm_csv(self, csvfile, nlmlist=None):
         """Saves <f|nlm> dictionary to CSV file.
 
         Arguments:
             csvfile: CSV file to create or append to
             nlmlist: specific coefficients to write out.
                 If None, then write all entries of self.f_nlm
-            modelName: optional marker saved to first column of csv
-                used in read() to pick out matching coefficients
 
         Recommended use:
             For slow calculations, save each new <f|nlm> coefficient to
             a CSV file, as writeFnlm_csv(csvname, nlmlist=[nlm])
         Also a human-readable output, good for inspection of coefficients.
         """
         # t0 = time.time()
         #'a': Always append, never overwrite. If file does not exist, open(...,'a') creates it.
-        # modelName is saved as 0th column, in case data of multiple types needs to be saved to the same file (avoid this)
         # Default: writeFnlm for all nlm that have been evaluated.
         #    Alternative: only the nlm in nlmlist.
         #    Can use this option to save-as-you-go, with nlmlist=[(nlm)].
         # If this is the first time we write to csvfile, generate a header row:
         makeHeader = not os.path.exists(csvfile)
         self.basis['nMax'] = self.nMax
         self.basis['ellMax'] = self.ellMax
@@ -567,62 +604,58 @@
                 bparams = [r'#'] + [str(lbl) + ': ' + str(prm)
                                      for lbl,prm in self.basis.items()]
                 writer.writerow(bparams)
             if nlmlist is None:
                 nlmlist = self.getNLMlist()
             for nlm in nlmlist:
                 f = self.f_nlm[nlm]
-                mean, std = f.mean, f.sdev
-                newline = [modelName, nlm[0], nlm[1], nlm[2], mean, std]
+                if self.use_gvar:
+                    mean, std = f.mean, f.sdev
+                else:
+                    mean, std = f, 0
+                newline = [nlm[0], nlm[1], nlm[2], mean, std]
                 writer.writerow(newline)
 
     @staticmethod
-    def readFnlm_csv(csvfile, modelName=None):
+    def readFnlm_csv(csvfile, use_gvar=True):
         """Reads <f|nlm> coefficients from CSV file."""
-        # modelName: only import f(nlm) for entries with modelName==modelName
-        # File format (each row): modelName, n,l,m, f.mean, f.sdev
+        # File format (each row): n,l,m, f.mean, f.sdev
         # all rows that are not commented out with '#,' should follow this format
         data_fnlm = {}
         with open(csvfile, 'r') as csvfile:
             reader = csv.reader(csvfile, delimiter=',',
                                 quoting=csv.QUOTE_MINIMAL)
             for row in reader:
                 if row[0]=='#':
                     # skip commented lines and the header
                     continue
-                mName, str_n, str_l, str_m, f_mean, f_std = row
+                str_n, str_l, str_m, f_mean, f_std = row
                 nlm = (int(str_n),int(str_l),int(str_m))
-                # isheader = (mName=="#")
-                # iscomment = False
-                # if len(mName) > 0:
-                #     iscomment = (mName[0]=="#")
-                if (modelName is None or mName==modelName):
+                if use_gvar:
                     data_fnlm[nlm] = gvar.gvar(float(f_mean), float(f_std))
+                else:
+                    data_fnlm[nlm] = float(f_mean)
         #Doesn't create any self.data object, just returns a fnlm_gvar dict.
         # If there are repeated instances of (nlm), data_fnlm is overwritten with the most recent version.
         return data_fnlm
 
-    def importFnlm_csv(self, csvfile, modelName=None):
+    def importFnlm_csv(self, csvfile):
         """Imports <f|nlm> coefficients from CSV file, add to f_nlm.
 
         Note: can be run repeatedly for different files, to add or overwrite
             previous f_nlm values.
 
         * Caution: Basis.basis dictionary items are saved in commented
             header line in CSV file, but not automatically imported.
         * User needs to ensure that Fnlm input 'bdict' matches CSV file.
         Items self.nMax, ellMax will be updated using self.update_maxes().
-
-        * Caution: modelName input here is different from the hdf5 'model'
-            This modelName is an optional string in the first CSV column
-            Only rows with the matching modelName are read into Fnlm.
         """
         # reads the file, and overwrites f_nlm with the results
         t0 = time.time()
-        data_fnlm = self.readFnlm_csv(csvfile, modelName=modelName)
+        data_fnlm = self.readFnlm_csv(csvfile, use_gvar=self.use_gvar)
         for nlm,fdata in data_fnlm.items():
             self.f_nlm[nlm] = fdata
             self.update_maxes(nlm)
         self.t_eval += time.time() - t0
 
     def importFromProjF(self, projF, nlmlist):
         """Fill in f_nlm from a different ProjectFnlm instance."""
```

### Comparing `vsdm-0.1.0/vsdm/ratecalc.py` & `vsdm-0.2.9/vsdm/ratecalc.py`

 * *Files identical despite different names*

### Comparing `vsdm-0.1.0/vsdm/units.py` & `vsdm-0.2.9/vsdm/units.py`

 * *Files identical despite different names*

### Comparing `vsdm-0.1.0/vsdm/wigner.py` & `vsdm-0.2.9/vsdm/wigner.py`

 * *Files identical despite different names*

