# Comparing `tmp/vector_vault-4.4.2.tar.gz` & `tmp/vector_vault-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.2.tar", last modified: Wed Apr 10 23:20:13 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.tar", last modified: Thu Apr 11 17:18:31 2024, max compression
```

## Comparing `vector_vault-4.4.2.tar` & `vector_vault-4.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-10 23:20:13.484107 vector_vault-4.4.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-10 23:20:13.483965 vector_vault-4.4.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-10 23:20:13.484143 vector_vault-4.4.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-10 23:20:05.000000 vector_vault-4.4.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-10 23:20:13.481092 vector_vault-4.4.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-10 23:20:13.000000 vector_vault-4.4.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-10 23:20:13.000000 vector_vault-4.4.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-10 23:20:13.000000 vector_vault-4.4.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-10 23:20:13.000000 vector_vault-4.4.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-10 23:20:13.000000 vector_vault-4.4.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-10 23:20:13.483796 vector_vault-4.4.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.2/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5996 2024-04-08 20:07:11.000000 vector_vault-4.4.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.4.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-08 20:07:01.000000 vector_vault-4.4.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-10 23:19:06.000000 vector_vault-4.4.2/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62968 2024-04-09 00:50:55.000000 vector_vault-4.4.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.689371 vector_vault-4.4.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-11 17:18:31.689211 vector_vault-4.4.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 17:18:31.689408 vector_vault-4.4.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-11 17:18:23.000000 vector_vault-4.4.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.684867 vector_vault-4.4.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.688820 vector_vault-4.4.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1882 2024-04-11 17:16:38.000000 vector_vault-4.4.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62968 2024-04-11 17:17:59.000000 vector_vault-4.4.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.2/LICENSE` & `vector_vault-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/PKG-INFO` & `vector_vault-4.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.2
+Version: 4.4.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.2/README.md` & `vector_vault-4.4.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/setup.py` & `vector_vault-4.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.2",
+    version="4.4.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.2
+Version: 4.4.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.2/vectorvault/ai.py` & `vector_vault-4.4.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/cloud_api.py` & `vector_vault-4.4.3/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/cloudmanager.py` & `vector_vault-4.4.3/vectorvault/cloudmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.user = user
         self.api = api_key
         self.vault = vault
         # Create credentials
         self.credentials = CustomCredentials(user, self.api)
         # Instantiate the client 
         self.storage_client = storage.Client(project=call_proj(), credentials=self.credentials)
-        self.username = self.username(self.user)
+        self.username = self.username(user)
         self.cloud = self.storage_client.bucket(self.username)
         self.cloud_name = cloud_name
         self.req_count = 0 
 
     def vault_exists(self, vault_name):
         return storage.Blob(bucket=self.cloud, name=vault_name).exists(self.storage_client)
```

### Comparing `vector_vault-4.4.2/vectorvault/creds.py` & `vector_vault-4.4.3/vectorvault/creds.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # patents in process, and are protected by trade secret or copyright law.
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault. See license for consent.
 
 from google.auth.credentials import Credentials
 import requests
+import time
 import datetime
 
 class CustomCredentials(Credentials):
     def __init__(self, user, api):
         self.user = user
         self.api = api
         self.token = None
@@ -28,15 +29,15 @@
     def apply(self, headers, token=None):
         headers["Authorization"] = f"Bearer {self.token}"
 
     @property
     def valid(self):
         if self.expiry is None:
             return False
-        return datetime.datetime.utcnow() < self.expiry
+        return time.gmtime() < self.expiry
 
     def refresh(self, request):
         if not self.valid:
             data = {
                 "user_id": self.user,
                 "api_key": self.api,
             }
```

### Comparing `vector_vault-4.4.2/vectorvault/download.py` & `vector_vault-4.4.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/itemize.py` & `vector_vault-4.4.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/tools_gpt.py` & `vector_vault-4.4.3/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/vault.py` & `vector_vault-4.4.3/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.2/vectorvault/vecreq.py` & `vector_vault-4.4.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

