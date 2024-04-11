# Comparing `tmp/myla-0.2.8-py3-none-any.whl.zip` & `tmp/myla-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 572513 bytes, number of entries: 59
+Zip file size: 187915 bytes, number of entries: 57
 -rw-r--r--  2.0 unx      171 b- defN 23-Dec-06 07:03 myla/__init__.py
 -rw-r--r--  2.0 unx     2949 b- defN 23-Dec-08 09:36 myla/__main__.py
--rw-r--r--  2.0 unx    17302 b- defN 23-Dec-19 06:39 myla/_api.py
+-rw-r--r--  2.0 unx    17471 b- defN 23-Dec-19 07:14 myla/_api.py
 -rw-r--r--  2.0 unx     1057 b- defN 23-Dec-06 07:03 myla/_auth.py
 -rw-r--r--  2.0 unx     3015 b- defN 23-Dec-13 08:42 myla/_entry.py
 -rw-r--r--  2.0 unx      301 b- defN 23-Nov-30 04:00 myla/_env.py
 -rw-r--r--  2.0 unx     5705 b- defN 23-Dec-18 06:44 myla/_llm.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Nov-30 04:00 myla/_logging.py
 -rw-r--r--  2.0 unx     5257 b- defN 23-Dec-08 09:36 myla/_models.py
 -rw-r--r--  2.0 unx     2917 b- defN 23-Nov-30 04:00 myla/_run_scheduler.py
 -rw-r--r--  2.0 unx      721 b- defN 23-Nov-30 04:00 myla/_tools.py
--rw-r--r--  2.0 unx       18 b- defN 23-Dec-19 06:44 myla/_version.py
+-rw-r--r--  2.0 unx       18 b- defN 23-Dec-19 07:39 myla/_version.py
 -rw-r--r--  2.0 unx     2728 b- defN 23-Dec-06 07:03 myla/assistants.py
 -rw-r--r--  2.0 unx     2446 b- defN 23-Dec-06 07:03 myla/files.py
 -rw-r--r--  2.0 unx     1587 b- defN 23-Nov-30 04:00 myla/iur.py
 -rw-r--r--  2.0 unx     4223 b- defN 23-Dec-14 04:26 myla/messages.py
 -rw-r--r--  2.0 unx     1548 b- defN 23-Nov-30 04:00 myla/persistence.py
 -rw-r--r--  2.0 unx     3364 b- defN 23-Nov-30 05:40 myla/retrieval.py
 -rw-r--r--  2.0 unx     5183 b- defN 23-Dec-07 03:07 myla/runs.py
@@ -27,35 +27,33 @@
 -rw-r--r--  2.0 unx     1501 b- defN 23-Nov-30 04:00 myla/extensions/tools/qa_summary.py
 -rw-r--r--  2.0 unx     1486 b- defN 23-Nov-30 04:00 myla/llms/__init__.py
 -rw-r--r--  2.0 unx      311 b- defN 23-Nov-30 04:00 myla/llms/backend.py
 -rw-r--r--  2.0 unx     1564 b- defN 23-Nov-30 04:00 myla/llms/chatglm.py
 -rw-r--r--  2.0 unx      573 b- defN 23-Nov-30 04:00 myla/llms/mock.py
 -rw-r--r--  2.0 unx     2059 b- defN 23-Nov-30 04:00 myla/llms/openai.py
 -rw-r--r--  2.0 unx      222 b- defN 23-Nov-30 04:00 myla/llms/utils.py
--rw-r--r--  2.0 unx     3449 b- defN 23-Dec-19 06:38 myla/vectorstores/__init__.py
+-rw-r--r--  2.0 unx     3528 b- defN 23-Dec-19 07:12 myla/vectorstores/__init__.py
 -rw-r--r--  2.0 unx     2425 b- defN 23-Dec-19 06:28 myla/vectorstores/_base.py
 -rw-r--r--  2.0 unx      842 b- defN 23-Dec-19 06:40 myla/vectorstores/_embeddings.py
 -rw-r--r--  2.0 unx     3089 b- defN 23-Dec-11 08:59 myla/vectorstores/chromadb_vectorstore.py
--rw-r--r--  2.0 unx    10057 b- defN 23-Dec-19 06:36 myla/vectorstores/faiss_group.py
+-rw-r--r--  2.0 unx    10092 b- defN 23-Dec-19 07:34 myla/vectorstores/faiss_group.py
 -rw-r--r--  2.0 unx     4637 b- defN 23-Dec-07 09:28 myla/vectorstores/faiss_vectorstore.py
 -rw-r--r--  2.0 unx     4264 b- defN 23-Dec-08 09:36 myla/vectorstores/lancedb_vectorstore.py
 -rw-r--r--  2.0 unx      214 b- defN 23-Nov-30 04:00 myla/vectorstores/loaders.py
 -rw-r--r--  2.0 unx      668 b- defN 23-Nov-30 04:00 myla/vectorstores/pandas_loader.py
 -rw-r--r--  2.0 unx     1190 b- defN 23-Dec-06 07:03 myla/vectorstores/pdf_loader.py
--rw-r--r--  2.0 unx     2318 b- defN 23-Dec-19 06:40 myla/vectorstores/sentence_transformers_embeddings.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-Dec-19 07:38 myla/vectorstores/sentence_transformers_embeddings.py
 -rw-r--r--  2.0 unx      294 b- defN 23-Dec-13 08:41 myla/webui/__init__.py
 -rw-r--r--  2.0 unx      838 b- defN 23-Dec-13 08:42 myla/webui/_web_template.py
 -rw-r--r--  2.0 unx      754 b- defN 23-Dec-13 08:42 myla/webui/__pycache__/__init__.cpython-311.pyc
 -rw-r--r--  2.0 unx      499 b- defN 23-Dec-07 03:09 myla/webui/__pycache__/__init__.cpython-39.pyc
 -rw-r--r--  2.0 unx     1652 b- defN 23-Dec-13 08:42 myla/webui/__pycache__/_web_template.cpython-311.pyc
 -rw-r--r--  2.0 unx       83 b- defN 23-Nov-21 13:27 myla/webui/statics/welcome.md
--rw-r--r--  2.0 unx   235977 b- defN 23-Dec-19 06:45 myla/webui/statics/aify/aify.css
--rw-r--r--  2.0 unx  1180725 b- defN 23-Dec-19 06:45 myla/webui/statics/aify/aify.js
 -rw-r--r--  2.0 unx   149653 b- defN 23-Nov-21 13:27 myla/webui/statics/images/screenshot.png
 -rw-r--r--  2.0 unx      905 b- defN 23-Dec-13 08:34 myla/webui/templates/index.html
--rwxr-xr-x  2.0 unx       36 b- defN 23-Nov-15 04:13 myla-0.2.8.data/scripts/myla
--rw-r--r--  2.0 unx     1066 b- defN 23-Dec-19 06:45 myla-0.2.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3904 b- defN 23-Dec-19 06:45 myla-0.2.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-19 06:45 myla-0.2.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Dec-19 06:45 myla-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4746 b- defN 23-Dec-19 06:45 myla-0.2.8.dist-info/RECORD
-59 files, 1699059 bytes uncompressed, 565085 bytes compressed:  66.7%
+-rwxr-xr-x  2.0 unx       36 b- defN 23-Nov-15 04:13 myla-0.2.9.data/scripts/myla
+-rw-r--r--  2.0 unx     1066 b- defN 23-Dec-19 07:40 myla-0.2.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3904 b- defN 23-Dec-19 07:40 myla-0.2.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Dec-19 07:40 myla-0.2.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Dec-19 07:40 myla-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4564 b- defN 23-Dec-19 07:40 myla-0.2.9.dist-info/RECORD
+57 files, 282430 bytes uncompressed, 180765 bytes compressed:  36.0%
```

## zipnote {}

```diff
@@ -141,38 +141,32 @@
 
 Filename: myla/webui/__pycache__/_web_template.cpython-311.pyc
 Comment: 
 
 Filename: myla/webui/statics/welcome.md
 Comment: 
 
-Filename: myla/webui/statics/aify/aify.css
-Comment: 
-
-Filename: myla/webui/statics/aify/aify.js
-Comment: 
-
 Filename: myla/webui/statics/images/screenshot.png
 Comment: 
 
 Filename: myla/webui/templates/index.html
 Comment: 
 
-Filename: myla-0.2.8.data/scripts/myla
+Filename: myla-0.2.9.data/scripts/myla
 Comment: 
 
-Filename: myla-0.2.8.dist-info/LICENSE
+Filename: myla-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: myla-0.2.8.dist-info/METADATA
+Filename: myla-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: myla-0.2.8.dist-info/WHEEL
+Filename: myla-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: myla-0.2.8.dist-info/top_level.txt
+Filename: myla-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: myla-0.2.8.dist-info/RECORD
+Filename: myla-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## myla/_api.py

```diff
@@ -356,19 +356,27 @@
     # Create a vectorstore loading task
     # TODO: background task and failover
     ftype = filename.split(".")[-1]
 
     if purpose == "assistants":
         logger.info(f"Build vectorstore: id={id}, ftype={ftype}")
         async def _vs_load_task():
-            load_vectorstore_from_file(collection=id, fname=fname, ftype=ftype, embeddings_columns=embeddings_columns, loader=loader, instruction=metadata.get('instruction'))
+            load_vectorstore_from_file(
+                collection=id,
+                fname=fname,
+                ftype=ftype,
+                embeddings_columns=embeddings_columns,
+                loader=loader,
+                group_by=metadata.get('group_by'),
+                instruction=metadata.get('instruction')
+            )
         try:
             await _vs_load_task()
         except Exception as e:
-            logger.warn(f"Build vectorstore failed: {e}")
+            logger.warn(f"Build vectorstore failed:", exc_info=e)
             raise HTTPException(status_code=400, detail=f"Can't build vectorstore. {e}")
 
     return files.create(id=id, file=file_upload, bytes=bytes, filename=filename, user_id=request.user.id)
 
 
 @api.get("/v1/files", response_model=files.FileList, tags=["Files"])
 @requires(['authenticated'])
```

## myla/_version.py

```diff
@@ -1 +1 @@
-VERSION = '0.2.8'
+VERSION = '0.2.9'
```

## myla/vectorstores/__init__.py

```diff
@@ -95,8 +95,14 @@
     records = list(loader_.load(file=fname))
 
     if len(records) == 0:
         return
 
     vs.create_collection(collection=collection, schema=records[0], mode='overwrite')
 
-    vs.add(collection=collection, records=records, embeddings_columns=embeddings_columns, instruction=kwargs.get('instruction'))
+    vs.add(
+        collection=collection,
+        records=records,
+        embeddings_columns=embeddings_columns,
+        group_by=kwargs.get('group_by'),
+        instruction=kwargs.get('instruction')
+    )
```

## myla/vectorstores/faiss_group.py

```diff
@@ -1,12 +1,13 @@
 import os
 import threading
 import pickle
 import gc
 import numpy as np
+import pandas as pd
 from typing import Any, Dict, List, Optional
 from ._base import Record, VectorStore
 from ._embeddings import Embeddings
 from .. import utils
 
 
 class FAISSGroupException(Exception):
@@ -121,15 +122,15 @@
             # save data
             self._save_data(collection=collection, data=data)
             gid_to_saved = groups.keys()
             for gid in gid_to_saved:
                 self._save_group(collection=collection, gid=gid, index=indexes[gid], ids=ids[gid])
 
     def _group_id(self, v=None):
-        if v is None:
+        if v is None or pd.isnull(v):
             v = ""
         if not isinstance(v, str):
             v = str(v)
         return utils.sha256(v.encode()).hex()
 
     def _group_records(self, records: List[Record], group_by: str):
         groups = {}
@@ -141,15 +142,14 @@
                 gid = records[i].get(group_by)
                 gid = self._group_id(gid)
                 g = groups.get(gid)
                 if not g:
                     g = []
                     groups[gid] = g
                 g.append(i)
-
         return groups
 
     def _save_data(self, collection, data):
         fname = os.path.join(self._path, collection, "data.pkl")
         with open(fname, 'wb') as f:
             pickle.dump(data, f)
```

## myla/vectorstores/sentence_transformers_embeddings.py

```diff
@@ -41,16 +41,16 @@
         self.tansformer = sentence_transformers.SentenceTransformer(
             self.model_name, **self.model_kwargs
         )
 
     def embed_batch(self, texts: List[str], **kwargs) -> List[List[float]]:
         import sentence_transformers
 
-        instruction = self.instruction if 'instruction' not in kwargs else kwargs['instruction']
-        print(instruction)
+        instruction = kwargs['instruction'] if kwargs.get('instruction') else self.instruction
+
         texts = list(map(lambda x: (instruction if self.is_bge_model else '') + x.replace("\n", " "), texts))
 
         if self.multi_process:
             pool = self.tansformer.start_multi_process_pool()
             embeddings = self.tansformer.encode_multi_process(texts, pool)
             sentence_transformers.SentenceTransformer.stop_multi_process_pool(
                 pool)
```

## Comparing `myla-0.2.8.dist-info/LICENSE` & `myla-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `myla-0.2.8.dist-info/METADATA` & `myla-0.2.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myla
-Version: 0.2.8
+Version: 0.2.9
 Summary: A local implementation of OpenAI Assistants API: Myla stands for MY Local Assistant
 Home-page: https://github.com/muyuworks/myla
 Author-email: shenggong.wang@gmail.com
 Keywords: AI assistant,LLM,Myla,chatbot
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `myla-0.2.8.dist-info/RECORD` & `myla-0.2.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 myla/__init__.py,sha256=wxKKWUGEZdi2AuJ5VAhgb2KpwdNZi--_U5tbErLgVrQ,171
 myla/__main__.py,sha256=zIoU89z4X-hzBUqVTLtEcfxDVD1CggUncb_oUpAF83I,2949
-myla/_api.py,sha256=bAnUkMc6p7wMRz6AC3s14x__LHLiYpWxwom8tA51toE,17302
+myla/_api.py,sha256=PINC_Kql-ROB7O8PD9y52ns3eKmE8k4vGQliwhyLy4E,17471
 myla/_auth.py,sha256=ON3nTOEHK4uSsWKUj1gGT6aP7RDoC8ZK0JpJkFMXA80,1057
 myla/_entry.py,sha256=v-V1g1AKo17oDTiXzqYL783vQJNfwsbfu2EzTaqDIn4,3015
 myla/_env.py,sha256=J2NIp36Tj9TFeanzZSXfvUwSDuWiTmbXqAYzhKuVk1I,301
 myla/_llm.py,sha256=nomw-Jqp8Bj8i8LtWA4DN3_9gaelLRxXoComTNOlpco,5705
 myla/_logging.py,sha256=2_RAiF-AXziKjdf2JLFs9g3lt89AEsOlhNRBE5IQJMM,51
 myla/_models.py,sha256=EigLf_TvmamwYKbPw8aMmGvP8NIl-F1lX4cfZ2B9fzo,5257
 myla/_run_scheduler.py,sha256=7gldiGIKszVj6Uv1Q28YljFkIKrRtLglHwkCr7WOqVE,2917
 myla/_tools.py,sha256=l0-M7AGhUONW89U9huU1o9CgnnW4npqlIE1kfhmEqj8,721
-myla/_version.py,sha256=sNaan8850lcBLCYwKL-eZxGZtGjSUrCfhHXl-ZLpX-w,18
+myla/_version.py,sha256=vBZ8jfpqbYXwqFqktplIXDG2JMkY9cZwbqi375q8Jqc,18
 myla/assistants.py,sha256=z-ZWap3IhDp-NgNpbQmEsisNd56aSWEHhFxRjS4-fNo,2728
 myla/files.py,sha256=wgA7gUvh-8UBHWlAffnT7XvZz6oPRhVUEojVeZIhKiw,2446
 myla/iur.py,sha256=IwDWSj5pcw0IVvdD-IqNdqYgfelDPfWbQyyXIlYlJoU,1587
 myla/messages.py,sha256=8N_mPRdptrjfxkWdtqDIcOSXcUmQspL5irXVIzwubEQ,4223
 myla/persistence.py,sha256=EPIfOVUktI48nhpN4XMsuD3EGy_J8h6i02SMOqM5ym4,1548
 myla/retrieval.py,sha256=ic6faqoGC0xjBiw1A1uO_u6YXBi27k9kMkgzpg3mNxM,3364
 myla/runs.py,sha256=FlbJR8nLgO7Bv0GaFc6qb5g9ENPk7dXUVFuiiMpE0dA,5183
@@ -26,34 +26,32 @@
 myla/extensions/tools/qa_summary.py,sha256=oHPo-sPPihr0LllL7K84BMUgoOdKXNf2mD3_n-VEcys,1501
 myla/llms/__init__.py,sha256=R33hPBhuvTtzIESzxC4uFI2q0wpf41kqCqoLNUl8Oss,1486
 myla/llms/backend.py,sha256=VMowXPN1GOrWTOo7bXsDXLdBw6xC_3tWY8n4rii-zXc,311
 myla/llms/chatglm.py,sha256=0zHxEuC6g-SdVysJ8TULNmYNnupm8u4jJJLTXuiviCs,1564
 myla/llms/mock.py,sha256=Zw-lRQBj5WHGMpqpECCVAMTNE2hLuurQEs7xYvDitHI,573
 myla/llms/openai.py,sha256=dxexfa9V2i1-7rfIstsnEqifLZt1SB9woFY1CIqFBb8,2059
 myla/llms/utils.py,sha256=ejSHdDR2F9Bk2rLAVWm96JcHSOy5zyk66xyAteT6SZI,222
-myla/vectorstores/__init__.py,sha256=7KpK5zldSEoy3-ioKXASGW0daeL72fmbJC9qiflws3I,3449
+myla/vectorstores/__init__.py,sha256=sx7mMiOLycgCLkC0g9nZQ32X91Gb8GiR9roEflpfpZQ,3528
 myla/vectorstores/_base.py,sha256=f-tJgnHso5jxW87tiIYlYzl_WUr0jk9amIxGXBf0LTg,2425
 myla/vectorstores/_embeddings.py,sha256=x9IXXEF3Ji6gdYafEwTk1-9rAVJpQpxTgxdC3oF0qZE,842
 myla/vectorstores/chromadb_vectorstore.py,sha256=T7n-p7gcSrJE1X0XL0TmZSD4tGxsIbvk7ZIfc8vChcI,3089
-myla/vectorstores/faiss_group.py,sha256=IR3y8SRja1s4vPIOlCLCvC_mYdClkLsv-cF74bsOiWw,10057
+myla/vectorstores/faiss_group.py,sha256=DDYtVcdVtpY79jVH1NPy5zjz2kCk8_0aaCUlG7xT6Gw,10092
 myla/vectorstores/faiss_vectorstore.py,sha256=FeqoqW6udmz4esA8VLn8svoLcEEOsczLMLv2wbmZ4Qw,4637
 myla/vectorstores/lancedb_vectorstore.py,sha256=FP--iE5Zu9HOcaYQfToQ77oHBeoizOg9TovTwVg6V7U,4264
 myla/vectorstores/loaders.py,sha256=eamlt7p0dhCNFRI5MJ7XDk7dEsscnCCBCYoL-Yy7YSA,214
 myla/vectorstores/pandas_loader.py,sha256=IEL-POUO4czbXad_JmkOw_hzwr5bHlX7Vo9GklzHlxg,668
 myla/vectorstores/pdf_loader.py,sha256=gI3e3bXVHDSaxyS4WlkHwWWfPiPuvBklsY5bFDzSCTU,1190
-myla/vectorstores/sentence_transformers_embeddings.py,sha256=Vqq2-3Uski2CYUErJx4EfTNZwcmuZoYLctb_4xfbqx0,2318
+myla/vectorstores/sentence_transformers_embeddings.py,sha256=zUL9HFwLTlzZRXHOd-3TJ0h9IPMvFpWPdUtFwHBFhJo,2290
 myla/webui/__init__.py,sha256=3oBcu8T7jq8jEMmB18z6oXxmiBiVdg_ohROB2p3VMpo,294
 myla/webui/_web_template.py,sha256=F5DoNd20Xp9X4RbYyRcAKrrn_hWiOpE7-TcPLMzquEU,838
 myla/webui/__pycache__/__init__.cpython-311.pyc,sha256=nGdbcAs8zEw6q_FXzHyKihd1JANls9hIW4R2wul3dTQ,754
 myla/webui/__pycache__/__init__.cpython-39.pyc,sha256=Gmg6MM2kpt0TSNBQ7Vu2qiSQIFy5joar5uXPlVw2j-c,499
 myla/webui/__pycache__/_web_template.cpython-311.pyc,sha256=Ynv5vGb3S7gqlDON-0vTFqyWwSXtQsav6uPc_4sJN0Y,1652
 myla/webui/statics/welcome.md,sha256=UPxvELUUu_8nV1o3R6tosqyNv4v1VGNuZgwWezcCJfo,83
-myla/webui/statics/aify/aify.css,sha256=cLJbMLgn_Qt3d01TACWFjv3DaCeC5qiYuvHQfA4H6ho,235977
-myla/webui/statics/aify/aify.js,sha256=2kmuYVxda-LaPnfufRpR-g0oMYKuN9M25TuoB6nv8eA,1180725
 myla/webui/statics/images/screenshot.png,sha256=eQysExmaAkWRZcJe0CMYuVTbxNSNKHSuQrjut0QvaHE,149653
 myla/webui/templates/index.html,sha256=OZXZBjubVBkMH9IKbRM9gKfUgOrrGiXW60ZgwnC5cjY,905
-myla-0.2.8.data/scripts/myla,sha256=Kvq6DW72t-vLHJKUgLscxuM35AOd213_prYKWgiZhtQ,36
-myla-0.2.8.dist-info/LICENSE,sha256=bt0q0ALtboR48A9K-U9QMZr3uY2xIENanfQTPs0ow3c,1066
-myla-0.2.8.dist-info/METADATA,sha256=QjK8uI4ogQDG0kndM6m-JxwsPr-H1lFfSVTQ9DY_C0M,3904
-myla-0.2.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-myla-0.2.8.dist-info/top_level.txt,sha256=ssKInz5r36q2XxrcXxssf0JdOze4IXZ6ogc-h8bUrmw,5
-myla-0.2.8.dist-info/RECORD,,
+myla-0.2.9.data/scripts/myla,sha256=Kvq6DW72t-vLHJKUgLscxuM35AOd213_prYKWgiZhtQ,36
+myla-0.2.9.dist-info/LICENSE,sha256=bt0q0ALtboR48A9K-U9QMZr3uY2xIENanfQTPs0ow3c,1066
+myla-0.2.9.dist-info/METADATA,sha256=KFRm5qv_fHlzTQfBMPNQq9kcHISpdsj59JpPf38rvkk,3904
+myla-0.2.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+myla-0.2.9.dist-info/top_level.txt,sha256=ssKInz5r36q2XxrcXxssf0JdOze4IXZ6ogc-h8bUrmw,5
+myla-0.2.9.dist-info/RECORD,,
```

