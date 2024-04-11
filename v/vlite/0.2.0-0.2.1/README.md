# Comparing `tmp/vlite-0.2.0.tar.gz` & `tmp/vlite-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.2.0.tar", last modified: Fri Apr  5 11:56:22 2024, max compression
+gzip compressed data, was "vlite-0.2.1.tar", last modified: Thu Apr 11 04:25:00 2024, max compression
```

## Comparing `vlite-0.2.0.tar` & `vlite-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.415560 vlite-0.2.0/
--rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.0/LICENSE
--rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-05 11:56:22.415428 vlite-0.2.0/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     2635 2024-04-05 11:47:06.000000 vlite-0.2.0/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-05 11:56:22.415604 vlite-0.2.0/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)      558 2024-04-05 11:54:26.000000 vlite-0.2.0/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.414493 vlite-0.2.0/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       80 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     8527 2024-04-05 10:47:15.000000 vlite-0.2.0/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     1799 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     6650 2024-04-05 10:43:40.000000 vlite-0.2.0/vlite/omom.py
--rw-r--r--   0 sdan       (501) staff       (20)     7747 2024-04-03 19:37:27.000000 vlite-0.2.0/vlite/server.py
--rw-r--r--   0 sdan       (501) staff       (20)     7687 2024-04-05 11:37:40.000000 vlite-0.2.0/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-05 11:56:22.415262 vlite-0.2.0/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      262 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)      118 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-05 11:56:22.000000 vlite-0.2.0/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.230357 vlite-0.2.1/
+-rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.1/LICENSE
+-rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-11 04:25:00.230217 vlite-0.2.1/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     2635 2024-04-05 11:47:06.000000 vlite-0.2.1/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-11 04:25:00.230404 vlite-0.2.1/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)      558 2024-04-11 04:24:38.000000 vlite-0.2.1/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.229364 vlite-0.2.1/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       80 2024-04-11 04:24:48.000000 vlite-0.2.1/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     6915 2024-04-11 03:44:32.000000 vlite-0.2.1/vlite/ctx.py
+-rw-r--r--   0 sdan       (501) staff       (20)    10160 2024-04-11 04:17:33.000000 vlite-0.2.1/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     3156 2024-04-11 02:57:53.000000 vlite-0.2.1/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7747 2024-04-11 04:24:51.000000 vlite-0.2.1/vlite/server.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7733 2024-04-11 04:23:32.000000 vlite-0.2.1/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-11 04:25:00.230027 vlite-0.2.1/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      218 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      261 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)      118 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-11 04:25:00.000000 vlite-0.2.1/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.2.0/LICENSE` & `vlite-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vlite-0.2.0/README.md` & `vlite-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vlite-0.2.0/setup.py` & `vlite-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vlite',
-    version='0.2.0',
+    version='0.2.1',
     author='Surya Dantuluri',
     author_email='surya@suryad.com',
     description='A simple vector database that stores vectors in a numpy array.',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'PyPDF2',
```

### Comparing `vlite-0.2.0/vlite/main.py` & `vlite-0.2.1/vlite/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,215 +1,247 @@
 import numpy as np
 from uuid import uuid4
 from .model import EmbeddingModel
 from .utils import chop_and_chunk
 import datetime
-from .omom import Omom
+from .ctx import Ctx
 
 class VLite:
     def __init__(self, collection=None, device='cpu', model_name='mixedbread-ai/mxbai-embed-large-v1'):
         if collection is None:
             current_datetime = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
             collection = f"vlite_{current_datetime}"
         self.collection = f"{collection}"
         self.device = device
         self.model = EmbeddingModel(model_name) if model_name else EmbeddingModel()
         
-        self.omom = Omom()
+        self.ctx = Ctx()
         self.index = {}
 
         try:
-            with self.omom.read(collection) as omom_file:
-                self.index = {
-                    chunk_id: {
-                        'text': chunk_data['text'],
-                        'metadata': chunk_data['metadata'],
-                        'binary_vector': np.array(chunk_data['binary_vector'])
-                    }
-                    for chunk_id, chunk_data in omom_file.metadata.items()
+            ctx_file = self.ctx.read(collection)
+            ctx_file.load()
+            # debug print
+            print("Number of embeddings: ", len(ctx_file.embeddings))
+            print("Number of metadata: ", len(ctx_file.metadata))
+            self.index = {
+                chunk_id: {
+                    'text': ctx_file.contexts[idx] if idx < len(ctx_file.contexts) else "",
+                    'metadata': ctx_file.metadata.get(chunk_id, {}),
+                    'binary_vector': np.array(ctx_file.embeddings[idx]) if idx < len(ctx_file.embeddings) else np.zeros(self.model.embedding_size)
                 }
+                for idx, chunk_id in enumerate(ctx_file.metadata.keys())
+            }
         except FileNotFoundError:
             print(f"Collection file {self.collection} not found. Initializing empty attributes.")
 
-    def add(self, data, metadata=None, need_chunks=True, fast=True):
-        print("Adding text to the collection...", self.collection)
+    def add(self, data, metadata=None, item_id=None, need_chunks=True, fast=True):
         data = [data] if not isinstance(data, list) else data
         results = []
         all_chunks = []
         all_metadata = []
         all_ids = []
 
         for item in data:
             if isinstance(item, dict):
                 text_content = item['text']
                 item_metadata = item.get('metadata', {})
-                item_id = item_metadata.get('id', str(uuid4()))
             else:
                 text_content = item
                 item_metadata = {}
+
+            if item_id is None:
                 item_id = str(uuid4())
 
             item_metadata.update(metadata or {})
-            item_metadata['id'] = item_id
 
             if need_chunks:
                 chunks = chop_and_chunk(text_content, fast=fast)
             else:
                 chunks = [text_content]
                 print("Encoding text... not chunking")
 
             all_chunks.extend(chunks)
             all_metadata.extend([item_metadata] * len(chunks))
             all_ids.extend([item_id] * len(chunks))
 
         encoded_data = self.model.embed(all_chunks, device=self.device)
         binary_encoded_data = self.model.quantize(encoded_data, precision="binary")
-        
-        for idx, (chunk, binary_vector, metadata, item_id) in enumerate(zip(all_chunks, binary_encoded_data, all_metadata, all_ids)):
+
+        for idx, (chunk, binary_vector, metadata) in enumerate(zip(all_chunks, binary_encoded_data, all_metadata)):
             chunk_id = f"{item_id}_{idx}"
             self.index[chunk_id] = {
                 'text': chunk,
                 'metadata': metadata,
                 'binary_vector': binary_vector.tolist()
             }
 
-            if item_id not in [result[0] for result in results]:
-                results.append((item_id, binary_encoded_data, metadata))
+        if item_id not in [result[0] for result in results]:
+            results.append((item_id, binary_encoded_data, metadata))
 
         self.save()
         print("Text added successfully.")
         return results
 
-    def retrieve(self, text=None, top_k=5, metadata=None):
+    def retrieve(self, text=None, top_k=5, metadata=None, return_scores=False):
         print("Retrieving similar texts...")
         if text:
             print(f"Retrieving top {top_k} similar texts for query: {text}")
             query_chunks = chop_and_chunk(text, fast=True)
             query_vectors = self.model.embed(query_chunks, device=self.device)
             query_binary_vectors = self.model.quantize(query_vectors, precision="binary")
-
+            
             results = []
             for query_binary_vector in query_binary_vectors:
                 chunk_results = self.search(query_binary_vector, top_k, metadata)
                 results.extend(chunk_results)
-
+            
             results.sort(key=lambda x: x[1], reverse=True)
             results = results[:top_k]
-
+            
             print("Retrieval completed.")
-            return [(self.index[idx]['text'], score, self.index[idx]['metadata']) for idx, score in results]
+            if return_scores:
+                return [(self.index[idx]['text'], score, self.index[idx]['metadata']) for idx, score in results]
+            else:
+                return [(self.index[idx]['text'], self.index[idx]['metadata']) for idx, _ in results]
         
     def search(self, query_binary_vector, top_k, metadata=None):
         # Reshape query_binary_vector to 1D array
         query_binary_vector = query_binary_vector.reshape(-1)
 
         # Perform binary search
         binary_vectors = np.array([item['binary_vector'] for item in self.index.values()])
         binary_similarities = np.einsum('i,ji->j', query_binary_vector, binary_vectors)
         top_k_indices = np.argpartition(binary_similarities, -top_k)[-top_k:]
         top_k_ids = [list(self.index.keys())[idx] for idx in top_k_indices]
 
         # Apply metadata filter on the retrieved top_k items
         if metadata:
             filtered_ids = []
-            for item_id in top_k_ids:
-                item_metadata = self.index[item_id]['metadata']
+            for chunk_id in top_k_ids:
+                item_metadata = self.index[chunk_id]['metadata']
                 if all(item_metadata.get(key) == value for key, value in metadata.items()):
-                    filtered_ids.append(item_id)
+                    filtered_ids.append(chunk_id)
             top_k_ids = filtered_ids[:top_k]
 
         # Get the similarity scores for the top_k items
         top_k_scores = binary_similarities[top_k_indices]
 
         return list(zip(top_k_ids, top_k_scores))
 
+
+    def update(self, id, text=None, metadata=None, vector=None):
+        chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
+        if chunk_ids:
+            for chunk_id in chunk_ids:
+                if text is not None:
+                    self.index[chunk_id]['text'] = text
+                if metadata is not None:
+                    self.index[chunk_id]['metadata'].update(metadata)
+                if vector is not None:
+                    self.index[chunk_id]['vector'] = vector
+            self.save()
+            print(f"Item with ID '{id}' updated successfully.")
+            return True
+        else:
+            print(f"Item with ID '{id}' not found.")
+            return False
+
+
     def delete(self, ids):
         if isinstance(ids, str):
             ids = [ids]
 
         deleted_count = 0
         for id in ids:
-            if id in self.index:
-                del self.index[id]
-                deleted_count += 1
+            chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
+            for chunk_id in chunk_ids:
+                if chunk_id in self.index:
+                    del self.index[chunk_id]
+                    deleted_count += 1
 
         if deleted_count > 0:
             self.save()
             print(f"Deleted {deleted_count} item(s) from the collection.")
         else:
             print("No items found with the specified IDs.")
 
         return deleted_count
-    
-    def update(self, id, text=None, metadata=None, vector=None):
-        if id in self.index:
-            if text is not None:
-                self.index[id]['text'] = text
 
-            if metadata is not None:
-                self.index[id]['metadata'].update(metadata)
-
-            if vector is not None:
-                self.index[id]['vector'] = vector
-
-            self.save()
-            print(f"Item with ID '{id}' updated successfully.")
-            return True
-        else:
-            print(f"Item with ID '{id}' not found.")
-            return False
     
+
     def get(self, ids=None, where=None):
         if ids is not None:
-            id_set = set(ids)
-            items = [(self.index[id]['text'], self.index[id]['metadata']) for id in self.index if id in id_set]
+            if isinstance(ids, str):
+                ids = [ids]
+            items = []
+            for id in ids:
+                item_chunks = []
+                item_metadata = {}
+                for chunk_id, chunk_data in self.index.items():
+                    if chunk_id.startswith(f"{id}_"):
+                        item_chunks.append(chunk_data['text'])
+                        item_metadata.update(chunk_data['metadata'])
+                if item_chunks:
+                    item_text = ' '.join(item_chunks)
+                    items.append((item_text, item_metadata))
         else:
-            items = [(self.index[id]['text'], self.index[id]['metadata']) for id in self.index]
+            items = []
+            item_dict = {}
+            for chunk_id, chunk_data in self.index.items():
+                item_id = chunk_id.split('_')[0]
+                if item_id not in item_dict:
+                    item_dict[item_id] = {'chunks': [], 'metadata': {}}
+                item_dict[item_id]['chunks'].append(chunk_data['text'])
+                item_dict[item_id]['metadata'].update(chunk_data['metadata'])
+            for item_id, item_data in item_dict.items():
+                item_text = ' '.join(item_data['chunks'])
+                item_metadata = item_data['metadata']
+                items.append((item_text, item_metadata))
 
         if where is not None:
             items = [item for item in items if all(item[1].get(key) == value for key, value in where.items())]
 
         return items
 
     def set(self, id, text=None, metadata=None, vector=None):
         print(f"Setting attributes for item with ID: {id}")
-        if id in self.index:
-            if text is not None:
-                self.index[id]['text'] = text
-            if metadata is not None:
-                self.index[id]['metadata'].update(metadata)
-            if vector is not None:
-                self.index[id]['vector'] = vector
-            self.save()
+        chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
+        if chunk_ids:
+            self.update(id, text, metadata, vector)
         else:
-            print(f"Item with ID {id} not found.")
+            self.add(text, metadata=metadata, item_id=id)
+            print(f"Item with ID '{id}' created successfully.")
+            
+                
 
     def count(self):
         return len(self.index)
     
 
     def save(self):
         print(f"Saving collection to {self.collection}")
-        with self.omom.create(self.collection) as omom_file:
-            omom_file.set_header(
-                embedding_model=self.model.model_metadata['general.name'],
+        with self.ctx.create(self.collection) as ctx_file:
+            ctx_file.set_header(
+                embedding_model="mixedbread-ai/mxbai-embed-large-v1",
                 embedding_size=self.model.model_metadata.get('bert.embedding_length', 1024),
                 embedding_dtype=self.model.embedding_dtype,
                 context_length=self.model.model_metadata.get('bert.context_length', 512)
             )
             for chunk_id, chunk_data in self.index.items():
-                omom_file.add_embedding(chunk_data['binary_vector'])
-                omom_file.add_context(chunk_data['text'])
-                omom_file.add_metadata(chunk_id, chunk_data['metadata'])
+                ctx_file.add_embedding(chunk_data['binary_vector'])
+                ctx_file.add_context(chunk_data['text'])
+                if 'metadata' in chunk_data:
+                    ctx_file.add_metadata(chunk_id, chunk_data['metadata'])
         print("Collection saved successfully.")
 
     def clear(self):
         print("Clearing the collection...")
         self.index = {}
-        self.omom.delete(self.collection)
+        self.ctx.delete(self.collection)
         print("Collection cleared.")
     
     def info(self):
         print("Collection Information:")
         print(f"  Items: {self.count()}")
         print(f"  Collection file: {self.collection}")
         print(f"  Embedding model: {self.model}")
```

### Comparing `vlite-0.2.0/vlite/omom.py` & `vlite-0.2.1/vlite/ctx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import struct
 import json
 from enum import Enum
 from typing import List, Dict, Union
 import numpy as np
 
-class OmomSectionType(Enum):
+class CtxSectionType(Enum):
     HEADER = 0
     EMBEDDINGS = 1
     CONTEXTS = 2
     METADATA = 3
 
-class OmomFile:
-    MAGIC_NUMBER = b"OMOM"
+class CtxFile:
+    MAGIC_NUMBER = b"CTXF"
     VERSION = 1
 
     def __init__(self, file_path):
         self.file_path = file_path
         self.header = {
             "embedding_model": "default",
             "embedding_size": 0,
@@ -39,39 +39,43 @@
     def add_context(self, context: str):
         self.contexts.append(context)
 
     def add_metadata(self, key: str, value: Union[int, float, str]):
         self.metadata[key] = value
 
     def save(self):
+        print("Number of embeddings to save: ", len(self.embeddings))
+        print("Number of metadata keys to save: ", len(self.metadata))
         with open(self.file_path, "wb") as file:
             file.write(self.MAGIC_NUMBER)
             file.write(struct.pack("<I", self.VERSION))
 
             header_json = json.dumps(self.header).encode("utf-8")
-            file.write(struct.pack("<II", OmomSectionType.HEADER.value, len(header_json)))
+            file.write(struct.pack("<II", CtxSectionType.HEADER.value, len(header_json)))
             file.write(header_json)
 
             if self.embeddings:
                 embeddings_data = b"".join(
                     struct.pack(f"<{len(emb)}f", *[float(x) if not np.isnan(x) else 0.0 for x in emb])
                     for emb in self.embeddings
                 )
-                file.write(struct.pack("<II", OmomSectionType.EMBEDDINGS.value, len(embeddings_data)))
+                file.write(struct.pack("<II", CtxSectionType.EMBEDDINGS.value, len(embeddings_data)))
                 file.write(embeddings_data)
 
             contexts_data = b"".join(struct.pack("<I", len(context.encode("utf-8"))) + context.encode("utf-8") for context in self.contexts)
-            file.write(struct.pack("<II", OmomSectionType.CONTEXTS.value, len(contexts_data)))
+            file.write(struct.pack("<II", CtxSectionType.CONTEXTS.value, len(contexts_data)))
             file.write(contexts_data)
 
             metadata_json = json.dumps(self.metadata).encode("utf-8")
-            file.write(struct.pack("<II", OmomSectionType.METADATA.value, len(metadata_json)))
+            file.write(struct.pack("<II", CtxSectionType.METADATA.value, len(metadata_json)))
             file.write(metadata_json)
         
     def load(self):
+        print("Number of embeddings loaded: ", len(self.embeddings))
+        print("Number of metadata keys loaded: ", len(self.metadata))
         try:
             with open(self.file_path, "rb") as file:
                 # Read and verify header
                 magic_number = file.read(len(self.MAGIC_NUMBER))
                 if magic_number != self.MAGIC_NUMBER:
                     raise ValueError(f"Invalid magic number: {magic_number}")
 
@@ -82,49 +86,49 @@
                 # Read sections
                 while True:
                     section_header = file.read(8)
                     if not section_header:
                         break
                     section_type, section_length = struct.unpack("<II", section_header)
 
-                    if section_type == OmomSectionType.HEADER.value:
+                    if section_type == CtxSectionType.HEADER.value:
                         header_json = file.read(section_length).decode("utf-8")
                         self.header = json.loads(header_json)
-                    elif section_type == OmomSectionType.EMBEDDINGS.value:
+                    elif section_type == CtxSectionType.EMBEDDINGS.value:
                         embeddings_data = file.read(section_length)
                         if embeddings_data:
                             embedding_size = len(embeddings_data) // 4
                             self.embeddings = [
                                 list(struct.unpack_from(f"<{embedding_size // len(self.embeddings)}f", embeddings_data, i * embedding_size))
                                 for i in range(len(self.embeddings))
                             ] if self.embeddings else [list(struct.unpack_from(f"<{embedding_size}f", embeddings_data))]
-                    elif section_type == OmomSectionType.CONTEXTS.value:
+                    elif section_type == CtxSectionType.CONTEXTS.value:
                         contexts_data = file.read(section_length)
                         self.contexts = []
                         offset = 0
                         while offset < len(contexts_data):
                             context_length = struct.unpack_from("<I", contexts_data, offset)[0]
                             offset += 4
                             try:
                                 context = contexts_data[offset : offset + context_length].decode("utf-8")
                                 self.contexts.append(context)
                             except UnicodeDecodeError as e:
                                 print(f"Error decoding context: {e}")
                             offset += context_length
-                    elif section_type == OmomSectionType.METADATA.value:
+                    elif section_type == CtxSectionType.METADATA.value:
                         metadata_json = file.read(section_length).decode("utf-8")
                         self.metadata = json.loads(metadata_json)
                     else:
                         raise ValueError(f"Unknown section type: {section_type}")
 
         except FileNotFoundError:
             pass
     
     def __repr__(self):
-        output = "OmomFile:\n\n"
+        output = "CtxFile:\n\n"
         output += "Header:\n"
         for key, value in self.header.items():
             output += f"  {key}: {value}\n"
         output += "\nEmbeddings:\n"
         for i, embedding in enumerate(self.embeddings):
             output += f"  {i}: {embedding}\n"
         output += "\nContexts:\n"
@@ -138,28 +142,28 @@
     def __enter__(self):
         self.load()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.save()
     
-class Omom:
-    def __init__(self, directory="omnoms"):
+class Ctx:
+    def __init__(self, directory="contexts"):
         self.directory = directory
         if not os.path.exists(directory):
             os.makedirs(directory)
 
     def get(self, user):
-        return os.path.join(self.directory, f"{user}.omom")
+        return os.path.join(self.directory, f"{user}.ctx")
 
-    def create(self, user: str) -> OmomFile:
+    def create(self, user: str) -> CtxFile:
         file_path = self.get(user)
-        return OmomFile(file_path)
+        return CtxFile(file_path)
 
-    def read(self, user_id: str) -> OmomFile:
+    def read(self, user_id: str) -> CtxFile:
         file_path = self.get(user_id)
-        return OmomFile(file_path)
+        return CtxFile(file_path)
 
     def delete(self, user_id: str):
         file_path = self.get(user_id)
         if os.path.exists(file_path):
             os.remove(file_path)
```

### Comparing `vlite-0.2.0/vlite/server.py` & `vlite-0.2.1/vlite/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Optional, Union
 from vlite.main import VLite
 from vlite.utils import process_file, process_pdf, process_webpage
 
 app = FastAPI(
     title="VLite API",
     description="API for VLite, a simple vector database for text embedding and retrieval.",
-    version="0.2.0",
+    version="0.2.1",
 )
 
 vlite = VLite()
 
 class TextData(BaseModel):
     text: str
     metadata: Optional[dict] = None
```

### Comparing `vlite-0.2.0/vlite/utils.py` & `vlite-0.2.1/vlite/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import PyPDF2
 import docx2txt
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 from typing import List
 import tiktoken
+import numpy as np
+import itertools
 
 try:
     from surya.ocr import run_ocr
     from surya.model.detection import segformer
     from surya.model.recognition.model import load_model
     from surya.model.recognition.processor import load_processor
     from surya.input.load import load_from_file, load_pdf
@@ -23,30 +25,30 @@
     Chop text into chunks of max_seq_length tokens or max_seq_length*4 characters (fast mode).
     """
     if isinstance(text, str):
         text = [text]
     enc = tiktoken.get_encoding("cl100k_base")
     chunks = []
     print(f"Length of text: {len(text)}")
-    print(f"Original text: {text}")
+    # print(f"Original text: {text}")
     for t in text:
         if fast:
             chunk_size = max_seq_length * 4
             chunks.extend([t[i:i + chunk_size] for i in range(0, len(t), chunk_size)])
         else:
             token_ids = enc.encode(t, disallowed_special=())
             num_tokens = len(token_ids)
             if num_tokens <= max_seq_length:
                 chunks.append(t)
             else:
                 for i in range(0, num_tokens, max_seq_length):
                     chunk = enc.decode(token_ids[i:i + max_seq_length])
                     chunks.append(chunk)
-    print("Chopped text into these chunks:", chunks)
-    print(f"Chopped text into {len(chunks)} chunks.")
+    # print("Chopped text into these chunks:", chunks)
+    # print(f"Chopped text into {len(chunks)} chunks.")
     return chunks
 
 def process_pdf(file_path: str, chunk_size: int = 512, use_ocr: bool = False, langs: List[str] = None) -> List[str]:
     """
     Process a PDF file and return a list of text chunks.
 
     Args:
@@ -188,16 +190,16 @@
         return process_pdf(file_path, chunk_size)
     elif extension == '.txt':
         return process_txt(file_path, chunk_size)
     elif extension == '.docx':
         return process_docx(file_path, chunk_size)
     elif extension == '.csv':
         return process_csv(file_path, chunk_size)
-    elif extension == '.pptx':
-        return process_pptx(file_path, chunk_size)
+    # elif extension == '.pptx':
+    #     return process_pptx(file_path, chunk_size)
     else:
         raise ValueError(f"Unsupported file type: {extension}")
     
     
 ## Other functions
 
 def cos_sim(a, b):
```

