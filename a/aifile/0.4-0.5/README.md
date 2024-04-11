# Comparing `tmp/aifile-0.4.tar.gz` & `tmp/aifile-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifile-0.4.tar", last modified: Thu Apr 11 12:02:51 2024, max compression
+gzip compressed data, was "aifile-0.5.tar", last modified: Thu Apr 11 11:56:57 2024, max compression
```

## Comparing `aifile-0.4.tar` & `aifile-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 12:02:51.850692 aifile-0.4/
--rw-rw-rw-   0        0        0     3048 2024-04-11 12:02:51.849693 aifile-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2867 2024-04-11 12:00:25.000000 aifile-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 12:02:51.817695 aifile-0.4/aifile/
--rw-rw-rw-   0        0        0        0 2024-03-12 09:21:34.000000 aifile-0.4/aifile/__init__.py
--rw-rw-rw-   0        0        0     2817 2024-04-11 11:38:23.000000 aifile-0.4/aifile/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:02:51.848699 aifile-0.4/aifile.egg-info/
--rw-rw-rw-   0        0        0     3048 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 12:02:51.000000 aifile-0.4/aifile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 12:02:51.850692 aifile-0.4/setup.cfg
--rw-rw-rw-   0        0        0      467 2024-04-11 12:01:58.000000 aifile-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:56:57.128359 aifile-0.5/
+-rw-rw-rw-   0        0        0     2733 2024-04-11 11:56:57.127359 aifile-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2552 2024-03-12 11:10:02.000000 aifile-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 11:56:57.098037 aifile-0.5/aifile/
+-rw-rw-rw-   0        0        0        0 2024-03-12 09:21:34.000000 aifile-0.5/aifile/__init__.py
+-rw-rw-rw-   0        0        0     2817 2024-04-11 11:38:23.000000 aifile-0.5/aifile/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-11 11:56:57.124187 aifile-0.5/aifile.egg-info/
+-rw-rw-rw-   0        0        0     2733 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 11:56:56.000000 aifile-0.5/aifile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 11:56:57.128359 aifile-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      467 2024-04-11 11:56:49.000000 aifile-0.5/setup.py
```

### Comparing `aifile-0.4/PKG-INFO` & `aifile-0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aifile
-Version: 0.4
+Version: 0.5
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: speechrecognition
 
 **AIFile: Intelligent File Management Module**
 
@@ -50,22 +50,12 @@
 **Next Steps:**
 Explore opportunities to further enhance AIFile's capabilities, such as integrating with cloud services, extending voice recognition features, or implementing more sophisticated machine learning algorithms.
 
 **Version: 0.2**
 
 **Author: [SAHAJ A]**
 
-
-**Write a Script or Use Python Interactive Shell:**
-Create a Python script or use the Python interactive shell to interact with your module. For example, you can create a new script (e.g., my_script.py) with the following content:
-
-from aifile.filely import main
-
-if __name__ == "__main__":
-    main()
-
-
 *Note: Customize the abstract, features, usage, and next steps based on your specific implementation and goals.*
 
 FOR MORE INFO :-
 
 GITHUB :- https://github.com/SahajA25/Ai_File
```

### Comparing `aifile-0.4/README.md` & `aifile-0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,22 +42,12 @@
 **Next Steps:**
 Explore opportunities to further enhance AIFile's capabilities, such as integrating with cloud services, extending voice recognition features, or implementing more sophisticated machine learning algorithms.
 
 **Version: 0.2**
 
 **Author: [SAHAJ A]**
 
-
-**Write a Script or Use Python Interactive Shell:**
-Create a Python script or use the Python interactive shell to interact with your module. For example, you can create a new script (e.g., my_script.py) with the following content:
-
-from aifile.filely import main
-
-if __name__ == "__main__":
-    main()
-
-
 *Note: Customize the abstract, features, usage, and next steps based on your specific implementation and goals.*
 
 FOR MORE INFO :-
 
 GITHUB :- https://github.com/SahajA25/Ai_File
```

### Comparing `aifile-0.4/aifile/file_manager.py` & `aifile-0.5/aifile/file_manager.py`

 * *Files identical despite different names*

### Comparing `aifile-0.4/aifile.egg-info/PKG-INFO` & `aifile-0.5/aifile.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aifile
-Version: 0.4
+Version: 0.5
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: numpy
 Requires-Dist: speechrecognition
 
 **AIFile: Intelligent File Management Module**
 
@@ -50,22 +50,12 @@
 **Next Steps:**
 Explore opportunities to further enhance AIFile's capabilities, such as integrating with cloud services, extending voice recognition features, or implementing more sophisticated machine learning algorithms.
 
 **Version: 0.2**
 
 **Author: [SAHAJ A]**
 
-
-**Write a Script or Use Python Interactive Shell:**
-Create a Python script or use the Python interactive shell to interact with your module. For example, you can create a new script (e.g., my_script.py) with the following content:
-
-from aifile.filely import main
-
-if __name__ == "__main__":
-    main()
-
-
 *Note: Customize the abstract, features, usage, and next steps based on your specific implementation and goals.*
 
 FOR MORE INFO :-
 
 GITHUB :- https://github.com/SahajA25/Ai_File
```

