# Comparing `tmp/qrawl-0.1.3.tar.gz` & `tmp/qrawl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.1.3.tar", max compression
+gzip compressed data, was "qrawl-0.1.4.tar", max compression
```

## Comparing `qrawl-0.1.3.tar` & `qrawl-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.3/LICENSE
--rw-r--r--   0        0        0      794 2024-04-11 03:01:53.855704 qrawl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.3/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.3/qrawl/common.py
--rw-r--r--   0        0        0      352 2024-04-10 20:17:48.317729 qrawl-0.1.3/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.3/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.3/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.3/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.3/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.3/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.3/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.3/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3969 2024-04-11 03:01:43.987146 qrawl-0.1.3/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.3/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.3/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     6682 2024-04-10 20:17:48.321751 qrawl-0.1.3/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     1769 2024-04-10 20:17:48.318749 qrawl-0.1.3/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    15739 2024-04-10 20:18:05.786010 qrawl-0.1.3/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.3/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.3/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.1.4/LICENSE
+-rw-r--r--   0        0        0      794 2024-04-11 05:25:18.900104 qrawl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.1.4/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.1.4/qrawl/common.py
+-rw-r--r--   0        0        0      352 2024-04-10 20:17:48.317729 qrawl-0.1.4/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.1.4/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.1.4/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.1.4/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.1.4/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.1.4/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.1.4/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.1.4/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3976 2024-04-11 05:24:25.355092 qrawl-0.1.4/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.1.4/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.1.4/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     6682 2024-04-10 20:17:48.321751 qrawl-0.1.4/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     1769 2024-04-10 20:17:48.318749 qrawl-0.1.4/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    15739 2024-04-10 20:18:05.786010 qrawl-0.1.4/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.1.4/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.1.4/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.1.4/PKG-INFO
```

### Comparing `qrawl-0.1.3/LICENSE` & `qrawl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/pyproject.toml` & `qrawl-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.1.3/qrawl/common.py` & `qrawl-0.1.4/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/google_sheets/column.py` & `qrawl-0.1.4/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.1.4/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/playwright/async_api/common.py` & `qrawl-0.1.4/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/playwright/sync_api/common.py` & `qrawl-0.1.4/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.1.4/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 def wait_for_text(page: Page, selector: str):
     """
     Wait for element to have text.
     """
     page.wait_for_selector(selector)
     # Wait for the text to not be empty
-    page.wait_for_function(
+    return page.wait_for_function(
         f"() => {{return document.querySelector('{selector}').innerText.trim() !== '';}}"
     )
 
 
 class QSyncPlaywright:
     def __init__(self):
         self._p = None
```

### Comparing `qrawl-0.1.3/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.1.4/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/selenium/exceptions.py` & `qrawl-0.1.4/qrawl/selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/selenium/selenium.py` & `qrawl-0.1.4/qrawl/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.1.3/qrawl/xpath.py` & `qrawl-0.1.4/qrawl/xpath.py`

 * *Files identical despite different names*

