# Comparing `tmp/proxlist-1.0.0.tar.gz` & `tmp/proxlist-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxlist-1.0.0.tar", last modified: Sun Jul  2 02:22:49 2023, max compression
+gzip compressed data, was "proxlist-1.0.1.tar", last modified: Thu Apr 11 15:34:51 2024, max compression
```

## Comparing `proxlist-1.0.0.tar` & `proxlist-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:22:21.000000 proxlist-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 02:22:49.900431 proxlist-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-02 02:22:21.000000 proxlist-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/proxlist/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/proxlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:22:21.000000 proxlist-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:22:49.904431 proxlist-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-02 02:22:21.000000 proxlist-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.896431 proxlist-1.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:21.000000 proxlist-1.0.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-02 02:22:21.000000 proxlist-1.0.0/test/unit/test_proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:51.052726 proxlist-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 15:34:24.000000 proxlist-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-11 15:34:51.052726 proxlist-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-11 15:34:24.000000 proxlist-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:51.048726 proxlist-1.0.1/proxlist/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-11 15:34:24.000000 proxlist-1.0.1/proxlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 15:34:24.000000 proxlist-1.0.1/proxlist/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-11 15:34:24.000000 proxlist-1.0.1/proxlist/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:24.000000 proxlist-1.0.1/proxlist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:51.048726 proxlist-1.0.1/proxlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-11 15:34:51.000000 proxlist-1.0.1/proxlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 15:34:51.000000 proxlist-1.0.1/proxlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:34:51.000000 proxlist-1.0.1/proxlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 15:34:51.000000 proxlist-1.0.1/proxlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 15:34:51.000000 proxlist-1.0.1/proxlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-11 15:34:24.000000 proxlist-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:34:51.052726 proxlist-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-11 15:34:24.000000 proxlist-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:51.048726 proxlist-1.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:51.048726 proxlist-1.0.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 15:34:24.000000 proxlist-1.0.1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-11 15:34:24.000000 proxlist-1.0.1/test/unit/test_proxies.py
```

### Comparing `proxlist-1.0.0/LICENSE` & `proxlist-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proxlist-1.0.0/PKG-INFO` & `proxlist-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: proxlist
-Version: 1.0.0
-Summary: Retrieve free, open-source proxy servers.
-Home-page: http://github.com/Justintime50/proxlist
-Author: Justintime50
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 
 # Proxlist
 
 Retrieve free, open-source proxy servers.
 
 [![Build Status](https://github.com/Justintime50/proxlist/workflows/build/badge.svg)](https://github.com/Justintime50/proxlist/actions)
```

### Comparing `proxlist-1.0.0/proxlist/proxies.py` & `proxlist-1.0.1/proxlist/proxies.py`

 * *Files identical despite different names*

### Comparing `proxlist-1.0.0/proxlist.egg-info/PKG-INFO` & `proxlist-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 Metadata-Version: 2.1
 Name: proxlist
-Version: 1.0.0
+Version: 1.0.1
 Summary: Retrieve free, open-source proxy servers.
 Home-page: http://github.com/Justintime50/proxlist
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: beautifulsoup4==4.*
+Requires-Dist: requests==2.*
+Requires-Dist: woodchips==1.*
+Provides-Extra: dev
+Requires-Dist: bandit==1.7.*; extra == "dev"
+Requires-Dist: black==23.*; extra == "dev"
+Requires-Dist: build==0.10.*; extra == "dev"
+Requires-Dist: flake8==6.*; extra == "dev"
+Requires-Dist: isort==5.*; extra == "dev"
+Requires-Dist: mypy==1.5.*; extra == "dev"
+Requires-Dist: pytest==7.*; extra == "dev"
+Requires-Dist: pytest-cov==4.*; extra == "dev"
+Requires-Dist: twine==4.*; extra == "dev"
+Requires-Dist: types-requests; extra == "dev"
 
 <div align="center">
 
 # Proxlist
 
 Retrieve free, open-source proxy servers.
```

### Comparing `proxlist-1.0.0/setup.py` & `proxlist-1.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,45 @@
+import re
+
 import setuptools
 
 
-with open('README.md', 'r') as fh:
-    long_description = fh.read()
+with open('README.md', 'r') as readme_file:
+    long_description = readme_file.read()
+
+# Inspiration: https://stackoverflow.com/a/7071358/6064135
+with open('proxlist/_version.py', 'r') as version_file:
+    version_groups = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file.read(), re.M)
+    if version_groups:
+        version = version_groups.group(1)
+    else:
+        raise RuntimeError('Unable to find version string!')
 
 REQUIREMENTS = [
     'beautifulsoup4 == 4.*',
     'requests == 2.*',
-    'woodchips == 0.2.*',
+    'woodchips == 1.*',
 ]
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
     'black == 23.*',
     'build == 0.10.*',
     'flake8 == 6.*',
     'isort == 5.*',
-    'mypy == 1.3.*',
+    'mypy == 1.5.*',
     'pytest == 7.*',
     'pytest-cov == 4.*',
     'twine == 4.*',
     'types-requests',
 ]
 
 setuptools.setup(
     name='proxlist',
-    version='1.0.0',
+    version=version,
     description='Retrieve free, open-source proxy servers.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/Justintime50/proxlist',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
```

### Comparing `proxlist-1.0.0/test/unit/test_proxies.py` & `proxlist-1.0.1/test/unit/test_proxies.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for _ in range(3):
         try:
             random_proxy = proxlist.random_proxy()
         except Exception:
             # If we fail to find a valid proxy, try again a couple more times before failing
             continue
 
-        assert type(random_proxy) == str
+        assert isinstance(random_proxy, str)
         assert ':' in random_proxy
         assert 12 < len(random_proxy) < 25
 
 
 def test_random_proxy_filter_country():
     """Tests that we can retrieve a random proxy when filtering by country."""
     countries_to_try = [
@@ -31,29 +31,29 @@
     for country in countries_to_try:
         try:
             random_proxy = proxlist.random_proxy(country=country)
         except Exception:
             # If we fail to find a valid proxy from one country, try another country
             continue
 
-        assert type(random_proxy) == str
+        assert isinstance(random_proxy, str)
         assert ':' in random_proxy
         assert 12 < len(random_proxy) < 25
 
 
 def test_random_proxy_filter_google_verified():
     """Tests that we can retrieve a random proxy when filtering for a google verified proxy."""
     for _ in range(3):
         try:
             random_proxy = proxlist.random_proxy(google_verified=True)
         except Exception:
             # If we fail to find a valid proxy, try again a couple more times before failing
             continue
 
-        assert type(random_proxy) == str
+        assert isinstance(random_proxy, str)
         assert ':' in random_proxy
         assert 12 < len(random_proxy) < 25
 
 
 @patch('proxlist.proxies.get_proxies', return_value=[])
 def test_random_proxy_no_proxies_list(mock_get_proxies):
     """Tests that we raise an error when no proxies are found."""
@@ -93,15 +93,15 @@
     assert str(error.value) == 'mock-error'
 
 
 def test_list_proxies():
     """Tests that we can retrieve a list of proxies from the free proxy website."""
     proxy_list = proxlist.list_proxies()
 
-    assert type(proxy_list) == list
+    assert isinstance(proxy_list, list)
     assert len(proxy_list) > 50  # The list should typically be ~100 records
 
 
 @patch('woodchips.Logger')
 def test_setup_logger(mock_logger):
     proxlist.proxies._setup_logger()
```

