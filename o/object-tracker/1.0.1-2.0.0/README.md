# Comparing `tmp/object-tracker-1.0.1.tar.gz` & `tmp/object-tracker-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object-tracker-1.0.1.tar", last modified: Fri Mar 17 20:11:34 2023, max compression
+gzip compressed data, was "object-tracker-2.0.0.tar", last modified: Thu Apr 11 15:28:10 2024, max compression
```

## Comparing `object-tracker-1.0.1.tar` & `object-tracker-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-03-17 20:11:34.332324 object-tracker-1.0.1/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1501 2023-03-15 10:10:18.000000 object-tracker-1.0.1/LICENSE
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     2295 2023-03-17 20:11:34.332324 object-tracker-1.0.1/PKG-INFO
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1444 2023-03-17 16:00:46.000000 object-tracker-1.0.1/README.rst
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-03-17 20:11:34.328324 object-tracker-1.0.1/object_tracker/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      360 2023-03-17 16:32:28.000000 object-tracker-1.0.1/object_tracker/__init__.py
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      923 2023-03-17 15:22:27.000000 object-tracker-1.0.1/object_tracker/entry.py
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      505 2023-03-17 13:50:41.000000 object-tracker-1.0.1/object_tracker/exceptions.py
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     2798 2023-03-17 15:26:40.000000 object-tracker-1.0.1/object_tracker/query_log.py
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     4074 2023-03-17 15:32:24.000000 object-tracker-1.0.1/object_tracker/tracker.py
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     2824 2023-03-17 15:03:18.000000 object-tracker-1.0.1/object_tracker/wrapper.py
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-03-17 20:11:34.328324 object-tracker-1.0.1/object_tracker.egg-info/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     2295 2023-03-17 20:11:34.000000 object-tracker-1.0.1/object_tracker.egg-info/PKG-INFO
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      361 2023-03-17 20:11:34.000000 object-tracker-1.0.1/object_tracker.egg-info/SOURCES.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)        1 2023-03-17 20:11:34.000000 object-tracker-1.0.1/object_tracker.egg-info/dependency_links.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       15 2023-03-17 20:11:34.000000 object-tracker-1.0.1/object_tracker.egg-info/top_level.txt
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       38 2023-03-17 20:11:34.332324 object-tracker-1.0.1/setup.cfg
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1212 2023-03-17 20:11:05.000000 object-tracker-1.0.1/setup.py
-drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2023-03-17 20:11:34.332324 object-tracker-1.0.1/tests/
--rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     3984 2023-03-17 14:22:03.000000 object-tracker-1.0.1/tests/test_tracker.py
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 15:28:10.041253 object-tracker-2.0.0/
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1501 2024-04-08 04:37:02.000000 object-tracker-2.0.0/LICENSE
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2921 2024-04-11 15:28:10.037253 object-tracker-2.0.0/PKG-INFO
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     2050 2024-04-11 15:08:50.000000 object-tracker-2.0.0/README.rst
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 15:28:10.037253 object-tracker-2.0.0/object_tracker/
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     6010 2024-04-11 15:08:50.000000 object-tracker-2.0.0/object_tracker/__init__.py
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     8508 2024-04-11 15:08:50.000000 object-tracker-2.0.0/object_tracker/changelog.py
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      780 2024-04-11 15:08:50.000000 object-tracker-2.0.0/object_tracker/exceptions.py
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     6229 2024-04-11 15:08:50.000000 object-tracker-2.0.0/object_tracker/tracker.py
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      268 2024-04-11 15:08:50.000000 object-tracker-2.0.0/object_tracker/types.py
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 15:28:10.037253 object-tracker-2.0.0/object_tracker.egg-info/
+-rw-r--r--   0 saurabh   (1000) saurabh   (1000)     2921 2024-04-11 15:28:10.000000 object-tracker-2.0.0/object_tracker.egg-info/PKG-INFO
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)      335 2024-04-11 15:28:10.000000 object-tracker-2.0.0/object_tracker.egg-info/SOURCES.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)        1 2024-04-11 15:28:10.000000 object-tracker-2.0.0/object_tracker.egg-info/dependency_links.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       15 2024-04-11 15:28:10.000000 object-tracker-2.0.0/object_tracker.egg-info/top_level.txt
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)       38 2024-04-11 15:28:10.041253 object-tracker-2.0.0/setup.cfg
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     1255 2024-04-11 15:08:50.000000 object-tracker-2.0.0/setup.py
+drwxrwxr-x   0 saurabh   (1000) saurabh   (1000)        0 2024-04-11 15:28:10.037253 object-tracker-2.0.0/tests/
+-rw-rw-r--   0 saurabh   (1000) saurabh   (1000)     6462 2024-04-11 15:08:50.000000 object-tracker-2.0.0/tests/test_tracker.py
```

### Comparing `object-tracker-1.0.1/LICENSE` & `object-tracker-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `object-tracker-1.0.1/PKG-INFO` & `object-tracker-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: object-tracker
-Version: 1.0.1
+Version: 2.0.0
 Summary: A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.
 Home-page: https://github.com/saurabh0719/object-tracker
 Author: Saurabh Pujari
 Author-email: saurabhpuj99@gmail.com
 License: three-clause BSD
 Project-URL: Documentation, https://github.com/saurabh0719/object-tracker#README
 Project-URL: Source, https://github.com/saurabh0719/object-tracker
-Keywords: object_tracker,object-tracker,changelog,object history,tracker,change tracker,history
+Keywords: object_tracker,object-tracker,changelog,object history,tracker,change tracker,history,state,state tracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 object-tracker
 --------------
 
-A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.
+A pure python object state tracker. Monitor all changes in your object's lifecycle, query the history changelog, and trigger callback functions to capture them.
 
 View the `Github repository <https://github.com/saurabh0719/object-tracker>`__ and the `official docs <https://github.com/saurabh0719/object-tracker#README>`__.
 
 .. code:: sh
 
     $ pip install object-tracker
 
 Tested for python 3.6, 3.7 and above.
 
 Key Features
 ------------
 
--  Determine if a python object has changed.
--  Investigate change history through the changelog.
--  Trigger callback functions whenever the object or an attribute has changed.
--  Simple and structured API. 
--  Queryable change history log.
+-  Determine if a python object has changed state during it's lifecycle.
+-  Investigate change history by querying a structured changelog.
+-  Trigger callback functions whenever an (or any) attribute has changed.
+-  Use it as a decorator, a class mixin or on its own.
 
 License
 -------
 
 ::
 
     Copyright (c) Saurabh Pujari
@@ -48,29 +47,56 @@
 
     This source code is licensed under the BSD-style license found in the LICENSE file in the root directory of this source tree.
 
 
 Usage :
 ~~~~~~~~~~~~~
 
+Use the `@track` decorator to track an object's attributes.
+
 .. code:: python
 
-   from object_tracker import ObjectTracker
+    from object_tracker import track
 
     def observer(attr, old, new):
         print(f"Observer : {attr} -> {old} - {new}")
 
-    class User(ObjectTracker):
-        def __init__(self, name) -> None:
-            ObjectTracker.__init__(self, observers=[observer,])
+    @track('name', 'age', observers=[observer,])
+    class User:
+        def __init__(self, name, age):
             self.name = name
+            self.age = age
 
+    user = User(name='Alice', age=30)
+    user.name = 'Bob'
+    # Observer : name -> Alice - Bob
+    print(user.tracker.has_changed()) 
+    # True
+    print(user.tracker.has_attribute_changed('name'))
+    # True
 
-    user = User("A")
-    print(user.tracker.changed()) 
-    # False
+Or use the `Tracker` class 
 
-    user.name = "B" # observers will be triggered
-    # Observer : name -> A - B
+.. code:: python
 
-    print(user.tracker.changed()) 
+    class MyClass:
+        pass
+    
+    obj = MyClass()
+    tracker = Tracker(obj)
+    obj.attribute = 'new_value'
+    print(tracker.has_changed(obj))
     # True
+
+
+Or use it with the mixin class `TrackerMixin`:
+
+
+.. code:: python
+
+   from object_tracker import TrackerMixin, Tracker
+    
+    class User(TrackerMixin):
+        def __init__(self, name, age):
+            self.name = name
+            self.age = age
+            self.tracker = Tracker()
```

### Comparing `object-tracker-1.0.1/README.rst` & `object-tracker-2.0.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 object-tracker
 --------------
 
-A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.
+A pure python object state tracker. Monitor all changes in your object's lifecycle, query the history changelog, and trigger callback functions to capture them.
 
 View the `Github repository <https://github.com/saurabh0719/object-tracker>`__ and the `official docs <https://github.com/saurabh0719/object-tracker#README>`__.
 
 .. code:: sh
 
     $ pip install object-tracker
 
 Tested for python 3.6, 3.7 and above.
 
 Key Features
 ------------
 
--  Determine if a python object has changed.
--  Investigate change history through the changelog.
--  Trigger callback functions whenever the object or an attribute has changed.
--  Simple and structured API. 
--  Queryable change history log.
+-  Determine if a python object has changed state during it's lifecycle.
+-  Investigate change history by querying a structured changelog.
+-  Trigger callback functions whenever an (or any) attribute has changed.
+-  Use it as a decorator, a class mixin or on its own.
 
 License
 -------
 
 ::
 
     Copyright (c) Saurabh Pujari
@@ -30,29 +29,56 @@
 
     This source code is licensed under the BSD-style license found in the LICENSE file in the root directory of this source tree.
 
 
 Usage :
 ~~~~~~~~~~~~~
 
+Use the `@track` decorator to track an object's attributes.
+
 .. code:: python
 
-   from object_tracker import ObjectTracker
+    from object_tracker import track
 
     def observer(attr, old, new):
         print(f"Observer : {attr} -> {old} - {new}")
 
-    class User(ObjectTracker):
-        def __init__(self, name) -> None:
-            ObjectTracker.__init__(self, observers=[observer,])
+    @track('name', 'age', observers=[observer,])
+    class User:
+        def __init__(self, name, age):
             self.name = name
+            self.age = age
 
+    user = User(name='Alice', age=30)
+    user.name = 'Bob'
+    # Observer : name -> Alice - Bob
+    print(user.tracker.has_changed()) 
+    # True
+    print(user.tracker.has_attribute_changed('name'))
+    # True
 
-    user = User("A")
-    print(user.tracker.changed()) 
-    # False
+Or use the `Tracker` class 
 
-    user.name = "B" # observers will be triggered
-    # Observer : name -> A - B
+.. code:: python
 
-    print(user.tracker.changed()) 
+    class MyClass:
+        pass
+    
+    obj = MyClass()
+    tracker = Tracker(obj)
+    obj.attribute = 'new_value'
+    print(tracker.has_changed(obj))
     # True
+
+
+Or use it with the mixin class `TrackerMixin`:
+
+
+.. code:: python
+
+   from object_tracker import TrackerMixin, Tracker
+    
+    class User(TrackerMixin):
+        def __init__(self, name, age):
+            self.name = name
+            self.age = age
+            self.tracker = Tracker()
```

### Comparing `object-tracker-1.0.1/object_tracker.egg-info/PKG-INFO` & `object-tracker-2.0.0/object_tracker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 Metadata-Version: 2.1
 Name: object-tracker
-Version: 1.0.1
+Version: 2.0.0
 Summary: A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.
 Home-page: https://github.com/saurabh0719/object-tracker
 Author: Saurabh Pujari
 Author-email: saurabhpuj99@gmail.com
 License: three-clause BSD
 Project-URL: Documentation, https://github.com/saurabh0719/object-tracker#README
 Project-URL: Source, https://github.com/saurabh0719/object-tracker
-Keywords: object_tracker,object-tracker,changelog,object history,tracker,change tracker,history
+Keywords: object_tracker,object-tracker,changelog,object history,tracker,change tracker,history,state,state tracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 object-tracker
 --------------
 
-A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.
+A pure python object state tracker. Monitor all changes in your object's lifecycle, query the history changelog, and trigger callback functions to capture them.
 
 View the `Github repository <https://github.com/saurabh0719/object-tracker>`__ and the `official docs <https://github.com/saurabh0719/object-tracker#README>`__.
 
 .. code:: sh
 
     $ pip install object-tracker
 
 Tested for python 3.6, 3.7 and above.
 
 Key Features
 ------------
 
--  Determine if a python object has changed.
--  Investigate change history through the changelog.
--  Trigger callback functions whenever the object or an attribute has changed.
--  Simple and structured API. 
--  Queryable change history log.
+-  Determine if a python object has changed state during it's lifecycle.
+-  Investigate change history by querying a structured changelog.
+-  Trigger callback functions whenever an (or any) attribute has changed.
+-  Use it as a decorator, a class mixin or on its own.
 
 License
 -------
 
 ::
 
     Copyright (c) Saurabh Pujari
@@ -48,29 +47,56 @@
 
     This source code is licensed under the BSD-style license found in the LICENSE file in the root directory of this source tree.
 
 
 Usage :
 ~~~~~~~~~~~~~
 
+Use the `@track` decorator to track an object's attributes.
+
 .. code:: python
 
-   from object_tracker import ObjectTracker
+    from object_tracker import track
 
     def observer(attr, old, new):
         print(f"Observer : {attr} -> {old} - {new}")
 
-    class User(ObjectTracker):
-        def __init__(self, name) -> None:
-            ObjectTracker.__init__(self, observers=[observer,])
+    @track('name', 'age', observers=[observer,])
+    class User:
+        def __init__(self, name, age):
             self.name = name
+            self.age = age
 
+    user = User(name='Alice', age=30)
+    user.name = 'Bob'
+    # Observer : name -> Alice - Bob
+    print(user.tracker.has_changed()) 
+    # True
+    print(user.tracker.has_attribute_changed('name'))
+    # True
 
-    user = User("A")
-    print(user.tracker.changed()) 
-    # False
+Or use the `Tracker` class 
 
-    user.name = "B" # observers will be triggered
-    # Observer : name -> A - B
+.. code:: python
 
-    print(user.tracker.changed()) 
+    class MyClass:
+        pass
+    
+    obj = MyClass()
+    tracker = Tracker(obj)
+    obj.attribute = 'new_value'
+    print(tracker.has_changed(obj))
     # True
+
+
+Or use it with the mixin class `TrackerMixin`:
+
+
+.. code:: python
+
+   from object_tracker import TrackerMixin, Tracker
+    
+    class User(TrackerMixin):
+        def __init__(self, name, age):
+            self.name = name
+            self.age = age
+            self.tracker = Tracker()
```

### Comparing `object-tracker-1.0.1/setup.py` & `object-tracker-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,32 @@
 from distutils.core import setup
 
 long_description = pathlib.Path("README.rst").read_text()
 
 setup(
     name="object-tracker",
     packages=["object_tracker"],
-    version="1.0.1",
+    version="2.0.0",
     license="three-clause BSD",
     description="A pure python object change and history tracker. Monitor all changes in your objects lifecycle and trigger callback functions to capture them.",
     long_description=long_description,
     long_description_content_type= 'text/x-rst',
     author="Saurabh Pujari",
     author_email="saurabhpuj99@gmail.com",
     url="https://github.com/saurabh0719/object-tracker",
     keywords=[
         "object_tracker", 
         "object-tracker", 
         "changelog",
         "object history", 
         "tracker", 
         "change tracker", 
-        "history"
+        "history",
+        "state",
+        "state tracker",
     ],
     project_urls={
         "Documentation": "https://github.com/saurabh0719/object-tracker#README",
         "Source": "https://github.com/saurabh0719/object-tracker",
     },
     install_requires=[],
     classifiers=[
```

