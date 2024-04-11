# Comparing `tmp/ToolsStr-1.0.1.tar.gz` & `tmp/ToolsStr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ToolsStr-1.0.1.tar", last modified: Thu Apr 11 10:17:57 2024, max compression
+gzip compressed data, was "ToolsStr-1.1.0.tar", last modified: Thu Apr 11 10:58:19 2024, max compression
```

## Comparing `ToolsStr-1.0.1.tar` & `ToolsStr-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 10:17:57.735202 ToolsStr-1.0.1/
--rw-rw-rw-   0        0        0     1094 2024-04-09 13:17:14.000000 ToolsStr-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      532 2024-04-11 10:17:57.725205 ToolsStr-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 10:17:57.722201 ToolsStr-1.0.1/ToolsStr.egg-info/
--rw-rw-rw-   0        0        0      532 2024-04-11 10:17:57.000000 ToolsStr-1.0.1/ToolsStr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-11 10:17:57.000000 ToolsStr-1.0.1/ToolsStr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 10:17:57.000000 ToolsStr-1.0.1/ToolsStr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 10:17:57.000000 ToolsStr-1.0.1/ToolsStr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 10:17:57.736203 ToolsStr-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      788 2024-04-11 09:57:58.000000 ToolsStr-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 10:17:57.715202 ToolsStr-1.0.1/toolsstr/
--rw-rw-rw-   0        0        0       31 2024-04-11 09:39:53.000000 ToolsStr-1.0.1/toolsstr/__init__.py
--rw-rw-rw-   0        0        0      263 2024-04-11 09:36:56.000000 ToolsStr-1.0.1/toolsstr/toolsstr.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:58:19.923804 ToolsStr-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2024-04-09 13:17:14.000000 ToolsStr-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      532 2024-04-11 10:58:19.921804 ToolsStr-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 10:58:19.918806 ToolsStr-1.1.0/ToolsStr.egg-info/
+-rw-rw-rw-   0        0        0      532 2024-04-11 10:58:19.000000 ToolsStr-1.1.0/ToolsStr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-11 10:58:19.000000 ToolsStr-1.1.0/ToolsStr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 10:58:19.000000 ToolsStr-1.1.0/ToolsStr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 10:58:19.000000 ToolsStr-1.1.0/ToolsStr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 10:58:19.924801 ToolsStr-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      788 2024-04-11 10:57:27.000000 ToolsStr-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 10:58:19.911802 ToolsStr-1.1.0/toolsstr/
+-rw-rw-rw-   0        0        0        0 2024-04-11 10:51:20.000000 ToolsStr-1.1.0/toolsstr/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-11 10:29:14.000000 ToolsStr-1.1.0/toolsstr/toolsstr.py
```

### Comparing `ToolsStr-1.0.1/LICENSE` & `ToolsStr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolsStr-1.0.1/PKG-INFO` & `ToolsStr-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolsStr
-Version: 1.0.1
+Version: 1.1.0
 Summary: A small package for keyboard typing in Python
 Author: Amirmahdi Mohammadi
 Author-email: amirmahdi21r21@gmail.com
 Keywords: python,type,master,toolsstr,rubika,library,strtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ToolsStr-1.0.1/ToolsStr.egg-info/PKG-INFO` & `ToolsStr-1.1.0/ToolsStr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolsStr
-Version: 1.0.1
+Version: 1.1.0
 Summary: A small package for keyboard typing in Python
 Author: Amirmahdi Mohammadi
 Author-email: amirmahdi21r21@gmail.com
 Keywords: python,type,master,toolsstr,rubika,library,strtools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `ToolsStr-1.0.1/setup.py` & `ToolsStr-1.1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
         name="ToolsStr", 
-        version='1.0.1',
+        version='1.1.0',
         author="Amirmahdi Mohammadi",
         author_email="amirmahdi21r21@gmail.com",
         description='A small package for keyboard typing in Python',
         long_description='Keyboard Typing . . .\n\nMy GitHub page: https://gitHub.com/FrameworkPython',
         packages=find_packages(),
         
         install_requires=[],
```

