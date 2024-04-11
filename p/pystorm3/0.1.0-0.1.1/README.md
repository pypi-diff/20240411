# Comparing `tmp/pystorm3-0.1.0.tar.gz` & `tmp/pystorm3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystorm3-0.1.0.tar", last modified: Wed Apr 10 16:23:30 2024, max compression
+gzip compressed data, was "pystorm3-0.1.1.tar", last modified: Thu Apr 11 12:26:43 2024, max compression
```

## Comparing `pystorm3-0.1.0.tar` & `pystorm3-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-10 16:23:30.281748 pystorm3-0.1.0/
--rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.0/LICENSE
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2652 2024-04-10 16:23:30.281748 pystorm3-0.1.0/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-10 16:21:02.000000 pystorm3-0.1.0/README.md
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-10 16:23:30.281748 pystorm3-0.1.0/pystorm/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       77 2024-04-10 16:12:15.000000 pystorm3-0.1.0/pystorm/__init__.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-10 16:23:30.281748 pystorm3-0.1.0/pystorm/timefreq/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       24 2024-04-10 16:12:02.000000 pystorm3-0.1.0/pystorm/timefreq/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2377 2024-04-10 16:09:04.000000 pystorm3-0.1.0/pystorm/timefreq/welch_psd.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-10 16:23:30.281748 pystorm3-0.1.0/pystorm/utils/
--rw-r--r--   0 dboutet   (3170) meg       (1042)       51 2024-04-10 16:00:40.000000 pystorm3-0.1.0/pystorm/utils/__init__.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)    19391 2024-04-08 13:08:25.000000 pystorm3-0.1.0/pystorm/utils/minitorch.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)      649 2024-04-08 12:59:22.000000 pystorm3-0.1.0/pystorm/utils/type_safety.py
--rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-10 16:03:10.000000 pystorm3-0.1.0/pystorm/version.py
-drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-10 16:23:30.281748 pystorm3-0.1.0/pystorm3.egg-info/
--rw-r--r--   0 dboutet   (3170) meg       (1042)     2652 2024-04-10 16:23:30.000000 pystorm3-0.1.0/pystorm3.egg-info/PKG-INFO
--rw-r--r--   0 dboutet   (3170) meg       (1042)      365 2024-04-10 16:23:30.000000 pystorm3-0.1.0/pystorm3.egg-info/SOURCES.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-10 16:23:30.000000 pystorm3-0.1.0/pystorm3.egg-info/dependency_links.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       25 2024-04-10 16:23:30.000000 pystorm3-0.1.0/pystorm3.egg-info/requires.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-10 16:23:30.000000 pystorm3-0.1.0/pystorm3.egg-info/top_level.txt
--rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-10 16:23:30.281748 pystorm3-0.1.0/setup.cfg
--rw-r--r--   0 dboutet   (3170) meg       (1042)     1487 2024-04-10 16:06:04.000000 pystorm3-0.1.0/setup.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.776595 pystorm3-0.1.1/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    35140 2024-04-10 15:50:21.000000 pystorm3-0.1.1/LICENSE
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:26:43.775595 pystorm3-0.1.1/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1841 2024-04-10 16:21:02.000000 pystorm3-0.1.1/README.md
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      111 2024-04-11 11:59:21.000000 pystorm3-0.1.1/pystorm/__init__.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/signal_processing/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       26 2024-04-11 11:12:00.000000 pystorm3-0.1.1/pystorm/signal_processing/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     4742 2024-04-11 12:21:03.000000 pystorm3-0.1.1/pystorm/signal_processing/band_filter.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/timefreq/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       47 2024-04-11 11:56:35.000000 pystorm3-0.1.1/pystorm/timefreq/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2647 2024-04-11 12:22:38.000000 pystorm3-0.1.1/pystorm/timefreq/hilbert.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2377 2024-04-10 16:09:04.000000 pystorm3-0.1.1/pystorm/timefreq/welch_psd.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm/utils/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       51 2024-04-10 16:00:40.000000 pystorm3-0.1.1/pystorm/utils/__init__.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)    29490 2024-04-11 12:24:01.000000 pystorm3-0.1.1/pystorm/utils/minitorch.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      716 2024-04-11 12:18:49.000000 pystorm3-0.1.1/pystorm/utils/type_safety.py
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       19 2024-04-11 11:50:54.000000 pystorm3-0.1.1/pystorm/version.py
+drwxr-sr-x   0 dboutet   (3170) meg       (1042)        0 2024-04-11 12:26:43.775595 pystorm3-0.1.1/pystorm3.egg-info/
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     2714 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/PKG-INFO
+-rw-r--r--   0 dboutet   (3170) meg       (1042)      472 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/SOURCES.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        1 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/dependency_links.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       57 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/requires.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)        8 2024-04-11 12:26:43.000000 pystorm3-0.1.1/pystorm3.egg-info/top_level.txt
+-rw-r--r--   0 dboutet   (3170) meg       (1042)       38 2024-04-11 12:26:43.776595 pystorm3-0.1.1/setup.cfg
+-rw-r--r--   0 dboutet   (3170) meg       (1042)     1573 2024-04-11 10:25:02.000000 pystorm3-0.1.1/setup.py
```

### Comparing `pystorm3-0.1.0/LICENSE` & `pystorm3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.0/PKG-INFO` & `pystorm3-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
@@ -13,16 +13,18 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.2.0
+Requires-Dist: torch>=2.2.0
 Requires-Dist: numpy>=1.26
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: torchaudio>=2.2.0
 
 # Pystorm
 Python implementation of various functions from the [Brainstorm](https://neuroimage.usc.edu/brainstorm/) [repository](https://github.com/brainstorm-tools/brainstorm3), often written for GPU compatibility and/or jit compilation.
 
 ## Note on the current scope of Pystorm
 Pystorm does not handle interactions with Brainstorm or matlab and, in its current state, does not handle loading of data files.
```

### Comparing `pystorm3-0.1.0/README.md` & `pystorm3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.0/pystorm/timefreq/welch_psd.py` & `pystorm3-0.1.1/pystorm/timefreq/welch_psd.py`

 * *Files identical despite different names*

### Comparing `pystorm3-0.1.0/pystorm/utils/minitorch.py` & `pystorm3-0.1.1/pystorm/utils/minitorch.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,50 @@
 A module that serves as lightweight pytorch.
 
 The intent is to possibly minimize RAM usage from functions that would be executed by multiple processes in parallel on the GPU.
 """
 
 from torch.fft import rfft as trfft
 from torch.fft import rfftfreq as trfftfreq 
+from torch.fft import fft as tfft
+from torch.fft import ifft as tifft
+from torch.fft import fftfreq as tfftfreq 
 from torch import cat as tcat
 from torch import linspace as tlinspace
 from torch import pi as tpi
 from torch import arange as tarange
 from torch import zeros as tzeros
 from torch import zeros_like as  tzeros_like
 from torch import ones_like as  tones_like
 from torch import ones as tones
 from torch import as_tensor as tas_tensor
 from torch import from_numpy as tfrom_numpy
 from torch import complex64, complex128
 from torch import cos as tcos
 from torch import eye as teye
-
+from torch import argwhere as targwhere
+from torchaudio.functional import convolve as tconvolve
+from torchaudio.functional import fftconvolve as tfftconvolve
+from torch import float16,float32,float64
+from torch import set_default_dtype
 pi = tpi
 
+__default_dtype__ = float64
+set_default_dtype(__default_dtype__)
+def set_minitorch_default_dtype(default_type = "float64"):
+    global __default_dtype__
+    if default_type == "float16":
+        __default_dtype__ = float16
+        print("Warning: Pytorch only supports FFT of signals whose length are powers of 2 in this float type")
+    elif default_type == "float32":
+        __default_dtype__ = float32
+    else:
+        __default_dtype__ = float64
+    set_default_dtype(__default_dtype__)
+    
 
 def eye(*args, **kwargs):
     """
     eye(n, m=None, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
 
     Returns a 2-D tensor with ones on the diagonal and zeros elsewhere.
 
@@ -417,8 +437,217 @@
 
     Args:
         input (Tensor): the input tensor.
 
     Keyword args:
         out (Tensor, optional): the output tensor.
     """
-    return tcos(*args,**kwargs)
+    return tcos(*args,**kwargs)
+
+
+def fft(*args,**kwargs):
+    """  
+    fft(input, n=None, dim=-1, norm=None, *, out=None) -> Tensor
+
+    Computes the one dimensional discrete Fourier transform of :attr:`input`.
+
+    Note:
+        The Fourier domain representation of any real signal satisfies the
+        Hermitian property: `X[i] = conj(X[-i])`. This function always returns both
+        the positive and negative frequency terms even though, for real inputs, the
+        negative frequencies are redundant. :func:`~torch.fft.rfft` returns the
+        more compact one-sided representation where only the positive frequencies
+        are returned.
+
+    Note:
+        Supports torch.half and torch.chalf on CUDA with GPU Architecture SM53 or greater.
+        However it only supports powers of 2 signal length in every transformed dimension.
+
+    Args:
+        input (Tensor): the input tensor
+        n (int, optional): Signal length. If given, the input will either be zero-padded
+            or trimmed to this length before computing the FFT.
+        dim (int, optional): The dimension along which to take the one dimensional FFT.
+        norm (str, optional): Normalization mode. For the forward transform
+            (:func:`~torch.fft.fft`), these correspond to:
+
+            * ``"forward"`` - normalize by ``1/n``
+            * ``"backward"`` - no normalization
+            * ``"ortho"`` - normalize by ``1/sqrt(n)`` (making the FFT orthonormal)
+
+            Calling the backward transform (:func:`~torch.fft.ifft`) with the same
+            normalization mode will apply an overall normalization of ``1/n`` between
+            the two transforms. This is required to make :func:`~torch.fft.ifft`
+            the exact inverse.
+
+            Default is ``"backward"`` (no normalization).
+
+    Keyword args:
+        out (Tensor, optional): the output tensor.
+    """
+    return tfft(*args,**kwargs)
+
+def ifft(*args,**kwargs):
+    """
+    ifft(input, n=None, dim=-1, norm=None, *, out=None) -> Tensor
+
+    Computes the one dimensional inverse discrete Fourier transform of :attr:`input`.
+
+    Note:
+        Supports torch.half and torch.chalf on CUDA with GPU Architecture SM53 or greater.
+        However it only supports powers of 2 signal length in every transformed dimension.
+
+    Args:
+        input (Tensor): the input tensor
+        n (int, optional): Signal length. If given, the input will either be zero-padded
+            or trimmed to this length before computing the IFFT.
+        dim (int, optional): The dimension along which to take the one dimensional IFFT.
+        norm (str, optional): Normalization mode. For the backward transform
+            (:func:`~torch.fft.ifft`), these correspond to:
+
+            * ``"forward"`` - no normalization
+            * ``"backward"`` - normalize by ``1/n``
+            * ``"ortho"`` - normalize by ``1/sqrt(n)`` (making the IFFT orthonormal)
+
+            Calling the forward transform (:func:`~torch.fft.fft`) with the same
+            normalization mode will apply an overall normalization of ``1/n`` between
+            the two transforms. This is required to make :func:`~torch.fft.ifft`
+            the exact inverse.
+
+            Default is ``"backward"`` (normalize by ``1/n``).
+
+    Keyword args:
+        out (Tensor, optional): the output tensor.
+    """
+    return tifft(*args,**kwargs)
+
+def fftfreq(*args,**kwargs):
+    """
+    fftfreq(n, d=1.0, *, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False) -> Tensor
+
+    Computes the discrete Fourier Transform sample frequencies for a signal of size :attr:`n`.
+
+    Note:
+        By convention, :func:`~torch.fft.fft` returns positive frequency terms
+        first, followed by the negative frequencies in reverse order, so that
+        ``f[-i]`` for all :math:`0 < i \leq n/2`` in Python gives the negative
+        frequency terms. For an FFT of length :attr:`n` and with inputs spaced in
+        length unit :attr:`d`, the frequencies are::
+
+            f = [0, 1, ..., (n - 1) // 2, -(n // 2), ..., -1] / (d * n)
+
+    Note:
+        For even lengths, the Nyquist frequency at ``f[n/2]`` can be thought of as
+        either negative or positive. :func:`~torch.fft.fftfreq` follows NumPy's
+        convention of taking it to be negative.
+
+    Args:
+        n (int): the FFT length
+        d (float, optional): The sampling length scale.
+            The spacing between individual samples of the FFT input.
+            The default assumes unit spacing, dividing that result by the actual
+            spacing gives the result in physical frequency units.
+
+    Keyword Args:
+        out (Tensor, optional): the output tensor.
+        dtype (:class:`torch.dtype`, optional): the desired data type of returned tensor.
+            Default: if ``None``, uses a global default (see :func:`torch.set_default_dtype`).
+        layout (:class:`torch.layout`, optional): the desired layout of returned Tensor.
+            Default: ``torch.strided``.
+        device (:class:`torch.device`, optional): the desired device of returned tensor.
+            Default: if ``None``, uses the current device for the default tensor type
+            (see :func:`torch.set_default_device`). :attr:`device` will be the CPU
+            for CPU tensor types and the current CUDA device for CUDA tensor types.
+        requires_grad (bool, optional): If autograd should record operations on the
+            returned tensor. Default: ``False``.
+
+    """
+    return tfftfreq(*args,**kwargs)
+
+
+def convolve(*args, **kwargs):
+    r"""
+    Convolves inputs along their last dimension using the direct method.
+    Note that, in contrast to :meth:`torch.nn.functional.conv1d`, which actually applies the valid cross-correlation
+    operator, this function applies the true `convolution`_ operator.
+
+    .. devices:: CPU CUDA
+
+    .. properties:: Autograd TorchScript
+
+    Args:
+        x (torch.Tensor): First convolution operand, with shape `(..., N)`.
+        y (torch.Tensor): Second convolution operand, with shape `(..., M)`
+            (leading dimensions must be broadcast-able with those of ``x``).
+        mode (str, optional): Must be one of ("full", "valid", "same").
+
+            * "full": Returns the full convolution result, with shape `(..., N + M - 1)`. (Default)
+            * "valid": Returns the segment of the full convolution result corresponding to where
+              the two inputs overlap completely, with shape `(..., max(N, M) - min(N, M) + 1)`.
+            * "same": Returns the center segment of the full convolution result, with shape `(..., N)`.
+
+    Returns:
+        torch.Tensor: Result of convolving ``x`` and ``y``, with shape `(..., L)`, where
+        the leading dimensions match those of ``x`` and `L` is dictated by ``mode``.
+
+    .. _convolution:
+        https://en.wikipedia.org/wiki/Convolution
+    """
+    return tconvolve(*args,**kwargs)
+
+    
+def fftconvolve(*args, **kwargs):
+    r"""
+    Convolves inputs along their last dimension using FFT. For inputs with large last dimensions, this function
+    is generally much faster than :meth:`convolve`.
+    Note that, in contrast to :meth:`torch.nn.functional.conv1d`, which actually applies the valid cross-correlation
+    operator, this function applies the true `convolution`_ operator.
+    Also note that this function can only output float tensors (int tensor inputs will be cast to float).
+
+    .. devices:: CPU CUDA
+
+    .. properties:: Autograd TorchScript
+
+    Args:
+        x (torch.Tensor): First convolution operand, with shape `(..., N)`.
+        y (torch.Tensor): Second convolution operand, with shape `(..., M)`
+            (leading dimensions must be broadcast-able with those of ``x``).
+        mode (str, optional): Must be one of ("full", "valid", "same").
+
+            * "full": Returns the full convolution result, with shape `(..., N + M - 1)`. (Default)
+            * "valid": Returns the segment of the full convolution result corresponding to where
+              the two inputs overlap completely, with shape `(..., max(N, M) - min(N, M) + 1)`.
+            * "same": Returns the center segment of the full convolution result, with shape `(..., N)`.
+
+    Returns:
+        torch.Tensor: Result of convolving ``x`` and ``y``, with shape `(..., L)`, where
+        the leading dimensions match those of ``x`` and `L` is dictated by ``mode``.
+
+    .. _convolution:
+        https://en.wikipedia.org/wiki/Convolution
+    """
+    return tfftconvolve(*args,**kwargs)
+
+
+def argwhere(*args, **kwargs):
+    """
+    argwhere(input) -> Tensor
+
+    Returns a tensor containing the indices of all non-zero elements of
+    :attr:`input`.  Each row in the result contains the indices of a non-zero
+    element in :attr:`input`. The result is sorted lexicographically, with
+    the last index changing the fastest (C-style).
+
+    If :attr:`input` has :math:`n` dimensions, then the resulting indices tensor
+    :attr:`out` is of size :math:`(z \times n)`, where :math:`z` is the total number of
+    non-zero elements in the :attr:`input` tensor.
+
+    .. note::
+        This function is similar to NumPy's `argwhere`.
+
+        When :attr:`input` is on CUDA, this function causes host-device synchronization.
+
+    Args:
+        {input}
+
+    """
+    return targwhere(*args,**kwargs)
```

### Comparing `pystorm3-0.1.0/pystorm/utils/type_safety.py` & `pystorm3-0.1.1/pystorm/utils/type_safety.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from .minitorch import as_tensor, from_numpy
+from .minitorch import as_tensor, from_numpy, __default_dtype__
 
 def ensure_torch(x, type_float = False):
     try:
         x = as_tensor(x)
         if type_float:
-            x = x.float()
+            x = x.type(__default_dtype__)
     except:
         try:
             x = from_numpy(x)
             if type_float:
-                x = x.float()
+                x = x.type(__default_dtype__)
         except:
             pass
     
     if type_float:
         try:
-            x = x.float()
+            x = x.type(__default_dtype__)
         except:
             pass
     return x
 
 def ensure_numpy(x):
     
     try:
```

### Comparing `pystorm3-0.1.0/pystorm3.egg-info/PKG-INFO` & `pystorm3-0.1.1/pystorm3.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystorm3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of some Brainstorm functions
 Home-page: https://github.com/NeuroLife77/pystorm
 Author: Dominic Boutet
 Author-email: dominic.boutet@mail.mcgill.ca
 Maintainer: Dominic Boutet
 Maintainer-email: dominic.boutet@mail.mcgill.ca
 License: GPL-3.0 license
@@ -13,16 +13,18 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch==2.2.0
+Requires-Dist: torch>=2.2.0
 Requires-Dist: numpy>=1.26
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: torchaudio>=2.2.0
 
 # Pystorm
 Python implementation of various functions from the [Brainstorm](https://neuroimage.usc.edu/brainstorm/) [repository](https://github.com/brainstorm-tools/brainstorm3), often written for GPU compatibility and/or jit compilation.
 
 ## Note on the current scope of Pystorm
 Pystorm does not handle interactions with Brainstorm or matlab and, in its current state, does not handle loading of data files.
```

### Comparing `pystorm3-0.1.0/setup.py` & `pystorm3-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,18 @@
    author='Dominic Boutet',
    author_email='dominic.boutet@mail.mcgill.ca',
    maintainer='Dominic Boutet',
    maintainer_email='dominic.boutet@mail.mcgill.ca',
    url='https://github.com/NeuroLife77/pystorm',
    packages=find_packages(),
    install_requires=[
-                        'torch==2.2.0',
-                        'numpy>=1.26'
+                        'torch>=2.2.0',
+                        'numpy>=1.26',
+                        'scipy>=1.13.0',
+                        'torchaudio>=2.2.0'
     ],
    python_requires='>=3.9',
    keywords = [
                     'neuroscience',
                     'neuroimaging',
                     'neural oscillations',
                     'time series analysis',
```

