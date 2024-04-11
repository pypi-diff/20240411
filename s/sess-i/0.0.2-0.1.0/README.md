# Comparing `tmp/sess_i-0.0.2.tar.gz` & `tmp/sess_i-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sess_i-0.0.2.tar", last modified: Tue Nov 21 13:36:52 2023, max compression
+gzip compressed data, was "sess_i-0.1.0.tar", max compression
```

## Comparing `sess_i-0.0.2.tar` & `sess_i-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-11-21 13:36:52.765632 sess_i-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-11-21 10:46:56.000000 sess_i-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      601 2023-11-21 13:36:52.763645 sess_i-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5930 2023-11-21 13:33:25.000000 sess_i-0.0.2/README.md
--rw-rw-rw-   0        0        0      104 2023-11-21 10:47:33.000000 sess_i-0.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-11-21 13:36:52.728879 sess_i-0.0.2/sess_i/
--rw-rw-rw-   0        0        0       21 2023-11-21 10:51:42.000000 sess_i-0.0.2/sess_i/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-21 13:36:52.749738 sess_i-0.0.2/sess_i/base/
--rw-rw-rw-   0        0        0        0 2023-11-21 10:47:33.000000 sess_i-0.0.2/sess_i/base/__init__.py
--rw-rw-rw-   0        0        0     5492 2023-11-21 13:07:06.000000 sess_i-0.0.2/sess_i/base/main.py
-drwxrwxrwx   0        0        0        0 2023-11-21 13:36:52.756195 sess_i-0.0.2/sess_i/gui/
--rw-rw-rw-   0        0        0        0 2023-11-21 10:47:33.000000 sess_i-0.0.2/sess_i/gui/__init__.py
--rw-rw-rw-   0        0        0     1026 2023-11-21 10:47:33.000000 sess_i-0.0.2/sess_i/gui/home.py
-drwxrwxrwx   0        0        0        0 2023-11-21 13:36:52.760168 sess_i-0.0.2/sess_i.egg-info/
--rw-rw-rw-   0        0        0      601 2023-11-21 13:36:52.000000 sess_i-0.0.2/sess_i.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-11-21 13:36:52.000000 sess_i-0.0.2/sess_i.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-21 13:36:52.000000 sess_i-0.0.2/sess_i.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-11-21 13:36:52.000000 sess_i-0.0.2/sess_i.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-11-21 13:36:52.000000 sess_i-0.0.2/sess_i.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      628 2023-11-21 13:36:52.767122 sess_i-0.0.2/setup.cfg
+-rw-r--r--   0        0        0    35823 2023-11-21 10:46:56.421250 sess_i-0.1.0/LICENSE
+-rw-r--r--   0        0        0      611 2024-04-11 14:59:51.977398 sess_i-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5930 2023-11-21 13:33:25.094228 sess_i-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 14:59:51.985373 sess_i-0.1.0/sess_i/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-10 18:16:26.980117 sess_i-0.1.0/sess_i/base/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-19 18:38:12.940029 sess_i-0.1.0/sess_i/base/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      175 2024-04-11 07:23:55.473831 sess_i-0.1.0/sess_i/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8771 2023-11-21 10:32:44.475992 sess_i-0.1.0/sess_i/base/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0        0        0     8388 2024-04-11 10:17:38.508674 sess_i-0.1.0/sess_i/base/__pycache__/main.cpython-39.pyc
+-rw-r--r--   0        0        0     8380 2024-04-11 12:48:21.332829 sess_i-0.1.0/sess_i/base/main.py
+-rw-r--r--   0        0        0     6467 1970-01-01 00:00:00.000000 sess_i-0.1.0/PKG-INFO
```

### Comparing `sess_i-0.0.2/LICENSE` & `sess_i-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sess_i-0.0.2/README.md` & `sess_i-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sess_i-0.0.2/sess_i/base/main.py` & `sess_i-0.1.0/sess_i/base/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,61 +16,128 @@
     1) If first pass: Initialize session, create page widget space and Global Space in session_state. Put the widget
     space object into the Global Space. Initialize widget defaults from user kwargs.
     Create object space, add to session state and create objects container inside the Space.
     On leave: add widget values inside widgets container. Update Object in session state from object space.
     2) Else: Initialize session. Initialize widget values from Widget Space stored values.
 """
 
-import streamlit as st
+
+
+class SessI:
+
+    def __init__(self, session_state, page=None):
+        """
+        Initialise session interface object
+        :param session_state: The state of the current session.
+        :param page: The id of the page. If not provided, it defaults to the name of the current file.
+        """
+        self.session_state = session_state
+        self.page = page if page is not None else __file__.split("\\")[-1][:-3]
+        self.object_space = ObjectSpace(self.session_state)
+        self.widget_space = WidgetSpace.initialize_session(self.session_state, self.page)
+
+    def __repr__(self):
+        return f"Page = {self.page}\n" \
+               f"Registered Objects = {self.object_space.objects}\n" \
+               f"Widgets = {self.widget_space.widgets}"
+
+    def set_widget_defaults(self,mapping=None, **kwargs):
+        """
+        Sets the default values for the widgets in the widget space.
+
+        :param mapping: A dictionary containing the default values for the widgets. If not provided, it defaults to None.
+        :param kwargs: The default values for the widgets as keyword arguments.
+        """
+        self.widget_space.set_widget_defaults(mapping, **kwargs)
+
+    def register_widgets(self, mapping=None, **kwargs):
+        """
+        Registers widgets in the widget space.
+
+        :param mapping: A dictionary containing the widgets to be registered. If not provided, it defaults to None.
+        :param kwargs: The widgets to be registered as keyword arguments.
+        """
+        self.widget_space.register_widgets(mapping, **kwargs)
+
+    def register_object(self, obj, key):
+        """
+        Registers an object in the object space.
+
+        :param obj: The object to be registered.
+        :param key: The key associated with the object.
+        """
+        self.object_space[key] = obj
+
+    def get_object(self, key):
+        return self.object_space[key]
 
 
 # Object Space
 class ObjectSpace:
     """
     The object space contains the objects and their data.
     A method is needed to register objects with specific keys
     """
 
     def __init__(self, session_state):
+        """
+        Constructs all the necessary attributes for the ObjectSpace object.
+
+        :param session_state: The state of the session.
+        """
         self.session_state = session_state
-        if "Object_Space" not in self.session_state.keys():
-            self.session_state["Object_Space"] = {}
-        self.objects = self.session_state["Object_Space"]
+        self.objects = self.session_state.setdefault("Object_Space", {})
 
     def __repr__(self):
+        """
+        Returns a string representation of the ObjectSpace object.
+
+        :return: A string representation of the stored objects.
+        """
         return f"Stored objects:\n{self.objects}"
 
     def __getitem__(self, item):
+        """
+        Returns the object associated with the key.
+
+        :param item: The key of the object.
+        :return: The object associated with the key.
+        """
         return self.objects.get(item)
 
     def __setitem__(self, key, value):
-        self.session_state["Object_Space"].update({key: value})
+        """
+        Sets the value of the object associated with the key and updates the session state.
+
+        :param key: The key of the object.
+        :param value: The value of the object.
+        """
         self.objects[key] = value
+        self.session_state["Object_Space"] = self.objects
 
 
 # Widget Space
 class WidgetSpace:
     """
     Every widget space must contain two base parameters:
         * The id of the page it communicates with
         * A container with the widgets and their state metadata (key & value)
     """
 
     def __init__(self, session_state, page):
 
         self.page = page
         self.session_state = session_state
-        self.widgets = {}
-
         if "Global_Widget_Space" not in session_state.keys():
             self.session_state["Global_Widget_Space"] = {page: self}
+        self.widgets = {key: value for key, value in session_state.items() if str(self.page) in key}
 
-        for key, value in session_state.items():
-            if str(self.page) in key:
-                self.widgets.update({key: value})
+        # for key, value in session_state.items():
+        #     if str(self.page) in key:
+        #         self.widgets.update({key: value})
 
     def __repr__(self):
         return f"WidgetSpace.widgets({self.widgets})"
 
     def __getitem__(self, item):
         return self.widgets.get(item)
 
@@ -78,65 +145,59 @@
     def initialize_session(cls, session_state, page=None):
         """
         Initialize widget space and add to Global Space
         :param page: page number
         :param session_state: streamlit session state
         :return:
         """
-        if page is None:
-            page = __file__.split("\\")[-1][:-3]
-        if "Global_Widget_Space" not in session_state.keys():
-            space = WidgetSpace(session_state, page)
-            session_state["Global_Widget_Space"] = {page: space}
-            return st.session_state["Global_Widget_Space"][page]
-        else:
-            if page not in session_state["Global_Widget_Space"].keys():
-                session_state["Global_Widget_Space"].update({page: WidgetSpace(session_state, page)})
-            return st.session_state["Global_Widget_Space"][page]
-
-    def set_widget_defaults(self, mapping=None, **kwargs):
 
-        if not self.widgets:
-            if mapping:
-                self.widgets = mapping
-            else:
-                self.widgets = {key: value for key, value in kwargs.items()}
+        # if page is None:
+        #     page = __file__.split("\\")[-1][:-3]
+        # if "Global_Widget_Space" not in session_state.keys():
+        #     space = WidgetSpace(session_state, page)
+        #     session_state["Global_Widget_Space"] = {page: space}
+        #     return st.session_state["Global_Widget_Space"][page]
+        # else:
+        #     if page not in session_state["Global_Widget_Space"].keys():
+        #         session_state["Global_Widget_Space"].update({page: WidgetSpace(session_state, page)})
+        #     return st.session_state["Global_Widget_Space"][page]
+
+        # Refactored: to test #
+        page = page or __file__.split("\\")[-1][:-3]
+        global_space = session_state.get("Global_Widget_Space", {})
 
-    def register_widgets(self, mapping=None, **kwargs):
-        if not self.session_state["Global_Widget_Space"][self.page]:
-            raise KeyError(
-                f"Widget space for page '{self.page}' doesn't exist."
-            )
-        if mapping:
-            self.widgets.update(mapping)
-        if kwargs:
-            self.widgets.update(**kwargs)
-
-
-class SessI:
-
-    def __init__(self, session_state, page=None):
-        self.session_state = session_state
-        self.page = page if page is not None else __file__.split("\\")[-1][:-3]
-        self.object_space = ObjectSpace(self.session_state)
-        self.widget_space = WidgetSpace.initialize_session(self.session_state, self.page)
+        if page not in global_space:
+            global_space[page] = WidgetSpace(session_state, page)
 
-    def __repr__(self):
-        return f"Page = {self.page}\n" \
-               f"Registered Objects = {self.object_space.objects}\n" \
-               f"Widgets = {self.widget_space.widgets}"
+        session_state["Global_Widget_Space"] = global_space
+        return session_state["Global_Widget_Space"][page]
 
-    def set_widget_defaults(self,mapping=None, **kwargs):
-        self.widget_space.set_widget_defaults(**kwargs)
+    def set_widget_defaults(self, mapping=None, **kwargs):
+        """
+        Add default values to widgets in the widget space. If the widget space is empty, initialize it.
+        :param mapping: Widget defaults as key-value pairs. Default is None.
+        :param kwargs: Widget defaults as keyword arguments.
+        :return:
+        """
+        self.widgets = mapping or {key: value for key, value in kwargs.items()} \
+            if not self.widgets else self.widgets
 
     def register_widgets(self, mapping=None, **kwargs):
-        self.widget_space.register_widgets(mapping, **kwargs)
-
-    def register_object(self, obj, key):
-        self.object_space[key] = obj
+        """
+        This method is used to register widgets in the widget space. It updates the widgets dictionary with the provided
+        mapping and keyword arguments. If the widget space for the current page does not exist, it raises a KeyError.
 
-    def get_object(self, key):
-        return self.object_space[key]
+        :param mapping: A dictionary containing widget mappings. Default is None.
+        :param kwargs: Keyword arguments for adding to the mapping of widgets.
+        :raises KeyError: If the widget space for the current page does not exist in the Global_Widget_Space.
+        """
+        # Get specific widget space for the page
+        if not self.session_state["Global_Widget_Space"].get(self.page):
+            raise KeyError(
+                f"Widget space for page '{self.page}' doesn't exist."
+            )
+        # Update widget space with mapping and kwargs
+        self.widgets.update(mapping or {}, **kwargs)
 
 
 if __name__ == "__main__":
     pass
```

