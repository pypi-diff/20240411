# Comparing `tmp/DFO-LS-1.4.0.tar.gz` & `tmp/DFO-LS-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFO-LS-1.4.0.tar", last modified: Mon Jan 29 06:21:35 2024, max compression
+gzip compressed data, was "DFO-LS-1.4.1.tar", last modified: Thu Apr 11 06:25:18 2024, max compression
```

## Comparing `DFO-LS-1.4.0.tar` & `DFO-LS-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxrwxr-x   0 lindon    (1000) lindon    (1000)        0 2024-01-29 06:21:35.604946 DFO-LS-1.4.0/
-drwxrwxr-x   0 lindon    (1000) lindon    (1000)        0 2024-01-29 06:21:35.592946 DFO-LS-1.4.0/DFO_LS.egg-info/
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     7688 2024-01-29 06:21:35.000000 DFO-LS-1.4.0/DFO_LS.egg-info/PKG-INFO
--rw-rw-r--   0 lindon    (1000) lindon    (1000)      397 2024-01-29 06:21:35.000000 DFO-LS-1.4.0/DFO_LS.egg-info/SOURCES.txt
--rw-rw-r--   0 lindon    (1000) lindon    (1000)        1 2024-01-29 06:21:35.000000 DFO-LS-1.4.0/DFO_LS.egg-info/dependency_links.txt
--rw-rw-r--   0 lindon    (1000) lindon    (1000)       69 2024-01-29 06:21:35.000000 DFO-LS-1.4.0/DFO_LS.egg-info/requires.txt
--rw-rw-r--   0 lindon    (1000) lindon    (1000)        6 2024-01-29 06:21:35.000000 DFO-LS-1.4.0/DFO_LS.egg-info/top_level.txt
--rw-rw-r--   0 lindon    (1000) lindon    (1000)        1 2024-01-23 00:39:34.000000 DFO-LS-1.4.0/DFO_LS.egg-info/zip-safe
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    35147 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/LICENSE.txt
--rw-rw-r--   0 lindon    (1000) lindon    (1000)       20 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/MANIFEST.in
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     7688 2024-01-29 06:21:35.604946 DFO-LS-1.4.0/PKG-INFO
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     6403 2024-01-25 03:48:53.000000 DFO-LS-1.4.0/README.rst
-drwxrwxr-x   0 lindon    (1000) lindon    (1000)        0 2024-01-29 06:21:35.604946 DFO-LS-1.4.0/dfols/
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     1626 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/__init__.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    42769 2024-01-25 03:33:30.000000 DFO-LS-1.4.0/dfols/controller.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     6081 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/diagnostic_info.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     4262 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/hessian.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    18809 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/model.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    17557 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/params.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    61264 2024-01-25 03:46:51.000000 DFO-LS-1.4.0/dfols/solver.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)    24603 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/trust_region.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     9852 2024-01-23 00:29:43.000000 DFO-LS-1.4.0/dfols/util.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)      926 2024-01-29 04:50:33.000000 DFO-LS-1.4.0/dfols/version.py
--rw-rw-r--   0 lindon    (1000) lindon    (1000)       38 2024-01-29 06:21:35.604946 DFO-LS-1.4.0/setup.cfg
--rw-rw-r--   0 lindon    (1000) lindon    (1000)     2745 2024-01-29 06:18:37.000000 DFO-LS-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:25:18.987245 DFO-LS-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:25:18.987245 DFO-LS-1.4.1/DFO_LS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-11 06:25:18.000000 DFO-LS-1.4.1/DFO_LS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-11 06:25:18.000000 DFO-LS-1.4.1/DFO_LS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 06:25:18.000000 DFO-LS-1.4.1/DFO_LS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 06:25:18.000000 DFO-LS-1.4.1/DFO_LS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 06:25:18.000000 DFO-LS-1.4.1/DFO_LS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-11 06:25:18.987245 DFO-LS-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 06:25:18.987245 DFO-LS-1.4.1/dfols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42769 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/diagnostic_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18809 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17557 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61264 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/dfols/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-11 06:25:14.000000 DFO-LS-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 06:25:18.987245 DFO-LS-1.4.1/setup.cfg
```

### Comparing `DFO-LS-1.4.0/DFO_LS.egg-info/PKG-INFO` & `DFO-LS-1.4.1/DFO_LS.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 Metadata-Version: 2.1
 Name: DFO-LS
-Version: 1.4.0
+Version: 1.4.1
 Summary: A flexible derivative-free solver for (bound constrained) nonlinear least-squares minimization
-Home-page: https://github.com/numericalalgorithmsgroup/dfols/
-Author: Lindon Roberts
-Author-email: lindon.roberts@anu.edu.au
-License: GNU GPL
-Download-URL: https://github.com/numericalalgorithmsgroup/dfols/archive/v1.4.0.tar.gz
-Keywords: mathematics derivative free optimization nonlinear least squares
-Platform: UNKNOWN
+Author-email: Lindon Roberts <lindon.roberts@sydney.edu.au>
+Maintainer-email: Lindon Roberts <lindon.roberts@sydney.edu.au>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/numericalalgorithmsgroup/dfols
+Project-URL: Download, https://github.com/numericalalgorithmsgroup/dfols/releases/
+Project-URL: Bug Tracker, https://github.com/numericalalgorithmsgroup/dfols/issues/
+Project-URL: Documentation, https://numericalalgorithmsgroup.github.io/dfols/
+Project-URL: Source Code, https://github.com/numericalalgorithmsgroup/dfols
+Keywords: mathematics,optimization,least squares,derivative free optimization,nonlinear least squares
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Provides-Extra: trustregion
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.11
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: Sphinx; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Provides-Extra: trustregion
+Requires-Dist: trustregion>=1.1; extra == "trustregion"
 
 ===================================================
 DFO-LS: Derivative-Free Optimizer for Least-Squares
 ===================================================
 
 .. image::  https://github.com/numericalalgorithmsgroup/dfols/actions/workflows/python_testing.yml/badge.svg
    :target: https://github.com/numericalalgorithmsgroup/dfols/actions
@@ -66,27 +80,27 @@
 --------
 If you use DFO-LS in a paper, please cite:
 
 Cartis, C., Fiala, J., Marteau, B. and Roberts, L., `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41.
 
 If you use DFO-LS for problems with constraints, including bound constraints, please also cite:
 
-Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://arxiv.org/abs/2111.05443>`_, *arXiv preprint arXiv:2111.05443*, (2021).
+Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://doi.org/10.1137/21M1460971>`_, *SIAM Journal on Optimization*, 21:4 (2022), pp. 2552-2579.
 
 Requirements
 ------------
 DFO-LS requires the following software to be installed:
 
-* Python 2.7 or Python 3 (http://www.python.org/)
+* Python 3.9 or higher (http://www.python.org/)
 
 Additionally, the following python packages should be installed (these will be installed automatically if using *pip*, see `Installation using pip`_):
 
-* NumPy 1.11 or higher (http://www.numpy.org/)
-* SciPy 1.11 or higher (http://www.scipy.org/)
-* Pandas 0.17 or higher (http://pandas.pydata.org/)
+* NumPy (http://www.numpy.org/)
+* SciPy version 1.11 or higher (http://www.scipy.org/)
+* Pandas (http://pandas.pydata.org/)
 
 **Optional package:** DFO-LS versions 1.2 and higher also support the `trustregion <https://github.com/lindonroberts/trust-region>`_ package for fast trust-region subproblem solutions. To install this, make sure you have a Fortran compiler (e.g. `gfortran <https://gcc.gnu.org/wiki/GFortran>`_) and NumPy installed, then run :code:`pip install trustregion`. You do not have to have trustregion installed for DFO-LS to work, and it is not installed by default.
 
 Installation using conda
 ------------------------
 DFO-LS can be directly installed in Anaconda environments using `conda-forge <https://anaconda.org/conda-forge/dfo-ls>`_:
 
@@ -143,28 +157,29 @@
 
  .. code-block:: bash
 
     $ pip install --user .
 
 instead.
 
-To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`setup.py`) and rerun the installation using :code:`pip`, as above:
+To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`pyproject.toml`) and rerun the installation using :code:`pip`, as above:
 
  .. code-block:: bash
 
     $ git pull
     $ [sudo] pip install .  # with admin privileges
 
 Testing
 -------
-If you installed DFO-LS manually, you can test your installation by running:
+If you installed DFO-LS manually, you can test your installation using the pytest package:
 
  .. code-block:: bash
 
-    $ python setup.py test
+    $ pip install pytest
+    $ python -m pytest --pyargs dfols
 
 Alternatively, the HTML documentation provides some simple examples of how to run DFO-LS.
 
 Examples
 --------
 Examples of how to run DFO-LS are given in the `documentation <https://numericalalgorithmsgroup.github.io/dfols/>`_, and the `examples <https://github.com/numericalalgorithmsgroup/dfols/tree/master/examples>`_ directory in Github.
 
@@ -176,14 +191,12 @@
 
     $ [sudo] pip uninstall DFO-LS
 
 If DFO-LS was installed manually you have to remove the installed files by hand (located in your python site-packages directory).
 
 Bugs
 ----
-Please report any bugs using GitHub's issue tracker.
+Please report any bugs using `GitHub's issue tracker <https://github.com/numericalalgorithmsgroup/dfols/issues>`_.
 
 License
 -------
 This algorithm is released under the GNU GPL license. Please `contact NAG <http://www.nag.com/content/worldwide-contact-information>`_ for alternative licensing.
-
-
```

### Comparing `DFO-LS-1.4.0/LICENSE.txt` & `DFO-LS-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/PKG-INFO` & `DFO-LS-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 Metadata-Version: 2.1
 Name: DFO-LS
-Version: 1.4.0
+Version: 1.4.1
 Summary: A flexible derivative-free solver for (bound constrained) nonlinear least-squares minimization
-Home-page: https://github.com/numericalalgorithmsgroup/dfols/
-Author: Lindon Roberts
-Author-email: lindon.roberts@anu.edu.au
-License: GNU GPL
-Download-URL: https://github.com/numericalalgorithmsgroup/dfols/archive/v1.4.0.tar.gz
-Keywords: mathematics derivative free optimization nonlinear least squares
-Platform: UNKNOWN
+Author-email: Lindon Roberts <lindon.roberts@sydney.edu.au>
+Maintainer-email: Lindon Roberts <lindon.roberts@sydney.edu.au>
+License: GPL-3.0-or-later
+Project-URL: Homepage, https://github.com/numericalalgorithmsgroup/dfols
+Project-URL: Download, https://github.com/numericalalgorithmsgroup/dfols/releases/
+Project-URL: Bug Tracker, https://github.com/numericalalgorithmsgroup/dfols/issues/
+Project-URL: Documentation, https://numericalalgorithmsgroup.github.io/dfols/
+Project-URL: Source Code, https://github.com/numericalalgorithmsgroup/dfols
+Keywords: mathematics,optimization,least squares,derivative free optimization,nonlinear least squares
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: IPython
 Classifier: Framework :: Jupyter
-Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Provides-Extra: trustregion
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: numpy
+Requires-Dist: scipy>=1.11
+Requires-Dist: pandas
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: Sphinx; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
+Provides-Extra: trustregion
+Requires-Dist: trustregion>=1.1; extra == "trustregion"
 
 ===================================================
 DFO-LS: Derivative-Free Optimizer for Least-Squares
 ===================================================
 
 .. image::  https://github.com/numericalalgorithmsgroup/dfols/actions/workflows/python_testing.yml/badge.svg
    :target: https://github.com/numericalalgorithmsgroup/dfols/actions
@@ -66,27 +80,27 @@
 --------
 If you use DFO-LS in a paper, please cite:
 
 Cartis, C., Fiala, J., Marteau, B. and Roberts, L., `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41.
 
 If you use DFO-LS for problems with constraints, including bound constraints, please also cite:
 
-Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://arxiv.org/abs/2111.05443>`_, *arXiv preprint arXiv:2111.05443*, (2021).
+Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://doi.org/10.1137/21M1460971>`_, *SIAM Journal on Optimization*, 21:4 (2022), pp. 2552-2579.
 
 Requirements
 ------------
 DFO-LS requires the following software to be installed:
 
-* Python 2.7 or Python 3 (http://www.python.org/)
+* Python 3.9 or higher (http://www.python.org/)
 
 Additionally, the following python packages should be installed (these will be installed automatically if using *pip*, see `Installation using pip`_):
 
-* NumPy 1.11 or higher (http://www.numpy.org/)
-* SciPy 1.11 or higher (http://www.scipy.org/)
-* Pandas 0.17 or higher (http://pandas.pydata.org/)
+* NumPy (http://www.numpy.org/)
+* SciPy version 1.11 or higher (http://www.scipy.org/)
+* Pandas (http://pandas.pydata.org/)
 
 **Optional package:** DFO-LS versions 1.2 and higher also support the `trustregion <https://github.com/lindonroberts/trust-region>`_ package for fast trust-region subproblem solutions. To install this, make sure you have a Fortran compiler (e.g. `gfortran <https://gcc.gnu.org/wiki/GFortran>`_) and NumPy installed, then run :code:`pip install trustregion`. You do not have to have trustregion installed for DFO-LS to work, and it is not installed by default.
 
 Installation using conda
 ------------------------
 DFO-LS can be directly installed in Anaconda environments using `conda-forge <https://anaconda.org/conda-forge/dfo-ls>`_:
 
@@ -143,28 +157,29 @@
 
  .. code-block:: bash
 
     $ pip install --user .
 
 instead.
 
-To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`setup.py`) and rerun the installation using :code:`pip`, as above:
+To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`pyproject.toml`) and rerun the installation using :code:`pip`, as above:
 
  .. code-block:: bash
 
     $ git pull
     $ [sudo] pip install .  # with admin privileges
 
 Testing
 -------
-If you installed DFO-LS manually, you can test your installation by running:
+If you installed DFO-LS manually, you can test your installation using the pytest package:
 
  .. code-block:: bash
 
-    $ python setup.py test
+    $ pip install pytest
+    $ python -m pytest --pyargs dfols
 
 Alternatively, the HTML documentation provides some simple examples of how to run DFO-LS.
 
 Examples
 --------
 Examples of how to run DFO-LS are given in the `documentation <https://numericalalgorithmsgroup.github.io/dfols/>`_, and the `examples <https://github.com/numericalalgorithmsgroup/dfols/tree/master/examples>`_ directory in Github.
 
@@ -176,14 +191,12 @@
 
     $ [sudo] pip uninstall DFO-LS
 
 If DFO-LS was installed manually you have to remove the installed files by hand (located in your python site-packages directory).
 
 Bugs
 ----
-Please report any bugs using GitHub's issue tracker.
+Please report any bugs using `GitHub's issue tracker <https://github.com/numericalalgorithmsgroup/dfols/issues>`_.
 
 License
 -------
 This algorithm is released under the GNU GPL license. Please `contact NAG <http://www.nag.com/content/worldwide-contact-information>`_ for alternative licensing.
-
-
```

### Comparing `DFO-LS-1.4.0/README.rst` & `DFO-LS-1.4.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,27 +36,27 @@
 --------
 If you use DFO-LS in a paper, please cite:
 
 Cartis, C., Fiala, J., Marteau, B. and Roberts, L., `Improving the Flexibility and Robustness of Model-Based Derivative-Free Optimization Solvers <https://doi.org/10.1145/3338517>`_, *ACM Transactions on Mathematical Software*, 45:3 (2019), pp. 32:1-32:41.
 
 If you use DFO-LS for problems with constraints, including bound constraints, please also cite:
 
-Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://arxiv.org/abs/2111.05443>`_, *arXiv preprint arXiv:2111.05443*, (2021).
+Hough, M. and Roberts, L., `Model-Based Derivative-Free Methods for Convex-Constrained Optimization <https://doi.org/10.1137/21M1460971>`_, *SIAM Journal on Optimization*, 21:4 (2022), pp. 2552-2579.
 
 Requirements
 ------------
 DFO-LS requires the following software to be installed:
 
-* Python 2.7 or Python 3 (http://www.python.org/)
+* Python 3.9 or higher (http://www.python.org/)
 
 Additionally, the following python packages should be installed (these will be installed automatically if using *pip*, see `Installation using pip`_):
 
-* NumPy 1.11 or higher (http://www.numpy.org/)
-* SciPy 1.11 or higher (http://www.scipy.org/)
-* Pandas 0.17 or higher (http://pandas.pydata.org/)
+* NumPy (http://www.numpy.org/)
+* SciPy version 1.11 or higher (http://www.scipy.org/)
+* Pandas (http://pandas.pydata.org/)
 
 **Optional package:** DFO-LS versions 1.2 and higher also support the `trustregion <https://github.com/lindonroberts/trust-region>`_ package for fast trust-region subproblem solutions. To install this, make sure you have a Fortran compiler (e.g. `gfortran <https://gcc.gnu.org/wiki/GFortran>`_) and NumPy installed, then run :code:`pip install trustregion`. You do not have to have trustregion installed for DFO-LS to work, and it is not installed by default.
 
 Installation using conda
 ------------------------
 DFO-LS can be directly installed in Anaconda environments using `conda-forge <https://anaconda.org/conda-forge/dfo-ls>`_:
 
@@ -113,28 +113,29 @@
 
  .. code-block:: bash
 
     $ pip install --user .
 
 instead.
 
-To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`setup.py`) and rerun the installation using :code:`pip`, as above:
+To upgrade DFO-LS to the latest version, navigate to the top-level directory (i.e. the one containing :code:`pyproject.toml`) and rerun the installation using :code:`pip`, as above:
 
  .. code-block:: bash
 
     $ git pull
     $ [sudo] pip install .  # with admin privileges
 
 Testing
 -------
-If you installed DFO-LS manually, you can test your installation by running:
+If you installed DFO-LS manually, you can test your installation using the pytest package:
 
  .. code-block:: bash
 
-    $ python setup.py test
+    $ pip install pytest
+    $ python -m pytest --pyargs dfols
 
 Alternatively, the HTML documentation provides some simple examples of how to run DFO-LS.
 
 Examples
 --------
 Examples of how to run DFO-LS are given in the `documentation <https://numericalalgorithmsgroup.github.io/dfols/>`_, and the `examples <https://github.com/numericalalgorithmsgroup/dfols/tree/master/examples>`_ directory in Github.
 
@@ -146,12 +147,12 @@
 
     $ [sudo] pip uninstall DFO-LS
 
 If DFO-LS was installed manually you have to remove the installed files by hand (located in your python site-packages directory).
 
 Bugs
 ----
-Please report any bugs using GitHub's issue tracker.
+Please report any bugs using `GitHub's issue tracker <https://github.com/numericalalgorithmsgroup/dfols/issues>`_.
 
 License
 -------
 This algorithm is released under the GNU GPL license. Please `contact NAG <http://www.nag.com/content/worldwide-contact-information>`_ for alternative licensing.
```

### Comparing `DFO-LS-1.4.0/dfols/__init__.py` & `DFO-LS-1.4.1/dfols/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,14 @@
 
 
 """
 
 # Ensure compatibility with Python 2
 from __future__ import absolute_import, division, print_function, unicode_literals
 
-from .version import __version__
-__all__ = ['__version__']
+# DFO-LS version
+__version__ = '1.4.1'
 
 # Main solver & exit flags
 from .solver import *
-__all__ += ['solve']
+__all__ = ['solve']
```

### Comparing `DFO-LS-1.4.0/dfols/controller.py` & `DFO-LS-1.4.1/dfols/controller.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/diagnostic_info.py` & `DFO-LS-1.4.1/dfols/diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/hessian.py` & `DFO-LS-1.4.1/dfols/hessian.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/model.py` & `DFO-LS-1.4.1/dfols/model.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/params.py` & `DFO-LS-1.4.1/dfols/params.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/solver.py` & `DFO-LS-1.4.1/dfols/solver.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/trust_region.py` & `DFO-LS-1.4.1/dfols/trust_region.py`

 * *Files identical despite different names*

### Comparing `DFO-LS-1.4.0/dfols/util.py` & `DFO-LS-1.4.1/dfols/util.py`

 * *Files identical despite different names*

