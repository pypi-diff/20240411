# Comparing `tmp/arxiv_client-0.2.5.tar.gz` & `tmp/arxiv_client-0.2.6.tar.gz`

## Comparing `arxiv_client-0.2.5.tar` & `arxiv_client-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/link.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/LICENSE
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/PKG-INFO
```

### Comparing `arxiv_client-0.2.5/src/arxiv_client/article.py` & `arxiv_client-0.2.6/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/src/arxiv_client/author.py` & `arxiv_client-0.2.6/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/src/arxiv_client/category.py` & `arxiv_client-0.2.6/src/arxiv_client/category.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/src/arxiv_client/client.py` & `arxiv_client-0.2.6/src/arxiv_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             for entry in feed.entries:
                 yield Article.from_feed_entry(entry)
 
             if not feed.entries or total_retrieved >= total_results:
                 return
 
             if page_size is not None:
-                subquery.start += page_size
+                subquery.start += len(feed.entries)
                 if query.max_results is not None:
                     subquery.max_results = min(query.max_results - total_retrieved, page_size)
 
     def _get_sub_page(self, query: Query, paging_delay_ms: int, paging_max_retries: int) -> feedparser.FeedParserDict:
         """
         Get a chunk of search results from the Arxiv API.
 
@@ -88,18 +88,18 @@
         :param paging_max_retries: The max number of retries for each chunk request
         :return: The search results
         """
         try_count = 0
         while try_count <= paging_max_retries:
             try:
                 self._apply_paging_delay(paging_delay_ms)
-                response = self._session.get(self.base_search_url, params=query._to_url_params())  # noqa SLF001
-                self._last_request_dt = datetime.now(tz=UTC)
-                response.raise_for_status()
-                feed = feedparser.parse(response.content)
+                with self._session.get(self.base_search_url, params=query._to_url_params(), stream=False) as r: # noqa SLF001
+                    self._last_request_dt = datetime.now(tz=UTC)
+                    r.raise_for_status()
+                    feed = feedparser.parse(r.content)
             except (requests.HTTPError, requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout) as e:
                 logger.warning("Failed to retrieve page of articles: %s", e)
                 try_count += 1
             else:
                 logger.debug("Successfully retrieved page of %d articles", len(feed.entries))
                 return feed
```

### Comparing `arxiv_client-0.2.5/src/arxiv_client/link.py` & `arxiv_client-0.2.6/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/src/arxiv_client/query.py` & `arxiv_client-0.2.6/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/.gitignore` & `arxiv_client-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/LICENSE` & `arxiv_client-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/README.md` & `arxiv_client-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/pyproject.toml` & `arxiv_client-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.5/PKG-INFO` & `arxiv_client-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
```

