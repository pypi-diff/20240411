# Comparing `tmp/mymodules-7.0.5.tar.gz` & `tmp/mymodules-7.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mymodules-7.0.5.tar", last modified: Fri Mar  1 07:39:17 2024, max compression
+gzip compressed data, was "mymodules-7.0.6.tar", last modified: Thu Apr 11 06:54:53 2024, max compression
```

## Comparing `mymodules-7.0.5.tar` & `mymodules-7.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-03-01 07:39:17.186584 mymodules-7.0.5/
--rw-r--r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      761 2024-03-01 07:39:17.186584 mymodules-7.0.5/PKG-INFO
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      245 2024-03-01 06:36:15.000000 mymodules-7.0.5/README.md
-drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-03-01 07:39:17.186584 mymodules-7.0.5/Xbyte_Common_Scrape/
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-01-01 14:57:45.000000 mymodules-7.0.5/Xbyte_Common_Scrape/__init__.py
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)    37256 2024-03-01 06:36:05.000000 mymodules-7.0.5/Xbyte_Common_Scrape/mymodules.py
-drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-03-01 07:39:17.186584 mymodules-7.0.5/mymodules.egg-info/
--rw-r--r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      761 2024-03-01 07:39:17.000000 mymodules-7.0.5/mymodules.egg-info/PKG-INFO
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      215 2024-03-01 07:39:17.000000 mymodules-7.0.5/mymodules.egg-info/SOURCES.txt
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        1 2024-03-01 07:39:17.000000 mymodules-7.0.5/mymodules.egg-info/dependency_links.txt
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)       20 2024-03-01 07:39:17.000000 mymodules-7.0.5/mymodules.egg-info/top_level.txt
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)       38 2024-03-01 07:39:17.186584 mymodules-7.0.5/setup.cfg
--rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)     1157 2024-03-01 07:38:52.000000 mymodules-7.0.5/setup.py
+drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-04-11 06:54:53.921875 mymodules-7.0.6/
+-rw-r--r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      761 2024-04-11 06:54:53.921875 mymodules-7.0.6/PKG-INFO
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      245 2024-04-11 06:51:20.000000 mymodules-7.0.6/README.md
+drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-04-11 06:54:53.921875 mymodules-7.0.6/Xbyte_Common_Scrape/
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-01-01 14:57:45.000000 mymodules-7.0.6/Xbyte_Common_Scrape/__init__.py
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)    37333 2024-04-11 06:50:02.000000 mymodules-7.0.6/Xbyte_Common_Scrape/mymodules.py
+drwxrwxr-x   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        0 2024-04-11 06:54:53.921875 mymodules-7.0.6/mymodules.egg-info/
+-rw-r--r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      761 2024-04-11 06:54:53.000000 mymodules-7.0.6/mymodules.egg-info/PKG-INFO
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)      215 2024-04-11 06:54:53.000000 mymodules-7.0.6/mymodules.egg-info/SOURCES.txt
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)        1 2024-04-11 06:54:53.000000 mymodules-7.0.6/mymodules.egg-info/dependency_links.txt
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)       20 2024-04-11 06:54:53.000000 mymodules-7.0.6/mymodules.egg-info/top_level.txt
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)       38 2024-04-11 06:54:53.921875 mymodules-7.0.6/setup.cfg
+-rw-rw-r--   0 ravi.bambhaniya  (1001) ravi.bambhaniya  (1001)     1157 2024-04-11 06:51:13.000000 mymodules-7.0.6/setup.py
```

### Comparing `mymodules-7.0.5/PKG-INFO` & `mymodules-7.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymodules
-Version: 7.0.5
+Version: 7.0.6
 Summary: Simple helping tool for scraping
 Author: XBYTE
 Author-email: <mail@neuralnine.com>
 Keywords: json,pymysql,requests,random_user_agent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,8 +23,8 @@
 <li>Python 3.4+</li>
 <li>Works on Linux, Windows, Mac</li>
 </ul>
 
 <h2>Install</h2>
 
 <p>The quick way:</p>
-<pre>pip install mymodules==7.0.5</pre>
+<pre>pip install mymodules==7.0.6</pre>
```

### Comparing `mymodules-7.0.5/Xbyte_Common_Scrape/mymodules.py` & `mymodules-7.0.6/Xbyte_Common_Scrape/mymodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pandas as pd
 import pymongo
 import json
 import collections
 import pymysql
 from scrapy import Selector
 from typing import Union
+import emoji
 
 class YourFrameworkErrorCodes:
     SUCCESS = 0
     ERROR_CODE = 1
 
 class ScrapyAutomation:
 
@@ -363,14 +364,15 @@
             html = re.sub("<script[^>]*>([\w\W]*?)</script>", " ", html)
             html = re.sub("\* style specs start[^>]*>([\w\W]*?)style specs end *", " ", html)
             html = re.sub("<style[^>]*>([\w\W]*?)</style>", " ", html)
             html = re.sub("<!--([\w\W]*?)-->", " ", html)
             html = re.sub("<([\w\W]*?)>", " ", html)
             html = re.sub("<.*?>", " ", html)
             html = re.sub(" +", " ", html)
+            html = str(emoji.get_emoji_regexp().sub(u'', html))
 
             return html.strip()
 
         elif isinstance(html, list):
             return [j for j in [ScrapyAutomation.c_replace(i) for i in html] if j]
         else:
             raise TypeError(f'must be str or list - object pass is ({type(html)}) object....')
```

### Comparing `mymodules-7.0.5/mymodules.egg-info/PKG-INFO` & `mymodules-7.0.6/mymodules.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mymodules
-Version: 7.0.5
+Version: 7.0.6
 Summary: Simple helping tool for scraping
 Author: XBYTE
 Author-email: <mail@neuralnine.com>
 Keywords: json,pymysql,requests,random_user_agent
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -23,8 +23,8 @@
 <li>Python 3.4+</li>
 <li>Works on Linux, Windows, Mac</li>
 </ul>
 
 <h2>Install</h2>
 
 <p>The quick way:</p>
-<pre>pip install mymodules==7.0.5</pre>
+<pre>pip install mymodules==7.0.6</pre>
```

### Comparing `mymodules-7.0.5/setup.py` & `mymodules-7.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '7.0.5'
+VERSION = '7.0.6'
 DESCRIPTION = 'use for easy scraping'
 LONG_DESCRIPTION = 'scraping'
 
 # Setting up
 setup(
     name="mymodules",
     version=VERSION,
```

