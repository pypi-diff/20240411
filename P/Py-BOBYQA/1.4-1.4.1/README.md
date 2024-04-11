# Comparing `tmp/Py-BOBYQA-1.4.tar.gz` & `tmp/Py-BOBYQA-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Py-BOBYQA-1.4.tar", last modified: Tue May 16 02:37:47 2023, max compression
+gzip compressed data, was "Py-BOBYQA-1.4.1.tar", last modified: Thu Apr 11 07:18:29 2024, max compression
```

## Comparing `Py-BOBYQA-1.4.tar` & `Py-BOBYQA-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9704 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/PKG-INFO
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/pybobyqa/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    31506 2021-11-10 06:40:49.000000 Py-BOBYQA-1.4/pybobyqa/controller.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     6179 2021-04-14 00:51:00.000000 Py-BOBYQA-1.4/pybobyqa/diagnostic_info.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     4352 2021-02-25 02:56:44.000000 Py-BOBYQA-1.4/pybobyqa/hessian.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    19959 2021-11-03 06:24:10.000000 Py-BOBYQA-1.4/pybobyqa/model.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    12892 2020-04-20 01:52:14.000000 Py-BOBYQA-1.4/pybobyqa/params.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    49042 2021-11-03 06:32:05.000000 Py-BOBYQA-1.4/pybobyqa/solver.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)    16009 2021-10-11 06:29:48.000000 Py-BOBYQA-1.4/pybobyqa/trust_region.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     8657 2021-11-03 06:24:53.000000 Py-BOBYQA-1.4/pybobyqa/util.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)      924 2023-05-16 02:28:16.000000 Py-BOBYQA-1.4/pybobyqa/version.py
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     1562 2020-04-20 01:52:14.000000 Py-BOBYQA-1.4/pybobyqa/__init__.py
-drwxrwxrwx   0 lindon    (1000) lindon    (1000)        0 2023-05-16 02:39:13.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/dependency_links.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     9704 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/PKG-INFO
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)       69 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/requires.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)      421 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/SOURCES.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        9 2023-05-16 02:39:11.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/top_level.txt
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)        1 2020-04-21 23:25:10.000000 Py-BOBYQA-1.4/Py_BOBYQA.egg-info/zip-safe
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     7208 2021-12-09 02:59:49.000000 Py-BOBYQA-1.4/README.rst
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)       38 2023-05-16 02:39:14.000000 Py-BOBYQA-1.4/setup.cfg
--rwxrwxrwx   0 lindon    (1000) lindon    (1000)     2734 2023-05-16 02:30:14.000000 Py-BOBYQA-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:18:29.326900 Py-BOBYQA-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-11 07:18:29.326900 Py-BOBYQA-1.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:18:29.326900 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-04-11 07:18:29.000000 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-11 07:18:29.000000 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:18:29.000000 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 07:18:29.000000 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 07:18:29.000000 Py-BOBYQA-1.4.1/Py_BOBYQA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:18:29.326900 Py-BOBYQA-1.4.1/pybobyqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31506 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/diagnostic_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49042 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pybobyqa/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-11 07:18:22.000000 Py-BOBYQA-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:18:29.326900 Py-BOBYQA-1.4.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Py-BOBYQA-1.4/pybobyqa/controller.py` & `Py-BOBYQA-1.4.1/pybobyqa/controller.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/diagnostic_info.py` & `Py-BOBYQA-1.4.1/pybobyqa/diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/hessian.py` & `Py-BOBYQA-1.4.1/pybobyqa/hessian.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/model.py` & `Py-BOBYQA-1.4.1/pybobyqa/model.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/params.py` & `Py-BOBYQA-1.4.1/pybobyqa/params.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/solver.py` & `Py-BOBYQA-1.4.1/pybobyqa/solver.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/trust_region.py` & `Py-BOBYQA-1.4.1/pybobyqa/trust_region.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/util.py` & `Py-BOBYQA-1.4.1/pybobyqa/util.py`

 * *Files identical despite different names*

### Comparing `Py-BOBYQA-1.4/pybobyqa/__init__.py` & `Py-BOBYQA-1.4.1/pybobyqa/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,13 @@
 
 
 """
 
 # Ensure compatibility with Python 2
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from .version import __version__
-__all__ = ['__version__']
+__version__ = '1.4.1'
 
 # Main solver & exit flags
 from .solver import *
-__all__ += ['solve']
+__all__ = ['solve']
```

### Comparing `Py-BOBYQA-1.4/README.rst` & `Py-BOBYQA-1.4.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    :alt: Total downloads
 
 Py-BOBYQA is a flexible package for solving bound-constrained general objective minimization, without requiring derivatives of the objective. At its core, it is a Python implementation of the BOBYQA algorithm by Powell, but Py-BOBYQA has extra features improving its performance on some problems (see the papers below for details). Py-BOBYQA is particularly useful when evaluations of the objective function are expensive and/or noisy.
 
 More details about Py-BOBYQA and its enhancements over BOBYQA can be found in our papers:
 
 1. Coralia Cartis, Jan Fiala, Benjamin Marteau and Lindon Roberts, `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41 [`arXiv preprint: 1804.00154 <https://arxiv.org/abs/1804.00154>`_] 
-2. Coralia Cartis, Lindon Roberts and Oliver Sheridan-Methven, `Escaping local minima with derivative-free methods: a numerical investigation <https://doi.org/10.1080/02331934.2021.1883015>`_, *Optimization* (2021). [`arXiv preprint: 1812.11343 <https://arxiv.org/abs/1812.11343>`_] 
+2. Coralia Cartis, Lindon Roberts and Oliver Sheridan-Methven, `Escaping local minima with derivative-free methods: a numerical investigation <https://doi.org/10.1080/02331934.2021.1883015>`_, *Optimization*, 71:8 (2022), pp. 2343-2373. [`arXiv preprint: 1812.11343 <https://arxiv.org/abs/1812.11343>`_] 
 
 Please cite [1] when using Py-BOBYQA for local optimization, and [1,2] when using Py-BOBYQA's global optimization heuristic functionality. For reproducibility of all figures, please feel free to contact the authors.
 
 The original paper by Powell is: M. J. D. Powell, The BOBYQA algorithm for bound constrained optimization without derivatives, technical report DAMTP 2009/NA06, University of Cambridge (2009), and the original Fortran implementation is available `here <http://mat.uc.pt/~zhang/software.html>`_.
 
 If you are interested in solving least-squares minimization problems, you may wish to try `DFO-LS <https://github.com/numericalalgorithmsgroup/dfols>`_, which has the same features as Py-BOBYQA (plus some more), and exploits the least-squares problem structure, so performs better on such problems.
 
@@ -43,27 +43,27 @@
 --------
 If you use Py-BOBYQA in a paper, please cite:
 
 Cartis, C., Fiala, J., Marteau, B. and Roberts, L., Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41.
 
 If you use Py-BOBYQA's global optimization heuristic, please cite the above and also
 
-Cartis, C., Roberts, L. and Sheridan-Methven, O., Escaping local minima with derivative-free methods: a numerical investigation, Optimization, (2021). 
+Cartis, C., Roberts, L. and Sheridan-Methven, O., Escaping local minima with derivative-free methods: a numerical investigation, Optimization, 71:8 (2022), pp. 2343-2373. 
 
 Requirements
 ------------
 Py-BOBYQA requires the following software to be installed:
 
-* Python 2.7 or Python 3 (http://www.python.org/)
+* Python 3.8 or higher (http://www.python.org/)
 
 Additionally, the following python packages should be installed (these will be installed automatically if using *pip*, see `Installation using pip`_):
 
-* NumPy 1.11 or higher (http://www.numpy.org/)
-* SciPy 0.18 or higher (http://www.scipy.org/)
-* Pandas 0.17 or higher (http://pandas.pydata.org/)
+* NumPy (http://www.numpy.org/)
+* SciPy (http://www.scipy.org/)
+* Pandas (http://pandas.pydata.org/)
 
 **Optional package:** Py-BOBYQA versions 1.2 and higher also support the `trustregion <https://github.com/lindonroberts/trust-region>`_ package for fast trust-region subproblem solutions. To install this, make sure you have a Fortran compiler (e.g. `gfortran <https://gcc.gnu.org/wiki/GFortran>`_) and NumPy installed, then run :code:`pip install trustregion`. You do not have to have trustregion installed for Py-BOBYQA to work, and it is not installed by default.
 
 Installation using pip
 ----------------------
 For easy installation, use `pip <http://www.pip-installer.org/>`_ as root:
 
@@ -121,19 +121,20 @@
  .. code-block:: bash
 
     $ git pull
     $ [sudo] pip install .  # with admin privileges
 
 Testing
 -------
-If you installed Py-BOBYQA manually, you can test your installation by running:
+If you installed Py-BOBYQA manually, you can test your installation using the pytest package:
 
  .. code-block:: bash
 
-    $ python setup.py test
+    $ pip install pytest
+    $ python -m pytest --pyargs pybobyqa
 
 Alternatively, the HTML documentation provides some simple examples of how to run Py-BOBYQA.
 
 Examples
 --------
 Examples of how to run Py-BOBYQA are given in the `online documentation <https://numericalalgorithmsgroup.github.io/pybobyqa/>`_, and the `examples directory <https://github.com/numericalalgorithmsgroup/pybobyqa/tree/master/examples>`_ in Github.
```

