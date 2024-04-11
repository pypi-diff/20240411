# Comparing `tmp/srpenergy-1.3.6.tar.gz` & `tmp/srpenergy-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srpenergy-1.3.6.tar", last modified: Wed Feb  9 03:35:08 2022, max compression
+gzip compressed data, was "srpenergy-1.3.7.tar", last modified: Thu Apr 11 17:44:36 2024, max compression
```

## Comparing `srpenergy-1.3.6.tar` & `srpenergy-1.3.7.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 03:35:08.753635 srpenergy-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-02-09 03:34:53.000000 srpenergy-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-02-09 03:35:08.753635 srpenergy-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8689 2022-02-09 03:34:53.000000 srpenergy-1.3.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-02-09 03:35:08.753635 srpenergy-1.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-02-09 03:34:53.000000 srpenergy-1.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 03:35:08.749634 srpenergy-1.3.6/srpenergy/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-09 03:34:53.000000 srpenergy-1.3.6/srpenergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11295 2022-02-09 03:34:53.000000 srpenergy-1.3.6/srpenergy/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 03:35:08.753635 srpenergy-1.3.6/srpenergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-02-09 03:35:08.000000 srpenergy-1.3.6/srpenergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-02-09 03:35:08.000000 srpenergy-1.3.6/srpenergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 03:35:08.000000 srpenergy-1.3.6/srpenergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-09 03:35:08.000000 srpenergy-1.3.6/srpenergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-02-09 03:35:08.000000 srpenergy-1.3.6/srpenergy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:44:36.371352 srpenergy-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 17:44:27.000000 srpenergy-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-11 17:44:36.371352 srpenergy-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-04-11 17:44:27.000000 srpenergy-1.3.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-11 17:44:27.000000 srpenergy-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:44:36.371352 srpenergy-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:44:36.367352 srpenergy-1.3.7/srpenergy/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 17:44:27.000000 srpenergy-1.3.7/srpenergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-11 17:44:27.000000 srpenergy-1.3.7/srpenergy/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:44:36.367352 srpenergy-1.3.7/srpenergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9847 2024-04-11 17:44:36.000000 srpenergy-1.3.7/srpenergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-11 17:44:36.000000 srpenergy-1.3.7/srpenergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:44:36.000000 srpenergy-1.3.7/srpenergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:44:36.000000 srpenergy-1.3.7/srpenergy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 17:44:36.000000 srpenergy-1.3.7/srpenergy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:44:36.371352 srpenergy-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-11 17:44:27.000000 srpenergy-1.3.7/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-11 17:44:27.000000 srpenergy-1.3.7/tests/test_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25112 2024-04-11 17:44:27.000000 srpenergy-1.3.7/tests/test_time_of_use.py
```

### Comparing `srpenergy-1.3.6/LICENSE` & `srpenergy-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `srpenergy-1.3.6/PKG-INFO` & `srpenergy-1.3.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 Metadata-Version: 2.1
 Name: srpenergy
-Version: 1.3.6
+Version: 1.3.7
 Summary: An unofficial Python module for interacting with Srp Energy data.
-Home-page: https://github.com/lamoreauxlab/srpenergy-api-client-python
-Author: Lamoreaux Lab
-Author-email: bklamoreaux@gmail.com
+Author-email: Lamoreaux Lab <info@golamoreaux.com>
 License: MIT
+Project-URL: Homepage, https://github.com/lamoreauxlab/srpenergy-api-client-python
+Project-URL: Source Code, https://github.com/lamoreauxlab/srpenergy-api-client-python.git
 Project-URL: Bug Reports, https://github.com/lamoreauxlab/srpenergy-api-client-python/issues
-Project-URL: Dev Docs, https://srpenergy-api-client-python.readthedocs.io//en/latest/
-Keywords: energy,API,wrapper,srp
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 **********************************
 Srp Energy Developer APIs - Python
 **********************************
-.. image:: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python.svg?branch=master
-    :target: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python
-
-.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=master
-    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=master
+.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=main
+    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=main
+    :alt: Coverage Status
 
 .. image:: https://readthedocs.org/projects/srpenergy-api-client-python/badge/?version=latest
     :target: https://srpenergy-api-client-python.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements.svg?branch=master
-    :target: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements/?branch=master
-    :alt: Requirements Status
-
 .. image:: https://badge.fury.io/py/srpenergy.svg
     :target: https://badge.fury.io/py/srpenergy
     :alt: Latest version on PyPi
 
 .. image:: https://img.shields.io/pypi/pyversions/srpenergy.svg
     :target: https://pypi.org/project/srpenergy/
     :alt: Supported Python versions
@@ -77,15 +66,15 @@
                 "totalCost": 0.08
             }
         ],
         "demandList":[]
     }
 
 .. note::
-    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the fomula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
+    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the formula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
 
     EZ3 customers show 0.0 for ``totalKwh`` and ``totalCost``. Those values are split between ``onPeak``, ``offPeak``, ``shoulder``, and ``superOffPeak``.
 
 Installing
 ==========
 
 It is distributed on PyPI_ and can be installed with pip::
@@ -132,37 +121,64 @@
 
     date, hour, isodate, kwh, cost = usage[0]
 
 
 Development
 ===========
 
-Configure Dev Environment
--------------------------
+You'll need to set up a development environment if you want to develop a new feature or fix issues. The project uses a docker based devcontainer to ensure a consistent development environment.
+- Open the project in VSCode and it will prompt you to open the project in a devcontainer. This will have all the required tools installed and configured.
+
+Setup local dev environment
+---------------------------
+
+If you want to develop outside of a docker devcontainer you can use the following commands to setup your environment.
 
-This section will configure your computer to develop, test, and debug the project.
+* Install Python
+* Configure linting and formatting tools
 
-.. code-block::bash
+.. code-block:: bash
 
-    # Copy Project to local computer
+    # Clone Project to local computer
     cd /path/to/src/
     git clone https://github.com/lamoreauxlab/srpenergy-api-client-python.git
-    cd /path/to/src/srpenergy-api-client-python
+    cd srpenergy-api-client-python
 
-    # Create Python Virtual Environment and activate
-    python -m venv .venv
-    source .venv/bin/activate
+    # Configure the environment variables. Copy example.env to .env and update the values
+    cp example.env .env
 
-    # Install Project
-    python -m pip install -r requirements_test.txt
-    python -m pip install -e .
+    # load .env vars
+    # [ ! -f .env ] || export $(grep -v '^#' .env | xargs)
+    # or this version allows variable substitution and quoted long values
+    # [ -f .env ] && while IFS= read -r line; do [[ $line =~ ^[^#]*= ]] && eval "export $line"; done < .env
+
+    # Linux
+    # virtualenv .venv /usr/local/bin/python3.10
+    python3 -m venv .venv
+    source .venv/bin/activate
 
-    # Create git hook scripts
+    # Windows
+    # virtualenv \path\to\.venv -p path\to\specific_version_python.exe
+    # C:\Users\!Admin\AppData\Local\Programs\Python\Python310\python.exe -m venv .venv
+    # .venv\scripts\activate
+
+    # Update pip
+    python -m pip install --upgrade pip
+
+    # Install dependencies
+    python -m pip install -r requirements_dev.txt
+
+    # Configure linting and formatting tools
+    sudo apt-get update
+    sudo apt-get install -y shellcheck
     pre-commit install
 
+    # Install the package locally
+    pip install --editable .
+
 Style Guidelines
 ----------------
 
 This project enforces quite strict `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_ and `PEP257 (Docstring Conventions) <https://www.python.org/dev/peps/pep-0257/>`_ compliance on all code submitted.
 
 We use `Black <https://github.com/psf/black>`_ for uncompromised code formatting.
 
@@ -207,33 +223,30 @@
 -------
 
 As it states in the `Style Guidelines`_ section all code is checked to verify the following:
 
 - All the unit tests pass
 - All code passes the checks from the linting tools
 
-Install the test dependencies into your Python environment:
-
 .. code-block:: bash
 
-    pip3 install -r requirements_test.txt
-
-Now that you have all test dependencies installed, you can run tests on the project:
+    # Use pre-commit scripts to run all linting
+    pre-commit run --all-files
 
-.. code-block:: bash
+    # Run a specific linter via pre-commit
+    pre-commit run --all-files codespell
 
-    isort .
-    codespell  --skip="./.*,*.csv,*.json,*.pyc,./docs/_build/*,./htmlcov/*"
-    black setup.py srpenergy tests
-    flake8 setup.py srpenergy tests
-    pylint setup.py srpenergy tests
-    pydocstyle setup.py srpenergy tests
+    # Run linters outside of pre-commit
+    codespell .
+    shellcheck -x ./script/*.sh
     rstcheck README.rst
+
+    # Run unit tests
     python -m pytest tests
-    python -m pytest --cov-report term-missing --cov=srpenergy tests
+    python -m pytest --cov-report=xml --cov-report term-missing --cov=srpenergy tests/
 
 Building Docs
 -------------
 
 Build the documentation locally with
 
 .. code-block:: bash
@@ -268,14 +281,15 @@
 Bump Version
 ^^^^^^^^^^^^
 
 Change the version in the following files:
 
 - srpenergy/__init__.py
 - docs/conf.py
+- pyproject.toml
 
 Tag Version
 ^^^^^^^^^^^
 
 Commit, tag, and push the new version
 
 .. code-block:: bash
@@ -295,24 +309,22 @@
 Release to pypi
 ^^^^^^^^^^^^^^^
 
 Upgrade to the latest version of setuptools and create package and test
 
 .. code-block:: bash
 
-    python -m pip install --user --upgrade setuptools wheel # Get latest version
-    python setup.py sdist bdist_wheel
+    python -m pip install --upgrade build twine
+    python -m build
     twine check dist/*
 
 Upload the package to test first
 
 .. code-block:: bash
 
     python -m twine upload --repository testpypi dist/*
 
 Check that package looks ok. After testing, upload to the main repository
 
 .. code-block:: bash
 
     python -m twine upload dist/*
-
-
```

### Comparing `srpenergy-1.3.6/README.rst` & `srpenergy-1.3.7/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 **********************************
 Srp Energy Developer APIs - Python
 **********************************
-.. image:: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python.svg?branch=master
-    :target: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python
-
-.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=master
-    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=master
+.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=main
+    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=main
+    :alt: Coverage Status
 
 .. image:: https://readthedocs.org/projects/srpenergy-api-client-python/badge/?version=latest
     :target: https://srpenergy-api-client-python.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements.svg?branch=master
-    :target: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements/?branch=master
-    :alt: Requirements Status
-
 .. image:: https://badge.fury.io/py/srpenergy.svg
     :target: https://badge.fury.io/py/srpenergy
     :alt: Latest version on PyPi
 
 .. image:: https://img.shields.io/pypi/pyversions/srpenergy.svg
     :target: https://pypi.org/project/srpenergy/
     :alt: Supported Python versions
@@ -52,15 +46,15 @@
                 "totalCost": 0.08
             }
         ],
         "demandList":[]
     }
 
 .. note::
-    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the fomula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
+    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the formula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
 
     EZ3 customers show 0.0 for ``totalKwh`` and ``totalCost``. Those values are split between ``onPeak``, ``offPeak``, ``shoulder``, and ``superOffPeak``.
 
 Installing
 ==========
 
 It is distributed on PyPI_ and can be installed with pip::
@@ -107,37 +101,64 @@
 
     date, hour, isodate, kwh, cost = usage[0]
 
 
 Development
 ===========
 
-Configure Dev Environment
--------------------------
+You'll need to set up a development environment if you want to develop a new feature or fix issues. The project uses a docker based devcontainer to ensure a consistent development environment.
+- Open the project in VSCode and it will prompt you to open the project in a devcontainer. This will have all the required tools installed and configured.
 
-This section will configure your computer to develop, test, and debug the project.
+Setup local dev environment
+---------------------------
 
-.. code-block::bash
+If you want to develop outside of a docker devcontainer you can use the following commands to setup your environment.
 
-    # Copy Project to local computer
+* Install Python
+* Configure linting and formatting tools
+
+.. code-block:: bash
+
+    # Clone Project to local computer
     cd /path/to/src/
     git clone https://github.com/lamoreauxlab/srpenergy-api-client-python.git
-    cd /path/to/src/srpenergy-api-client-python
+    cd srpenergy-api-client-python
 
-    # Create Python Virtual Environment and activate
-    python -m venv .venv
-    source .venv/bin/activate
+    # Configure the environment variables. Copy example.env to .env and update the values
+    cp example.env .env
 
-    # Install Project
-    python -m pip install -r requirements_test.txt
-    python -m pip install -e .
+    # load .env vars
+    # [ ! -f .env ] || export $(grep -v '^#' .env | xargs)
+    # or this version allows variable substitution and quoted long values
+    # [ -f .env ] && while IFS= read -r line; do [[ $line =~ ^[^#]*= ]] && eval "export $line"; done < .env
+
+    # Linux
+    # virtualenv .venv /usr/local/bin/python3.10
+    python3 -m venv .venv
+    source .venv/bin/activate
 
-    # Create git hook scripts
+    # Windows
+    # virtualenv \path\to\.venv -p path\to\specific_version_python.exe
+    # C:\Users\!Admin\AppData\Local\Programs\Python\Python310\python.exe -m venv .venv
+    # .venv\scripts\activate
+
+    # Update pip
+    python -m pip install --upgrade pip
+
+    # Install dependencies
+    python -m pip install -r requirements_dev.txt
+
+    # Configure linting and formatting tools
+    sudo apt-get update
+    sudo apt-get install -y shellcheck
     pre-commit install
 
+    # Install the package locally
+    pip install --editable .
+
 Style Guidelines
 ----------------
 
 This project enforces quite strict `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_ and `PEP257 (Docstring Conventions) <https://www.python.org/dev/peps/pep-0257/>`_ compliance on all code submitted.
 
 We use `Black <https://github.com/psf/black>`_ for uncompromised code formatting.
 
@@ -182,33 +203,30 @@
 -------
 
 As it states in the `Style Guidelines`_ section all code is checked to verify the following:
 
 - All the unit tests pass
 - All code passes the checks from the linting tools
 
-Install the test dependencies into your Python environment:
-
 .. code-block:: bash
 
-    pip3 install -r requirements_test.txt
+    # Use pre-commit scripts to run all linting
+    pre-commit run --all-files
 
-Now that you have all test dependencies installed, you can run tests on the project:
+    # Run a specific linter via pre-commit
+    pre-commit run --all-files codespell
 
-.. code-block:: bash
-
-    isort .
-    codespell  --skip="./.*,*.csv,*.json,*.pyc,./docs/_build/*,./htmlcov/*"
-    black setup.py srpenergy tests
-    flake8 setup.py srpenergy tests
-    pylint setup.py srpenergy tests
-    pydocstyle setup.py srpenergy tests
+    # Run linters outside of pre-commit
+    codespell .
+    shellcheck -x ./script/*.sh
     rstcheck README.rst
+
+    # Run unit tests
     python -m pytest tests
-    python -m pytest --cov-report term-missing --cov=srpenergy tests
+    python -m pytest --cov-report=xml --cov-report term-missing --cov=srpenergy tests/
 
 Building Docs
 -------------
 
 Build the documentation locally with
 
 .. code-block:: bash
@@ -243,14 +261,15 @@
 Bump Version
 ^^^^^^^^^^^^
 
 Change the version in the following files:
 
 - srpenergy/__init__.py
 - docs/conf.py
+- pyproject.toml
 
 Tag Version
 ^^^^^^^^^^^
 
 Commit, tag, and push the new version
 
 .. code-block:: bash
@@ -270,16 +289,16 @@
 Release to pypi
 ^^^^^^^^^^^^^^^
 
 Upgrade to the latest version of setuptools and create package and test
 
 .. code-block:: bash
 
-    python -m pip install --user --upgrade setuptools wheel # Get latest version
-    python setup.py sdist bdist_wheel
+    python -m pip install --upgrade build twine
+    python -m build
     twine check dist/*
 
 Upload the package to test first
 
 .. code-block:: bash
 
     python -m twine upload --repository testpypi dist/*
```

### Comparing `srpenergy-1.3.6/srpenergy/client.py` & `srpenergy-1.3.7/srpenergy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 from dateutil.parser import parse
 import requests
 
 BASE_USAGE_URL = "https://myaccount.srpnet.com/myaccountapi/api/"
 
 
 def get_pretty_date(date_part):
-    r"""Return a formatted date from an iso date."""
+    """Return a formatted date from an iso date."""
     date = parse(date_part)
     return date.strftime("%m/%d/%Y")
 
 
 def get_pretty_time(date_part):
-    r"""Return a formatted time from an iso date."""
+    """Return a formatted time from an iso date."""
     date = parse(date_part)
     return date.strftime("%H:%M %p")
 
 
 def get_rate(str_usage_time):
-    r"""Return the time of use pricing for the given time.
+    """Return the time of use pricing for the given time.
 
     From the SRP website
     peak times:
     Winter      Nov-Apr (5am-9am, 5pm-9pm) 9.51 peak, 6.91 offpeak
     Summer      May-Oct (2pm-8pm) 20.94 peak, 7.27 offpeak
     Summer Peak Jul,Aug (2pm-8pm) 24.09, 7.3
 
@@ -109,15 +109,15 @@
     else:
         rate = non_peak_rate
 
     return rate, is_peak
 
 
 class SrpEnergyClient:
-    r"""SrpEnergyClient(accountid, username, password).
+    """SrpEnergyClient(accountid, username, password).
 
     Client used to fetch srp energy usage.
 
     Parameters
     ----------
     accountid : string
         An srp account id.
@@ -160,15 +160,15 @@
             raise ValueError("Parameter account should only contain numbers.")
 
         self.accountid = accountid
         self.username = username
         self.password = password
 
     def validate(self):
-        r"""Validate user credentials.
+        """Validate user credentials.
 
         Returns
         -------
         bool
 
         Examples
         --------
@@ -200,15 +200,15 @@
 
                 return valid
 
         except Exception:  # pylint: disable=W0703
             return False
 
     def usage(self, startdate, enddate, is_tou=False):  # pylint: disable=R0914
-        r"""Get the energy usage for a given date range.
+        """Get the energy usage for a given date range.
 
         Parameters
         ----------
         startdate : datetime
             the start date
         enddate : datetime
             the end date
```

### Comparing `srpenergy-1.3.6/srpenergy.egg-info/PKG-INFO` & `srpenergy-1.3.7/srpenergy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 Metadata-Version: 2.1
 Name: srpenergy
-Version: 1.3.6
+Version: 1.3.7
 Summary: An unofficial Python module for interacting with Srp Energy data.
-Home-page: https://github.com/lamoreauxlab/srpenergy-api-client-python
-Author: Lamoreaux Lab
-Author-email: bklamoreaux@gmail.com
+Author-email: Lamoreaux Lab <info@golamoreaux.com>
 License: MIT
+Project-URL: Homepage, https://github.com/lamoreauxlab/srpenergy-api-client-python
+Project-URL: Source Code, https://github.com/lamoreauxlab/srpenergy-api-client-python.git
 Project-URL: Bug Reports, https://github.com/lamoreauxlab/srpenergy-api-client-python/issues
-Project-URL: Dev Docs, https://srpenergy-api-client-python.readthedocs.io//en/latest/
-Keywords: energy,API,wrapper,srp
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 **********************************
 Srp Energy Developer APIs - Python
 **********************************
-.. image:: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python.svg?branch=master
-    :target: https://travis-ci.org/lamoreauxlab/srpenergy-api-client-python
-
-.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=master
-    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=master
+.. image:: https://coveralls.io/repos/github/lamoreauxlab/srpenergy-api-client-python/badge.svg?branch=main
+    :target: https://coveralls.io/github/lamoreauxlab/srpenergy-api-client-python?branch=main
+    :alt: Coverage Status
 
 .. image:: https://readthedocs.org/projects/srpenergy-api-client-python/badge/?version=latest
     :target: https://srpenergy-api-client-python.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements.svg?branch=master
-    :target: https://requires.io/github/lamoreauxlab/srpenergy-api-client-python/requirements/?branch=master
-    :alt: Requirements Status
-
 .. image:: https://badge.fury.io/py/srpenergy.svg
     :target: https://badge.fury.io/py/srpenergy
     :alt: Latest version on PyPi
 
 .. image:: https://img.shields.io/pypi/pyversions/srpenergy.svg
     :target: https://pypi.org/project/srpenergy/
     :alt: Supported Python versions
@@ -77,15 +66,15 @@
                 "totalCost": 0.08
             }
         ],
         "demandList":[]
     }
 
 .. note::
-    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the fomula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
+    Time of use customers do not receive a ``totalKwh`` or ``totalCost`` from the api. These values are calculated from ``onPeakKwh``, ``offPeakKwh``, and the formula defined by the SRP `TOU price plan sheet <https://srpnet.com/prices/pdfx/April2015/E-26.pdf>`_
 
     EZ3 customers show 0.0 for ``totalKwh`` and ``totalCost``. Those values are split between ``onPeak``, ``offPeak``, ``shoulder``, and ``superOffPeak``.
 
 Installing
 ==========
 
 It is distributed on PyPI_ and can be installed with pip::
@@ -132,37 +121,64 @@
 
     date, hour, isodate, kwh, cost = usage[0]
 
 
 Development
 ===========
 
-Configure Dev Environment
--------------------------
+You'll need to set up a development environment if you want to develop a new feature or fix issues. The project uses a docker based devcontainer to ensure a consistent development environment.
+- Open the project in VSCode and it will prompt you to open the project in a devcontainer. This will have all the required tools installed and configured.
+
+Setup local dev environment
+---------------------------
+
+If you want to develop outside of a docker devcontainer you can use the following commands to setup your environment.
 
-This section will configure your computer to develop, test, and debug the project.
+* Install Python
+* Configure linting and formatting tools
 
-.. code-block::bash
+.. code-block:: bash
 
-    # Copy Project to local computer
+    # Clone Project to local computer
     cd /path/to/src/
     git clone https://github.com/lamoreauxlab/srpenergy-api-client-python.git
-    cd /path/to/src/srpenergy-api-client-python
+    cd srpenergy-api-client-python
 
-    # Create Python Virtual Environment and activate
-    python -m venv .venv
-    source .venv/bin/activate
+    # Configure the environment variables. Copy example.env to .env and update the values
+    cp example.env .env
 
-    # Install Project
-    python -m pip install -r requirements_test.txt
-    python -m pip install -e .
+    # load .env vars
+    # [ ! -f .env ] || export $(grep -v '^#' .env | xargs)
+    # or this version allows variable substitution and quoted long values
+    # [ -f .env ] && while IFS= read -r line; do [[ $line =~ ^[^#]*= ]] && eval "export $line"; done < .env
+
+    # Linux
+    # virtualenv .venv /usr/local/bin/python3.10
+    python3 -m venv .venv
+    source .venv/bin/activate
 
-    # Create git hook scripts
+    # Windows
+    # virtualenv \path\to\.venv -p path\to\specific_version_python.exe
+    # C:\Users\!Admin\AppData\Local\Programs\Python\Python310\python.exe -m venv .venv
+    # .venv\scripts\activate
+
+    # Update pip
+    python -m pip install --upgrade pip
+
+    # Install dependencies
+    python -m pip install -r requirements_dev.txt
+
+    # Configure linting and formatting tools
+    sudo apt-get update
+    sudo apt-get install -y shellcheck
     pre-commit install
 
+    # Install the package locally
+    pip install --editable .
+
 Style Guidelines
 ----------------
 
 This project enforces quite strict `PEP8 <https://www.python.org/dev/peps/pep-0008/>`_ and `PEP257 (Docstring Conventions) <https://www.python.org/dev/peps/pep-0257/>`_ compliance on all code submitted.
 
 We use `Black <https://github.com/psf/black>`_ for uncompromised code formatting.
 
@@ -207,33 +223,30 @@
 -------
 
 As it states in the `Style Guidelines`_ section all code is checked to verify the following:
 
 - All the unit tests pass
 - All code passes the checks from the linting tools
 
-Install the test dependencies into your Python environment:
-
 .. code-block:: bash
 
-    pip3 install -r requirements_test.txt
-
-Now that you have all test dependencies installed, you can run tests on the project:
+    # Use pre-commit scripts to run all linting
+    pre-commit run --all-files
 
-.. code-block:: bash
+    # Run a specific linter via pre-commit
+    pre-commit run --all-files codespell
 
-    isort .
-    codespell  --skip="./.*,*.csv,*.json,*.pyc,./docs/_build/*,./htmlcov/*"
-    black setup.py srpenergy tests
-    flake8 setup.py srpenergy tests
-    pylint setup.py srpenergy tests
-    pydocstyle setup.py srpenergy tests
+    # Run linters outside of pre-commit
+    codespell .
+    shellcheck -x ./script/*.sh
     rstcheck README.rst
+
+    # Run unit tests
     python -m pytest tests
-    python -m pytest --cov-report term-missing --cov=srpenergy tests
+    python -m pytest --cov-report=xml --cov-report term-missing --cov=srpenergy tests/
 
 Building Docs
 -------------
 
 Build the documentation locally with
 
 .. code-block:: bash
@@ -268,14 +281,15 @@
 Bump Version
 ^^^^^^^^^^^^
 
 Change the version in the following files:
 
 - srpenergy/__init__.py
 - docs/conf.py
+- pyproject.toml
 
 Tag Version
 ^^^^^^^^^^^
 
 Commit, tag, and push the new version
 
 .. code-block:: bash
@@ -295,24 +309,22 @@
 Release to pypi
 ^^^^^^^^^^^^^^^
 
 Upgrade to the latest version of setuptools and create package and test
 
 .. code-block:: bash
 
-    python -m pip install --user --upgrade setuptools wheel # Get latest version
-    python setup.py sdist bdist_wheel
+    python -m pip install --upgrade build twine
+    python -m build
     twine check dist/*
 
 Upload the package to test first
 
 .. code-block:: bash
 
     python -m twine upload --repository testpypi dist/*
 
 Check that package looks ok. After testing, upload to the main repository
 
 .. code-block:: bash
 
     python -m twine upload dist/*
-
-
```

