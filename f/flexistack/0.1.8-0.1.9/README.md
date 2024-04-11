# Comparing `tmp/flexistack-0.1.8.tar.gz` & `tmp/flexistack-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexistack-0.1.8.tar", last modified: Tue Mar 19 15:44:55 2024, max compression
+gzip compressed data, was "flexistack-0.1.9.tar", last modified: Tue Apr  9 11:46:34 2024, max compression
```

## Comparing `flexistack-0.1.8.tar` & `flexistack-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:44:55.367098 flexistack-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-19 15:44:48.000000 flexistack-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 15:44:48.000000 flexistack-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-03-19 15:44:55.367098 flexistack-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-03-19 15:44:48.000000 flexistack-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-19 15:44:48.000000 flexistack-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 15:44:55.367098 flexistack-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:44:55.363098 flexistack-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:44:55.363098 flexistack-0.1.8/src/flexistack/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-19 15:44:48.000000 flexistack-0.1.8/src/flexistack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22705 2024-03-19 15:44:48.000000 flexistack-0.1.8/src/flexistack/flexistack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-19 15:44:48.000000 flexistack-0.1.8/src/flexistack/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 15:44:55.367098 flexistack-0.1.8/src/flexistack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-03-19 15:44:55.000000 flexistack-0.1.8/src/flexistack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-19 15:44:55.000000 flexistack-0.1.8/src/flexistack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 15:44:55.000000 flexistack-0.1.8/src/flexistack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-19 15:44:55.000000 flexistack-0.1.8/src/flexistack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 15:44:55.000000 flexistack-0.1.8/src/flexistack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:34.641369 flexistack-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 11:46:29.000000 flexistack-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:29.000000 flexistack-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-04-09 11:46:34.637369 flexistack-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13416 2024-04-09 11:46:29.000000 flexistack-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-09 11:46:29.000000 flexistack-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 11:46:34.641369 flexistack-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:34.637369 flexistack-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:34.637369 flexistack-0.1.9/src/flexistack/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-09 11:46:29.000000 flexistack-0.1.9/src/flexistack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26638 2024-04-09 11:46:29.000000 flexistack-0.1.9/src/flexistack/flexistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-09 11:46:29.000000 flexistack-0.1.9/src/flexistack/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 11:46:34.637369 flexistack-0.1.9/src/flexistack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-04-09 11:46:34.000000 flexistack-0.1.9/src/flexistack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-09 11:46:34.000000 flexistack-0.1.9/src/flexistack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 11:46:34.000000 flexistack-0.1.9/src/flexistack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 11:46:34.000000 flexistack-0.1.9/src/flexistack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 11:46:34.000000 flexistack-0.1.9/src/flexistack.egg-info/top_level.txt
```

### Comparing `flexistack-0.1.8/LICENSE` & `flexistack-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flexistack-0.1.8/pyproject.toml` & `flexistack-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flexistack"
-version = "0.1.8"
+version = "0.1.9"
 description = "Simple and easy to use framework"
 readme = "README.md"
 authors = [{ name = "Ioannis D (devcoons)", email = "support@devcoons.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `flexistack-0.1.8/src/flexistack/flexistack.py` & `flexistack-0.1.9/src/flexistack/flexistack.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,40 +97,42 @@
 
 class Plugin:
     """
     A class that wraps a loaded module object and its description.
     """
     m = None
     d = None
-
+    c = None
+    
     # --------------------------------------------------------------------------------- #
     # --------------------------------------------------------------------------------- #
 
-    def __init__(self, m, d):
+    def __init__(self, m, d, c):
         """
         Constructor method for the Module class.
 
         Args:
         - m: A reference to a loaded module object.
         - d: A string that describes the module.
         """
         self.m = m
         self.d = d
+        self.c = c
 
     # --------------------------------------------------------------------------------- #
         
     def __call__(self, flexistack = None):
         """
         Returns the loaded module object when the Module instance 
         is called like a function.
 
         Returns:
         - The loaded module object.
         """
-        return self.m.Plugin(flexistack) if flexistack != None else self.m
+        return getattr(self.m,self.c)(flexistack) if flexistack != None else self.m
 
 #########################################################################################
 # CLASS                                                                                 #
 #########################################################################################
 
 class PluginPack(dict):
     """
@@ -141,14 +143,22 @@
         """
         Constructor method for the ModulePack class.
         """
         pass
 
     # --------------------------------------------------------------------------------- #
 
+    def __call__(self, flexistack = None):
+        """
+        Constructor method for the ModulePack class.
+        """
+        return self.latest(flexistack=flexistack)
+
+    # --------------------------------------------------------------------------------- #
+
     def latest(self, flexistack = None):
         """
         Returns the latest version of the module in the ModulePack.
 
         Returns:
         - The Module object with the latest version number.
         """
@@ -306,43 +316,37 @@
         in the Autoloader.
 
         Args:
         - dir_paths: A string or list of strings representing the path(s) to the directory(ies) 
           containing the plugins to load.  
         """  
         def _load(module_full_path):  
-            try:    
+            try:                     
                 module = SourceFileLoader("module_candidate", module_full_path).load_module()
-                if not hasattr(module,'Plugin'):
-                    del module
-                    return
-                plugin = module.Plugin(None)
-                if not hasattr(plugin,'_flexi_'):
-                    del plugin, module
-                    return     
-                autoload_structure = {"type":str, "name": str, "description": str, "version": str}
-                if not all(key in plugin._flexi_ and isinstance(plugin._flexi_[key], value_type)
-                    for key, value_type in autoload_structure.items()):
-                    del plugin, module
-                    return  
-                if plugin._flexi_.get("type") != "plugin":
-                    del plugin, module
-                    return                    
-                p_name = plugin._flexi_['name']
-                p_vers = plugin._flexi_['version']
-                p_desc = plugin._flexi_['description']
-                module_rnd = ''.join(random.choices(string.ascii_letters + string.digits, k=5))
-                if self.plugins.get(p_name) is None:
-                    self.plugins[p_name] = PluginPack()  
-                self.plugins[p_name][p_vers] = Plugin(SourceFileLoader( p_name + "v" \
-                                     + str(p_vers) \
-                                     + "_" + module_rnd, module_full_path).load_module(), p_desc)
+                for class_name,_class in inspect.getmembers(module,inspect.isclass):
+                    if hasattr(_class,'_flexi_'):
+                        if _class._flexi_.get('type') == "plugin":                
+                            autoload_structure = {"type":str, "name": str, "description": str, "version": str}
+                            if not all(key in  _class._flexi_ and isinstance(_class._flexi_[key], value_type)
+                                for key, value_type in autoload_structure.items()):
+                                continue                   
+                            p_name = _class._flexi_['name']
+                            p_vers = _class._flexi_['version']
+                            p_desc = _class._flexi_['description']
+                            module_rnd = ''.join(random.choices(string.ascii_letters + string.digits, k=5))
+                            if self.plugins.get(p_name) is None:
+                                self.plugins[p_name] = PluginPack()  
+                            self.plugins[p_name][p_vers] = Plugin(SourceFileLoader( p_name + "v" \
+                                                 + str(p_vers) \
+                                                 + "_" + module_rnd, module_full_path).load_module(), p_desc,class_name)   
             except  Exception as e:
                 pass 
-
+            if 'module_candidate' in sys.modules:
+                del sys.modules['module_candidate']
+                
         if dir_paths == None:
             return
         if isinstance(dir_paths,str):
             dir_paths = [dir_paths]
         if not isinstance(dir_paths,list):    
              raise Exception("Error: Flexistack `dir_paths` required argument is not a type of list[str]")   
         for dir_path in dir_paths:
@@ -369,15 +373,17 @@
                 for class_name,_class in classes:
                     if hasattr(_class,'_flexi_'):
                         if _class._flexi_.get('type') == "middleware":
                             _class(self.middleware)
                 del module
             except  Exception as e:
                 pass 
-        
+            if 'module_candidate' in sys.modules:
+                del sys.modules['module_candidate']
+                
         if dir_paths == None:
             return
         if isinstance(dir_paths,str):
             dir_paths = [dir_paths]
         if not isinstance(dir_paths,list):    
              raise Exception("Error: Flexistack `dir_paths` required argument is not a type of list[str]")   
         for dir_path in dir_paths:
@@ -522,10 +528,91 @@
                         if obj.init(pargs=parsed_args,project_dir=project_dir) == True:
                             return obj.run()                 
                         return False 
         except Exception as e: 
             print(e)
             return False
 
+
+#########################################################################################
+# CLASS DECORATOR                                                                       #
+######################################################################################### 
+
+def flexi_action(as_optional, description):
+    
+    def class_decorator(cls):
+        cls._flexi_ = {'type':'action',
+                       'as_optional' : as_optional,
+                       'description':description}      
+
+        def action_init(self, flexistack=None):
+            self.basename = os.path.basename(sys.modules[cls.__module__].__file__)
+            self.flexistack = flexistack 
+            try:
+                if hasattr(self, 'req_plugins'):
+                    if self.flexistack != None and self.req_plugins != None:
+                        if len(self.req_plugins) == 0:
+                            return
+                        if (set(self.req_plugins) - self.flexistack.plugins.keys()):
+                            print(str(self.__class__)+" - [warn] missing required plugins")
+            except:
+                print(str(self.__class__)+" - [warn] plugins could not be loaded")        
+        
+        cls.__init__ = action_init
+        return cls
+ 
+    return class_decorator
+
+#########################################################################################
+# CLASS DECORATOR                                                                       #
+######################################################################################### 
+
+def flexi_middleware(description):
+    
+    def class_decorator(cls):
+        cls._flexi_ = {'type':'middleware',
+                       'description':description}      
+
+        def middleware_init(self, middleware):
+            self.basename = os.path.basename(sys.modules[cls.__module__].__file__)
+            setattr(middleware, self.__class__.__name__.lower(), self)
+            if hasattr(self, 'init'):
+                self.init()       
+        
+        cls.__init__ = middleware_init
+        return cls
+ 
+    return class_decorator
+
+#########################################################################################
+# CLASS DECORATOR                                                                       #
+#########################################################################################         
+   
+def flexi_plugin(name,version,description):
+    
+    def class_decorator(cls):
+        cls._flexi_ = {'type':'plugin',
+                       'name': name,
+                       'version':version,
+                       'description':description}      
+
+        def plugin_init(self, flexistack=None):
+            self.basename = os.path.basename(sys.modules[cls.__module__].__file__)
+            self.flexistack = flexistack 
+            try:
+                if hasattr(self, 'req_plugins'):
+                    if self.flexistack != None and self.req_plugins != None:
+                        if len(self.req_plugins) == 0:
+                            return
+                        if (set(self.req_plugins) - self.flexistack.plugins.keys()):
+                            print(str(self.__class__)+" - [warn] missing required plugins")
+            except:
+                print(str(self.__class__)+" - [warn] plugins could not be loaded")        
+        
+        cls.__init__ = plugin_init
+        return cls
+ 
+    return class_decorator
+
 #########################################################################################
 # EOF                                                                                   #
 #########################################################################################
```

### Comparing `flexistack-0.1.8/src/flexistack/helper.py` & `flexistack-0.1.9/src/flexistack/helper.py`

 * *Files identical despite different names*

