# Comparing `tmp/devo-sdk-5.1.9.tar.gz` & `tmp/devo-sdk-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devo-sdk-5.1.9.tar", last modified: Wed Feb  7 07:49:00 2024, max compression
+gzip compressed data, was "devo-sdk-5.2.0.tar", last modified: Thu Apr 11 10:11:43 2024, max compression
```

## Comparing `devo-sdk-5.1.9.tar` & `devo-sdk-5.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.029696 devo-sdk-5.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-02-07 07:49:00.029696 devo-sdk-5.1.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     7850 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.021696 devo-sdk-5.1.9/devo/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/api/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35745 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/api/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/api/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/api/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/api/scripts/client_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/common/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/common/dates/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/dates/dateoperations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/dates/dateparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/dates/dateutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/common/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/generic/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/common/loadenv/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/loadenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/loadenv/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/common/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/common/logging/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/sender/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37794 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15061 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/pfx_to_pem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.025696 devo-sdk-5.1.9/devo/sender/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/scripts/sender_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/devo/sender/transformsyslog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 07:49:00.029696 devo-sdk-5.1.9/devo_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-07 07:49:00.000000 devo-sdk-5.1.9/devo_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-07 07:49:00.029696 devo-sdk-5.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-07 07:48:49.000000 devo-sdk-5.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.828169 devo-sdk-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-11 10:11:43.828169 devo-sdk-5.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5999 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.820169 devo-sdk-5.2.0/devo/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.820169 devo-sdk-5.2.0/devo/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35907 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/api/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/api/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/api/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/api/scripts/client_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/common/dates/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/dates/dateoperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/dates/dateparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/dates/dateutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/common/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/generic/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/common/loadenv/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/loadenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/loadenv/load_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/common/logging/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37794 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/pfx_to_pem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.824169 devo-sdk-5.2.0/devo/sender/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/scripts/sender_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/devo/sender/transformsyslog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:11:43.828169 devo-sdk-5.2.0/devo_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-11 10:11:43.000000 devo-sdk-5.2.0/devo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 10:11:43.828169 devo-sdk-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-11 10:11:36.000000 devo-sdk-5.2.0/setup.py
```

### Comparing `devo-sdk-5.1.9/LICENSE` & `devo-sdk-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/PKG-INFO` & `devo-sdk-5.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devo-sdk
-Version: 5.1.9
+Version: 5.2.0
 Summary: Devo Software Development Kit for Python.
 Home-page: https://github.com/DevoInc/python-sdk
 Author: Devo, Inc.
 Author-email: support@devo.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,23 +21,25 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests~=2.31
 Requires-Dist: click==8.1.7
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: pem~=21.2.0
-Requires-Dist: pyopenssl~=23.3
-Requires-Dist: pytz~=2023.3
-Requires-Dist: certifi~=2023.11.17
-Requires-Dist: cryptography~=41.0.7
+Requires-Dist: pyopenssl~=24.1.0
+Requires-Dist: pytz~=2024.1
+Requires-Dist: certifi~=2024.2.2
+Requires-Dist: cryptography~=42.0.5
 Provides-Extra: dev
 Requires-Dist: stopit==1.1.2; extra == "dev"
-Requires-Dist: msgpack~=1.0.7; extra == "dev"
-Requires-Dist: responses~=0.24; extra == "dev"
-Requires-Dist: pipdeptree~=2.13.1; extra == "dev"
+Requires-Dist: msgpack~=1.0.8; extra == "dev"
+Requires-Dist: responses~=0.25.0; extra == "dev"
+Requires-Dist: pipdeptree~=2.17.0; extra == "dev"
+Requires-Dist: pytest~=8.1.1; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
 
 ![License](https://img.shields.io/github/license/DevoInc/python-sdk)
 ![Wheel](https://img.shields.io/pypi/wheel/devo-sdk)
 ![Version](https://img.shields.io/pypi/v/devo-sdk)
 ![Python](https://img.shields.io/pypi/pyversions/devo-sdk)
 ![Tests](https://github.com/DevoInc/python-sdk/actions/workflows/python-pull-request.yml/badge.svg)
 
@@ -60,31 +62,31 @@
 ## Quick Start
 
 ### Installing the SDK
 
 You can install the Devo SDK by using `easy_install` or `pip`:
 
 ```console
-#option 1
+# option 1
 easy_install devo-sdk
 
-#option 2
+# option 2
 pip install devo-sdk
 ```
 
 You can use sources files, cloning the project too:
 
 ```console
-#option 3
+# option 3
 python setup.py install
 
-#option 4
+# option 4
 pip install .
 
-#option 5 - dev option
+# option 5 - dev option
 pip install -e .
 ```
 
 ### Documentation
 
 There is specific documentation in the _[docs](https://github.com/DevoInc/python-sdk/tree/master/docs)_ folder for each part of SDK:
 
@@ -146,96 +148,60 @@
 ### API authorization
 
 You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every
 Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab.
 
 ## Launch tests
 
-### run_tests script
+### Pytest
 
-You can run tests from the main folder of SDK
-To launch this script, you need either the environment variables loaded in the system, or the _environment.env_ file in the root of the SDK with the correct values, since to test all the SDK functionalities it is necessary to connect to Devo for the tests of sending and extracting data. There is an example file called _environment.env.example_
+The SDK uses Pytest for testing. This is a powerful tool for testing Python code. Pytest is a much more flexible and powerful tool than the built-in unittest module. It allows more testing functionality through the use of plugins. You can find more information in the [Pytest documentation](https://docs.pytest.org/en/stable/).
 
-Its normal, by the way, TCP tests fails in clients or not Devo developers systems.
+Install the testing requirements:
 
 ```console
-~/projects/devo-python-sdk > python setup.py test
+pip install -r requirements-test.txt
 ```
 
+You can run tests from the `tests` folder of SDK
+
 ```console
-~/projects/devo-python-sdk > python run_tests.py
+pytest
 ```
 
-You can add option "Coverage" for create HTML report about tests.
+Its normal that TCP tests fails in clients or not Devo developers systems.
+
+You can add the option `--cov` to create a coverage report.
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py --coverage
+pytest --cov
 ```
 
-You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
+Check the [pytest-cov documentation](https://pytest-cov.readthedocs.io/) for more details.
 
-```console
-~/projects/devo-python-sdk > python run_tests.py -m SENDER_CLI
-```
+The tests are divided into unit and integration tests. The integration tests require either a connection to Devo or to a local server that is launched when testing, so you need to have the environment variables in your system for all the tests that require connection to Devo can work.
 
-You can also exclude one or several tests with `-M` parameter:
+To run the unit tests only, you can use the `unit` folder:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -M SENDER_CLI,API_CLI
+pytest unit
 ```
 
-Using the --help flag prints the available modules to use:
+To run the integration tests only, you can use the `integration` folder:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py --help
-usage: run_tests.py [-h] [--coverage [COVERAGE]] [-m [MODULE]]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --coverage [COVERAGE]
-                        Generate coverage
-  -m [MODULES], --modules [MODULES]
-                        Run tests for selected modules: API_CLI, API_QUERY, API_TASKS, API_ERRORS, API_PARSER_DATE,
-                        API_PROCESSORS, API_KEEPALIVE, COMMON_CONFIGURATION, COMMON_DATE_PARSER, SENDER_CLI, SENDER_CSV,
-                        SENDER_NUMBER_LOOKUP, SENDER_SEND_DATA, SENDER_SEND_LOOKUP
-  -M [EXCLUDE_MODULES], --exclude-modules [EXCLUDE_MODULES]
-                        Exclude tests for modules: API_CLI, API_QUERY, API_TASKS, API_ERRORS, API_PARSER_DATE,
-                        API_PROCESSORS, API_KEEPALIVE, COMMON_CONFIGURATION, COMMON_DATE_PARSER, SENDER_CLI, SENDER_CSV,
-                        SENDER_NUMBER_LOOKUP, SENDER_SEND_DATA, SENDER_SEND_LOOKUP
+pytest integration
 ```
 
-- API_CLI: API Command-line interface tests.
-- API_QUERY: Query API tests.
-- API_TASKS: Task API tests.
-- API_ERRORS: Managing of API Errors tests.
-- API_PARSER_DATE: Parsing of dates in API tests.
-- API_PROCESSORS: Response processors in API tests.
-- API_KEEPALIVE: Keep Alive functionality in API tests.
-- COMMON_CONFIGURATION: Configuration tests.
-- COMMON_DATE_PARSER: Date parser tests.
-- SENDER_CLI: Lookup command-line interface tests.
-- SENDER_CSV: Lookup uploading through CSV tests.
-- SENDER_NUMBER_LOOKUP: Numbers in lookup tests
-- SENDER_SEND_DATA: Data sending tests.
-- SENDER_SEND_LOOKUP: Lookup sending tests.
-
-### Run using Unittest command
-
-You can see references in [unittest documentation](https://docs.python.org/3/library/unittest.html)
-
-For commands like:
+You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
 
 ```console
-python -m unittest discover -p "*.py"
+pytest unit/test_sender_encoding.py
 ```
 
-If you launch this command from the root directory of the SDK, you need to have the environment variables in your
-system for all the tests that require connection to Devo can work, not being able to use the environment.env file
-as in the script.
-
 ### Contact Us
 
 You can contact with us at _support@devo.com_.
 
 ## License
 
 MIT License
```

### Comparing `devo-sdk-5.1.9/README.md` & `devo-sdk-5.2.0/devo_sdk.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,46 @@
+Metadata-Version: 2.1
+Name: devo-sdk
+Version: 5.2.0
+Summary: Devo Software Development Kit for Python.
+Home-page: https://github.com/DevoInc/python-sdk
+Author: Devo, Inc.
+Author-email: support@devo.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests~=2.31
+Requires-Dist: click==8.1.7
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: pem~=21.2.0
+Requires-Dist: pyopenssl~=24.1.0
+Requires-Dist: pytz~=2024.1
+Requires-Dist: certifi~=2024.2.2
+Requires-Dist: cryptography~=42.0.5
+Provides-Extra: dev
+Requires-Dist: stopit==1.1.2; extra == "dev"
+Requires-Dist: msgpack~=1.0.8; extra == "dev"
+Requires-Dist: responses~=0.25.0; extra == "dev"
+Requires-Dist: pipdeptree~=2.17.0; extra == "dev"
+Requires-Dist: pytest~=8.1.1; extra == "dev"
+Requires-Dist: pytest-cov~=5.0.0; extra == "dev"
+
 ![License](https://img.shields.io/github/license/DevoInc/python-sdk)
 ![Wheel](https://img.shields.io/pypi/wheel/devo-sdk)
 ![Version](https://img.shields.io/pypi/v/devo-sdk)
 ![Python](https://img.shields.io/pypi/pyversions/devo-sdk)
 ![Tests](https://github.com/DevoInc/python-sdk/actions/workflows/python-pull-request.yml/badge.svg)
 
 # Devo Python SDK
@@ -23,52 +62,52 @@
 ## Quick Start
 
 ### Installing the SDK
 
 You can install the Devo SDK by using `easy_install` or `pip`:
 
 ```console
-#option 1
+# option 1
 easy_install devo-sdk
 
-#option 2
+# option 2
 pip install devo-sdk
 ```
 
 You can use sources files, cloning the project too:
 
 ```console
-#option 3
+# option 3
 python setup.py install
 
-#option 4
+# option 4
 pip install .
 
-#option 5 - dev option
+# option 5 - dev option
 pip install -e .
 ```
 
 ### Documentation
 
-There is specific documentation in the _[docs](docs)_ folder for each part of SDK:
+There is specific documentation in the _[docs](https://github.com/DevoInc/python-sdk/tree/master/docs)_ folder for each part of SDK:
 
-- [Sender](docs/sender/sender.md)
-  - [Data](docs/sender/data.md)
-  - [Lookups](docs/sender/lookup.md)
-- [Common](docs/common.md)
+- [Sender](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/sender.md)
+  - [Data](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/data.md)
+  - [Lookups](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/lookup.md)
+- [Common](https://github.com/DevoInc/python-sdk/tree/master/docs/common.md)
 - API:
-  - [Api query](docs/api/api.md)
-  - [Api tasks management](docs/api/task.md)
-    - [Destination: email](docs/api/destination_email.md)
-    - [Destination: redis](docs/api/destination_redis.md)
-    - [Destination: S3](docs/api/destination_s3.md)
+  - [Api query](https://github.com/DevoInc/python-sdk/tree/master/docs/api/api.md)
+  - [Api tasks management](https://github.com/DevoInc/python-sdk/tree/master/docs/api/task.md)
+    - [Destination: email](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_email.md)
+    - [Destination: redis](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_redis.md)
+    - [Destination: S3](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_s3.md)
 
 ## Contributing
 
-See [PyLibs contributing guide](CONTRIBUTING.md).<br/>
+See [PyLibs contributing guide](https://github.com/DevoInc/python-sdk/tree/master/CONTRIBUTING.md).<br/>
 Pull and merge requests are welcome ☺
 
 ## Endpoints
 
 ### Sender
 
 To send data with Devo SDK, first choose the required endpoint depending on the region your are accessing from:
@@ -109,96 +148,60 @@
 ### API authorization
 
 You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every
 Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab.
 
 ## Launch tests
 
-### run_tests script
+### Pytest
 
-You can run tests from the main folder of SDK
-To launch this script, you need either the environment variables loaded in the system, or the _environment.env_ file in the root of the SDK with the correct values, since to test all the SDK functionalities it is necessary to connect to Devo for the tests of sending and extracting data. There is an example file called _environment.env.example_
+The SDK uses Pytest for testing. This is a powerful tool for testing Python code. Pytest is a much more flexible and powerful tool than the built-in unittest module. It allows more testing functionality through the use of plugins. You can find more information in the [Pytest documentation](https://docs.pytest.org/en/stable/).
 
-Its normal, by the way, TCP tests fails in clients or not Devo developers systems.
+Install the testing requirements:
 
 ```console
-~/projects/devo-python-sdk > python setup.py test
+pip install -r requirements-test.txt
 ```
 
+You can run tests from the `tests` folder of SDK
+
 ```console
-~/projects/devo-python-sdk > python run_tests.py
+pytest
 ```
 
-You can add option "Coverage" for create HTML report about tests.
+Its normal that TCP tests fails in clients or not Devo developers systems.
+
+You can add the option `--cov` to create a coverage report.
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py --coverage
+pytest --cov
 ```
 
-You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
+Check the [pytest-cov documentation](https://pytest-cov.readthedocs.io/) for more details.
 
-```console
-~/projects/devo-python-sdk > python run_tests.py -m SENDER_CLI
-```
+The tests are divided into unit and integration tests. The integration tests require either a connection to Devo or to a local server that is launched when testing, so you need to have the environment variables in your system for all the tests that require connection to Devo can work.
 
-You can also exclude one or several tests with `-M` parameter:
+To run the unit tests only, you can use the `unit` folder:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -M SENDER_CLI,API_CLI
+pytest unit
 ```
 
-Using the --help flag prints the available modules to use:
+To run the integration tests only, you can use the `integration` folder:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py --help
-usage: run_tests.py [-h] [--coverage [COVERAGE]] [-m [MODULE]]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --coverage [COVERAGE]
-                        Generate coverage
-  -m [MODULES], --modules [MODULES]
-                        Run tests for selected modules: API_CLI, API_QUERY, API_TASKS, API_ERRORS, API_PARSER_DATE,
-                        API_PROCESSORS, API_KEEPALIVE, COMMON_CONFIGURATION, COMMON_DATE_PARSER, SENDER_CLI, SENDER_CSV,
-                        SENDER_NUMBER_LOOKUP, SENDER_SEND_DATA, SENDER_SEND_LOOKUP
-  -M [EXCLUDE_MODULES], --exclude-modules [EXCLUDE_MODULES]
-                        Exclude tests for modules: API_CLI, API_QUERY, API_TASKS, API_ERRORS, API_PARSER_DATE,
-                        API_PROCESSORS, API_KEEPALIVE, COMMON_CONFIGURATION, COMMON_DATE_PARSER, SENDER_CLI, SENDER_CSV,
-                        SENDER_NUMBER_LOOKUP, SENDER_SEND_DATA, SENDER_SEND_LOOKUP
+pytest integration
 ```
 
-- API_CLI: API Command-line interface tests.
-- API_QUERY: Query API tests.
-- API_TASKS: Task API tests.
-- API_ERRORS: Managing of API Errors tests.
-- API_PARSER_DATE: Parsing of dates in API tests.
-- API_PROCESSORS: Response processors in API tests.
-- API_KEEPALIVE: Keep Alive functionality in API tests.
-- COMMON_CONFIGURATION: Configuration tests.
-- COMMON_DATE_PARSER: Date parser tests.
-- SENDER_CLI: Lookup command-line interface tests.
-- SENDER_CSV: Lookup uploading through CSV tests.
-- SENDER_NUMBER_LOOKUP: Numbers in lookup tests
-- SENDER_SEND_DATA: Data sending tests.
-- SENDER_SEND_LOOKUP: Lookup sending tests.
-
-### Run using Unittest command
-
-You can see references in [unittest documentation](https://docs.python.org/3/library/unittest.html)
-
-For commands like:
+You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
 
 ```console
-python -m unittest discover -p "*.py"
+pytest unit/test_sender_encoding.py
 ```
 
-If you launch this command from the root directory of the SDK, you need to have the environment variables in your
-system for all the tests that require connection to Devo can work, not being able to use the environment.env file
-as in the script.
-
 ### Contact Us
 
 You can contact with us at _support@devo.com_.
 
 ## License
 
 MIT License
```

### Comparing `devo-sdk-5.1.9/devo/api/client.py` & `devo-sdk-5.2.0/devo/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Main class for pull data from Devo API (Client)."""
+
 import calendar
 import hashlib
 import hmac
 import json
 import logging
 import os
 import re
@@ -426,14 +427,15 @@
         self,
         query=None,
         query_id=None,
         dates=None,
         limit=None,
         offset=None,
         comment=None,
+        ip_as_string=False,
     ):
         """
         Query API by a custom query
         :param query: Query to perform
         :param query_id: Query ID to perform the query
         :param dates: Dict with "from" and "to" keys
         :param limit: Max number of rows
@@ -448,14 +450,15 @@
 
         query_opts = {
             "limit": limit,
             "response": self.config.response,
             "offset": offset,
             "destination": self.config.destination,
             "keepAliveToken": self.config.keepAliveToken,
+            "ip_as_string": ip_as_string,
         }
 
         if not self.stream_available(self.config.response) or not self.config.stream:
             if not dates["to"]:
                 dates["to"] = "now()"
             if self.config.stream:
                 logging.warning(ERROR_MSGS["stream_mode_not_supported"] % self.config.response)
@@ -678,14 +681,17 @@
                 payload["keepAlive"] = {"type": "token"}
             else:
                 payload["keepAlive"] = {
                     "type": "token",
                     "token": opts["keepAliveToken"],
                 }
 
+        if opts["ip_as_string"]:
+            payload["ipAsString"] = opts["ip_as_string"]
+
         return json.dumps(payload)
 
     def _get_headers(self, data):
         """
         Create headers for post call
         :param data: returned value from _get_payload()
         :return: Return the formed http headers
```

### Comparing `devo-sdk-5.1.9/devo/api/processors.py` & `devo-sdk-5.2.0/devo/api/processors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Defaults proccessors of API data."""
+
 import json
 
 
 def proc_default():
     """
     Default processor: return data in str/bytes, after strip
     :return: data
@@ -46,16 +47,16 @@
     return proc_json()
 
 
 def proc_json_compact_to_array():
     """
     :return: json object
     """
-    return (
-        lambda data: proc_json()(data)["object"]["d"]
+    return lambda data: (
+        proc_json()(data)["object"]["d"]
         if data and isinstance(data, str) and proc_bytes_to_str()(data) != ""
         else None
     )
 
 
 def json_compact_simple_names(data):
     if isinstance(data, str) and proc_bytes_to_str()(data) == "":
@@ -64,23 +65,25 @@
         return [item for item in sorted(data, key=lambda x: data[x]["index"])]
 
 
 def proc_json_compact_simple_to_jobj(names=None):
     return (
         proc_json_compact_simple_to_array()
         if not names
-        else lambda data: dict(zip(names, proc_json_compact_simple_to_array()(data)))
-        if data and isinstance(data, str) and proc_bytes_to_str()(data) != ""
-        else {}
+        else lambda data: (
+            dict(zip(names, proc_json_compact_simple_to_array()(data)))
+            if data and isinstance(data, str) and proc_bytes_to_str()(data) != ""
+            else {}
+        )
     )
 
 
 def proc_json_compact_simple_to_array():
-    return (
-        lambda data: proc_json()(data)["d"]
+    return lambda data: (
+        proc_json()(data)["d"]
         if data and isinstance(data, str) and proc_bytes_to_str()(data) != ""
         else []
     )
 
 
 def processors():
     """Return object with all functions availables"""
```

### Comparing `devo-sdk-5.1.9/devo/api/scripts/client_cli.py` & `devo-sdk-5.2.0/devo/api/scripts/client_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 """CLI for use Devo API from shell command line."""
+
 import os
 import sys
 
 import click
 
 from devo.__version__ import __version__
 from devo.api.client import ERROR_MSGS, Client, DevoClientException
@@ -80,14 +81,15 @@
     "--from",
     help="From date. For valid formats see API README. Default if now - 1 hour",
 )
 @click.option("--to", help="To date. For valid formats see API README")
 @click.option("--timeZone", help="Timezone info. For valid formats see API README")
 @click.option("--verify", type=bool, help="Verify certificates")
 @click.option("--debug/--no-debug", help="For testing purposes", default=False)
+@click.option("--ip-as-string", is_flag=True, help="Return IPs as strings", default=False)
 def query(**kwargs):
     """Perform query by query string"""
     api, config = configure(kwargs)
 
     if config is None:
         print_error("Error in config", show_help=True)
         if config["debug"]:
@@ -117,17 +119,17 @@
 
     if "response" in config.keys():
         if config["response"] in ["msgpack", "xls"]:
             if "output" not in config.keys():
                 print_error(ERROR_MSGS["binary_format_requires_output"], show_help=True)
                 exit()
 
-    reponse = api.query(query=config["query"], dates=dates)
+    response = api.query(query=config["query"], dates=dates, ip_as_string=config["ip_as_string"])
 
-    process_response(reponse, config)
+    process_response(response, config)
 
 
 def process_response(response, config):
     """
     process responses from Client API
     :param response: data received from Devo API
     :param config: array with launch options
```

### Comparing `devo-sdk-5.1.9/devo/common/__init__.py` & `devo-sdk-5.2.0/devo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/devo/common/dates/dateoperations.py` & `devo-sdk-5.2.0/devo/common/dates/dateoperations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """A collection of allowed operations on date parsing"""
+
 from datetime import datetime as dt
 from datetime import timedelta
 
 from .dateutils import to_millis, trunc_time, trunc_time_minute
 
 
 def month():
```

### Comparing `devo-sdk-5.1.9/devo/common/dates/dateparser.py` & `devo-sdk-5.2.0/devo/common/dates/dateparser.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/devo/common/dates/dateutils.py` & `devo-sdk-5.2.0/devo/common/dates/dateutils.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/devo/common/generic/configuration.py` & `devo-sdk-5.2.0/devo/common/generic/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-""" Util for load generic config file in devo standars"""
+"""Util for load generic config file in devo standars"""
+
 import json
 import os
 import sys
 from json import JSONDecodeError
 
 
 class ConfigurationException(Exception):
@@ -82,17 +83,15 @@
         :return: Returns a reference to the instance object
         """
         if path.endswith(".json"):
             return self.load_json(path, section)
         if path.endswith(".yaml") or path.endswith(".yml"):
             return self.load_yaml(path, section)
 
-        raise ConfigurationException(
-            "Configuration file type unknown or not supported: %s" % path
-        )
+        raise ConfigurationException(f"Configuration file type unknown or not supported: {path}")
 
     def save(self, path=None, save_bak=False):
         if path is None:
             return False
 
         if os.path.isfile(path):
             os.rename(path, "{}.bak".format(path))
@@ -126,19 +125,19 @@
             os.remove(file)
 
     @staticmethod
     def __search_default_config_file():
         return (
             "json"
             if os.path.exists(os.path.expanduser("~/.devo.json"))
-            else "yaml"
-            if os.path.exists(os.path.expanduser("~/.devo.yaml"))
-            else "yml"
-            if os.path.exists(os.path.expanduser("~/.devo.yml"))
-            else None
+            else (
+                "yaml"
+                if os.path.exists(os.path.expanduser("~/.devo.yaml"))
+                else "yml" if os.path.exists(os.path.expanduser("~/.devo.yml")) else None
+            )
         )
 
     def load_default_config(self, ext=None, section=None):
         """Function for load default configuration"""
         if not ext:
             ext = self.__search_default_config_file()
```

### Comparing `devo-sdk-5.1.9/devo/common/loadenv/load_env.py` & `devo-sdk-5.2.0/devo/common/loadenv/load_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Parsing .env file content and adding each value into os.environ
 For testing purposes
 """
+
 import ast
 import os
 
 
 def load_env_file(path=None):
     """
     Reads a .env file into os.environ.
```

### Comparing `devo-sdk-5.1.9/devo/common/logging/log.py` & `devo-sdk-5.2.0/devo/common/logging/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-""" Generic function to logging events in Devo SDK """
+"""Generic function to logging events in Devo SDK"""
+
 import logging
 import os
 import sys
 from logging.handlers import RotatingFileHandler
 
 
 def get_log(name="log", level=None, handler=None):
```

### Comparing `devo-sdk-5.1.9/devo/sender/data.py` & `devo-sdk-5.2.0/devo/sender/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
-""" File to group all the classes and functions related to the connection
-and sending of data to Devo """
+"""File to group all the classes and functions related to the connection
+and sending of data to Devo"""
+
 import errno
 import logging
 import select
 import socket
 import ssl
 import sys
 import time
@@ -22,14 +23,15 @@
 from .transformsyslog import (COMPOSE, COMPOSE_BYTES, FACILITY_USER, FORMAT_MY,
                               FORMAT_MY_BYTES, SEVERITY_INFO, priority_map)
 
 PYPY = hasattr(sys, "pypy_version_info")
 
 
 class ERROR_MSGS(str, Enum):
+
     def __str__(self):
         return str(self.value)
 
     WRONG_FILE_TYPE = ("'%s' is not a valid type to be opened as a file",)
     ADDRESS_TUPLE = ('Devo-SenderConfigSSL| address must be a tuple ("hostname", int(port))\'',)
     WRONG_SSL_CONFIG = ("Devo-SenderConfigSSL|Can't create SSL config: %s",)
     CONFIG_FILE_NOT_FOUND = (
```

### Comparing `devo-sdk-5.1.9/devo/sender/lookup.py` & `devo-sdk-5.2.0/devo/sender/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-""" File with utils for send Lookups to Devo """
+"""File with utils for send Lookups to Devo"""
+
 import csv
 import re
 import sys
 import time
 
 from devo.sender.data import open_file
```

### Comparing `devo-sdk-5.1.9/devo/sender/pfx_to_pem.py` & `devo-sdk-5.2.0/devo/sender/pfx_to_pem.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
-""" Util function to convert .pfx and .pkcs12 certs to key+cert+chain for
+"""Util function to convert .pfx and .pkcs12 certs to key+cert+chain for
 use in Python sockets"""
+
 import tempfile
 
 import OpenSSL.crypto
 
 
 def pfx_to_pem(path=None, password=None):
     """
```

### Comparing `devo-sdk-5.1.9/devo/sender/scripts/sender_cli.py` & `devo-sdk-5.2.0/devo/sender/scripts/sender_cli.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/devo/sender/transformsyslog.py` & `devo-sdk-5.2.0/devo/sender/transformsyslog.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/devo_sdk.egg-info/SOURCES.txt` & `devo-sdk-5.2.0/devo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.9/setup.py` & `devo-sdk-5.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,28 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 INSTALL_REQUIRES = [
     "requests~=2.31",
     "click==8.1.7",
     "PyYAML==6.0.1",
     "pem~=21.2.0",
-    "pyopenssl~=23.3",
-    "pytz~=2023.3",
-    "certifi~=2023.11.17",
-    "cryptography~=41.0.7",
+    "pyopenssl~=24.1.0",
+    "pytz~=2024.1",
+    "certifi~=2024.2.2",
+    "cryptography~=42.0.5",
 ]
 EXTRAS_REQUIRE = {
-    "dev": ["stopit==1.1.2", "msgpack~=1.0.7", "responses~=0.24", "pipdeptree~=2.13.1"]
+    "dev": [
+        "stopit==1.1.2",
+        "msgpack~=1.0.8",
+        "responses~=0.25.0",
+        "pipdeptree~=2.17.0",
+        "pytest~=8.1.1",
+        "pytest-cov~=5.0.0",
+    ]
 }
 CLI = [
     "devo-sender=devo.sender.scripts.sender_cli:cli",
     "devo-api=devo.api.scripts.client_cli:cli",
 ]
```

