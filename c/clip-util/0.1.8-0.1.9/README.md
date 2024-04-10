# Comparing `tmp/clip-util-0.1.8.tar.gz` & `tmp/clip-util-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip-util-0.1.8.tar", last modified: Wed May 25 05:31:43 2022, max compression
+gzip compressed data, was "clip-util-0.1.9.tar", last modified: Wed May 25 07:05:18 2022, max compression
```

## Comparing `clip-util-0.1.8.tar` & `clip-util-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-05-25 05:31:43.467089 clip-util-0.1.8/
--rw-rw-rw-   0        0        0     1190 2022-04-06 03:41:19.000000 clip-util-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2437 2022-05-25 05:31:43.466091 clip-util-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1671 2022-04-09 02:04:37.000000 clip-util-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2022-05-25 05:31:43.468088 clip-util-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1082 2022-05-25 05:29:42.000000 clip-util-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-05-25 05:31:43.428063 clip-util-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-05-25 05:31:43.456088 clip-util-0.1.8/src/clip_util.egg-info/
--rw-rw-rw-   0        0        0     2437 2022-05-25 05:31:42.000000 clip-util-0.1.8/src/clip_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2022-05-25 05:31:43.000000 clip-util-0.1.8/src/clip_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-25 05:31:42.000000 clip-util-0.1.8/src/clip_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-05-25 05:31:43.000000 clip-util-0.1.8/src/clip_util.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-25 05:31:43.465089 clip-util-0.1.8/src/clipboard/
--rw-rw-rw-   0        0        0      424 2022-05-25 04:36:21.000000 clip-util-0.1.8/src/clipboard/__init__.py
--rw-rw-rw-   0        0        0     2483 2022-05-25 03:31:21.000000 clip-util-0.1.8/src/clipboard/_c_interface.py
--rw-rw-rw-   0        0        0     1851 2022-05-25 03:31:21.000000 clip-util-0.1.8/src/clipboard/_logging.py
--rw-rw-rw-   0        0        0     9387 2022-05-25 05:03:29.000000 clip-util-0.1.8/src/clipboard/clipboard.py
--rw-rw-rw-   0        0        0       58 2022-05-25 03:31:21.000000 clip-util-0.1.8/src/clipboard/constants.py
--rw-rw-rw-   0        0        0     2565 2022-05-25 03:31:21.000000 clip-util-0.1.8/src/clipboard/formats.py
--rw-rw-rw-   0        0        0     6859 2022-05-25 03:31:21.000000 clip-util-0.1.8/src/clipboard/html_clipboard.py
+drwxrwxrwx   0        0        0        0 2022-05-25 07:05:18.243408 clip-util-0.1.9/
+-rw-rw-rw-   0        0        0     1190 2022-04-06 03:41:19.000000 clip-util-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2437 2022-05-25 07:05:18.241408 clip-util-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1671 2022-04-09 02:04:37.000000 clip-util-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-05-25 07:05:18.243408 clip-util-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2022-05-25 07:04:52.000000 clip-util-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-05-25 07:05:18.215408 clip-util-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-05-25 07:05:18.228408 clip-util-0.1.9/src/clip_util.egg-info/
+-rw-rw-rw-   0        0        0     2437 2022-05-25 07:05:17.000000 clip-util-0.1.9/src/clip_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2022-05-25 07:05:18.000000 clip-util-0.1.9/src/clip_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-05-25 07:05:17.000000 clip-util-0.1.9/src/clip_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2022-05-25 07:05:17.000000 clip-util-0.1.9/src/clip_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-05-25 07:05:18.238407 clip-util-0.1.9/src/clipboard/
+-rw-rw-rw-   0        0        0      424 2022-05-25 04:36:21.000000 clip-util-0.1.9/src/clipboard/__init__.py
+-rw-rw-rw-   0        0        0     2483 2022-05-25 03:31:21.000000 clip-util-0.1.9/src/clipboard/_c_interface.py
+-rw-rw-rw-   0        0        0     1851 2022-05-25 03:31:21.000000 clip-util-0.1.9/src/clipboard/_logging.py
+-rw-rw-rw-   0        0        0     9403 2022-05-25 07:04:24.000000 clip-util-0.1.9/src/clipboard/clipboard.py
+-rw-rw-rw-   0        0        0       58 2022-05-25 03:31:21.000000 clip-util-0.1.9/src/clipboard/constants.py
+-rw-rw-rw-   0        0        0     2565 2022-05-25 03:31:21.000000 clip-util-0.1.9/src/clipboard/formats.py
+-rw-rw-rw-   0        0        0     6859 2022-05-25 03:31:21.000000 clip-util-0.1.9/src/clipboard/html_clipboard.py
```

### Comparing `clip-util-0.1.8/LICENSE` & `clip-util-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clip-util-0.1.8/PKG-INFO` & `clip-util-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip-util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities for use with Python.
 Home-page: https://github.com/AceofSpades5757/clip-util
 Author: Kyle L. Davis
 Author-email: AceofSpades5757.github@gmail.com
 License: MIT
 Project-URL: Documentation, https://clip-util.readthedocs.io/en/latest/
 Project-URL: Author, https://github.com/AceofSpades5757
```

### Comparing `clip-util-0.1.8/README.md` & `clip-util-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clip-util-0.1.8/setup.py` & `clip-util-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fin:
     long_description = fin.read()
 
 
 setuptools.setup(
     name="clip-util",
-    version="0.1.8",
+    version="0.1.9",
     author="Kyle L. Davis",
     author_email="AceofSpades5757.github@gmail.com",
     url="https://github.com/AceofSpades5757/clip-util",
     project_urls={
         "Documentation": "https://clip-util.readthedocs.io/en/latest/",
         "Author": "https://github.com/AceofSpades5757",
     },
```

### Comparing `clip-util-0.1.8/src/clip_util.egg-info/PKG-INFO` & `clip-util-0.1.9/src/clip_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip-util
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities for use with Python.
 Home-page: https://github.com/AceofSpades5757/clip-util
 Author: Kyle L. Davis
 Author-email: AceofSpades5757.github@gmail.com
 License: MIT
 Project-URL: Documentation, https://clip-util.readthedocs.io/en/latest/
 Project-URL: Author, https://github.com/AceofSpades5757
```

### Comparing `clip-util-0.1.8/src/clipboard/_c_interface.py` & `clip-util-0.1.9/src/clipboard/_c_interface.py`

 * *Files identical despite different names*

### Comparing `clip-util-0.1.8/src/clipboard/_logging.py` & `clip-util-0.1.9/src/clipboard/_logging.py`

 * *Files identical despite different names*

### Comparing `clip-util-0.1.8/src/clipboard/clipboard.py` & `clip-util-0.1.9/src/clipboard/clipboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 hMem = HANDLE  # Type Alias
 logger = get_logger(__name__)
 
 
 def get_clipboard(format: Union[int, ClipboardFormat] = None) -> Optional[str]:
     """Conveniency wrapper to get clipboard."""
     with Clipboard() as cb:
-        return cb.get_clipboard(format=format)
+        text = cb.get_clipboard(format=format)
+    return text
 
 
 def set_clipboard(
     content: str, format: Union[int, ClipboardFormat] = None
 ) -> None:
     """Conveniency wrapper to set clipboard."""
     with Clipboard() as cb:
```

### Comparing `clip-util-0.1.8/src/clipboard/formats.py` & `clip-util-0.1.9/src/clipboard/formats.py`

 * *Files identical despite different names*

### Comparing `clip-util-0.1.8/src/clipboard/html_clipboard.py` & `clip-util-0.1.9/src/clipboard/html_clipboard.py`

 * *Files identical despite different names*

