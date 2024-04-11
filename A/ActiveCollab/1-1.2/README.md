# Comparing `tmp/ActiveCollab-1.tar.gz` & `tmp/ActiveCollab-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ActiveCollab-1.tar", last modified: Wed Apr 10 10:59:11 2024, max compression
+gzip compressed data, was "ActiveCollab-1.2.tar", last modified: Thu Apr 11 02:28:04 2024, max compression
```

## Comparing `ActiveCollab-1.tar` & `ActiveCollab-1.2.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:59:11.812249 ActiveCollab-1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:59:11.812249 ActiveCollab-1/ActiveCollab/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-10 10:59:06.000000 ActiveCollab-1/ActiveCollab/ActiveCollab.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 10:59:06.000000 ActiveCollab-1/ActiveCollab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:59:11.812249 ActiveCollab-1/ActiveCollab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 10:59:11.000000 ActiveCollab-1/ActiveCollab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-10 10:59:11.000000 ActiveCollab-1/ActiveCollab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:59:11.000000 ActiveCollab-1/ActiveCollab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 10:59:11.000000 ActiveCollab-1/ActiveCollab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 10:59:11.000000 ActiveCollab-1/ActiveCollab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 10:59:06.000000 ActiveCollab-1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 10:59:11.812249 ActiveCollab-1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 10:59:06.000000 ActiveCollab-1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:59:11.812249 ActiveCollab-1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 10:59:06.000000 ActiveCollab-1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.755606 ActiveCollab-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.751605 ActiveCollab-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.751605 ActiveCollab-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-11 02:27:59.000000 ActiveCollab-1.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 02:27:59.000000 ActiveCollab-1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.751605 ActiveCollab-1.2/ActiveCollab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-11 02:27:59.000000 ActiveCollab-1.2/ActiveCollab/ActiveCollab.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 02:27:59.000000 ActiveCollab-1.2/ActiveCollab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.751605 ActiveCollab-1.2/ActiveCollab/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-11 02:27:59.000000 ActiveCollab-1.2/ActiveCollab/__pycache__/ActiveCollab.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:28:04.755606 ActiveCollab-1.2/ActiveCollab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 02:28:04.000000 ActiveCollab-1.2/ActiveCollab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-11 02:28:04.000000 ActiveCollab-1.2/ActiveCollab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:28:04.000000 ActiveCollab-1.2/ActiveCollab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-11 02:28:04.000000 ActiveCollab-1.2/ActiveCollab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 02:28:04.000000 ActiveCollab-1.2/ActiveCollab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-11 02:27:59.000000 ActiveCollab-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-11 02:28:04.755606 ActiveCollab-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-11 02:27:59.000000 ActiveCollab-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-11 02:27:59.000000 ActiveCollab-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:28:04.755606 ActiveCollab-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-11 02:27:59.000000 ActiveCollab-1.2/setup.py_bck
```

### Comparing `ActiveCollab-1/ActiveCollab/ActiveCollab.py` & `ActiveCollab-1.2/ActiveCollab/ActiveCollab.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from selenium.webdriver.common.by import By
 import undetected_chromedriver as uc
 from urllib.parse import quote
 from re import fullmatch
 import time , os
 
 
-class Main:
+class Connect:
     def __init__(self , host_url , login_email , login_password):
         self.host_url = host_url.rsplit('/' , (host_url.count('/') - 2))[0]
         chrome_service = Service(ChromeDriverManager(chrome_type=ChromeType.CHROMIUM).install())
 
         chrome_options = Options()
         options = [
             "--headless" ,
```

### Comparing `ActiveCollab-1/ActiveCollab.egg-info/PKG-INFO` & `ActiveCollab-1.2/ActiveCollab.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 1
-Summary: A Python module to interact with ActiveCollab
-Home-page: https://github.com/Ankushtpss/ActiveCollab
-Author: ankushtpss
-Author-email: ankushkumartpss@gmail.com
-Keywords: ActiveCollab active collab
-Requires-Python: >=3.10
+Version: 1.2
+Summary: A Python module to interact with ActiveCollab and perform certain actions
+Author-email: Ankushtpss <ankushkumartpss@gmail.com>
+Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
+Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: webdriver_manager
 
 # ActiveCollab
```

### Comparing `ActiveCollab-1/LICENSE` & `ActiveCollab-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ActiveCollab-1/PKG-INFO` & `ActiveCollab-1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: ActiveCollab
-Version: 1
-Summary: A Python module to interact with ActiveCollab
-Home-page: https://github.com/Ankushtpss/ActiveCollab
-Author: ankushtpss
-Author-email: ankushkumartpss@gmail.com
-Keywords: ActiveCollab active collab
-Requires-Python: >=3.10
+Version: 1.2
+Summary: A Python module to interact with ActiveCollab and perform certain actions
+Author-email: Ankushtpss <ankushkumartpss@gmail.com>
+Project-URL: Homepage, https://github.com/Ankushtpss/ActiveCollab
+Project-URL: Bug Tracker, https://github.com/Ankushtpss/ActiveCollab/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: selenium
 Requires-Dist: webdriver_manager
 
 # ActiveCollab
```

### Comparing `ActiveCollab-1/setup.py` & `ActiveCollab-1.2/setup.py_bck`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     description="A Python module to interact with ActiveCollab",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     author="ankushtpss",
     author_email="ankushkumartpss@gmail.com",
     packages = find_packages(),
-    python_requires='>=3.10',
+    python_requires='>=3.8',
     url='https://github.com/Ankushtpss/ActiveCollab',
     keywords='ActiveCollab active collab',
     install_requires=[
           'selenium',
           'webdriver_manager',
       ],
```

