# Comparing `tmp/jemma-0.1.42.tar.gz` & `tmp/jemma-0.1.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.42.tar", last modified: Wed Apr 10 02:16:21 2024, max compression
+gzip compressed data, was "jemma-0.1.420.tar", last modified: Thu Apr 11 01:36:10 2024, max compression
```

## Comparing `jemma-0.1.42.tar` & `jemma-0.1.420.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.286081 jemma-0.1.42/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-10 02:16:21.285615 jemma-0.1.42/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      797 2024-04-09 23:33:37.000000 jemma-0.1.42/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.263654 jemma-0.1.42/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:18:01.000000 jemma-0.1.42/jemma/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.268390 jemma-0.1.42/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:33.000000 jemma-0.1.42/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.269619 jemma-0.1.42/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:44.000000 jemma-0.1.42/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-09 00:41:16.000000 jemma-0.1.42/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.274154 jemma-0.1.42/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:40.000000 jemma-0.1.42/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-08 20:02:41.000000 jemma-0.1.42/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-09 19:55:34.000000 jemma-0.1.42/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.276028 jemma-0.1.42/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:52.000000 jemma-0.1.42/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-09 05:44:45.000000 jemma-0.1.42/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.277745 jemma-0.1.42/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:18.000000 jemma-0.1.42/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-08 23:31:38.000000 jemma-0.1.42/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.282765 jemma-0.1.42/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:16.000000 jemma-0.1.42/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-09 05:43:50.000000 jemma-0.1.42/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 01:17:50.000000 jemma-0.1.42/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6878 2024-04-09 05:44:06.000000 jemma-0.1.42/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-09 05:44:11.000000 jemma-0.1.42/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 01:45:32.000000 jemma-0.1.42/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3371 2024-04-09 19:42:05.000000 jemma-0.1.42/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.284599 jemma-0.1.42/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-09 05:29:26.000000 jemma-0.1.42/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-09 05:43:40.000000 jemma-0.1.42/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-10 02:16:21.267764 jemma-0.1.42/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      100 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      720 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-10 02:16:21.000000 jemma-0.1.42/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-10 02:16:21.286214 jemma-0.1.42/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      468 2024-04-10 02:16:07.000000 jemma-0.1.42/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.785275 jemma-0.1.420/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-11 01:36:10.784601 jemma-0.1.420/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.420/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.757615 jemma-0.1.420/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-10 04:55:55.000000 jemma-0.1.420/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.764318 jemma-0.1.420/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.766093 jemma-0.1.420/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.769306 jemma-0.1.420/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.771416 jemma-0.1.420/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.773662 jemma-0.1.420/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.780982 jemma-0.1.420/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     7571 2024-04-11 01:32:04.000000 jemma-0.1.420/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3651 2024-04-11 01:30:43.000000 jemma-0.1.420/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.783140 jemma-0.1.420/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-10 21:15:08.000000 jemma-0.1.420/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.763304 jemma-0.1.420/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-11 01:36:10.785457 jemma-0.1.420/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-11 01:35:14.000000 jemma-0.1.420/setup.py
```

### Comparing `jemma-0.1.42/jemma/prompt/business/owner.py` & `jemma-0.1.420/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/prompt/engineer/clarify.py` & `jemma-0.1.420/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/prompt/engineer/code.py` & `jemma-0.1.420/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/prompt/tester/test.py` & `jemma-0.1.420/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/requirements/feature.py` & `jemma-0.1.420/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/team/business_owner.py` & `jemma-0.1.420/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/team/engineer.py` & `jemma-0.1.420/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/team/project_manager.py` & `jemma-0.1.420/jemma/team/project_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,31 @@
-from jemma.tools import say, color, open_local_browser
+import os
+from jemma.tools import say, color, open_local_browser, name_to_file_name
 from jemma.requirements.feature import Feature, UserStory
 
 class ProjectManager:
     def __init__(self, feature, project_name="project", role = "Project Manager"):
         self.feature = feature
         self.role = role
         self.project_name = project_name
 
+    def record_requirement(self,
+                           name,
+                           requirement,
+                           path):
+        # create the directory if it doesn't exist
+        os.makedirs(path, exist_ok=True)
+
+        requirement_path = os.path.join(path,
+                                        name_to_file_name(name))
+        with open(requirement_path, "w") as requirement_file:
+            requirement_file.write(requirement)
+
+        print(f"storing requirements for \"{name}\" in \"{requirement_path}\"")
+
     def meet_to_create_user_stories(self,
                                     thinker,
                                     business_owner):
         say(self.role, "\nDear Business Owner, in this meeting we'll work on splitting the requirements and creating user stories.",
             who_color = color.CYAN, message_color = color.YELLOW)
 
         refined = business_owner.split_and_refine(thinker,
@@ -138,13 +153,16 @@
 
     def user_stories_to_requirement(self):
         self.feature = Feature(self.feature.export_user_stories_titles_and_criteria())
 
     def meet_to_create_requirements(self,
                                     thinker,
                                     business_owner,
-                                    idea):
+                                    idea,
+                                    store_path="requirements"):
         say(self.role, "\nDear Business Owner, in this meeting we'll work on creating requirements based on the 💡 idea",
             who_color = color.CYAN, message_color = color.YELLOW)
 
         requirements = business_owner.idea_to_prompt(thinker, idea)
+        self.record_requirement(idea, requirements, store_path)
+
         self.feature = Feature(requirements)
```

### Comparing `jemma-0.1.42/jemma/team/tester.py` & `jemma-0.1.420/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/thinker.py` & `jemma-0.1.420/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma/tools.py` & `jemma-0.1.420/jemma/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import webbrowser
 import os, argparse, sys, re
 
+from datetime import datetime
+
 class color:
    PURPLE = '\033[95m'
    CYAN = '\033[96m'
    DARKCYAN = '\033[36m'
    BLUE = '\033[94m'
    GREEN = '\033[92m'
    YELLOW = '\033[93m'
@@ -24,14 +26,21 @@
    print(message_color + message)
 
 def read_file(path):
     with open(path, 'r') as file:
         data = file.read()
     return data
 
+def name_to_file_name(name, extension="txt"):
+
+    clean_name = re.sub(r'[^a-zA-Z0-9\s-]', '', name).replace(' ', '-').lower()
+
+    timestamp = datetime.now().strftime("%Y-%m-%d.%H-%M-%S-%f")[:-3]
+    return f"{clean_name}.{timestamp}.{extension}"
+
 def open_local_browser(dir_path):
    current_dir = os.getcwd()
    try:
       # Get the absolute path of the file
       abs_path = os.path.abspath(dir_path)
 
       # Check if the file exists
```

### Comparing `jemma-0.1.42/jemma/work/flow.py` & `jemma-0.1.420/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.42/jemma.egg-info/SOURCES.txt` & `jemma-0.1.420/jemma.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 jemma/__init__.py
+jemma/huddle.py
 jemma/thinker.py
 jemma/tools.py
 jemma.egg-info/PKG-INFO
 jemma.egg-info/SOURCES.txt
 jemma.egg-info/dependency_links.txt
 jemma.egg-info/entry_points.txt
 jemma.egg-info/requires.txt
```

