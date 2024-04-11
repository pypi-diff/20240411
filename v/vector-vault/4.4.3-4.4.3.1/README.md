# Comparing `tmp/vector_vault-4.4.3.tar.gz` & `tmp/vector_vault-4.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.3.tar", last modified: Thu Apr 11 17:18:31 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.1.tar", last modified: Thu Apr 11 17:26:48 2024, max compression
```

## Comparing `vector_vault-4.4.3.tar` & `vector_vault-4.4.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.689371 vector_vault-4.4.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-11 17:18:31.689211 vector_vault-4.4.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 17:18:31.689408 vector_vault-4.4.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-11 17:18:23.000000 vector_vault-4.4.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.684867 vector_vault-4.4.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 17:18:31.000000 vector_vault-4.4.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:18:31.688820 vector_vault-4.4.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1882 2024-04-11 17:16:38.000000 vector_vault-4.4.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62968 2024-04-11 17:17:59.000000 vector_vault-4.4.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:26:48.232055 vector_vault-4.4.3.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 17:26:48.231909 vector_vault-4.4.3.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 17:26:48.232088 vector_vault-4.4.3.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 17:26:44.000000 vector_vault-4.4.3.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:26:48.228619 vector_vault-4.4.3.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 17:26:48.000000 vector_vault-4.4.3.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 17:26:48.000000 vector_vault-4.4.3.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 17:26:48.000000 vector_vault-4.4.3.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 17:26:48.000000 vector_vault-4.4.3.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 17:26:48.000000 vector_vault-4.4.3.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 17:26:48.231564 vector_vault-4.4.3.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.1/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1882 2024-04-11 17:16:38.000000 vector_vault-4.4.3.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.1/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62970 2024-04-11 17:26:28.000000 vector_vault-4.4.3.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.1/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.3/LICENSE` & `vector_vault-4.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/PKG-INFO` & `vector_vault-4.4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.3
+Version: 4.4.3.1
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3/README.md` & `vector_vault-4.4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/setup.py` & `vector_vault-4.4.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.3",
+    version="4.4.3.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3.1/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.3
+Version: 4.4.3.1
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3/vectorvault/ai.py` & `vector_vault-4.4.3.1/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/cloud_api.py` & `vector_vault-4.4.3.1/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/cloudmanager.py` & `vector_vault-4.4.3.1/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/creds.py` & `vector_vault-4.4.3.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/download.py` & `vector_vault-4.4.3.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/itemize.py` & `vector_vault-4.4.3.1/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/tools_gpt.py` & `vector_vault-4.4.3.1/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3/vectorvault/vault.py` & `vector_vault-4.4.3.1/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,15 +725,15 @@
 
 
     def get_similar_local(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
         '''
             Returns similar items from the Vault as the one you entered, but locally
             (saves a few milliseconds and is sometimes used on production builds)
         '''
-        self.cloud_manager.update() if not self.cuid else None
+        # self.cloud_manager.update() if not self.cuid else None
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
         return self.get_items_by_vector(vector, n, include_distances = include_distances, vault = vault if vault else self.vault)
     
 
     def get_similar(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
         '''
             Returns similar items from the Vault as the text you enter.
```

### Comparing `vector_vault-4.4.3/vectorvault/vecreq.py` & `vector_vault-4.4.3.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

