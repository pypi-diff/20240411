# Comparing `tmp/arxiv_client-0.2.3.tar.gz` & `tmp/arxiv_client-0.2.4.tar.gz`

## Comparing `arxiv_client-0.2.3.tar` & `arxiv_client-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/link.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/LICENSE
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 arxiv_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.4/PKG-INFO
```

### Comparing `arxiv_client-0.2.3/src/arxiv_client/article.py` & `arxiv_client-0.2.4/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/src/arxiv_client/author.py` & `arxiv_client-0.2.4/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/src/arxiv_client/category.py` & `arxiv_client-0.2.4/src/arxiv_client/category.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/src/arxiv_client/client.py` & `arxiv_client-0.2.4/src/arxiv_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         :param page_size: The number of results to get in each page. None will fetch all results in one chunk
         :param paging_delay_ms: The delay in milliseconds between each page request
         :param paging_max_retries: The max number of retries for each page request
         :return: The search results
         """
         logger.debug("Searching arXiv with query: %r", query)
         subquery = copy.deepcopy(query)
-        if page_size is not None:
+        if page_size is not None and page_size < query.max_results:
             subquery.max_results = page_size
 
         total_retrieved = 0
         while total_retrieved < (query.max_results or float("inf")):
             feed = self._get_sub_page(subquery, paging_delay_ms, paging_max_retries)
             total_retrieved += len(feed.entries)
             total_results = int(feed.feed.opensearch_totalresults)
```

### Comparing `arxiv_client-0.2.3/src/arxiv_client/link.py` & `arxiv_client-0.2.4/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/src/arxiv_client/query.py` & `arxiv_client-0.2.4/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/.gitignore` & `arxiv_client-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/LICENSE` & `arxiv_client-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/README.md` & `arxiv_client-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 
 ## Usage
 
 In a nutshell:
 
 ```py
 import arxiv_client as arx
-import pprint
+
 
 categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
 client = arx.Client()
-articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=2))
+articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=10))
 for article in articles:
-  pprint.pprint(article)  # Formatted pretty print is supported
+    print(article)
 ```
 
 ### Structured Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
@@ -47,24 +47,27 @@
 - `article_ids`: arXiv article IDs
 - `custom_params`: custom query string
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
-# Query(keywords=['llm'],
-#       title_keywords=[],
-#       author_names=[],
-#       categories=[<Category.CS_AI: 'cs.AI'>, <Category.CS_IR: 'cs.IR'>],
-#       article_ids=[],
-#       custom_params=None,
-#       sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>,
-#                                    sort_order=<SortOrder.DESC: 'descending'>),
-#       start=None,
-#       max_results=5)
+# Query(
+#     keywords=['llm'],
+#     title_keywords=[],
+#     author_names=[],
+#     categories=[<Category.CS_AI: 'cs.AI'>, <Category.CS_IR: 'cs.IR'>],
+#     abstract_keywords=[],
+#     comment_keywords=[],
+#     article_ids=[],
+#     custom_params=None,
+#     sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>, sort_order=<SortOrder.DESC: 'descending'>),
+#     start=0,
+#     max_results=5
+# )
 ```
 
 Results in the following query logic:
 
 ```
 ("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
@@ -78,24 +81,27 @@
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
 ```py
 custom = f"cat:{Category.CS_AI.value} ANDNOT cat:{Category.CS_RO.value}"
 Query(keywords=["paged attention", "attention window"], custom_params=custom)
-# Query(keywords=['paged attention', 'attention window'],
-#       title_keywords=[],
-#       author_names=[],
-#       categories=[],
-#       article_ids=[],
-#       custom_params='cat:cs.AI ANDNOT cat:cs.RO',
-#       sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>,
-#                                    sort_order=<SortOrder.DESC: 'descending'>),
-#       start=None,
-#       max_results=10)
+# Query(
+#     keywords=['paged attention', 'attention window'],
+#     title_keywords=[],
+#     author_names=[],
+#     categories=[],
+#     abstract_keywords=[],
+#     comment_keywords=[],
+#     article_ids=[],
+#     custom_params='cat:cs.AI ANDNOT cat:cs.RO',
+#     sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>, sort_order=<SortOrder.DESC: 'descending'>),
+#     start=0,
+#     max_results=10
+# )
 ```
 
 Results in the following query logic:
 
 ```
 ("paged attention" OR "attention window") in any field AND (cs.AI AND NOT cs.RO) in the categories
 ```
```

### Comparing `arxiv_client-0.2.3/pyproject.toml` & `arxiv_client-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.3/PKG-INFO` & `arxiv_client-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -53,21 +53,21 @@
 
 ## Usage
 
 In a nutshell:
 
 ```py
 import arxiv_client as arx
-import pprint
+
 
 categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
 client = arx.Client()
-articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=2))
+articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=10))
 for article in articles:
-  pprint.pprint(article)  # Formatted pretty print is supported
+    print(article)
 ```
 
 ### Structured Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
@@ -84,24 +84,27 @@
 - `article_ids`: arXiv article IDs
 - `custom_params`: custom query string
 
 #### Example
 
 ```py
 Query(keywords=["llm"], categories=[Category.CS_AI, Category.CS_IR], max_results=5)
-# Query(keywords=['llm'],
-#       title_keywords=[],
-#       author_names=[],
-#       categories=[<Category.CS_AI: 'cs.AI'>, <Category.CS_IR: 'cs.IR'>],
-#       article_ids=[],
-#       custom_params=None,
-#       sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>,
-#                                    sort_order=<SortOrder.DESC: 'descending'>),
-#       start=None,
-#       max_results=5)
+# Query(
+#     keywords=['llm'],
+#     title_keywords=[],
+#     author_names=[],
+#     categories=[<Category.CS_AI: 'cs.AI'>, <Category.CS_IR: 'cs.IR'>],
+#     abstract_keywords=[],
+#     comment_keywords=[],
+#     article_ids=[],
+#     custom_params=None,
+#     sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>, sort_order=<SortOrder.DESC: 'descending'>),
+#     start=0,
+#     max_results=5
+# )
 ```
 
 Results in the following query logic:
 
 ```
 ("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
@@ -115,24 +118,27 @@
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
 ```py
 custom = f"cat:{Category.CS_AI.value} ANDNOT cat:{Category.CS_RO.value}"
 Query(keywords=["paged attention", "attention window"], custom_params=custom)
-# Query(keywords=['paged attention', 'attention window'],
-#       title_keywords=[],
-#       author_names=[],
-#       categories=[],
-#       article_ids=[],
-#       custom_params='cat:cs.AI ANDNOT cat:cs.RO',
-#       sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>,
-#                                    sort_order=<SortOrder.DESC: 'descending'>),
-#       start=None,
-#       max_results=10)
+# Query(
+#     keywords=['paged attention', 'attention window'],
+#     title_keywords=[],
+#     author_names=[],
+#     categories=[],
+#     abstract_keywords=[],
+#     comment_keywords=[],
+#     article_ids=[],
+#     custom_params='cat:cs.AI ANDNOT cat:cs.RO',
+#     sort_criterion=SortCriterion(sort_by=<SortBy.LAST_UPDATED_DATE: 'lastUpdatedDate'>, sort_order=<SortOrder.DESC: 'descending'>),
+#     start=0,
+#     max_results=10
+# )
 ```
 
 Results in the following query logic:
 
 ```
 ("paged attention" OR "attention window") in any field AND (cs.AI AND NOT cs.RO) in the categories
 ```
```

