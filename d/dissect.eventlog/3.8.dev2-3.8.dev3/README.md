# Comparing `tmp/dissect.eventlog-3.8.dev2.tar.gz` & `tmp/dissect.eventlog-3.8.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.eventlog-3.8.dev2.tar", last modified: Thu Mar 21 10:15:55 2024, max compression
+gzip compressed data, was "dissect.eventlog-3.8.dev3.tar", last modified: Thu Mar 28 17:21:53 2024, max compression
```

## Comparing `dissect.eventlog-3.8.dev2.tar` & `dissect.eventlog-3.8.dev3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.534538 dissect.eventlog-3.8.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-21 10:15:55.534538 dissect.eventlog-3.8.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.522538 dissect.eventlog-3.8.dev2/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.526538 dissect.eventlog-3.8.dev2/dissect/eventlog/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22978 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/bxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/evtx.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/wevt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/wevt_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/dissect/eventlog/wevtutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.530538 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-21 10:15:55.000000 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-21 10:15:55.000000 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:15:55.000000 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-21 10:15:55.000000 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-21 10:15:55.000000 dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.530538 dissect.eventlog-3.8.dev2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/parse_wevt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/pool_evtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/pool_wevtutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/scrape_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/scrape_evtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/splunkify_evtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/examples/splunkify_wevtutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-21 10:15:50.000000 dissect.eventlog-3.8.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:15:55.534538 dissect.eventlog-3.8.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.530538 dissect.eventlog-3.8.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.530538 dissect.eventlog-3.8.dev2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/data/TestLog-dirty.evt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/data/TestLog.evt
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/data/TestLogX.evtx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:15:55.530538 dissect.eventlog-3.8.dev2/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_binxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_crim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_evt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_evtx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_maps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_wevt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_wevt_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tests/test_wevtobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-21 10:15:46.000000 dissect.eventlog-3.8.dev2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.094890 dissect.eventlog-3.8.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-28 17:21:53.090890 dissect.eventlog-3.8.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.082890 dissect.eventlog-3.8.dev3/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.086890 dissect.eventlog-3.8.dev3/dissect/eventlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22978 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/bxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/evtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/wevt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/wevt_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/dissect/eventlog/wevtutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.090890 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-03-28 17:21:53.000000 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-28 17:21:53.000000 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:21:53.000000 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:21:53.000000 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:21:53.000000 dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.086890 dissect.eventlog-3.8.dev3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/parse_wevt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/pool_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/pool_wevtutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/scrape_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/scrape_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/splunkify_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/examples/splunkify_wevtutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-28 17:21:46.000000 dissect.eventlog-3.8.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:21:53.094890 dissect.eventlog-3.8.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.090890 dissect.eventlog-3.8.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.090890 dissect.eventlog-3.8.dev3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    65536 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/data/TestLog-dirty.evt
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/data/TestLog.evt
+-rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/data/TestLogX.evtx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:21:53.090890 dissect.eventlog-3.8.dev3/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_binxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_crim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_evt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_evtx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_maps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_wevt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_wevt_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tests/test_wevtobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-28 17:21:40.000000 dissect.eventlog-3.8.dev3/tox.ini
```

### Comparing `dissect.eventlog-3.8.dev2/LICENSE` & `dissect.eventlog-3.8.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/PKG-INFO` & `dissect.eventlog-3.8.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.eventlog
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.eventlog
 Project-URL: repository, https://github.com/fox-it/dissect.eventlog
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.eventlog-3.8.dev2/README.md` & `dissect.eventlog-3.8.dev3/README.md`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/bxml.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/bxml.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/evt.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/evtx.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/wevt.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/wevt_object.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/wevt_object.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect/eventlog/wevtutil.py` & `dissect.eventlog-3.8.dev3/dissect/eventlog/wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/PKG-INFO` & `dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.eventlog
-Version: 3.8.dev2
+Version: 3.8.dev3
 Summary: A Dissect module implementing parsers for the Windows EVT, EVTX and WEVT log file formats
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.eventlog
 Project-URL: repository, https://github.com/fox-it/dissect.eventlog
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.eventlog-3.8.dev2/dissect.eventlog.egg-info/SOURCES.txt` & `dissect.eventlog-3.8.dev3/dissect.eventlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/parse_wevt.py` & `dissect.eventlog-3.8.dev3/examples/parse_wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/pool_evtx.py` & `dissect.eventlog-3.8.dev3/examples/pool_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/pool_wevtutil.py` & `dissect.eventlog-3.8.dev3/examples/pool_wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/scrape_evt.py` & `dissect.eventlog-3.8.dev3/examples/scrape_evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/scrape_evtx.py` & `dissect.eventlog-3.8.dev3/examples/scrape_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/splunkify_evtx.py` & `dissect.eventlog-3.8.dev3/examples/splunkify_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/examples/splunkify_wevtutil.py` & `dissect.eventlog-3.8.dev3/examples/splunkify_wevtutil.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/pyproject.toml` & `dissect.eventlog-3.8.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/_utils.py` & `dissect.eventlog-3.8.dev3/tests/_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/data/TestLog-dirty.evt` & `dissect.eventlog-3.8.dev3/tests/data/TestLog-dirty.evt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/data/TestLog.evt` & `dissect.eventlog-3.8.dev3/tests/data/TestLog.evt`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/data/TestLogX.evtx` & `dissect.eventlog-3.8.dev3/tests/data/TestLogX.evtx`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/docs/Makefile` & `dissect.eventlog-3.8.dev3/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/docs/conf.py` & `dissect.eventlog-3.8.dev3/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_binxml.py` & `dissect.eventlog-3.8.dev3/tests/test_binxml.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_crim.py` & `dissect.eventlog-3.8.dev3/tests/test_crim.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_evt.py` & `dissect.eventlog-3.8.dev3/tests/test_evt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_evtx.py` & `dissect.eventlog-3.8.dev3/tests/test_evtx.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_maps.py` & `dissect.eventlog-3.8.dev3/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_wevt.py` & `dissect.eventlog-3.8.dev3/tests/test_wevt.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_wevt_type.py` & `dissect.eventlog-3.8.dev3/tests/test_wevt_type.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tests/test_wevtobj.py` & `dissect.eventlog-3.8.dev3/tests/test_wevtobj.py`

 * *Files identical despite different names*

### Comparing `dissect.eventlog-3.8.dev2/tox.ini` & `dissect.eventlog-3.8.dev3/tox.ini`

 * *Files identical despite different names*

