# Comparing `tmp/joo-0.1.0.138.tar.gz` & `tmp/joo-0.1.0.139.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joo-0.1.0.138.tar", last modified: Wed Apr  3 08:50:30 2024, max compression
+gzip compressed data, was "joo-0.1.0.139.tar", last modified: Thu Apr 11 09:21:51 2024, max compression
```

## Comparing `joo-0.1.0.138.tar` & `joo-0.1.0.139.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.627232 joo-0.1.0.138/
--rw-rw-rw-   0        0        0      625 2024-04-03 08:50:30.624237 joo-0.1.0.138/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-03 08:50:27.000000 joo-0.1.0.138/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.542096 joo-0.1.0.138/lib/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.569032 joo-0.1.0.138/lib/joo/
--rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.138/lib/joo/LICENSE
--rw-rw-rw-   0        0        0     4178 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/__version__.py
--rw-rw-rw-   0        0        0     2780 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/cli.py
--rw-rw-rw-   0        0        0    11405 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/logging.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.620250 joo-0.1.0.138/lib/joo/scraping/
--rw-rw-rw-   0        0        0     4374 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/__init__.py
--rw-rw-rw-   0        0        0     4927 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/http.py
--rw-rw-rw-   0        0        0    10402 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/selenium.py
--rw-rw-rw-   0        0        0    12263 2024-03-30 12:37:13.000000 joo-0.1.0.138/lib/joo/sysutil.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.606935 joo-0.1.0.138/lib/joo.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-03 08:50:29.000000 joo-0.1.0.138/lib/joo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:50:30.627232 joo-0.1.0.138/setup.cfg
--rw-rw-rw-   0        0        0     1424 2024-04-03 08:50:27.000000 joo-0.1.0.138/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.800181 joo-0.1.0.139/
+-rw-rw-rw-   0        0        0      625 2024-04-11 09:21:51.797304 joo-0.1.0.139/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-11 09:21:46.000000 joo-0.1.0.139/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.651939 joo-0.1.0.139/lib/
+drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.708979 joo-0.1.0.139/lib/joo/
+-rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.139/lib/joo/LICENSE
+-rw-rw-rw-   0        0        0     4178 2024-04-03 08:59:24.000000 joo-0.1.0.139/lib/joo/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/__version__.py
+-rw-rw-rw-   0        0        0     2780 2024-04-03 08:58:39.000000 joo-0.1.0.139/lib/joo/cli.py
+-rw-rw-rw-   0        0        0    12338 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/datetimeutil.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.791174 joo-0.1.0.139/lib/joo/dc/
+-rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/dc/__init__.py
+-rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.139/lib/joo/dc/http.py
+-rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.139/lib/joo/dc/selenium.py
+-rw-rw-rw-   0        0        0     5119 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/httpapi.py
+-rw-rw-rw-   0        0        0    12685 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/logging.py
+-rw-rw-rw-   0        0        0    15596 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/sysutil.py
+drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.773643 joo-0.1.0.139/lib/joo.egg-info/
+-rw-rw-rw-   0        0        0      625 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 09:21:51.805202 joo-0.1.0.139/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2024-04-11 09:21:46.000000 joo-0.1.0.139/setup.py
```

### Comparing `joo-0.1.0.138/PKG-INFO` & `joo-0.1.0.139/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.138
+Version: 0.1.0.139
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.138/lib/joo/LICENSE` & `joo-0.1.0.139/lib/joo/LICENSE`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.138/lib/joo/__init__.py` & `joo-0.1.0.139/lib/joo/__init__.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.138/lib/joo/__version__.py` & `joo-0.1.0.139/lib/joo/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 __VERSION__ = {
     "name": "joo",
     "description": "joo library",
     "version": "0.1.0",
-    "build": 138,
+    "build": 139,
     "license": "MIT License",
     "author": "Wooloo Studio",
     "author_email": "max.wu@wooloostudio.com",
     "url": "https://github.com/metatutu/joo",
     "project_urls": {
         "Documentation": "https://github.com/metatutu/joo",
         "Source Code": "https://github.com/metatutu/joo",
```

### Comparing `joo-0.1.0.138/lib/joo/cli.py` & `joo-0.1.0.139/lib/joo/cli.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.138/lib/joo/logging.py` & `joo-0.1.0.139/lib/joo/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -317,8 +317,40 @@
     def critical(self, message, depth=0, level=MessageLevel.CRITICAL):
         if self._logger: self._logger.critical(message, depth, level)
 
     def separator(self, ch="=", width=80, level=MessageLevel.SEPARATOR):
         if self._logger: self._logger.separator(ch, width, level)
 
     def exception(self, ex, depth=0, level=MessageLevel.DEBUG):
-        if self._logger: self._logger.exception(ex, depth, level)
+        if self._logger: self._logger.exception(ex, depth, level)
+
+    def error_x(self, x, message, depth=0, level=MessageLevel.ERROR):
+        self.error(message, depth, level)
+        return x
+
+    def error_n(self, message, depth=0, level=MessageLevel.ERROR):
+        return self.error_x(None, message, depth, level)
+
+    def error_f(self, message, depth=0, level=MessageLevel.ERROR):
+        return self.error_x(False, message, depth, level)
+
+    def error_0(self, message, depth=0, level=MessageLevel.ERROR):
+        return self.error_x(0, message, depth, level)
+
+    def error_1(self, message, depth=0, level=MessageLevel.ERROR):
+        return self.error_x(1, message, depth, level)
+    
+    def exception_x(self, x, ex, depth=0, level=MessageLevel.DEBUG):
+        self.exception(ex, depth, level)
+        return x
+    
+    def exception_n(self, ex, depth=0, level=MessageLevel.DEBUG):
+        return self.exception_x(None, ex, depth, level)
+
+    def exception_f(self, ex, depth=0, level=MessageLevel.DEBUG):
+        return self.exception_x(False, ex, depth, level)
+
+    def exception_0(self, ex, depth=0, level=MessageLevel.DEBUG):
+        return self.exception_x(0, ex, depth, level)
+
+    def exception_1(self, ex, depth=0, level=MessageLevel.DEBUG):
+        return self.exception_x(1, ex, depth, level)
```

### Comparing `joo-0.1.0.138/lib/joo/scraping/http.py` & `joo-0.1.0.139/lib/joo/dc/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     This file is part of joo library.
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 import requests
 import joo.sysutil as sysutil
-from joo.scraping import Session, Cache
+from joo.dc import Session, Cache
 
 class HttpSession(Session):
     def __init__(self):
         Session.__init__(self)
 
         # settings
         self.user_agent = None
```

### Comparing `joo-0.1.0.138/lib/joo/scraping/selenium.py` & `joo-0.1.0.139/lib/joo/dc/selenium.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,40 +3,26 @@
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 import os
 import time
 from selenium import webdriver
 from selenium.webdriver.common.by import By
-from selenium.webdriver.chrome.options import Options
 from bs4 import BeautifulSoup
 import joo.sysutil as sysutil
-from joo.scraping import Session, Cache
+from joo.dc import Session, Cache
 
 class WebDriverSession(Session):
     def __init__(self):
         Session.__init__(self)
 
         # settings
         self.webdriver = "chrome"
         self.desired_capabilities = None
-        options = Options()
-        options.add_argument("--no-sandbox")
-        options.add_argument("--disable-gpu")
-        options.add_argument("--disable-setuid-sandbox")
-        options.add_argument("--disable-extensions")
-        options.add_argument("--incognito")
-        options.add_argument("--disable-application-cache")
-        options.add_argument("--test-type")
-        options.add_argument("--js-flags=--expose-gc")
-        options.add_argument("--enable-precise-memory-info")
-        options.add_argument("--disable-default-apps")
-        options.add_argument("--window-size=1920,1080")
-        options.add_argument("--headless")
-        self.options = options
+        self.options = None
         self.default_timeout = 10.0
         self.default_wait = 0.5
         self.default_by = By.XPATH
 
     def open(self, **kwargs):
         try:
             if self._handle: return self._handle
```

### Comparing `joo-0.1.0.138/lib/joo/sysutil.py` & `joo-0.1.0.139/lib/joo/sysutil.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import uuid
 import shutil
 import base64
 import getopt
 import datetime
 import tempfile
 from joo import ManagedObject, ManagedObjects
+if os.name == "posix":
+    import fcntl
 
 def create_folder(folderpath):
     try:
         if not os.path.exists(folderpath): os.makedirs(folderpath)
     except:
         pass
     return os.path.isdir(folderpath)
@@ -309,14 +311,121 @@
     def get_temp_folderpath(self):
         return self.get_path(".temp")
     
     def create_temp_file(self): return create_temp_file(self.get_temp_folderpath())
 
     def create_temp_folder(self): return create_temp_folder(self.get_temp_folderpath())
 
+class ResourceLock(ManagedObject, FileSystemDataStore):
+    def __init__(self, id, temp_folderpath=None):
+        ManagedObject.__init__(self)
+        FileSystemDataStore.__init__(self, None)
+
+        # control
+        self.id = id
+        if temp_folderpath is None: temp_folderpath = tempfile.gettempdir()
+        self.root_folderpath = os.path.join(temp_folderpath, id)
+        self.lockfile = None
+
+    def __del__(self):
+        self.unlock()
+
+    @property
+    def state(self):
+        return self._state
+
+    def lockfile_filepath(self):
+        return self.get_path("lock.ctl", True)
+    
+    def is_locked(self):
+        filepath = self.lockfile_filepath()
+        if not file_exists(filepath): return False
+        if os.name == "nt":
+            try:
+                os.remove(filepath)
+                return False
+            except:
+                return True
+        elif os.name == "posix":
+            f = None
+            try:
+                f = open(filepath, "w")
+                fcntl.flock(f.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
+                f.close()
+                return False
+            except:
+                if f: f.close()
+                return True
+        else: raise Exception()
+
+    def lock(self):
+        if self._state: return self._state
+       
+        if self.is_locked():
+            self._state = "visitor"
+        else:
+            try:
+                # lock
+                self.lockfile = open(self.lockfile_filepath(), "w")
+                if os.name == "nt":
+                    pass
+                elif os.name == "posix":
+                    fcntl.flock(self.lockfile.fileno(), fcntl.LOCK_EX | fcntl.LOCK_NB)
+                else: raise Exception()
+
+                # update state
+                self._state = "owner"
+
+                # initialize workspace
+                self.initialize_workspace()
+            except:
+                if self.lockfile:
+                    self.lockfile.close()
+                    self.lockfile = None
+                self._state = None
+        return self._state
+    
+    def unlock(self):
+        if self._state == "owner":
+            # clean up workspace
+            self.cleanup_workspace()
+
+            # unlock
+            if os.name == "nt":
+                pass
+            elif os.name == "posix":
+                fcntl.flock(self.lockfile.fileno(), fcntl.LOCK_UN)
+            else: raise Exception()
+            self.lockfile.close()
+            self.lockfile = None
+            delete_file(self.lockfile_filepath())
+
+            # delete parent folder
+            delete_folder(self.root_folderpath)
+        self._state = None
+
+    def delete(self, gc=False):
+        self.unlock()
+
+    def initialize_workspace(self):
+        self.cleanup_workspace()
+
+    def cleanup_workspace(self):
+        fpath_lockfile = self.lockfile_filepath()
+        items = list_all(self.root_folderpath)
+        for fpath, is_folder in items:
+            print(fpath)
+            if is_folder:
+                delete_folder(fpath)
+            else:
+                if fpath == fpath_lockfile:
+                    print("skip")
+                    continue
+                delete_file(fpath)
+
 def parse_command_line(parts):
     """Parse command line.
 
     Syntax of command list is as:
     program <command 1> <command 2> ... [option 1] [option 2] ...
 
     Commands are required and options are optional, and commands are always
```

### Comparing `joo-0.1.0.138/lib/joo.egg-info/PKG-INFO` & `joo-0.1.0.139/lib/joo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.138
+Version: 0.1.0.139
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.138/setup.py` & `joo-0.1.0.139/setup.py`

 * *Files identical despite different names*

