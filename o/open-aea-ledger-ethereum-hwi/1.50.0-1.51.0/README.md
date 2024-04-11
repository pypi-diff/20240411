# Comparing `tmp/open-aea-ledger-ethereum-hwi-1.50.0.tar.gz` & `tmp/open-aea-ledger-ethereum-hwi-1.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.50.0.tar", last modified: Fri Mar 15 09:35:32 2024, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-hwi-1.51.0.tar", last modified: Thu Apr 11 03:16:28 2024, max compression
```

## Comparing `open-aea-ledger-ethereum-hwi-1.50.0.tar` & `open-aea-ledger-ethereum-hwi-1.51.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/bip32.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/hwi.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-15 09:35:32.000000 open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 09:35:32.320964 open-aea-ledger-ethereum-hwi-1.50.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-03-15 09:35:01.000000 open-aea-ledger-ethereum-hwi-1.50.0/tests/test_account.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:28.137447 open-aea-ledger-ethereum-hwi-1.51.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 03:16:28.137447 open-aea-ledger-ethereum-hwi-1.51.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:28.133447 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/bip32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/hwi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:28.137447 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 03:16:28.000000 open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:16:28.137447 open-aea-ledger-ethereum-hwi-1.51.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:16:28.137447 open-aea-ledger-ethereum-hwi-1.51.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-11 03:15:53.000000 open-aea-ledger-ethereum-hwi-1.51.0/tests/test_account.py
```

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/LICENSE` & `open-aea-ledger-ethereum-hwi-1.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.51.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.50.0
+Version: 1.51.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,13 +22,13 @@
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: open-aea<2.0.0,>=1.0.0
 Requires-Dist: web3<7,>=6.0.0
 Requires-Dist: ipfshttpclient==0.8.0a2
 Requires-Dist: eth-account<0.9.0,>=0.8.0
-Requires-Dist: open-aea-ledger-ethereum~=1.50.0
+Requires-Dist: open-aea-ledger-ethereum~=1.51.0
 Requires-Dist: ledgerwallet==0.1.3
 Requires-Dist: protobuf<4.25.0,>=4.21.6
 Requires-Dist: construct<=2.10.61
 
 Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
```

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/__init__.py` & `open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/account.py` & `open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/account.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/bip32.py` & `open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/bip32.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/exceptions.py` & `open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/aea_ledger_ethereum_hwi/hwi.py` & `open-aea-ledger-ethereum-hwi-1.51.0/aea_ledger_ethereum_hwi/hwi.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-hwi
-Version: 1.50.0
+Version: 1.51.0
 Summary: Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,13 +22,13 @@
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: open-aea<2.0.0,>=1.0.0
 Requires-Dist: web3<7,>=6.0.0
 Requires-Dist: ipfshttpclient==0.8.0a2
 Requires-Dist: eth-account<0.9.0,>=0.8.0
-Requires-Dist: open-aea-ledger-ethereum~=1.50.0
+Requires-Dist: open-aea-ledger-ethereum~=1.51.0
 Requires-Dist: ledgerwallet==0.1.3
 Requires-Dist: protobuf<4.25.0,>=4.21.6
 Requires-Dist: construct<=2.10.61
 
 Python package wrapping the public and private key cryptography and support for hardware wallet interactions.
```

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-hwi-1.51.0/open_aea_ledger_ethereum_hwi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/setup.py` & `open-aea-ledger-ethereum-hwi-1.51.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_hwi" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-hwi",
-    version="1.50.0",
+    version="1.51.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description="Python package wrapping the public and private key cryptography and support for hardware wallet interactions.",
     long_description_content_type="text/markdown",
     packages=find_packages(include=["aea_ledger_ethereum_hwi*"]),
     package_data={
@@ -38,15 +38,15 @@
         ]
     },
     install_requires=[
         "open-aea>=1.0.0, <2.0.0",
         "web3>=6.0.0,<7",
         "ipfshttpclient==0.8.0a2",
         "eth-account>=0.8.0,<0.9.0",
-        "open-aea-ledger-ethereum~=1.50.0",
+        "open-aea-ledger-ethereum~=1.51.0",
         "ledgerwallet==0.1.3",
         "protobuf<4.25.0,>=4.21.6",
         "construct<=2.10.61",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": ["ethereum_hwi = aea_ledger_ethereum_hwi:EthereumHWICrypto"],
```

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/tests/__init__.py` & `open-aea-ledger-ethereum-hwi-1.51.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-hwi-1.50.0/tests/test_account.py` & `open-aea-ledger-ethereum-hwi-1.51.0/tests/test_account.py`

 * *Files identical despite different names*

