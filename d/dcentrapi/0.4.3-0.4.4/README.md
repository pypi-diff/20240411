# Comparing `tmp/dcentrapi-0.4.3.tar.gz` & `tmp/dcentrapi-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcentrapi-0.4.3.tar", last modified: Fri Mar 22 17:16:36 2024, max compression
+gzip compressed data, was "dcentrapi-0.4.4.tar", last modified: Thu Apr 11 06:49:10 2024, max compression
```

## Comparing `dcentrapi-0.4.3.tar` & `dcentrapi-0.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:16:36.170288 dcentrapi-0.4.3/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/LICENSE.rst
--rw-r--r--   0 root         (0) root         (0)     6780 2024-03-22 17:16:36.170288 dcentrapi-0.4.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6211 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:16:36.168288 dcentrapi-0.4.3/dcentrapi/
--rw-rw-rw-   0 root         (0) root         (0)     1806 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/Base.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8891 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/eventPolling.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/gasMonitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/hackMitigation.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/merkleTree.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/requests_dappi.py
--rw-rw-rw-   0 root         (0) root         (0)     3107 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/rpcAggregation.py
--rw-rw-rw-   0 root         (0) root         (0)     1438 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/tokenPrices.py
--rw-rw-rw-   0 root         (0) root         (0)     1408 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/txSimulation.py
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/dcentrapi/web3Index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 17:16:36.169288 dcentrapi-0.4.3/dcentrapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6780 2024-03-22 17:16:36.000000 dcentrapi-0.4.3/dcentrapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-03-22 17:16:36.000000 dcentrapi-0.4.3/dcentrapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 17:16:36.000000 dcentrapi-0.4.3/dcentrapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-22 17:16:36.000000 dcentrapi-0.4.3/dcentrapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-22 17:16:36.000000 dcentrapi-0.4.3/dcentrapi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-22 17:16:36.170288 dcentrapi-0.4.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1140 2024-03-22 17:16:29.000000 dcentrapi-0.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:49:10.024402 dcentrapi-0.4.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/LICENSE.rst
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-04-11 06:49:10.024402 dcentrapi-0.4.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6211 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:49:10.023402 dcentrapi-0.4.4/dcentrapi/
+-rw-rw-rw-   0 root         (0) root         (0)     1932 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/Base.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8891 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/eventPolling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2159 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/gasMonitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2049 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/hackMitigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/merkleTree.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/requests_dappi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/rpcAggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1438 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/tokenPrices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/txSimulation.py
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/dcentrapi/web3Index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 06:49:10.024402 dcentrapi-0.4.4/dcentrapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-04-11 06:49:09.000000 dcentrapi-0.4.4/dcentrapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-11 06:49:09.000000 dcentrapi-0.4.4/dcentrapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 06:49:09.000000 dcentrapi-0.4.4/dcentrapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-11 06:49:09.000000 dcentrapi-0.4.4/dcentrapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 06:49:09.000000 dcentrapi-0.4.4/dcentrapi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 06:49:10.024402 dcentrapi-0.4.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1140 2024-04-11 06:49:03.000000 dcentrapi-0.4.4/setup.py
```

### Comparing `dcentrapi-0.4.3/LICENSE.rst` & `dcentrapi-0.4.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/PKG-INFO` & `dcentrapi-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.4.3
+Version: 0.4.4
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.4.3/README.md` & `dcentrapi-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/Base.py` & `dcentrapi-0.4.4/dcentrapi/Base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class Base:
     def __init__(self, stage, username=None, key=None):
-        self.__version__ = "0.4.3"  # update here and in setup.py
+        self.__version__ = "0.4.4"  # update here and in setup.py
         if stage == "develop":
             self.headers = {
                 "Authorization": username + "," + key,
                 "Api_key": username + "," + key
             }
             self.url = "https://test-api.dcentralab.com/"
             self.arbitrage_url = "https://test-api.web3index.info/arb/"
@@ -34,11 +34,13 @@
                 "Authorization": username + "," + key,
                 "Api_key": username + "," + key
             }
             self.url = "https://staging-api.dcentralab.com/"
             self.arbitrage_url = "https://staging-api.web3index.info/arb/"
 
 
-class DapiError:
-    def __init__(self, response, exception):
+class DapiError(Exception):
+    def __init__(self, message=None, status_code=None, response=None, exception=None):
+        super().__init__(message)
+        self.status_code = status_code
         self.response = response
         self.exception = exception
```

### Comparing `dcentrapi-0.4.3/dcentrapi/__init__.py` & `dcentrapi-0.4.4/dcentrapi/__init__.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/eventPolling.py` & `dcentrapi-0.4.4/dcentrapi/eventPolling.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/hackMitigation.py` & `dcentrapi-0.4.4/dcentrapi/hackMitigation.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from dcentrapi.requests_dappi import requests_get
 
 logger = logging.getLogger()
 logger.setLevel("INFO")
 
 
 class HackMitigation(Base):
-    def are_addresses_blacklisted(self, addresses: [str], from_dapi_list: bool = True, from_sanctioned_api: bool = False):
+    def are_addresses_blacklisted(self, addresses: [str], check_malcon: bool = True, check_sanctioned: bool = False):
         url = self.url + "generic_freeze_signal/are_addresses_blacklisted"
         data = {
             "addresses": addresses,
-            "from_dapi_list": from_dapi_list,
-            "from_sanctioned_api": from_sanctioned_api,
+            "check_malcon": check_malcon,
+            "check_sanctioned": check_sanctioned,
         }
         response = None
         tries = 7
         while tries > 0:
             logger.info(f"{tries} more tries")
             before = datetime.datetime.now()
             logger.info(f"before request: {before}")
```

### Comparing `dcentrapi-0.4.3/dcentrapi/merkleTree.py` & `dcentrapi-0.4.4/dcentrapi/merkleTree.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/rpcAggregation.py` & `dcentrapi-0.4.4/dcentrapi/rpcAggregation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/tokenPrices.py` & `dcentrapi-0.4.4/dcentrapi/tokenPrices.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/txSimulation.py` & `dcentrapi-0.4.4/dcentrapi/txSimulation.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi/web3Index.py` & `dcentrapi-0.4.4/dcentrapi/web3Index.py`

 * *Files identical despite different names*

### Comparing `dcentrapi-0.4.3/dcentrapi.egg-info/PKG-INFO` & `dcentrapi-0.4.4/dcentrapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcentrapi
-Version: 0.4.3
+Version: 0.4.4
 Summary: Dcentralab Pypi packages
 Home-page: UNKNOWN
 Author: Dcentralab (Niv Shitrit)
 Author-email: <niv@dcentralab.com>
 License: MIT
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `dcentrapi-0.4.3/setup.py` & `dcentrapi-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     return result.group(1)
 
 
 DESCRIPTION = "Dcentralab Pypi packages"
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 project_name = "dcentrapi"
-VERSION = "0.4.3"  # update here and in Base.py
+VERSION = "0.4.4"  # update here and in Base.py
 
 
 # Setting up
 setup(
     name="dcentrapi",
     version=VERSION,
     author="Dcentralab (Niv Shitrit)",
```

