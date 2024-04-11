# Comparing `tmp/arxiv_client-0.2.6.tar.gz` & `tmp/arxiv_client-0.3.0.tar.gz`

## Comparing `arxiv_client-0.2.6.tar` & `arxiv_client-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/category.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/link.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/LICENSE
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 arxiv_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/README.md
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/PKG-INFO
```

### Comparing `arxiv_client-0.2.6/src/arxiv_client/article.py` & `arxiv_client-0.3.0/src/arxiv_client/article.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/src/arxiv_client/author.py` & `arxiv_client-0.3.0/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/src/arxiv_client/category.py` & `arxiv_client-0.3.0/src/arxiv_client/category.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,7 +184,25 @@
     # Statistics
     STAT_AP = "stat.AP", "Statistics - Applications"
     STAT_CO = "stat.CO", "Statistics - Computation"
     STAT_ME = "stat.ME", "Statistics - Methodology"
     STAT_ML = "stat.ML", "Statistics - Machine Learning"
     STAT_OT = "stat.OT", "Statistics - Other Statistics"
     STAT_TH = "stat.TH", "Statistics - Statistics Theory"
+
+
+class Subject(Enum):
+    """
+    This is what some parts of the arXiv documentation calls category, referring to the above as
+    subject class.
+    """
+    COMPUTER_SCIENCE = "cs"
+    ECONOMICS = "econ"
+    ELECTRICAL_ENGINEERING_AND_SYSTEMS_SCIENCE = "eess"
+    MATHEMATICS = "math"
+    ASTROPHYSICS = "astro-ph"
+    CONDENSED_MATTER = "cond-mat"
+    NONLINEAR_SCIENCES = "nlin"
+    PHYSICS = "physics"
+    QUANTITATIVE_BIOLOGY = "q-bio"
+    QUANTITATIVE_FINANCE = "q-fin"
+    STATISTICS = "stat"
```

### Comparing `arxiv_client-0.2.6/src/arxiv_client/link.py` & `arxiv_client-0.3.0/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/src/arxiv_client/query.py` & `arxiv_client-0.3.0/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/.gitignore` & `arxiv_client-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/LICENSE` & `arxiv_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.2.6/README.md` & `arxiv_client-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,33 +7,43 @@
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 ## Basic Features
 
 - Simple structured queries
 - Comprehensive entity models, with documentation
-  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
+  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's category taxonomy
 - Fully type annotated
 
 ## Usage
 
-In a nutshell:
+### Daily RSS Feed
+
+```py
+import arxiv_client as arx
+
+
+client = arx.Client()
+articles = client.rss_by_subject(arx.Subject.COMPUTER_SCIENCE)
+```
+
+### Search
 
 ```py
 import arxiv_client as arx
 
 
 categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
 client = arx.Client()
 articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=10))
 for article in articles:
     print(article)
 ```
 
-### Structured Query Logic
+### Structured Search Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
 #### Searchable Fields
 
 The `Query` object accepts the following field filters:
@@ -70,15 +80,15 @@
 
 ```
 ("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
 
 See the [Query](src/arxiv_client/query.py) class for more information.
 
-### Custom Queries
+### Custom Search Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
 
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
@@ -108,10 +118,28 @@
 
 Equivalent query string:
 
 ```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
+## Known Issues
+
+The arXiv search API is unreliable, especially for large queries.
+
+The API will sometimes return incomplete results or return no entries,
+although the response is valid. See this [GitHub issue](https://github.com/lukasschwab/arxiv.py/issues/43)
+for discussion on the topic.
+
+If you are encountering this problem, some things that may help include:
+
+- Reduce the page size; `100` seems to have a relatively high success rate
+- Increase paging retry and delay parameters
+- Break up large queries into smaller queries
+
+Retries often help with the issue, but are sometimes insufficient.
+If you need more reliable access to large query results, consider looking into
+the [arXiv Bulk Data Access](https://info.arxiv.org/help/bulk_data.html) options.
+
 ## Development
 
 This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

### Comparing `arxiv_client-0.2.6/pyproject.toml` & `arxiv_client-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 [tool.hatch.envs.default]
 type = "virtual"
 path = ".venv"
 dependencies = [
   "coverage[toml]>=6.5",
   "mypy",
   "pytest",
+  "rich",
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
```

### Comparing `arxiv_client-0.2.6/PKG-INFO` & `arxiv_client-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.2.6
+Version: 0.3.0
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
         
@@ -44,33 +44,43 @@
 in that it further abstracts away the arXiv API so you do not need to learn to construct
 query strings. The overall goal is to enable users to skip reading the API docs entirely.
 
 ## Basic Features
 
 - Simple structured queries
 - Comprehensive entity models, with documentation
-  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's subject taxonomy
+  - For example, see the [Category](src/arxiv_client/category.py) enum for arXiv's category taxonomy
 - Fully type annotated
 
 ## Usage
 
-In a nutshell:
+### Daily RSS Feed
+
+```py
+import arxiv_client as arx
+
+
+client = arx.Client()
+articles = client.rss_by_subject(arx.Subject.COMPUTER_SCIENCE)
+```
+
+### Search
 
 ```py
 import arxiv_client as arx
 
 
 categories = [arx.Category.CS_AI, arx.Category.CS_CL, arx.Category.CS_IR]
 client = arx.Client()
 articles = client.search(arx.Query(keywords=["llm"], categories=categories, max_results=10))
 for article in articles:
     print(article)
 ```
 
-### Structured Query Logic
+### Structured Search Query Logic
 
 When using the structured `Query` fields, multiple values within a single field are combined using `OR`, 
 and multiple fields are combined using `AND`.
 
 #### Searchable Fields
 
 The `Query` object accepts the following field filters:
@@ -107,15 +117,15 @@
 
 ```
 ("llm") in any field AND (cs.AI OR cs.IR) in the categories
 ```
 
 See the [Query](src/arxiv_client/query.py) class for more information.
 
-### Custom Queries
+### Custom Search Queries
 
 If the provided simple query logic is insufficient, the `Query` object takes a self-built query string through the `custom_params` attribute. You do not need to URL encode this value.
 
 See [arXiv Query Construction](https://info.arxiv.org/help/api/user-manual.html#51-details-of-query-construction) for more information on building your own queries.
 
 #### Example
 
@@ -145,10 +155,28 @@
 
 Equivalent query string:
 
 ```
 (all:"paged attention" OR all:"attention window") AND (cat:cs.AI ANDNOT cat:cs.RO)
 ```
 
+## Known Issues
+
+The arXiv search API is unreliable, especially for large queries.
+
+The API will sometimes return incomplete results or return no entries,
+although the response is valid. See this [GitHub issue](https://github.com/lukasschwab/arxiv.py/issues/43)
+for discussion on the topic.
+
+If you are encountering this problem, some things that may help include:
+
+- Reduce the page size; `100` seems to have a relatively high success rate
+- Increase paging retry and delay parameters
+- Break up large queries into smaller queries
+
+Retries often help with the issue, but are sometimes insufficient.
+If you need more reliable access to large query results, consider looking into
+the [arXiv Bulk Data Access](https://info.arxiv.org/help/bulk_data.html) options.
+
 ## Development
 
 This uses [hatch](https://hatch.pypa.io/latest/) for project management.
```

