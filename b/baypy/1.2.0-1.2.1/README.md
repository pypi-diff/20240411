# Comparing `tmp/baypy-1.2.0.tar.gz` & `tmp/baypy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/baypy-1.2.0.tar", last modified: Tue Apr  9 16:31:42 2024, max compression
+gzip compressed data, was "baypy-1.2.1.tar", last modified: Thu Apr 11 13:14:01 2024, max compression
```

## Comparing `baypy-1.2.0.tar` & `baypy-1.2.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-09 16:31:42.000000 baypy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-09 16:31:32.000000 baypy-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18485 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/analysis/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/diagnostics/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/model/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21163 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/regression/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-09 16:31:32.000000 baypy-1.2.0/baypy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-09 16:31:42.000000 baypy-1.2.0/baypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 16:31:41.000000 baypy-1.2.0/baypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 16:31:42.000000 baypy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-09 16:31:32.000000 baypy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.677600 baypy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 13:13:52.000000 baypy-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46879 2024-04-11 13:14:01.677600 baypy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-11 13:13:52.000000 baypy-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18625 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/analysis/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/diagnostics/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/diagnostics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/diagnostics/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-11 13:13:52.000000 baypy-1.2.1/baypy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:14:01.673600 baypy-1.2.1/baypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46879 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 13:14:01.000000 baypy-1.2.1/baypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-11 13:13:52.000000 baypy-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:14:01.677600 baypy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-11 13:13:52.000000 baypy-1.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `baypy-1.2.0/PKG-INFO` & `baypy-1.2.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,101 @@
-Metadata-Version: 2.1
-Name: baypy
-Version: 1.2.0
-Summary: A python package for solving bayesian regression models through a Monte Carlo Markov chain sampling
-Home-page: https://github.com/AndreaBlengino/baypy
-Author: Andrea Blengino
-Author-email: ing.andrea.blengino@gmail.com
-License: GNU GPL3
-Project-URL: Source, https://github.com/AndreaBlengino/baypy
-Project-URL: Tracker, https://github.com/AndreaBlengino/baypy/issues
-Project-URL: Documentation, https://baypy.readthedocs.io/en/latest/index.html
-Description: .. image:: https://github.com/AndreaBlengino/baypy/blob/master/docs/source/_static/logo.png?raw=true
-           :alt: Logo
-        
-        Bayesian Monte Carlo Markov Chain Regression
-        --------------------------------------------
-        
-        **baypy** is a python package for solving bayesian regression models
-        through a Monte Carlo Markov chain sampling.
-        
-        .. list-table::
-           :stub-columns: 1
-           :widths: auto
-           :width: 100%
-        
-           * - PyPI
-             - |pypi_release| |supported_python_versions| |build|
-           * - Tests
-             - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
-           * - Documentation
-             - |docs|
-           * - Code Quality
-             - |codefactor_grade| |codacy_grade| |issues|
-           * - License
-             - |license|
-        
-        .. |pypi_release| image:: https://img.shields.io/pypi/v/baypy?label=release&color=blue
-           :target: https://pypi.org/project/baypy/
-           :alt: PyPI - Library Version
-        
-        .. |supported_python_versions| image:: https://img.shields.io/pypi/pyversions/baypy?logo=python&logoColor=gold
-           :target: https://pypi.org/project/baypy/
-           :alt: PyPI - Supported Python Versions
-        
-        .. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/release.yml.svg?logo=github
-           :target: https://github.com/AndreaBlengino/baypy/actions/workflows/release.yml
-           :alt: Package Build
-        
-        .. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&label=Linux
-           :target: https://github.com/AndreaBlengino/baypy/actions/workflows/linux_test.yml
-           :alt: Linux Tests
-        
-        .. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/macos_test.yml.svg?logo=apple&label=macOS
-           :target: https://github.com/AndreaBlengino/baypy/actions/workflows/macos_test.yml
-           :alt: macOS Tests
-        
-        .. |windows_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/windows_test.yml.svg?logo=windows&label=Windows
-           :target: https://github.com/AndreaBlengino/baypy/actions/workflows/windows_test.yml
-           :alt: Windows Tests
-        
-        .. |test_coverage| image:: https://img.shields.io/codecov/c/github/AndreaBlengino/baypy/master?logo=codecov
-           :target: https://codecov.io/gh/AndreaBlengino/baypy
-           :alt: Test Coverage
-        
-        .. |docs| image:: https://img.shields.io/readthedocs/baypy/latest?logo=read%20the%20docs
-           :target: https://baypy.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Build Status
-        
-        .. |codefactor_grade| image:: https://img.shields.io/codefactor/grade/github/AndreaBlengino/baypy?logo=codefactor&label=CodeFactor
-           :target: https://www.codefactor.io/repository/github/andreablengino/baypy
-           :alt: CodeFactor Grade
-        
-        .. |codacy_grade| image:: https://img.shields.io/codacy/grade/132c2f3d93344ae0934ea808bbf17f05?logo=codacy&label=Codacy
-           :target: https://app.codacy.com/gh/AndreaBlengino/baypy/dashboard
-           :alt: Codacy Grade
-        
-        .. |issues| image:: https://img.shields.io/github/issues/AndreaBlengino/baypy?logo=github
-           :target: https://github.com/AndreaBlengino/baypy/issues
-           :alt: Open Issues
-        
-        .. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
-           :target: https://github.com/AndreaBlengino/baypy/blob/master/LICENSE
-           :alt: License
-        
-        
-        References
-        ----------
-        
-        - `Installation <https://baypy.readthedocs.io/en/latest/installation.html>`_
-        - `PyPI <https://pypi.org/project/baypy>`_
-        - `Documentation <https://baypy.readthedocs.io/en/latest/?badge=latest>`_
-        - `Usage Examples <https://baypy.readthedocs.io/en/latest/examples/index.html>`_
-        - `Issue tracker <https://github.com/AndreaBlengino/baypy/issues>`_
-        - `Source code <https://github.com/AndreaBlengino/baypy/tree/master/baypy>`_
-        - `GNU General Public License v3.0 <https://github.com/AndreaBlengino/baypy/blob/master/LICENSE>`_
-        
-        
-        Contributing
-        ------------
-        
-        The baypy project welcomes your expertise and enthusiasm!  
-        All contributions, bug reports, bug fixes, documentation improvements, 
-        enhancements and ideas are welcome.  
-        Writing code isn't the only way to contribute to baypy. You can also:
-        
-        - develop tutorials, presentations and other educational materials
-        - maintain and improve the `documentation <https://baypy.readthedocs.io/en/latest/?badge=latest>`_,
-        - help with outreach and onboard new contributors
-        
-        Have a look at the `contributing guide <https://github.com/AndreaBlengino/baypy/blob/master/.github/CONTRIBUTING.md>`_.
-        If you are new to contributing to open source, `this guide <https://opensource.guide/how-to-contribute/>`_ helps explain
-        why, what, and how to successfully get involved.
-Platform: UNKNOWN
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Manufacturing
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.9, <3.13
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: tests
+.. image:: https://github.com/AndreaBlengino/baypy/blob/master/docs/source/_static/logo.png?raw=true
+   :alt: Logo
+
+Bayesian Monte Carlo Markov Chain Regression
+--------------------------------------------
+
+**baypy** is a python package for solving bayesian regression models
+through a Monte Carlo Markov chain sampling.
+
+.. list-table::
+   :stub-columns: 1
+   :widths: auto
+   :width: 100%
+
+   * - PyPI
+     - |pypi_release| |supported_python_versions| |build|
+   * - Tests
+     - |linux_tests| |macos_tests| |windows_tests| |test_coverage|
+   * - Documentation
+     - |docs|
+   * - Code Quality
+     - |codefactor_grade| |codacy_grade| |issues|
+   * - License
+     - |license|
+
+.. |pypi_release| image:: https://img.shields.io/pypi/v/baypy?label=release&color=blue
+   :target: https://pypi.org/project/baypy/
+   :alt: PyPI - Library Version
+
+.. |supported_python_versions| image:: https://img.shields.io/pypi/pyversions/baypy?logo=python&logoColor=gold
+   :target: https://pypi.org/project/baypy/
+   :alt: PyPI - Supported Python Versions
+
+.. |build| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/release.yml.svg?logo=github
+   :target: https://github.com/AndreaBlengino/baypy/actions/workflows/release.yml
+   :alt: Package Build
+
+.. |linux_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/linux_test.yml.svg?logo=linux&label=Linux
+   :target: https://github.com/AndreaBlengino/baypy/actions/workflows/linux_test.yml
+   :alt: Linux Tests
+
+.. |macos_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/macos_test.yml.svg?logo=apple&label=macOS
+   :target: https://github.com/AndreaBlengino/baypy/actions/workflows/macos_test.yml
+   :alt: macOS Tests
+
+.. |windows_tests| image:: https://img.shields.io/github/actions/workflow/status/AndreaBlengino/baypy/windows_test.yml.svg?logo=windows&label=Windows
+   :target: https://github.com/AndreaBlengino/baypy/actions/workflows/windows_test.yml
+   :alt: Windows Tests
+
+.. |test_coverage| image:: https://img.shields.io/codecov/c/github/AndreaBlengino/baypy/master?logo=codecov
+   :target: https://codecov.io/gh/AndreaBlengino/baypy
+   :alt: Test Coverage
+
+.. |docs| image:: https://img.shields.io/readthedocs/baypy/latest?logo=read%20the%20docs
+   :target: https://baypy.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Build Status
+
+.. |codefactor_grade| image:: https://img.shields.io/codefactor/grade/github/AndreaBlengino/baypy?logo=codefactor&label=CodeFactor
+   :target: https://www.codefactor.io/repository/github/andreablengino/baypy
+   :alt: CodeFactor Grade
+
+.. |codacy_grade| image:: https://img.shields.io/codacy/grade/132c2f3d93344ae0934ea808bbf17f05?logo=codacy&label=Codacy
+   :target: https://app.codacy.com/gh/AndreaBlengino/baypy/dashboard
+   :alt: Codacy Grade
+
+.. |issues| image:: https://img.shields.io/github/issues/AndreaBlengino/baypy?logo=github
+   :target: https://github.com/AndreaBlengino/baypy/issues
+   :alt: Open Issues
+
+.. |license| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
+   :target: https://github.com/AndreaBlengino/baypy/blob/master/LICENSE
+   :alt: License
+
+
+References
+----------
+
+- `Installation <https://baypy.readthedocs.io/en/latest/installation.html>`_
+- `PyPI <https://pypi.org/project/baypy>`_
+- `Documentation <https://baypy.readthedocs.io/en/latest/?badge=latest>`_
+- `Usage Examples <https://baypy.readthedocs.io/en/latest/examples/index.html>`_
+- `Issue tracker <https://github.com/AndreaBlengino/baypy/issues>`_
+- `Source code <https://github.com/AndreaBlengino/baypy/tree/master/baypy>`_
+- `GNU General Public License v3.0 <https://github.com/AndreaBlengino/baypy/blob/master/LICENSE>`_
+
+
+Contributing
+------------
+
+The baypy project welcomes your expertise and enthusiasm!  
+All contributions, bug reports, bug fixes, documentation improvements, 
+enhancements and ideas are welcome.  
+Writing code isn't the only way to contribute to baypy. You can also:
+
+- develop tutorials, presentations and other educational materials
+- maintain and improve the `documentation <https://baypy.readthedocs.io/en/latest/?badge=latest>`_,
+- help with outreach and onboard new contributors
+
+Have a look at the `contributing guide <https://github.com/AndreaBlengino/baypy/blob/master/.github/CONTRIBUTING.md>`_.
+If you are new to contributing to open source, `this guide <https://opensource.guide/how-to-contribute/>`_ helps explain
+why, what, and how to successfully get involved.
```

### Comparing `baypy-1.2.0/baypy/analysis/functions.py` & `baypy-1.2.1/baypy/analysis/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
 import matplotlib.pyplot as plt
 from ..model import Model
 import numpy as np
 import pandas as pd
 from scipy.stats import gaussian_kde
 from ..utils import flatten_matrix
 
 
-def trace_plot(posteriors: dict) -> None:
+def trace_plot(posteriors: dict[str, np.ndarray]) -> None:
     """it plots the traces and the probability density for each posterior. \n
     The plot shows the traces for each Markov chain, for each regression variable and the relative posterior density.
     The plot layout has number of rows equal to the number of regression variables and two columns: traces on the left
     and densities on the right.
 
     Parameters
     ----------
@@ -80,15 +81,18 @@
 def _compute_kde(posterior: np.ndarray) -> tuple[np.ndarray, np.ndarray]:
     posterior_support = np.linspace(np.min(posterior), np.max(posterior), 1000)
     posterior_kde = gaussian_kde(posterior)(posterior_support)
 
     return posterior_support, posterior_kde
 
 
-def summary(posteriors: dict, alpha: float = 0.05, quantiles: list = None, print_summary: bool = True) -> dict:
+def summary(posteriors: dict[str, np.ndarray],
+            alpha: float = 0.05,
+            quantiles: list[float] = None,
+            print_summary: bool = True) -> dict[str, int | str]:
     """It prints a statistical summary for each posterior.
 
     Parameters
     ----------
     ``posteriors`` : :py:class:`dict`
         Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
         :py:class:`numpy.ndarray` with a number of rows equal to the number of iterations and a number of columns equal
@@ -289,15 +293,15 @@
     ax.tick_params(bottom = False, top = False, left = False, right = False)
 
     plt.tight_layout()
 
     plt.show()
 
 
-def compute_DIC(model: Model, print_summary: bool = True) -> dict:
+def compute_DIC(model: Model, print_summary: bool = True) -> dict[str, float]:
     r"""It computes and prints the Deviance Information Criterion (DIC) for the fitted model.
 
     Parameters
     ----------
     ``model`` : :py:class:`Model <baypy.model.model.Model>`
         The model with data, regressors, response variable and priors to be solved through Monte Carlo sampling.
     ``print_summary`` : :py:class:`bool`, optional
```

### Comparing `baypy-1.2.0/baypy/diagnostics/functions.py` & `baypy-1.2.1/baypy/diagnostics/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from ..utils import flatten_matrix
 
 
-def autocorrelation_plot(posteriors: dict, max_lags: int = 30) -> None:
+def autocorrelation_plot(posteriors: dict[str, np.ndarray], max_lags: int = 30) -> None:
     """It plots the auto-correlation for each Markov chain for each regression variable. \n
     The plot shows the auto-correlation trend from lag ``0`` (when auto-correlation is always ``1``) up to ``max_lags``.
     The plot layout has number of rows equal to the number of regression variables and a number of columns equal to the
     number of chains.
 
     Parameters
     ----------
@@ -101,15 +101,16 @@
 
         plt.tight_layout()
         plt.subplots_adjust(left = 0.14)
 
     plt.show()
 
 
-def autocorrelation_summary(posteriors: dict, lags: list = None, print_summary: bool = True) -> pd.DataFrame:
+def autocorrelation_summary(posteriors: dict[str, np.ndarray], lags: list[int] = None, print_summary: bool = True) \
+        -> pd.DataFrame:
     """It prints the auto-correlation summary for each regression variable. \n
     The summary reports the auto-correlation values at the lags listed in ``lags``.
 
     Parameters
     ----------
     ``posteriors`` : :py:class:`dict`
         Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
@@ -198,15 +199,15 @@
 
     if print_summary:
         print(acorr_summary.to_string())
 
     return acorr_summary
 
 
-def effective_sample_size(posteriors: dict, print_summary: bool = True) -> pd.DataFrame:
+def effective_sample_size(posteriors: dict[str, np.ndarray], print_summary: bool = True) -> pd.DataFrame:
     """It computes and prints the effective number of sample for each posterior.
 
     Parameters
     ----------
     ``posteriors`` : :py:class:`dict`
         Posterior samples. Posteriors and relative samples are key-value pairs. Each sample is a
         :py:class:`numpy.ndarray` with a number of rows equals to the number of iterations and a number of columns equal
```

### Comparing `baypy-1.2.0/baypy/model/linear_model.py` & `baypy-1.2.1/baypy/model/linear_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from .model import Model
 import pandas as pd
 import numpy as np
 from scipy.stats import norm
 from ..utils import flatten_matrix, matrices_to_frame, dot_product
 
 
@@ -100,15 +101,15 @@
     @response_variable.setter
     def response_variable(self, response_variable: str) -> None:
         super(LinearModel, type(self)).response_variable.fset(self, response_variable)
         self.__response_variable = response_variable
 
 
     @property
-    def priors(self) -> dict:
+    def priors(self) -> dict[str, dict[str, float | int]]:
         r"""Priors for the regressors' and variance parameters.
         Each prior is a key-value pair, where the value is a :py:class:`dict` with:
 
         - hyperparameter names as keys
         - hyperparameter values as values.
 
         Returns
@@ -181,15 +182,15 @@
            ...                 'x_3': {'mean': 0, 'variance': 1e6},
            ...                 'variance': {'shape': 1, 'scale': 1e-6}}
         """
         return self.__priors
 
 
     @priors.setter
-    def priors(self, priors: dict) -> None:
+    def priors(self, priors: dict[str, dict[str, float | int]]) -> None:
         super(LinearModel, type(self)).priors.fset(self, priors)
 
         if 'variance' not in priors.keys():
             raise KeyError("Parameter 'priors' must contain a 'variance' key")
 
         for prior, values in priors.items():
             if not isinstance(values, dict):
@@ -212,28 +213,28 @@
 
         self.__priors = priors
         self.__variable_names = list(priors.keys())
         self.__variable_names.insert(0, self.__variable_names.pop(self.__variable_names.index('intercept')))
 
 
     @property
-    def variable_names(self) -> list:
+    def variable_names(self) -> list[str]:
         r"""Variables of the linear model.
 
         Returns
         -------
         :py:class:`list`
             The list of all model variables: the regressors :math:`X`, including the ``'intercept'`` and the
             ``'variance'`` :math:`\sigma^2`.
         """
         return self.__variable_names
 
 
     @property
-    def posteriors(self) -> dict:
+    def posteriors(self) -> dict[str, np.ndarray]:
         r"""Posteriors of the regressors' and variance parameters.
         Posteriors and relative samples are key-value pairs. Each sample is a :py:class:`numpy.ndarray`
         with a number of rows equals to the number of iterations and a number of columns equal to the number of Markov
         chains.
 
         Returns
         -------
@@ -253,15 +254,15 @@
            ``ValueError``
                If a posterior sample is an empty :py:class:`numpy.ndarray`.
         """
         return self.__posteriors
 
 
     @posteriors.setter
-    def posteriors(self, posteriors: dict) -> None:
+    def posteriors(self, posteriors: dict[str, np.ndarray]) -> None:
         super(LinearModel, type(self)).posteriors.fset(self, posteriors)
 
         if 'variance' not in posteriors.keys():
             raise KeyError("Parameter 'posteriors' must contain a 'variance' key")
 
         self.__posteriors = posteriors
 
@@ -287,15 +288,15 @@
         if self.__posteriors is None:
             raise ValueError("Posteriors not available, run 'baypy.regression.LinearRegression.sample' to generate "
                              "posteriors")
         return matrices_to_frame(matrices_dict = self.__posteriors)
 
 
     def residuals(self) -> pd.DataFrame:
-        r"""It compute the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
+        r"""It computes the residuals :math:`\epsilon` with respect to predicted values :math:`\hat{y}`.
 
         Returns
         -------
         :py:class:`pandas.DataFrame`
             Returns a copy of :py:attr:`data` with 3 more columns: ``'intercept'``, ``'predicted'`` and ``'residuals'``.
 
         .. admonition:: Raises
@@ -338,15 +339,15 @@
         data['intercept'] = 1
         data['predicted'] = dot_product(data = data, regressors = posterior_means)
         data['residuals'] = data[self.__response_variable] - data['predicted']
 
         return data
 
 
-    def predict_distribution(self, predictors: dict) -> np.ndarray:
+    def predict_distribution(self, predictors: dict[str, float | int]) -> np.ndarray:
         """It predicts a posterior distribution for an unobserved values. For each posterior sample, it draws a sample
         from the likelihood.
 
         Parameters
         ----------
         ``predictors`` : :py:class:`dict`
             Values of predictors :math:`X` at which compute the posterior distribution. Each predictor has to be set as
@@ -492,15 +493,15 @@
         data['intercept'] = 1
         data['mean'] = dot_product(data = data, regressors = posterior_means)
         data['variance'] = flatten_matrix(self.__posteriors['variance']).mean()
 
         return data
 
 
-    def _compute_model_parameters_at_observation(self, i: int):
+    def _compute_model_parameters_at_observation(self, i: int) -> pd.DataFrame:
 
         posterior_means = {posterior: posterior_samples[i, :].mean()
                            for posterior, posterior_samples in self.__posteriors.items() if posterior != 'variance'}
 
         data = self.__data.copy()
         data['intercept'] = 1
         data['mean'] = dot_product(data = data, regressors = posterior_means)
```

### Comparing `baypy-1.2.0/baypy/model/model.py` & `baypy-1.2.1/baypy/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from abc import ABC, abstractmethod
 import numpy as np
 import pandas as pd
 
 
 class Model(ABC):
     """:py:class:`Model <baypy.model.model.Model>` object. \n
@@ -43,15 +44,15 @@
     @property
     @abstractmethod
     def priors(self) -> None: ...
 
 
     @priors.setter
     @abstractmethod
-    def priors(self, priors: dict) -> None:
+    def priors(self, priors: dict[str, dict[str, float | int]]) -> None:
         if not isinstance(priors, dict):
             raise TypeError("Parameter 'priors' must be a dictionary")
 
         if len(priors) == 0:
             raise ValueError("Parameter 'priors' cannot be an empty dictionary")
 
         if 'intercept' not in priors.keys():
@@ -66,15 +67,15 @@
     @property
     @abstractmethod
     def posteriors(self) -> None: ...
 
 
     @posteriors.setter
     @abstractmethod
-    def posteriors(self, posteriors: dict) -> None:
+    def posteriors(self, posteriors: dict[str, np.ndarray]) -> None:
         if not isinstance(posteriors, dict):
             raise TypeError("Parameter 'posteriors' must be a dictionary")
 
         if not all([isinstance(posterior_sample, np.ndarray) for posterior_sample in posteriors.values()]):
             raise TypeError("All posteriors data must be an instance of 'numpy.ndarray'")
 
         if 'intercept' not in posteriors.keys():
@@ -90,15 +91,15 @@
 
 
     @abstractmethod
     def residuals(self) -> None: ...
 
 
     @abstractmethod
-    def predict_distribution(self, predictors: dict) -> None:
+    def predict_distribution(self, predictors: dict[str, float | int]) -> None:
         if not isinstance(predictors, dict):
             raise TypeError("Parameter 'predictors' must be a dictionary")
 
         if len(predictors) == 0:
             raise ValueError("Parameter 'predictors' cannot be an empty dictionary")
```

### Comparing `baypy-1.2.0/baypy/regression/functions.py` & `baypy-1.2.1/baypy/regression/functions.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.0/baypy/regression/linear_regression.py` & `baypy-1.2.1/baypy/regression/linear_regression.py`

 * *Files identical despite different names*

### Comparing `baypy-1.2.0/baypy/regression/regression.py` & `baypy-1.2.1/baypy/regression/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         if model.response_variable not in model.data.columns:
             raise ValueError(f"Column '{model.response_variable}' not found in 'data'")
 
         if model.priors is None:
             raise ValueError("Missing 'priors' in 'model'")
 
         for prior in model.priors.keys():
-            if (prior not in  ['intercept', 'variance']) and (prior not in model.data.columns):
+            if (prior not in ['intercept', 'variance']) and (prior not in model.data.columns):
                 raise ValueError(f"Column '{prior}' not found in 'model.data'")
 
         if not isinstance(n_iterations, int):
             raise TypeError("Parameter 'n_iteration' must be an integer")
 
         if not isinstance(burn_in_iterations, int):
             raise TypeError("Parameter 'burn_in_iterations' must be an integer")
```

### Comparing `baypy-1.2.0/baypy/utils.py` & `baypy-1.2.1/baypy/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import numpy as np
 import pandas as pd
 
 
 def flatten_matrix(matrix: np.ndarray) -> np.ndarray:
     """Flattens a matrix of dimensions ``(M, N)`` to ``(M*N, )``.
 
@@ -40,15 +41,15 @@
 
     if matrix.size == 0:
         raise ValueError("Parameter 'matrix' is empty")
 
     return np.asarray(matrix).reshape(-1)
 
 
-def matrices_to_frame(matrices_dict: dict) -> pd.DataFrame:
+def matrices_to_frame(matrices_dict: dict[str, np.ndarray]) -> pd.DataFrame:
     """Organizes a dictionary of matrices in a ``pandas.DataFrame``. Each matrix becomes a frame column, with column
     name equal to the matrix' relative key in the dictionary. If the matrix has dimensions ``(M, N``), then the relative
     frame column has length ``M*N``.
 
     Parameters
     ----------
     matrices_dict : dict
@@ -95,15 +96,15 @@
 
         if matrix.size == 0:
             raise ValueError(f"Matrix '{matrix_name}' is empty")
 
     return pd.DataFrame({col: flatten_matrix(matrix) for col, matrix in matrices_dict.items()})
 
 
-def dot_product(data: pd.DataFrame, regressors: dict) -> np.ndarray:
+def dot_product(data: pd.DataFrame, regressors: dict[str, float | int]) -> np.ndarray:
     """Computes the dot product between columns of ``data`` and values of ``regressors``.
 
     Parameters
     ----------
     data : pandas.DataFrame
         The dataframe to be used for the dot product. It cannot be empty. It must contain all ``regressors`` keys.
```

### Comparing `baypy-1.2.0/baypy.egg-info/SOURCES.txt` & `baypy-1.2.1/baypy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.rst
+pyproject.toml
 setup.py
 baypy/__init__.py
 baypy/utils.py
 baypy.egg-info/PKG-INFO
 baypy.egg-info/SOURCES.txt
 baypy.egg-info/dependency_links.txt
 baypy.egg-info/requires.txt
```

