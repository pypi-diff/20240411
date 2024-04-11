# Comparing `tmp/DeFiLlama-1.1.0.tar.gz` & `tmp/DeFiLlama-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DeFiLlama-1.1.0.tar", last modified: Sat Jun 26 17:08:20 2021, max compression
+gzip compressed data, was "DeFiLlama-2.1.0.tar", last modified: Thu Apr 11 15:06:33 2024, max compression
```

## Comparing `DeFiLlama-1.1.0.tar` & `DeFiLlama-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-06-26 17:08:20.492964 DeFiLlama-1.1.0/
-drwxrwxrwx   0        0        0        0 2021-06-26 17:08:20.489531 DeFiLlama-1.1.0/DeFiLlama.egg-info/
--rw-rw-rw-   0        0        0     2682 2021-06-26 17:08:20.000000 DeFiLlama-1.1.0/DeFiLlama.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2021-06-26 17:08:20.000000 DeFiLlama-1.1.0/DeFiLlama.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-26 17:08:20.000000 DeFiLlama-1.1.0/DeFiLlama.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-06-26 17:08:20.000000 DeFiLlama-1.1.0/DeFiLlama.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-06-26 17:08:20.000000 DeFiLlama-1.1.0/DeFiLlama.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2682 2021-06-26 17:08:20.492610 DeFiLlama-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1587 2021-06-26 17:06:52.000000 DeFiLlama-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2021-06-26 17:08:20.491609 DeFiLlama-1.1.0/defillama/
--rw-rw-rw-   0        0        0      230 2021-05-18 09:41:18.000000 DeFiLlama-1.1.0/defillama/__init__.py
--rw-rw-rw-   0        0        0      336 2021-06-26 17:02:39.000000 DeFiLlama-1.1.0/defillama/__version__.py
--rw-rw-rw-   0        0        0     3047 2021-05-18 09:41:18.000000 DeFiLlama-1.1.0/defillama/defillama.py
--rw-rw-rw-   0        0        0       42 2021-06-26 17:08:20.492964 DeFiLlama-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1172 2021-05-18 09:42:52.000000 DeFiLlama-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.819090 DeFiLlama-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/DeFiLlama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 15:06:33.000000 DeFiLlama-2.1.0/DeFiLlama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/defillama/defillama.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:06:33.819090 DeFiLlama-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:06:33.815089 DeFiLlama-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-11 15:06:26.000000 DeFiLlama-2.1.0/tests/test_defillama.py
```

### Comparing `DeFiLlama-1.1.0/README.md` & `DeFiLlama-2.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-# DeFiLlama
-
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
-[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
-[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
-[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-
-[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-
-[![Build](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml/badge.svg)](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml)
-
--------
-
-### Unofficial [DeFi Llama API](https://defillama.com/home) client in python
-
-For detailed information about the API endpoints, see [DeFi Llama API Documentation](https://docs.llama.fi/api)
-
-### Installation:
-
-use pip to install:
-
-``` 
-pip install DeFiLlama
-```
-
------------
-
-### Authentication:
-
-Endpoints are accessible without an API key.
-
------------
-
-### Example usage:
-
-```
-from defillama import DefiLlama
-
-# initialize api client
-llama = DefiLlama()
-
-# Get all protocols data
-response = llama.get_all_protocols()
-
-# Get a protocol data
-response = llama.get_protocol(name='uniswap')
-
-# Get historical values of total TVL
-response = llama.get_historical_tvl()
-
-# Get protocol TVL
-response = llama.get_protocol_tvl(name='uniswap')
-```
+# DeFiLlama
+
+[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
+[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
+
+[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
+
+[![Build](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml/badge.svg)](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml)
+
+
+### Unofficial [DeFi Llama API](https://defillama.com/home) client in python
+
+For detailed information about the API endpoints, see [DeFi Llama API Documentation](https://defillama.com/docs/api)
+
+### Installation:
+
+use pip to install:
+
+``` 
+pip install DeFiLlama
+```
+
+-----------
+
+### Authentication:
+
+Endpoints are accessible without an API key.
+
+-----------
+
+### Example usage:
+
+```
+from defillama import DefiLlama
+
+# initialize api client
+llama = DefiLlama()
+
+# Get all protocols data
+response = llama.get_all_protocols()
+
+# Get a protocol data
+response = llama.get_protocol(name='uniswap')
+
+```
+-------
+#### Donate & Help maintain the library
+
+[![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
+
+-------
```

### Comparing `DeFiLlama-1.1.0/setup.py` & `DeFiLlama-2.1.0/setup.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import setuptools
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-packages = ['defillama']
-
-requires = [
-    'requests>=2.18.4',
-]
-
-about = {}
-
-with open(os.path.join(here, 'defillama', '__version__.py'), mode='r', encoding='utf-8') as f:
-    exec(f.read(), about)
-
-with open('README.md', mode='r', encoding='utf-8') as f:
-    readme = f.read()
-
-setuptools.setup(
-    name=about['__title__'],
-    version=about['__version__'],
-    description=about['__description__'],
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    author=about['__author__'],
-    author_email=about['__author_email__'],
-    url=about['__url__'],
-    packages=packages,
-    install_requires=requires,
-    license=about['__license__'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-)
+import setuptools
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+packages = ['defillama']
+
+requires = [
+    'requests>=2.18.4',
+]
+
+about = {}
+
+with open(os.path.join(here, 'defillama', '__version__.py'), mode='r', encoding='utf-8') as f:
+    exec(f.read(), about)
+
+with open('README.md', mode='r', encoding='utf-8') as f:
+    readme = f.read()
+
+setuptools.setup(
+    name=about['__title__'],
+    version=about['__version__'],
+    description=about['__description__'],
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    author=about['__author__'],
+    author_email=about['__author_email__'],
+    url=about['__url__'],
+    packages=packages,
+    install_requires=requires,
+    license=about['__license__'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+    ],
+)
```

