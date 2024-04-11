# Comparing `tmp/limoon-0.0.2.tar.gz` & `tmp/limoon-0.0.4.tar.gz`

## Comparing `limoon-0.0.2.tar` & `limoon-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 limoon-0.0.2/README.md
--rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.2/limoon-logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/constant.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/core.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/exception.py
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/model.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 limoon-0.0.2/src/limoon/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 limoon-0.0.2/tests/test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 limoon-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 limoon-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 limoon-0.0.4/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 limoon-0.0.4/README.md
+-rw-r--r--   0        0        0    31396 2020-02-02 00:00:00.000000 limoon-0.0.4/limoon-logo.png
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/doc.yml
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 limoon-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/constant.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/core.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/exception.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/model.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 limoon-0.0.4/src/limoon/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 limoon-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 limoon-0.0.4/tests/test.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 limoon-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 limoon-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 limoon-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 limoon-0.0.4/PKG-INFO
```

### Comparing `limoon-0.0.2/limoon-logo.png` & `limoon-0.0.4/limoon-logo.png`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/.github/workflows/publish.yml` & `limoon-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/.github/workflows/test.yml` & `limoon-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/src/limoon/core.py` & `limoon-0.0.4/src/limoon/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 from http import HTTPStatus
-from typing import Iterator
+from typing import TypeVar, Iterator, Callable
 from urllib.parse import urlparse
 
 from requests_html import HTMLResponse, HTMLSession
 
 from limoon import constant, exception, model, utils
 
+
 # Typings
-_EntryID = int
-_TopicKeywords = str
-_Nickname = str
-_SearchKeywords = str
+EntryID = TypeVar("EntryID", Callable, int)
+TopicKeywords = TypeVar("TopicKeywords", Callable, str)
+Nickname = TypeVar("Nickname", Callable, str)
+SearchKeywords = TypeVar("SearchKeywords", Callable, str)
 
 # Session
 session = HTMLSession()
 
 
 def request(endpoint: str) -> HTMLResponse:
     return session.get(constant.BASE_URL + endpoint)
 
 
-def get_topic(topic_keywords: _TopicKeywords, max_entry: int = None) -> model.Topic:
+def get_topic(topic_keywords: TopicKeywords, max_entry: int = None) -> model.Topic:
+    """This function get Ekşi Sözlük topic.
+
+    Arguments:
+    topic_keywords (str): Keywords (or path) of topic to be get.
+    max_entry (int=None): Maximum number of entrys to be get from page.
+
+    Returns:
+    model.Topic (class): Topic data class.
+    """
+
     r = request(constant.TOPIC_ROUTE.format(topic_keywords))
 
     if r.status_code == HTTPStatus.NOT_FOUND:
         raise exception.TopicNotFound()
 
     h1 = r.html.find("h1#title", first=True)
     path = h1.find("a", first=True).attrs["href"]
@@ -35,29 +46,47 @@
         h1.attrs["data-title"],
         path[1:],
         utils.entry_parser(r.html, max_entry),
         int(page_count),
     )
 
 
-def get_entry(entry_id: _EntryID) -> model.Entry:
+def get_entry(entry_id: EntryID) -> model.Entry:
+    """This function get Ekşi Sözlük entry.
+
+    Arguments:
+    entry_id (int): Unique entry identity. 
+
+    Returns:
+    model.Entry (class): Entry data class.
+    """
+
     if not isinstance(entry_id, int):
         raise TypeError
 
     r = request(constant.ENTRY_ROUTE.format(entry_id))
 
     if r.status_code == HTTPStatus.NOT_FOUND:
         raise exception.EntryNotFound()
     if r.html.find("h1", first=True).text == exception.SHIT_MESSAGE:
         raise exception.EntryNotFound()
 
     return next(utils.entry_parser(r.html))
 
 
-def get_author(nickname: _Nickname) -> model.Author:
+def get_author(nickname: Nickname) -> model.Author:
+    """This function get Ekşi Sözlük author.
+
+    Arguments:
+    nickname (str): Unique author nickname. 
+
+    Returns:
+    model.Author (class): Author data class.
+    """
+
     r = request(constant.AUTHOR_ROUTE.format(nickname))
 
     if r.status_code == HTTPStatus.NOT_FOUND:
         raise exception.AuthorNotFound()
 
     nickname = r.html.find("h1#user-profile-title", first=True)
     biography = r.html.find("div#profile-biography", first=True)
@@ -83,14 +112,24 @@
 
 
 def get_author_topic():
     pass
 
 
 def get_agenda(max_topic: int = None, max_entry: int = None) -> Iterator[model.Topic]:
+    """This function get Ekşi Sözlük agenda (gündem) page.
+
+    Arguments:
+    max_topic (int=None): Maximum number of topics to be get from agenda.
+    max_entry (int=None): Maximum number of entrys to be get from topic.
+
+    Returns:
+    Iterator[model.Topic]: Topic data classes.
+    """
+
     r = request(constant.AGENDA_ROUTE)
 
     if r.status_code != HTTPStatus.OK:
         raise exception.TopicNotFound()
 
     topic_list = r.html.find("ul.topic-list", first=True).find("a")
 
@@ -98,22 +137,31 @@
         yield get_topic(
             urlparse(topic.attrs["href"]).path.split("/")[-1],
             max_entry,
         )
 
 
 def get_debe(max_entry: int = None) -> Iterator[model.Entry]:
+    """This function get Ekşi Sözlük debe page.
+
+    Arguments:
+    max_entry (int=None): Maximum number of entrys to be get page.
+
+    Returns:
+    Iterator[model.Topic]: Entry data classes.
+    """
+
     r = request(constant.DEBE_ROUTE)
 
     if r.status_code != HTTPStatus.OK:
         raise exception.EntryNotFound()
 
     topic_list = r.html.find("ul.topic-list", first=True).find("a")
 
     for topic in topic_list[:max_entry]:
         yield get_entry(
             urlparse(topic.attrs["href"]).path.split("/")[-1],
         )
 
 
-def search_topic(search_keywords: _SearchKeywords):
+def search_topic(search_keywords: SearchKeywords):
     pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `limoon-0.0.2/src/limoon/utils.py` & `limoon-0.0.4/src/limoon/utils.py`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/tests/test.py` & `limoon-0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/.gitignore` & `limoon-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/LICENSE.txt` & `limoon-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `limoon-0.0.2/pyproject.toml` & `limoon-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,27 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["requests-html", "lxml==4.9.4"]
 
 [project.urls]
 Source = "https://github.com/beucismis/limoon"
 Issues = "https://github.com/beucismis/limoon/issues"
-Documentation = "https://github.com/beucismis/limoon#readme"
+Documentation = "https://github.com/beucismis/limoon/DOCUMENTATION.md"
 
 [tool.hatch.version]
 path = "src/limoon/__init__.py"
 
 [tool.hatch.envs.default]
-dependencies = ["pytest"]
+dependencies = ["pytest", "pydoc-markdown"]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest tests/* -v"
+doc = "pydoc-markdown -I src --render-toc > DOCUMENTATION.md"
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-path = "README.md"
+path = "README.md"
```

