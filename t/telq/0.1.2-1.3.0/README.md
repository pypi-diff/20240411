# Comparing `tmp/telq-0.1.2.tar.gz` & `tmp/telq-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telq-0.1.2.tar", max compression
+gzip compressed data, was "telq-1.3.0.tar", max compression
```

## Comparing `telq-0.1.2.tar` & `telq-1.3.0.tar`

### file list

```diff
@@ -1,11 +1,17 @@
--rw-r--r--   0        0        0    11345 2022-07-13 21:25:34.640037 telq-0.1.2/LICENSE
--rwxr-xr-x   0        0        0      394 2022-07-13 21:25:34.640037 telq-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-07-13 21:25:34.640037 telq-0.1.2/telq/.DS_Store
--rwxr-xr-x   0        0        0    10290 2022-07-13 21:25:34.644038 telq-0.1.2/telq/__init__.py
--rwxr-xr-x   0        0        0     2766 2022-07-13 21:25:34.644038 telq-0.1.2/telq/authentication/__init__.py
--rwxr-xr-x   0        0        0     1307 2022-07-13 21:25:34.644038 telq-0.1.2/telq/endpoints/__init__.py
--rwxr-xr-x   0        0        0     1973 2022-07-13 21:25:34.644038 telq-0.1.2/telq/networks/__init__.py
--rwxr-xr-x   0        0        0     1238 2022-07-13 21:25:34.644038 telq-0.1.2/telq/results/__init__.py
--rwxr-xr-x   0        0        0     5332 2022-07-13 21:25:34.644038 telq-0.1.2/telq/tests/__init__.py
--rw-r--r--   0        0        0      781 2022-07-13 21:25:48.941420 telq-0.1.2/setup.py
--rw-r--r--   0        0        0      568 2022-07-13 21:25:48.941691 telq-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-11 08:27:49.459812 telq-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0      461 2024-04-11 08:27:49.459812 telq-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-11 08:27:49.459812 telq-1.3.0/telq/.DS_Store
+-rwxr-xr-x   0        0        0     6325 2024-04-11 08:27:49.459812 telq-1.3.0/telq/__init__.py
+-rwxr-xr-x   0        0        0     3490 2024-04-11 08:27:49.463812 telq-1.3.0/telq/authentication/__init__.py
+-rwxr-xr-x   0        0        0     4481 2024-04-11 08:27:49.463812 telq-1.3.0/telq/endpoints/__init__.py
+-rwxr-xr-x   0        0        0     2004 2024-04-11 08:27:49.463812 telq-1.3.0/telq/networks/__init__.py
+-rwxr-xr-x   0        0        0     5066 2024-04-11 08:27:49.463812 telq-1.3.0/telq/session/__init__.py
+-rw-r--r--   0        0        0     1685 2024-04-11 08:27:49.463812 telq-1.3.0/telq/session/session_data.py
+-rwxr-xr-x   0        0        0     6376 2024-04-11 08:27:49.463812 telq-1.3.0/telq/supplier/__init__.py
+-rw-r--r--   0        0        0     1514 2024-04-11 08:27:49.463812 telq-1.3.0/telq/supplier/supplier_data.py
+-rwxr-xr-x   0        0        0       94 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/__init__.py
+-rwxr-xr-x   0        0        0     7267 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/lnt.py
+-rw-r--r--   0        0        0      277 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/model.py
+-rwxr-xr-x   0        0        0     5051 2024-04-11 08:27:49.463812 telq-1.3.0/telq/tests/mt.py
+-rw-r--r--   0        0        0     1876 2024-04-11 08:27:49.463812 telq-1.3.0/telq/util/rest.py
+-rw-r--r--   0        0        0      709 1970-01-01 00:00:00.000000 telq-1.3.0/PKG-INFO
```

### Comparing `telq-0.1.2/LICENSE` & `telq-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `telq-0.1.2/telq/.DS_Store` & `telq-1.3.0/telq/.DS_Store`

 * *Files identical despite different names*

### Comparing `telq-0.1.2/telq/authentication/__init__.py` & `telq-1.3.0/telq/authentication/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import warnings
+import os
 from dataclasses import dataclass
-
+import warnings
+import toml
 import requests
 import telq.endpoints as endpoints
 
 
 @dataclass
 class Authentication:
     """Performs authentication with the App Id and App Key
@@ -13,64 +14,81 @@
     Parameters
     ----------
     api_id : str
         TelQ uses API keypairs (appId, appKey) to allow access to the API.
         You can find your AppId and generate your AppKey on the API Menu of the TelQ App.
     api_key : str
         Your AppKey gotten from the API Menu of the TelQ App
-    api_version : str, default 'v2.1'
-        API version to use, defaults to version 'v2.1'
+    api_version : str, default 'v3'
+        API version to use, defaults to version 'v3'
         Versions 1.0, 1.1, 1.2, 1.3 and 1.4 have been deprecated. This means no new development or bug fixes
         will occur on those versions, but they will continue to be supported
         by our app through 2021. We may stop supporting them at some point in the future
         but we will give ample warning to all our customers about it.
+    base_url : str, default 'https://api.telqtele.com'
+        Base URL for TelQ App
 
     Raises
     ------
     ValueError
         if you pass an API version not supported
     """ ""
 
     api_id: str
     api_key: str
-    api_version: str = "v2.1"
+    base_url: str
+    api_version: str = "v3"
 
     def __post_init__(self) -> None:
         self.headers = {
             "accept": "application/json",
             "Content-Type": "application/json",
+            "User-Agent": f"python-sdk/{self.__get_sdk_version__()}"
         }
-        self.data = {"appId": self.api_id, "appKey": self.api_key}
+        self.data = {"appId": self.api_id, "appKey": self.api_key, "baseUrl": self.base_url}
         self._validate_api_version()
         self._authenticate_user()
 
+    def __get_sdk_version__(self):
+        pyproject_toml_path = os.path.abspath(
+            os.path.join(os.path.dirname(__file__), "..", "..", "pyproject.toml")
+        )
+        with open(pyproject_toml_path, "r") as file:
+            content = file.read()
+
+        # Parse the content using the toml library
+        data = toml.loads(content)
+
+        # Extract the version (assuming it's under [tool.poetry])
+        version = data["tool"]["poetry"]["version"]
+        return version
+
     def _validate_api_version(self) -> None:
         _deprecated_versions = ["v1.0", "v1.1", "v1.2", "v1.3", "v1.4"]
-        _currently_supported_versions = ["v1.5", "v2.1"]
+        _currently_supported_versions = ["v1.5", "v2.1", "v3"]
 
         if self.api_version in _deprecated_versions:
             warnings.warn(
                 "Versions 1.0 through 1.4 are deprecated and will not longer be supported in the future",
                 DeprecationWarning,
             )
         elif self.api_version in _currently_supported_versions:
             pass
         else:
             raise ValueError(
-                "Invalid TelQ API selected - choose a version like 'v2.1' or 'v1.5' and so on - see our documentation for more information"
+                "Invalid TelQ API selected - choose a version like 'v2.2' or 'v1.5' and so on - see our documentation for more information"
             )
 
     def _authenticate_user(self) -> None:
         # pass App Id and App Key to the token endpoint to authenticate user
-        url = endpoints.TokenURL(self.api_version).url()
+        url = endpoints.TokenURL(self.base_url, self.api_version).url()
         method = "POST"
         response = requests.request(method, url, headers=self.headers, json=self.data)
 
         try:
-
             res = response.json()
             if 'error' in res:
                 raise ValueError(res['message'])
             response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             raise Exception(e)
```

### Comparing `telq-0.1.2/telq/networks/__init__.py` & `telq-1.3.0/telq/networks/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """ ""
 
     def __init__(self, authentication: authentication.Authentication):
         self._authentication = authentication
 
     def get_networks(self):
         """Retrieves a list with all our currently available Networks"""
-        url = NetworksURL(self._authentication.api_version).url()
+        url = NetworksURL(self._authentication.base_url, self._authentication.api_version).url()
         method = "GET"
         headers = {
             "accept": "application/json",
             "Authorization": self._authentication._bearer_token,
         }
         response = requests.request(method, url, headers=headers)
         res = response.json()
```

### Comparing `telq-0.1.2/telq/tests/__init__.py` & `telq-1.3.0/telq/tests/mt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from typing import Dict, List, Union
 
-import requests
-import telq.authentication as authentication
-from telq.endpoints import TestsURL
+from telq.endpoints import ResultsURL, TestsURL
+from telq.util.rest import TelQRest
 
 
-class Tests:
-    """Receives a list with the Destination Networks where you want to send your tests. 
-    For each requested network, a test will be created if the network is still available 
-    at the time of the test request. 
-    Keep in mind that networks can go offline sometimes after the results 
+class MT(TelQRest):
+    """Receives a list with the Destination Networks where you want to send your tests.
+    For each requested network, a test will be created if the network is still available
+    at the time of the test request.
+    Keep in mind that networks can go offline sometimes after the results
     from the /networks endpoint have been returned.
 
     Parameters
     -------
     authentication: authentication.Authentication
         The authentication class after you have been authenticated
 
     Raises
     ------
     Exception
-        The Exception will display the error code and the message. 
+        The Exception will display the error code and the message.
         This will happen If there is an error with your request
     """ ""
 
-    def __init__(self, authentication: authentication.Authentication):
-        self._authentication = authentication
-
     def initiate_new_tests(
         self,
         destinationNetworks: List[Dict[str, str]],
         resultsCallbackUrl: Union[str, None] = None,
         maxCallbackRetries: int = 3,
         testIdTextType: str = "ALPHA",
         testIdTextCase: str = "MIXED",
@@ -38,74 +34,65 @@
         testTimeToLiveInSeconds: int = 3600,
     ):
         """Initiate a new test
 
         Parameters
         ----------
         destinationNetworks : List[Dict[str, str]]
-            The list of networks you want to issue tests to. This is required and cannot be empty. 
+            The list of networks you want to issue tests to. This is required and cannot be empty.
             Each network are required to have at least the mcc and mc as keys. optional are portedFromMnc
         resultsCallbackUrl : Union[str, None], optional
-            The callback URL where you would like to receive TestResult updates 
+            The callback URL where you would like to receive TestResult updates
             anytime your tests status changes, by default None
         maxCallbackRetries : int, optional
-            The maximum number of attemps you want us to try when calling your "callback url" with updates. 
+            The maximum number of attemps you want us to try when calling your "callback url" with updates.
             Maximum is 5, by default 3
         testIdTextType : str, optional
-            The type of testIdText to use in this test. 
+            The type of testIdText to use in this test.
             Options are: "ALPHA", "ALPHA_NUMERIC", "NUMERIC", "WHATSAPP_CODE", by default "ALPHA"
         testIdTextCase : str, optional
-            The case to use for letters in the testIdText. 
+            The case to use for letters in the testIdText.
             Applies only to ALPHA and ALPHA_NUMERIC types. Options are: "UPPER", "LOWER", "MIXED", by default "MIXED"
         testIdTextLength : int, optional
-            The number of characters to use for generating the testIdText. default=10, minimum=4, maximum=20. 
+            The number of characters to use for generating the testIdText. default=10, minimum=4, maximum=20.
             Doesn't apply to WHATSAPP_CODE type, since it has a fixed length of 7, by default 10
         testTimeToLiveInSeconds : int, optional
-            The maximum amount of time you want your tests to wait for a message. 
+            The maximum amount of time you want your tests to wait for a message.
             Default is 1 hour. (Minimum of 1 minute, maximum of 3 hours), by default 3600
 
         Returns
         -------
         JSON Response
-            The Response consists of an array of Test objects, containing each a destinationNetwork 
+            The Response consists of an array of Test objects, containing each a destinationNetwork
             and details about the test request. Here is a description of each of the keys contained by a Test object:
 
         Raises
         ------
         Exception
             When an error occurs, the associated error is returned
         """ ""
-        url = TestsURL(self._authentication.api_version).url()
+        url = TestsURL(self._authentication.base_url, self._authentication.api_version).url()
         method = "POST"
-        headers = {
-            "accept": "*/*",
-            "Content-Type": "application/json",
-            "Authorization": self._authentication._bearer_token,
-        }
 
         data = self._validate_parse_data(
             destinationNetworks,
             resultsCallbackUrl,
             maxCallbackRetries,
             testIdTextType,
             testIdTextCase,
             testIdTextLength,
             testTimeToLiveInSeconds,
         )
 
-        response = requests.request(method, url, headers=headers, json=data)
+        return self.request(url, method, data)
 
-        res = response.json()
-        try:
-            if 'error' in res:
-                raise ValueError(res['message'])
-            response.raise_for_status()
-        except requests.exceptions.HTTPError as e:
-            raise (e)
-        return res
+    def get_test_results(self, test_id: int):
+        url = ResultsURL(self._authentication.base_url, self._authentication.api_version).url(test_id=test_id)
+        method = "GET"
+        return self.request(url, method)
 
     def _validate_parse_data(
         self,
         destinationNetworks: List[Dict[str, str]],
         resultsCallbackUrl: Union[str, None],
         maxCallbackRetries,
         testIdTextType,
@@ -114,17 +101,17 @@
         testTimeToLiveInSeconds: int,
     ) -> Dict[str, str]:
         if not isinstance(destinationNetworks, list):
             raise ValueError(
                 "destinationNetworks is a list of networks you want to issue tests to, ensure its a list"
             )
         for network in destinationNetworks:
-            if not {"mcc", "mnc"}.issubset(network):
+            if not {"mcc", "mnc"}.issubset(network) and not {"phoneNumber"}.issubset(network):
                 raise KeyError(
-                    "destinationNetworks is missing one or two required parameters 'mcc' or 'mnc'"
+                    "destinationNetworks is missing one or two required parameters ('mcc' or 'mnc') or 'phoneNumber'"
                 )
 
         data = {
             "destinationNetworks": destinationNetworks,
             "resultsCallbackUrl": resultsCallbackUrl,
             "maxCallbackRetries": maxCallbackRetries,
             "testIdTextType": testIdTextType,
```

### Comparing `telq-0.1.2/PKG-INFO` & `telq-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: telq
-Version: 0.1.2
+Version: 1.3.0
 Summary: Python SDK for TelQ Telecom API
 Author: Tuvshinbayar Davaa
 Author-email: tuvshinbayar.davaa@telqtele.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
```

