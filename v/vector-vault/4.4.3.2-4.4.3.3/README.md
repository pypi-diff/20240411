# Comparing `tmp/vector_vault-4.4.3.2.tar.gz` & `tmp/vector_vault-4.4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.3.2.tar", last modified: Thu Apr 11 18:03:33 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.3.tar", last modified: Thu Apr 11 18:23:23 2024, max compression
```

## Comparing `vector_vault-4.4.3.2.tar` & `vector_vault-4.4.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:03:33.666542 vector_vault-4.4.3.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:03:33.666263 vector_vault-4.4.3.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 18:03:33.666613 vector_vault-4.4.3.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 18:03:06.000000 vector_vault-4.4.3.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:03:33.662843 vector_vault-4.4.3.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:03:33.000000 vector_vault-4.4.3.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 18:03:33.000000 vector_vault-4.4.3.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 18:03:33.000000 vector_vault-4.4.3.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 18:03:33.000000 vector_vault-4.4.3.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 18:03:33.000000 vector_vault-4.4.3.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:03:33.665897 vector_vault-4.4.3.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.2/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.2/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    63126 2024-04-11 18:03:23.000000 vector_vault-4.4.3.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.698822 vector_vault-4.4.3.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:23:23.698516 vector_vault-4.4.3.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 18:23:23.698898 vector_vault-4.4.3.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 18:23:08.000000 vector_vault-4.4.3.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.695154 vector_vault-4.4.3.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 18:23:23.000000 vector_vault-4.4.3.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 18:23:23.698341 vector_vault-4.4.3.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.3/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5991 2024-04-11 17:18:18.000000 vector_vault-4.4.3.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.3/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62777 2024-04-11 18:23:01.000000 vector_vault-4.4.3.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.3/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.3.2/LICENSE` & `vector_vault-4.4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/PKG-INFO` & `vector_vault-4.4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.3.2
+Version: 4.4.3.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.2/README.md` & `vector_vault-4.4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/setup.py` & `vector_vault-4.4.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.3.2",
+    version="4.4.3.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.3.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.3.2
+Version: 4.4.3.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.2/vectorvault/ai.py` & `vector_vault-4.4.3.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/cloud_api.py` & `vector_vault-4.4.3.3/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/cloudmanager.py` & `vector_vault-4.4.3.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/creds.py` & `vector_vault-4.4.3.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/download.py` & `vector_vault-4.4.3.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/itemize.py` & `vector_vault-4.4.3.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/tools_gpt.py` & `vector_vault-4.4.3.3/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.2/vectorvault/vault.py` & `vector_vault-4.4.3.3/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,30 +222,31 @@
 
 
     def save(self, trees: int = 10, vault = None):
         '''
             Saves all the data added locally to the Cloud. All Vault references are Cloud references.
             To add data to your Vault and access it later, you must first call add(), then get_vectors(), and finally save().
         '''
+        vault = vault if vault else self.vault
         if self.saved_already:
             self.clear_cache()
             print("The last save was aborted before the build process finished. Clearing cache to start again...")
         self.saved_already = True # Make sure the if the save process is interrupted, data will not get corrupted
         start_time = time.time()
         self.vectors.build(trees)
 
         total_saved_items = 0
 
         with ThreadPoolExecutor() as executor:
             for item in self.items:
                 item_text, item_id, item_meta = get_item(item)
-                executor.submit(self.cloud_manager.upload, self.map.get(str(item_id)), item_text, item_meta, vault = vault if vault else self.vault)
+                executor.submit(self.cloud_manager.upload, self.map.get(str(item_id)), item_text, item_meta, vault)
                 total_saved_items += 1
 
-        self.upload_vectors(vault if vault else self.vault)
+        self.upload_vectors(vault)
         print(f"upload time --- {(time.time() - start_time)} seconds --- {total_saved_items} items saved") if self.verbose else 0
             
 
     def clear_cache(self):
         '''
             Clears the cache for all the loaded items 
         '''
@@ -674,124 +675,122 @@
                 results[index] = result  # Insert each result at its corresponding index
             
         print(f"Retrieved {len(ids)} items --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
         
         return results
 
 
-    def get_items_by_vector(self, vector: list, n: int = 4, include_distances: bool = False, vault = None) -> list:
+    
+    def get_items_by_vector(self, vector: list, n: int = 4, include_distances: bool = False):
         '''
             Internal function that returns vector similar items. Requires input vector, returns similar items
         '''
         try:
-            vault = vault if vault else self.vault 
-            self.load_vectors(vault) if not self.vecs_loaded else None
+            self.load_vectors()
             start_time = time.time()
             if not include_distances:
                 vecs = self.vectors.get_nns_by_vector(vector, n)
                 results = [None] * len(vecs)  # Pre-fill the results list with placeholders
 
                 def fetch_item(index, vec):
                     # Function to fetch a single item, to be run in parallel
-                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, item=True))
-                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, meta=True))
+                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, item=True))
+                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, meta=True))
                     meta = json.loads(meta_data)
                     return index, build_return(item_data, meta)
                 
                 with ThreadPoolExecutor() as executor:
                     futures = [executor.submit(fetch_item, i, vec) for i, vec in enumerate(vecs)]
                     for future in as_completed(futures):
                         index, result = future.result()
                         results[index] = result  # Insert each result at its corresponding index
 
-                print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
-                   
+                if self.verbose:
+                    print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
                 return results
             else:
                 vecs, distances = self.vectors.get_nns_by_vector(vector, n, include_distances=include_distances)
                 results = [None] * len(vecs)  # Pre-fill the results list with placeholders
 
                 def fetch_item(index, vec, distance):
                     # Function to fetch a single item, to be run in parallel
-                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, item=True))
-                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, meta=True))
+                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, item=True))
+                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, meta=True))
                     meta = json.loads(meta_data)
                     return index, build_return(item_data, meta, distance)
 
                 with ThreadPoolExecutor() as executor:
                     futures = [executor.submit(fetch_item, i, vec, distances[i]) for i, vec in enumerate(vecs)]
                     for future in as_completed(futures):
                         index, result = future.result()
                         results[index] = result  # Insert each result at its corresponding index
 
-                print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))if self.verbose else 0
-                   
+                if self.verbose:
+                    print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))
                 return results
         except:
             return [{'data': 'No data has been added', 'metadata': {'no meta': 'No metadata has been added'}}]
 
 
-    def get_similar_local(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
+    def get_similar_local(self, text: str, n: int = 4, include_distances: bool = False):
         '''
             Returns similar items from the Vault as the one you entered, but locally
             (saves a few milliseconds and is sometimes used on production builds)
         '''
         # self.cloud_manager.update() if not self.cuid else None
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return self.get_items_by_vector(vector, n, include_distances = include_distances, vault = vault if vault else self.vault)
+        return self.get_items_by_vector(vector, n, include_distances = include_distances)
     
 
     def get_similar(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
         '''
             Returns similar items from the Vault as the text you enter.
 
             Param `include_distances = True` adds the "distance" field to the return.
             The distance can be useful for assessing similarity differences in the items returned. 
             Each item has its' own distance number, and this changes the structure of the output.
         '''
         return call_get_similar(self.user, vault if vault else self.vault, self.api, self.openai_key, text, n, include_distances=include_distances, verbose=self.verbose)
 
 
-    def add_item(self, text: str, meta: dict = None, name: str = None, vault = None):
+    def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         self.check_index()
-        new_item = itemize(vault if vault else self.vault, self.x, meta, text, name)
+        new_item = itemize(self.vault, self.x, meta, text, name)
         self.items.append(new_item)
         self.add_to_map()
 
-
-    def add(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000, vault = None):
+    def add(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000):
         """
             If your text length is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
         self.check_index()
 
         if len(text) > 15000 or split:
-            print('Using the built-in "split_text()" function to get a list of texts') if self.verbose else 0 
-                
+            if self.verbose:
+                print('Using the built-in "split_text()" function to get a list of texts') 
             texts = self.split_text(text, min_threshold=split_size, max_threshold=max_threshold) # returns list of text segments
         else:
             texts = [text]
         for text in texts:
-            self.add_item(text, meta, name, vault if vault else self.vault)
-
+            self.add_item(text, meta, name)
 
-    def add_n_save(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000, vault = None):
+    def add_n_save(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000):
         """
             Adds data, gets vectors, then saves the data to the cloud in one call
             If your text length is greater than 4000 tokens, your text will automatically be split by
             Vault.split_text(your_text).
         """
-        self.add(text=text, meta=meta, name=name, split=split, split_size=split_size, max_threshold=max_threshold, vault=vault if vault else self.vault)
+        self.add(text=text, meta=meta, name=name, split=split, split_size=split_size, max_threshold=max_threshold)
         self.get_vectors()
-        self.save(vault = vault if vault else self.vault)
+        self.save()
         T(target=self.clear_cache).start()
 
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
             If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
@@ -1309,15 +1308,15 @@
                 return []
 
         def golden_retriever(metadata_list): 
             one_hour_ago = datetime.now() - timedelta(hours=1)
             return [metadata['M'] for metadata in reversed(metadata_list) if datetime.fromtimestamp(float(metadata['M'])) >= one_hour_ago]
 
         def vector_search_conversation_history(message):
-            return self.get_similar_local(message, vault=f'{self.vault}/user_history/{conversation_id}/vectors')
+            return self.get_similar(message, vault=f'{self.vault}/user_history/{conversation_id}/vectors')
 
         try:
             meta = download_conversation_metadata()
         except:
             meta = None
 
         message_ids = golden_retriever(meta) if meta != None else []
```

### Comparing `vector_vault-4.4.3.2/vectorvault/vecreq.py` & `vector_vault-4.4.3.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

