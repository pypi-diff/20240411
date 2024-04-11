# Comparing `tmp/commonhealth_cloud_storage_client-1.0.2.tar.gz` & `tmp/commonhealth_cloud_storage_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonhealth_cloud_storage_client-1.0.2.tar", last modified: Sun Mar 31 12:56:30 2024, max compression
+gzip compressed data, was "commonhealth_cloud_storage_client-1.0.3.tar", last modified: Thu Apr 11 19:35:34 2024, max compression
```

## Comparing `commonhealth_cloud_storage_client-1.0.2.tar` & `commonhealth_cloud_storage_client-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-03-31 12:56:30.825598 commonhealth_cloud_storage_client-1.0.2/
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     1076 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.2/LICENSE
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7892 2024-03-31 12:56:30.825598 commonhealth_cloud_storage_client-1.0.2/PKG-INFO
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7187 2024-03-31 12:47:52.000000 commonhealth_cloud_storage_client-1.0.2/README.md
-drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-03-31 12:56:30.815597 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      220 2024-03-28 19:47:47.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/__init__.py
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)    13717 2024-03-31 12:48:36.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/client.py
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     3789 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/crypto.py
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      312 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/errors.py
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      699 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/jwt.py
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     4948 2024-03-28 19:47:47.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/sqlite_delegate.py
-drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-03-31 12:56:30.825598 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7892 2024-03-31 12:56:30.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/PKG-INFO
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      598 2024-03-31 12:56:30.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/SOURCES.txt
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)        1 2024-03-31 12:56:30.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/dependency_links.txt
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)       50 2024-03-31 12:56:30.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/requires.txt
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)       34 2024-03-31 12:56:30.000000 commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/top_level.txt
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      104 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.2/pyproject.toml
--rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      749 2024-03-31 12:56:30.825598 commonhealth_cloud_storage_client-1.0.2/setup.cfg
+drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-04-11 19:35:34.903317 commonhealth_cloud_storage_client-1.0.3/
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     1076 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.3/LICENSE
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7782 2024-04-11 19:35:34.903317 commonhealth_cloud_storage_client-1.0.3/PKG-INFO
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7077 2024-04-11 19:30:51.000000 commonhealth_cloud_storage_client-1.0.3/README.md
+drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-04-11 19:35:34.893317 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      220 2024-04-11 19:23:32.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/__init__.py
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)    13787 2024-04-11 19:28:29.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/client.py
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     3789 2024-04-11 19:23:32.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/crypto.py
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      312 2024-04-11 19:23:32.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/errors.py
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      699 2024-04-11 19:23:32.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/jwt.py
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     4948 2024-04-11 19:23:32.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/sqlite_delegate.py
+drwxr-xr-x   0 surfdoc   (1000) surfdoc   (1000)        0 2024-04-11 19:35:34.903317 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)     7782 2024-04-11 19:35:34.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/PKG-INFO
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      598 2024-04-11 19:35:34.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/SOURCES.txt
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)        1 2024-04-11 19:35:34.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/dependency_links.txt
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)       50 2024-04-11 19:35:34.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/requires.txt
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)       34 2024-04-11 19:35:34.000000 commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/top_level.txt
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      104 2024-02-28 21:22:01.000000 commonhealth_cloud_storage_client-1.0.3/pyproject.toml
+-rw-r--r--   0 surfdoc   (1000) surfdoc   (1000)      749 2024-04-11 19:35:34.903317 commonhealth_cloud_storage_client-1.0.3/setup.cfg
```

### Comparing `commonhealth_cloud_storage_client-1.0.2/LICENSE` & `commonhealth_cloud_storage_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `commonhealth_cloud_storage_client-1.0.2/PKG-INFO` & `commonhealth_cloud_storage_client-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: commonhealth_cloud_storage_client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Partner Client for CommonHealth Cloud Storage Service
 Home-page: https://github.com/the-commons-project/chcs-python-client
 Author: TheCommonsProjectFoundation
 Author-email: developers@commonhealth.org
 Project-URL: Bug Tracker, https://github.com/the-commons-project/chcs-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==42.0.4
-Requires-Dist: requests==2.31.0
-Requires-Dist: tink==1.9.0
+Requires-Dist: cryptography>=42.0.4
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tink>=1.9.0
 
 This is a lightweight Python client to interact with CommonHealth Cloud Storage Service. It requires Python 3.6+.
 
 # Installation
 
 You can use pip to install it like so: `pip install commonhealth-cloud-storage-client`
 
 It has dependencies on the following packages:
 
-    cryptography==42.0.4
-    PyJWT==2.8.0
-    requests==2.31.0
-    tink==1.9.0
+    cryptography>=42.0.4
+    PyJWT>=2.8.0
+    requests>=2.31.0
+    tink>=1.9.0
 
 # Configuration
 
 The client (represented by the class `CHClient`) requires parameters to be passed on initialization. They are:
 
 - _Partner Client ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Partner Client Secret_ -- a **secret** value issued by TCP to your organization. Store alongside any other secrets in your system. 
 - _Partner ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Delegate_ -- the client library requires a persistence layer. An object implementing an expected interface (a subclass of the `CHStorageDelegate` type) must be passed to the client. A default, SQlite-based implementation is included and provided through the `SQLiteDelegate` class. 
-- _CH Authorization Deeplink_ -- this is a CommonHealth URL. For production, this will be: `https://app.commonhealth.org/m/phr/cloud-sharing/authorize`; for dev it will be: `https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize`.
-- _Storage Service Host_ -- the URL to the TCP Storage Service. For dev, this is `chcs.tcpdev.org`
-- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Set to 443.  
-- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Set to "https". 
-- _Logging Enabled_ -- boolean indicating if logging is enabled 
+- _CH Authorization Deeplink_ -- this is a CommonHealth URL.
+- _Storage Service Host_ -- the URL to the TCP Storage Service.
+- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Default is `443`.(Optional) 
+- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Default is `https`.(Optional)
+- _Logging Enabled_ -- boolean indicating if logging is enabled. Default is `True`.(Optional)
 
 If you're using the provided SQLite-based delegate, through the `SQLiteDelegate` class, it requires some parameters as well:
 
 - _Path to DB file_ -- the path to where the DB file should be written to, including the name. The class will automatically create the DB file if it doesn't exist. 
 - _DB passphrase_ -- a **secret** value, ideally with high entropy, that's used to generate an encryption key to encrypt database contents under. 
 - _DB passphrase salt_ -- a **secret** value that's used to generate an encryption key using the passphrase. 
 - _(Optional) Logger_ -- an optional logger instance to use. If none provided, no logs will be emitted. 
@@ -72,18 +72,18 @@
 
 # create CHClient
 ch_client = CHClient(
     "5c1eeddd-81ca-45b9-901f-791184a6f57a", # Client ID, provided by TCP. Non-secret.
     "anothersecretvalue", # Client Secret, provided by TCP. Secret!
     "00e05764-bd84-4f11-9a4b-6f5c27f4519f", # Partner ID, provided by TCP. Non-secret.
     delegate,
-    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize",
-    "chcs.tcpdev.org",
-    443,
-    "https"
+    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize"(optional),
+    "chcs.tcpdev.org"(optional),
+    443(optional),
+    "https"(optional)
 )
 
 # you can now use the client...
 ```
 
 # Registering signing keys 
 
@@ -101,15 +101,15 @@
 # Generating a deeplink to share with a specific user 
 
 Each deeplink is specific to a given user and should not be re-used with other users. To generate a deeplink, call `construct_authorization_request_deeplink` with the following parameters. 
 
 - _Patient ID_ -- A stable identifier for a given patient. This can be a hash of an actual patient ID. 
 - _Scope_ -- The scope of data being requested as a string. Recommend the following to READ OpenMHealth BP and HR data: `OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read`.  
 - _Sharing duration seconds_ -- The number of seconds that the data is shared for. For now, put 2592000, or 30 days. 
-- _(Optional) Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. 
+- _Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. (Optional)
 
 A sample call:
 
 ```
 deeplink = ch_client.construct_authorization_request_deeplink(
     "patient123",
     "OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read",
```

### Comparing `commonhealth_cloud_storage_client-1.0.2/README.md` & `commonhealth_cloud_storage_client-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 # Installation
 
 You can use pip to install it like so: `pip install commonhealth-cloud-storage-client`
 
 It has dependencies on the following packages:
 
-    cryptography==42.0.4
-    PyJWT==2.8.0
-    requests==2.31.0
-    tink==1.9.0
+    cryptography>=42.0.4
+    PyJWT>=2.8.0
+    requests>=2.31.0
+    tink>=1.9.0
 
 # Configuration
 
 The client (represented by the class `CHClient`) requires parameters to be passed on initialization. They are:
 
 - _Partner Client ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Partner Client Secret_ -- a **secret** value issued by TCP to your organization. Store alongside any other secrets in your system. 
 - _Partner ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Delegate_ -- the client library requires a persistence layer. An object implementing an expected interface (a subclass of the `CHStorageDelegate` type) must be passed to the client. A default, SQlite-based implementation is included and provided through the `SQLiteDelegate` class. 
-- _CH Authorization Deeplink_ -- this is a CommonHealth URL. For production, this will be: `https://app.commonhealth.org/m/phr/cloud-sharing/authorize`; for dev it will be: `https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize`.
-- _Storage Service Host_ -- the URL to the TCP Storage Service. For dev, this is `chcs.tcpdev.org`
-- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Set to 443.  
-- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Set to "https". 
-- _Logging Enabled_ -- boolean indicating if logging is enabled 
+- _CH Authorization Deeplink_ -- this is a CommonHealth URL.
+- _Storage Service Host_ -- the URL to the TCP Storage Service.
+- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Default is `443`.(Optional) 
+- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Default is `https`.(Optional)
+- _Logging Enabled_ -- boolean indicating if logging is enabled. Default is `True`.(Optional)
 
 If you're using the provided SQLite-based delegate, through the `SQLiteDelegate` class, it requires some parameters as well:
 
 - _Path to DB file_ -- the path to where the DB file should be written to, including the name. The class will automatically create the DB file if it doesn't exist. 
 - _DB passphrase_ -- a **secret** value, ideally with high entropy, that's used to generate an encryption key to encrypt database contents under. 
 - _DB passphrase salt_ -- a **secret** value that's used to generate an encryption key using the passphrase. 
 - _(Optional) Logger_ -- an optional logger instance to use. If none provided, no logs will be emitted. 
@@ -54,18 +54,18 @@
 
 # create CHClient
 ch_client = CHClient(
     "5c1eeddd-81ca-45b9-901f-791184a6f57a", # Client ID, provided by TCP. Non-secret.
     "anothersecretvalue", # Client Secret, provided by TCP. Secret!
     "00e05764-bd84-4f11-9a4b-6f5c27f4519f", # Partner ID, provided by TCP. Non-secret.
     delegate,
-    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize",
-    "chcs.tcpdev.org",
-    443,
-    "https"
+    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize"(optional),
+    "chcs.tcpdev.org"(optional),
+    443(optional),
+    "https"(optional)
 )
 
 # you can now use the client...
 ```
 
 # Registering signing keys 
 
@@ -83,15 +83,15 @@
 # Generating a deeplink to share with a specific user 
 
 Each deeplink is specific to a given user and should not be re-used with other users. To generate a deeplink, call `construct_authorization_request_deeplink` with the following parameters. 
 
 - _Patient ID_ -- A stable identifier for a given patient. This can be a hash of an actual patient ID. 
 - _Scope_ -- The scope of data being requested as a string. Recommend the following to READ OpenMHealth BP and HR data: `OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read`.  
 - _Sharing duration seconds_ -- The number of seconds that the data is shared for. For now, put 2592000, or 30 days. 
-- _(Optional) Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. 
+- _Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. (Optional)
 
 A sample call:
 
 ```
 deeplink = ch_client.construct_authorization_request_deeplink(
     "patient123",
     "OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read",
```

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/client.py` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.partner_id = partner_id
         self.storage_delegate = storage_delegate
         self.ch_authorization_deeplink = ch_authorization_deeplink
         self.ch_host = ch_host
-        self.ch_port = ch_port
-        self.ch_scheme = ch_scheme
+        self.ch_port = ch_port if ch_port is not None else 443
+        self.ch_scheme = ch_scheme if ch_scheme is not None else "https"
         self.logging_enabled = logging_enabled
 
     @property
     def _host_with_port(self):
         return f'{self.ch_host}:{self.ch_port}'
 
     @property
```

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/crypto.py` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/crypto.py`

 * *Files identical despite different names*

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/jwt.py` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/jwt.py`

 * *Files identical despite different names*

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client/sqlite_delegate.py` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client/sqlite_delegate.py`

 * *Files identical despite different names*

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/PKG-INFO` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 Metadata-Version: 2.1
 Name: commonhealth_cloud_storage_client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Partner Client for CommonHealth Cloud Storage Service
 Home-page: https://github.com/the-commons-project/chcs-python-client
 Author: TheCommonsProjectFoundation
 Author-email: developers@commonhealth.org
 Project-URL: Bug Tracker, https://github.com/the-commons-project/chcs-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cryptography==42.0.4
-Requires-Dist: requests==2.31.0
-Requires-Dist: tink==1.9.0
+Requires-Dist: cryptography>=42.0.4
+Requires-Dist: requests>=2.31.0
+Requires-Dist: tink>=1.9.0
 
 This is a lightweight Python client to interact with CommonHealth Cloud Storage Service. It requires Python 3.6+.
 
 # Installation
 
 You can use pip to install it like so: `pip install commonhealth-cloud-storage-client`
 
 It has dependencies on the following packages:
 
-    cryptography==42.0.4
-    PyJWT==2.8.0
-    requests==2.31.0
-    tink==1.9.0
+    cryptography>=42.0.4
+    PyJWT>=2.8.0
+    requests>=2.31.0
+    tink>=1.9.0
 
 # Configuration
 
 The client (represented by the class `CHClient`) requires parameters to be passed on initialization. They are:
 
 - _Partner Client ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Partner Client Secret_ -- a **secret** value issued by TCP to your organization. Store alongside any other secrets in your system. 
 - _Partner ID_ -- a UUID issued by TCP to your organization. This is not secret. 
 - _Delegate_ -- the client library requires a persistence layer. An object implementing an expected interface (a subclass of the `CHStorageDelegate` type) must be passed to the client. A default, SQlite-based implementation is included and provided through the `SQLiteDelegate` class. 
-- _CH Authorization Deeplink_ -- this is a CommonHealth URL. For production, this will be: `https://app.commonhealth.org/m/phr/cloud-sharing/authorize`; for dev it will be: `https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize`.
-- _Storage Service Host_ -- the URL to the TCP Storage Service. For dev, this is `chcs.tcpdev.org`
-- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Set to 443.  
-- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Set to "https". 
-- _Logging Enabled_ -- boolean indicating if logging is enabled 
+- _CH Authorization Deeplink_ -- this is a CommonHealth URL.
+- _Storage Service Host_ -- the URL to the TCP Storage Service.
+- _Storage Service Port_ -- the port over which to connect to the TCP Storage Service. Default is `443`.(Optional) 
+- _Storage Service Scheme_ -- the connection scheme for HTTP connections to the TCP Storage Service. Default is `https`.(Optional)
+- _Logging Enabled_ -- boolean indicating if logging is enabled. Default is `True`.(Optional)
 
 If you're using the provided SQLite-based delegate, through the `SQLiteDelegate` class, it requires some parameters as well:
 
 - _Path to DB file_ -- the path to where the DB file should be written to, including the name. The class will automatically create the DB file if it doesn't exist. 
 - _DB passphrase_ -- a **secret** value, ideally with high entropy, that's used to generate an encryption key to encrypt database contents under. 
 - _DB passphrase salt_ -- a **secret** value that's used to generate an encryption key using the passphrase. 
 - _(Optional) Logger_ -- an optional logger instance to use. If none provided, no logs will be emitted. 
@@ -72,18 +72,18 @@
 
 # create CHClient
 ch_client = CHClient(
     "5c1eeddd-81ca-45b9-901f-791184a6f57a", # Client ID, provided by TCP. Non-secret.
     "anothersecretvalue", # Client Secret, provided by TCP. Secret!
     "00e05764-bd84-4f11-9a4b-6f5c27f4519f", # Partner ID, provided by TCP. Non-secret.
     delegate,
-    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize",
-    "chcs.tcpdev.org",
-    443,
-    "https"
+    "https://appdev.tcpdev.org/m/phr/cloud-sharing/authorize"(optional),
+    "chcs.tcpdev.org"(optional),
+    443(optional),
+    "https"(optional)
 )
 
 # you can now use the client...
 ```
 
 # Registering signing keys 
 
@@ -101,15 +101,15 @@
 # Generating a deeplink to share with a specific user 
 
 Each deeplink is specific to a given user and should not be re-used with other users. To generate a deeplink, call `construct_authorization_request_deeplink` with the following parameters. 
 
 - _Patient ID_ -- A stable identifier for a given patient. This can be a hash of an actual patient ID. 
 - _Scope_ -- The scope of data being requested as a string. Recommend the following to READ OpenMHealth BP and HR data: `OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read`.  
 - _Sharing duration seconds_ -- The number of seconds that the data is shared for. For now, put 2592000, or 30 days. 
-- _(Optional) Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. 
+- _Rotate encryption key_ -- Useful for testing, but recommend setting as `false`. (Optional)
 
 A sample call:
 
 ```
 deeplink = ch_client.construct_authorization_request_deeplink(
     "patient123",
     "OMHealthResource.HeartRate.Read OMHealthResource.BloodPressure.Read",
```

### Comparing `commonhealth_cloud_storage_client-1.0.2/commonhealth_cloud_storage_client.egg-info/SOURCES.txt` & `commonhealth_cloud_storage_client-1.0.3/commonhealth_cloud_storage_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonhealth_cloud_storage_client-1.0.2/setup.cfg` & `commonhealth_cloud_storage_client-1.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commonhealth_cloud_storage_client
-version = 1.0.2
+version = 1.0.3
 author = TheCommonsProjectFoundation
 author_email = developers@commonhealth.org
 description = Partner Client for CommonHealth Cloud Storage Service
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/the-commons-project/chcs-python-client
 project_urls = 
@@ -13,16 +13,16 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 install_requires = 
-	cryptography==42.0.4
-	requests==2.31.0
-	tink==1.9.0
+	cryptography>=42.0.4
+	requests>=2.31.0
+	tink>=1.9.0
 python_requires = >=3.6
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

