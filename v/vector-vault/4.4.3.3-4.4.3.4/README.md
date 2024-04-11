# Comparing `tmp/vector_vault-4.4.3.3.tar.gz` & `tmp/vector_vault-4.4.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.3.3.tar", last modified: Thu Apr 11 18:23:23 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.4.tar", last modified: Thu Apr 11 18:44:29 2024, max compression
```

## Comparing `vector_vault-4.4.3.3.tar` & `vector_vault-4.4.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.698822 vector_vault-4.4.3.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:23:23.698516 vector_vault-4.4.3.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 18:23:23.698898 vector_vault-4.4.3.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 18:23:08.000000 vector_vault-4.4.3.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.695154 vector_vault-4.4.3.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.698341 vector_vault-4.4.3.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.3/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.3/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62777 2024-04-11 18:23:01.000000 vector_vault-4.4.3.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:44:29.658571 vector_vault-4.4.3.4/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.4/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:44:29.658420 vector_vault-4.4.3.4/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.4/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 18:44:29.658609 vector_vault-4.4.3.4/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 18:44:19.000000 vector_vault-4.4.3.4/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:44:29.654957 vector_vault-4.4.3.4/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:44:29.000000 vector_vault-4.4.3.4/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 18:44:29.000000 vector_vault-4.4.3.4/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 18:44:29.000000 vector_vault-4.4.3.4/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 18:44:29.000000 vector_vault-4.4.3.4/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 18:44:29.000000 vector_vault-4.4.3.4/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:44:29.658241 vector_vault-4.4.3.4/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.4/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.4/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.4/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3.4/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.4/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.4/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.4/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.4/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62664 2024-04-11 18:44:14.000000 vector_vault-4.4.3.4/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.4/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.4/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.3.3/LICENSE` & `vector_vault-4.4.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/PKG-INFO` & `vector_vault-4.4.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.3.3
+Version: 4.4.3.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.3/README.md` & `vector_vault-4.4.3.4/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/setup.py` & `vector_vault-4.4.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.3.3",
+    version="4.4.3.4",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.3.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3.4/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.3.3
+Version: 4.4.3.4
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.3/vectorvault/ai.py` & `vector_vault-4.4.3.4/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/cloud_api.py` & `vector_vault-4.4.3.4/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/cloudmanager.py` & `vector_vault-4.4.3.4/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/creds.py` & `vector_vault-4.4.3.4/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/download.py` & `vector_vault-4.4.3.4/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/itemize.py` & `vector_vault-4.4.3.4/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/tools_gpt.py` & `vector_vault-4.4.3.4/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.3/vectorvault/vault.py` & `vector_vault-4.4.3.4/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,44 +74,38 @@
         '''
         self.user = user.lower()
         self.vault = vault.strip() if vault else 'home'
         self.api = api_key
         self.verbose = verbose
         self.embeddings_model = embeddings_model if embeddings_model else 'text-embedding-3-small'
         self.dims = 1536 if embeddings_model != 'text-embedding-3-large' else 3072
-        t = T(target=self.connect_to_cloud)
-        t.start()
         if openai_key:
             self.openai_key = openai_key
             openai.api_key = self.openai_key
+        try:
+            self.cloud_manager = CloudManager(self.user, self.api, self.vault)
+            if self.verbose:
+                print(f'Connected vault: {self.vault}')
+        except Exception as e:
+            print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work', e)
+            # user can still use the get_chat() function without an api key
+            self.cloud_manager = None
         self.vectors = get_vectors(self.dims)
         self.x = 0
         self.x_checked = False
         self.x_loaded_checked = False
         self.vecs_loaded = False
         self.map = {}
         self.items = []
         self.last_time = None
         self.saved_already = False
         self.ai_loaded = False
         self.tools = ToolsGPT(verbose=verbose)
         self.rate_limiter = RateLimiter(max_attempts=30)
         self.cuid = conversation_user_id
-        t.join()
-
-    def connect_to_cloud(self):
-        try:
-            self.cloud_manager = CloudManager(self.user, self.api, self.vault)
-            if self.verbose:
-                print(f'Connected vault: {self.vault}')
-        except Exception as e:
-            print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work', e)
-            # user can still use the get_chat() function without an api key
-            self.cloud_manager = None
-
 
     def get_vaults(self, vault: str = None):
         '''
             Returns a list of vaults within the current vault directory 
         '''
         vault = self.vault if vault is None else vault
         if self.cloud_manager is None:
```

### Comparing `vector_vault-4.4.3.3/vectorvault/vecreq.py` & `vector_vault-4.4.3.4/vectorvault/vecreq.py`

 * *Files identical despite different names*

