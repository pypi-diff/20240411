# Comparing `tmp/arxiv_client-0.2.4.tar.gz` & `tmp/arxiv_client-0.2.5.tar.gz`

## Comparing `arxiv_client-0.2.4.tar` & `arxiv_client-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/link.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/LICENSE
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/PKG-INFO
```

### Comparing `arxiv_client-0.2.4/src/arxiv_client/article.py` & `arxiv_client-0.2.5/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/src/arxiv_client/author.py` & `arxiv_client-0.2.5/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/src/arxiv_client/category.py` & `arxiv_client-0.2.5/src/arxiv_client/category.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     CS_CR = "cs.CR", "Computer Science - Cryptography and Security"
     CS_CV = "cs.CV", "Computer Science - Computer Vision and Pattern Recognition"
     CS_CY = "cs.CY", "Computer Science - Computers and Society"
     CS_DB = "cs.DB", "Computer Science - Databases"
     CS_DC = "cs.DC", "Computer Science - Distributed; Parallel; and Cluster Computing"
     CS_DL = "cs.DL", "Computer Science - Digital Libraries"
     CS_DM = "cs.DM", "Computer Science - Discrete Mathematics"
+    CS_DS = "cs.DS", "Computer Science - Data Structures and Algorithms"
     CS_ET = "cs.ET", "Computer Science - Emerging Technologies"
     CS_FL = "cs.FL", "Computer Science - Formal Languages and Automata Theory"
     CS_GL = "cs.GL", "Computer Science - General Literature"
     CS_GR = "cs.GR", "Computer Science - Graphics"
     CS_GT = "cs.GT", "Computer Science - Game Theory"
     CS_HC = "cs.HC", "Computer Science - Human-Computer Interaction"
     CS_IR = "cs.IR", "Computer Science - Information Retrieval"
```

### Comparing `arxiv_client-0.2.4/src/arxiv_client/client.py` & `arxiv_client-0.2.5/src/arxiv_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self._last_request_dt = None
 
     # TODO: Consider async io
     def search(
         self,
         query: Query,
         page_size: int | None = None,
-        paging_delay_ms: int = 500,
+        paging_delay_ms: int = 250,
         paging_max_retries: int = 1,
     ) -> Iterator[Article]:
         """
         Search the Arxiv API.
 
         The paging parameters allow for the search to be broken up into smaller queries.
         This is useful for large result sets, which can be processed as a stream of smaller pages.
```

### Comparing `arxiv_client-0.2.4/src/arxiv_client/link.py` & `arxiv_client-0.2.5/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/src/arxiv_client/query.py` & `arxiv_client-0.2.5/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/.gitignore` & `arxiv_client-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/LICENSE` & `arxiv_client-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/README.md` & `arxiv_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/pyproject.toml` & `arxiv_client-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.4/PKG-INFO` & `arxiv_client-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
```

