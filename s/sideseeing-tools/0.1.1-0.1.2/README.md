# Comparing `tmp/sideseeing-tools-0.1.1.tar.gz` & `tmp/sideseeing-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing-tools-0.1.1.tar", last modified: Thu Apr 11 18:59:44 2024, max compression
+gzip compressed data, was "sideseeing-tools-0.1.2.tar", last modified: Thu Apr 11 19:05:53 2024, max compression
```

## Comparing `sideseeing-tools-0.1.1.tar` & `sideseeing-tools-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 18:59:44.337139 sideseeing-tools-0.1.1/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing-tools-0.1.1/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 18:59:44.337139 sideseeing-tools-0.1.1/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3595 2024-04-11 18:55:32.000000 sideseeing-tools-0.1.1/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      881 2024-04-11 18:59:11.000000 sideseeing-tools-0.1.1/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-11 18:59:44.337139 sideseeing-tools-0.1.1/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 18:59:44.333140 sideseeing-tools-0.1.1/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 18:59:44.337139 sideseeing-tools-0.1.1/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1039 2024-04-11 18:29:12.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2846 2024-04-11 16:52:19.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    22581 2024-04-11 18:32:40.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5577 2024-04-11 18:31:34.000000 sideseeing-tools-0.1.1/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 18:59:44.337139 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 18:59:44.000000 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      448 2024-04-11 18:59:44.000000 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-11 18:59:44.000000 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      137 2024-04-11 18:59:44.000000 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-11 18:59:44.000000 sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing-tools-0.1.2/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3595 2024-04-11 18:55:32.000000 sideseeing-tools-0.1.2/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      881 2024-04-11 19:05:38.000000 sideseeing-tools-0.1.2/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.453845 sideseeing-tools-0.1.2/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1039 2024-04-11 18:29:12.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2846 2024-04-11 16:52:19.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    22581 2024-04-11 18:32:40.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5577 2024-04-11 18:31:34.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      448 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      137 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/top_level.txt
```

### Comparing `sideseeing-tools-0.1.1/LICENSE` & `sideseeing-tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/PKG-INFO` & `sideseeing-tools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: folium~=0.13.0
-Requires-Dist: imageio~=2.4.0
+Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
-Requires-Dist: matplotlib~=3.6.3
-Requires-Dist: numpy~=1.23.0
-Requires-Dist: pandas~=2.1.0
+Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: numpy~=1.24.1
+Requires-Dist: opencv-python~=4.7.0.68
+Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
```

### Comparing `sideseeing-tools-0.1.1/README.md` & `sideseeing-tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/pyproject.toml` & `sideseeing-tools-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "sideseeing-tools"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-  "opencv-python~=4.7.0.68",
   "folium~=0.13.0",
-  "imageio~=2.4.0",
+  "imageio~=2.5.0",
   "librosa~=0.10.0",
-  "matplotlib~=3.6.3",
-  "numpy~=1.23.0",
-  "pandas~=2.1.0",
+  "matplotlib~=3.7.1",
+  "numpy~=1.24.1",
+  "opencv-python~=4.7.0.68",
+  "pandas~=2.0.3",
   "reverse-geocode==1.6",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
```

### Comparing `sideseeing-tools-0.1.1/src/sideseeing_tools/constants.py` & `sideseeing-tools-0.1.2/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/src/sideseeing_tools/media.py` & `sideseeing-tools-0.1.2/src/sideseeing_tools/media.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/src/sideseeing_tools/sideseeing.py` & `sideseeing-tools-0.1.2/src/sideseeing_tools/sideseeing.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/src/sideseeing_tools/utils.py` & `sideseeing-tools-0.1.2/src/sideseeing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.1/src/sideseeing_tools.egg-info/PKG-INFO` & `sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: folium~=0.13.0
-Requires-Dist: imageio~=2.4.0
+Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
-Requires-Dist: matplotlib~=3.6.3
-Requires-Dist: numpy~=1.23.0
-Requires-Dist: pandas~=2.1.0
+Requires-Dist: matplotlib~=3.7.1
+Requires-Dist: numpy~=1.24.1
+Requires-Dist: opencv-python~=4.7.0.68
+Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
```

