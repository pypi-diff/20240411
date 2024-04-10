# Comparing `tmp/VLCDA-1.0.4.tar.gz` & `tmp/VLCDA-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.4.tar", last modified: Sat Jun 17 19:00:36 2023, max compression
+gzip compressed data, was "VLCDA-1.0.5.tar", last modified: Wed Apr 10 21:43:16 2024, max compression
```

## Comparing `VLCDA-1.0.4.tar` & `VLCDA-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.903096 VLCDA-1.0.4/
--rw-rw-rw-   0        0        0     1077 2023-06-16 00:19:36.000000 VLCDA-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2066 2023-06-17 19:00:36.902094 VLCDA-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-06-16 00:33:20.000000 VLCDA-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.866977 VLCDA-1.0.4/VLCDA/
--rw-rw-rw-   0        0        0    19674 2023-06-17 19:00:23.000000 VLCDA-1.0.4/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-06-13 23:22:24.000000 VLCDA-1.0.4/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.877556 VLCDA-1.0.4/VLCDA.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 19:00:36.000000 VLCDA-1.0.4/VLCDA.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 19:00:36.898568 VLCDA-1.0.4/dist/
--rw-rw-rw-   0        0        0     7475 2023-06-16 00:24:22.000000 VLCDA-1.0.4/dist/VLCDA-1.0.0-py3-none-any.whl
--rw-rw-rw-   0        0        0     7746 2023-06-16 00:24:20.000000 VLCDA-1.0.4/dist/VLCDA-1.0.0.tar.gz
--rw-rw-rw-   0        0        0     7472 2023-06-16 00:29:29.000000 VLCDA-1.0.4/dist/VLCDA-1.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     7531 2023-06-16 00:29:28.000000 VLCDA-1.0.4/dist/VLCDA-1.0.1.tar.gz
--rw-rw-rw-   0        0        0     8172 2023-06-16 00:39:38.000000 VLCDA-1.0.4/dist/VLCDA-1.0.2-py3-none-any.whl
--rw-rw-rw-   0        0        0     8301 2023-06-16 00:39:37.000000 VLCDA-1.0.4/dist/VLCDA-1.0.2.tar.gz
--rw-rw-rw-   0        0        0     8181 2023-06-17 18:55:00.000000 VLCDA-1.0.4/dist/VLCDA-1.0.3-py3-none-any.whl
--rw-rw-rw-   0        0        0    50423 2023-06-17 18:54:59.000000 VLCDA-1.0.4/dist/VLCDA-1.0.3.tar.gz
--rw-rw-rw-   0        0        0       42 2023-06-17 19:00:36.903096 VLCDA-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-06-17 18:55:14.000000 VLCDA-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:43:16.192088 VLCDA-1.0.5/
+-rw-rw-rw-   0        0        0     1077 2023-11-28 23:29:37.000000 VLCDA-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2043 2024-04-10 21:43:16.191089 VLCDA-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2023-11-28 23:29:37.000000 VLCDA-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 21:43:16.101075 VLCDA-1.0.5/VLCDA/
+-rw-rw-rw-   0        0        0    35446 2024-04-10 21:37:51.000000 VLCDA-1.0.5/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-11-28 23:29:37.000000 VLCDA-1.0.5/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 21:43:16.125085 VLCDA-1.0.5/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0     2043 2024-04-10 21:43:16.000000 VLCDA-1.0.5/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2024-04-10 21:43:16.000000 VLCDA-1.0.5/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 21:43:16.000000 VLCDA-1.0.5/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 21:43:16.000000 VLCDA-1.0.5/VLCDA.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 21:43:16.189101 VLCDA-1.0.5/dist/
+-rw-rw-rw-   0        0        0     7475 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7746 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.0.tar.gz
+-rw-rw-rw-   0        0        0     7472 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7531 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.1.tar.gz
+-rw-rw-rw-   0        0        0     8172 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0     8301 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     8181 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.3-py3-none-any.whl
+-rw-rw-rw-   0        0        0    50423 2023-11-28 23:29:37.000000 VLCDA-1.0.5/dist/VLCDA-1.0.3.tar.gz
+-rw-rw-rw-   0        0        0       42 2024-04-10 21:43:16.193089 VLCDA-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-04-10 21:42:56.000000 VLCDA-1.0.5/setup.py
```

### Comparing `VLCDA-1.0.4/LICENSE.txt` & `VLCDA-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/PKG-INFO` & `VLCDA-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.4
+Version: 1.0.5
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 VLCDA
 ## Virtual Logic Circuits Design Automation
@@ -58,9 +57,7 @@
 ```sh
 python -m pip install --upgrade pip
 ```
 ## License
 
 MIT
 
-
-
```

### Comparing `VLCDA-1.0.4/README.md` & `VLCDA-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/VLCDA.egg-info/PKG-INFO` & `VLCDA-1.0.5/VLCDA.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.4
+Version: 1.0.5
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 VLCDA
 ## Virtual Logic Circuits Design Automation
@@ -58,9 +57,7 @@
 ```sh
 python -m pip install --upgrade pip
 ```
 ## License
 
 MIT
 
-
-
```

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.0-py3-none-any.whl` & `VLCDA-1.0.5/dist/VLCDA-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.0.tar.gz` & `VLCDA-1.0.5/dist/VLCDA-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.1-py3-none-any.whl` & `VLCDA-1.0.5/dist/VLCDA-1.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.1.tar.gz` & `VLCDA-1.0.5/dist/VLCDA-1.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.2-py3-none-any.whl` & `VLCDA-1.0.5/dist/VLCDA-1.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.2.tar.gz` & `VLCDA-1.0.5/dist/VLCDA-1.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.3-py3-none-any.whl` & `VLCDA-1.0.5/dist/VLCDA-1.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/dist/VLCDA-1.0.3.tar.gz` & `VLCDA-1.0.5/dist/VLCDA-1.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.4/setup.py` & `VLCDA-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup(
     name = "VLCDA",
-    version = "1.0.4",
+    version = "1.0.5",
     license='MIT',
     description = "Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos",
     author = "Humberto Távora, Stefan Blawid, Yasmin Maria",
     author_email = 'humbertocctg@gmail.com',
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
```

