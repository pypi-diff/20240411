# Comparing `tmp/sideseeing-tools-0.1.2.tar.gz` & `tmp/sideseeing-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing-tools-0.1.2.tar", last modified: Thu Apr 11 19:05:53 2024, max compression
+gzip compressed data, was "sideseeing-tools-0.1.3.tar", last modified: Thu Apr 11 19:09:02 2024, max compression
```

## Comparing `sideseeing-tools-0.1.2.tar` & `sideseeing-tools-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing-tools-0.1.2/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3595 2024-04-11 18:55:32.000000 sideseeing-tools-0.1.2/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      881 2024-04-11 19:05:38.000000 sideseeing-tools-0.1.2/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.453845 sideseeing-tools-0.1.2/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1039 2024-04-11 18:29:12.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2846 2024-04-11 16:52:19.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    22581 2024-04-11 18:32:40.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5577 2024-04-11 18:31:34.000000 sideseeing-tools-0.1.2/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:05:53.457845 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      448 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      137 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-11 19:05:53.000000 sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:09:02.044262 sideseeing-tools-0.1.3/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-07 01:01:40.000000 sideseeing-tools-0.1.3/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:09:02.040262 sideseeing-tools-0.1.3/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3595 2024-04-11 18:55:32.000000 sideseeing-tools-0.1.3/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      881 2024-04-11 19:08:52.000000 sideseeing-tools-0.1.3/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-11 19:09:02.044262 sideseeing-tools-0.1.3/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:09:02.036262 sideseeing-tools-0.1.3/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:09:02.036262 sideseeing-tools-0.1.3/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-07 00:47:46.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1039 2024-04-11 18:29:12.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-11 14:29:01.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2846 2024-04-11 16:52:19.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    22581 2024-04-11 18:32:40.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5577 2024-04-11 18:31:34.000000 sideseeing-tools-0.1.3/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-11 19:09:02.040262 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4477 2024-04-11 19:09:02.000000 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      448 2024-04-11 19:09:02.000000 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-11 19:09:02.000000 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      137 2024-04-11 19:09:02.000000 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-11 19:09:02.000000 sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/top_level.txt
```

### Comparing `sideseeing-tools-0.1.2/LICENSE` & `sideseeing-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/PKG-INFO` & `sideseeing-tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.2
+Version: 0.1.3
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
 Requires-Dist: folium~=0.13.0
 Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
 Requires-Dist: matplotlib~=3.7.1
-Requires-Dist: numpy~=1.24.1
+Requires-Dist: numpy~=1.25.0
 Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
```

### Comparing `sideseeing-tools-0.1.2/README.md` & `sideseeing-tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/pyproject.toml` & `sideseeing-tools-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "sideseeing-tools"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "folium~=0.13.0",
   "imageio~=2.5.0",
   "librosa~=0.10.0",
   "matplotlib~=3.7.1",
-  "numpy~=1.24.1",
+  "numpy~=1.25.0",
   "opencv-python~=4.7.0.68",
   "pandas~=2.0.3",
   "reverse-geocode==1.6",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `sideseeing-tools-0.1.2/src/sideseeing_tools/constants.py` & `sideseeing-tools-0.1.3/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/src/sideseeing_tools/media.py` & `sideseeing-tools-0.1.3/src/sideseeing_tools/media.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/src/sideseeing_tools/sideseeing.py` & `sideseeing-tools-0.1.3/src/sideseeing_tools/sideseeing.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/src/sideseeing_tools/utils.py` & `sideseeing-tools-0.1.3/src/sideseeing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sideseeing-tools-0.1.2/src/sideseeing_tools.egg-info/PKG-INFO` & `sideseeing-tools-0.1.3/src/sideseeing_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.2
+Version: 0.1.3
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
 Requires-Dist: folium~=0.13.0
 Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
 Requires-Dist: matplotlib~=3.7.1
-Requires-Dist: numpy~=1.24.1
+Requires-Dist: numpy~=1.25.0
 Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
```

