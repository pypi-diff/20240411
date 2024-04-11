# Comparing `tmp/htagui-0.0.1.tar.gz` & `tmp/htagui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.0.1.tar", max compression
+gzip compressed data, was "htagui-0.0.2.tar", max compression
```

## Comparing `htagui-0.0.1.tar` & `htagui-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-10 20:29:35.582419 htagui-0.0.1/LICENSE
--rw-r--r--   0        0        0     2472 2024-04-10 20:29:35.582419 htagui-0.0.1/README.md
--rw-r--r--   0        0        0      802 2024-04-10 20:29:36.174420 htagui-0.0.1/htagui/__init__.py
--rw-r--r--   0        0        0     3027 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/basics/__init__.py
--rw-r--r--   0        0        0     1100 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/common.py
--rw-r--r--   0        0        0     1856 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/form.py
--rw-r--r--   0        0        0     1545 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/no_bulma/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/no_shoelace/__init__.py
--rw-r--r--   0        0        0     2075 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/splitters.py
--rw-r--r--   0        0        0     2033 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/tabs.py
--rw-r--r--   0        0        0     5315 2024-04-10 20:29:35.582419 htagui-0.0.1/htagui/uiservice.py
--rw-r--r--   0        0        0     1071 2024-04-10 20:29:36.174420 htagui-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 htagui-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 11:46:06.340489 htagui-0.0.2/LICENSE
+-rw-r--r--   0        0        0     6371 2024-04-11 11:46:06.340489 htagui-0.0.2/README.md
+-rw-r--r--   0        0        0     1106 2024-04-11 11:46:06.596492 htagui-0.0.2/htagui/__init__.py
+-rw-r--r--   0        0        0     3549 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/common.py
+-rw-r--r--   0        0        0     5335 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/form.py
+-rw-r--r--   0        0        0     2075 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-11 11:46:06.340489 htagui-0.0.2/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-11 11:46:06.596492 htagui-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 htagui-0.0.2/PKG-INFO
```

### Comparing `htagui-0.0.1/LICENSE` & `htagui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.0.1/htagui/__init__.py` & `htagui-0.0.2/htagui/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,30 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.1" # auto updated
+__version__ = "0.0.2" # auto updated
 
+from htag import Tag
 ########################################################################################
 from .basics import Button,Input,Menu,Spinner,Select
 ########################################################################################
 from .form import Form
 from .tabs import Tabs
-from .uiservice import UI
+from .dialog import Dialog
 from .splitters import HSplit #VSplit
 from .flex import hflex,vflex  # utilities (Htag contructor methods)
 
-ALL=[Button,Input,Select,Menu,Spinner,Form,Tabs,UI,HSplit]
+class App(Tag.body):
+    _ui=None
+    
+    @property
+    def ui(self):
+        if self._ui is None:
+            self._ui = Dialog(self)
+        return self._ui
+
+ALL=[App,Button,Input,Select,Menu,Spinner,Form,Tabs,Dialog,HSplit]
+__all__=["App","Button","Input","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",      "hflex","vflex"]
```

### Comparing `htagui-0.0.1/htagui/basics/__init__.py` & `htagui-0.0.2/htagui/basics/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -144,9 +144,20 @@
 
 class Menu(Tag.div):
     statics=CSS
     def init(self,entries:dict):
         self["class"].add("menu")
         def call(ev):
             ev.target.method()
+
+            #auto close the ui.Dialog, if this "Menu" is in a Dialog interaction
+            #------------------------------------------------------------------------
+            current = self.parent
+            while current is not None:
+                if repr(current).startswith("<Dialog'div"): #TODO: not top (can do better)
+                    current.close()
+                    break
+                current = current.parent
+            #------------------------------------------------------------------------
+
         for k,v in entries.items():
             self += Tag.div(k,method=v,_onclick=call)
```

### Comparing `htagui-0.0.1/htagui/flex.py` & `htagui-0.0.2/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.1/htagui/form.py` & `htagui-0.0.2/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.1/htagui/splitters.py` & `htagui-0.0.2/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.1/htagui/tabs.py` & `htagui-0.0.2/htagui/tabs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
 from htag import Tag
-from .common import StepRules
+from .common import TagStep
 
-class Tabs(Tag.div,StepRules):
+class Tabs(Tag.div,TagStep):
     statics="""
     .tab {
         border:0px;
         cursor:pointer;
         margin:2px;
     }
     .tab.selected {
@@ -32,22 +32,22 @@
     #-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:
 
     def init(self,*objs,onchange=lambda x:x,**a):
         self._previous_selected=None
         self._selected=0
         self.onchange=onchange
         self._tabs=list(objs)
-        StepRules.init(self)
+        TagStep.init(self)
 
-    def rules(self,**params):
+    def step(self,**params):
         if "select" in params:
             self._selected=int(params["select"])
 
         if self._selected != self._previous_selected:
-            self.go( Tabs.Show, self._selected )
+            self( Tabs.Show, self._selected )
             self._previous_selected=self._selected
             self.onchange(self)
 
     @property
     def selected(self):
          return self._selected
```

### Comparing `htagui-0.0.1/htagui/uiservice.py` & `htagui-0.0.2/htagui/dialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
 from htag import Tag,expose
-from .common import StepRules
+from .common import TagStep
 from .form import Form
 from .basics import Voile,Button,Input
 
-class UI(Tag.div,StepRules):
+class Dialog(Tag.div,TagStep):
     imports=[Voile,Button,Input]
     #-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:
     class Empty(Tag.div):
         def init(self,main):
             self.clear()
             
     class Modal(Tag.div):
@@ -36,47 +36,47 @@
                 cb(ev.target.val)
                 main.step()
             box=[ 
                 Tag.div(obj),
                 Button("Yes",val=True,_onclick=call),
                 Button("No",val=False,_onclick=call),
             ]
-            UI.Modal.__init__(self,main,box)
+            Dialog.Modal.__init__(self,main,box)
 
     class ModalPrompt(Modal):
         def __init__(self,main, value,title,cb):
             def call(dico):
                 cb(dico["promptvalue"])
                 main.step()
             with Form(onsubmit=call) as f:
                 f+=Tag.div( title )
                 f+=Tag.div( Input(_value=value,_name="promptvalue",js="self.focus();self.setSelectionRange(0, self.value.length)") )
                 f+=Button("Ok" )
                 f+=Button("Cancel",_type="button",_onclick=main.stepevent())
-            UI.Modal.__init__(self,main,f)
+            Dialog.Modal.__init__(self,main,f)
 
     class Pop(Tag.div):
         def init(self,main,obj,xy:tuple):
             x,y=xy
             self <= Voile(_onmousedown=main.stepevent())
             self <= Tag.div( obj ,_style=f"position:fixed;top:{y}px;left:{x}px;z-index:1001;background:white")
 
     class Toast(Tag.div):
         def init(self,main_non_used,obj,timeout=1000):
-            self <= Tag.div(obj,_style="position:fixed;right:10px;bottom:10px;z-index:999;background:white;padding:10px;border:2px solid black")
+            self <= Tag.div(obj,_style="position:fixed;right:10px;bottom:10px;z-index:1001;background:white;padding:10px;border:2px solid black")
             self.js="setTimeout( function() {self.remove()} , %s)" % timeout
     #-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:-:
 
     def init(self,parent):
         self["info"]="UI.current object"
         self._toasts = Tag.div(_info="UI.toasts objects")
         parent += self  # auto add
         parent += self._toasts  # add a personnal place for toasts
             
-        StepRules.init(self)
+        TagStep.init(self)
 
     def alert(self,obj):
         self.step( alert = obj )
         
     def confirm(self,obj,cbresponse=lambda bool:bool):
         self.step( confirm = obj, cb=cbresponse )
         
@@ -95,35 +95,35 @@
 
     def block(self,obj=None):
         self.step( block=obj )
 
     def close(self):
         self.step()
 
-    def rules(self,**params):
+    def step(self,**params):
         if "alert" in params:
-            self.go( UI.Modal, params["alert"] )
+            self( Dialog.Modal, params["alert"] )
         elif "block" in params:
-            self.go( UI.Modal, params["block"],("50%","50%","50%","50%"),closable=False )
+            self( Dialog.Modal, params["block"],("50%","50%","50%","50%"),closable=False )
         elif "confirm" in params:
-            self.go( UI.ModalConfirm, params["confirm"], params["cb"] )
+            self( Dialog.ModalConfirm, params["confirm"], params["cb"] )
         elif "prompt" in params:
-            self.go( UI.ModalPrompt, params["prompt"],params["title"], params["cb"] )
+            self( Dialog.ModalPrompt, params["prompt"],params["title"], params["cb"] )
         elif "pop" in params:
-            self.go( UI.Pop, params["pop"],params["xy"] )
+            self( Dialog.Pop, params["pop"],params["xy"] )
         elif "drawer" in params:
             size=params["size"]
             if params["mode"]=="left":
-                self.go( UI.Modal, params["drawer"], ("0px",f"{size}%","0px","0px"),radius=0 )
+                self( Dialog.Modal, params["drawer"], ("0px",f"{size}%","0px","0px"),radius=0 )
             elif params["mode"]=="right":
-                self.go( UI.Modal, params["drawer"], ("0px","0px","0px",f"{size}%"),radius=0 )
+                self( Dialog.Modal, params["drawer"], ("0px","0px","0px",f"{size}%"),radius=0 )
             elif params["mode"]=="bottom":
-                self.go( UI.Modal, params["drawer"], (f"{size}%","0px","0px","0px"),radius=0 )
+                self( Dialog.Modal, params["drawer"], (f"{size}%","0px","0px","0px"),radius=0 )
             elif params["mode"]=="top":
-                self.go( UI.Modal, params["drawer"], ("0px","0px",f"{size}%","0px"),radius=0 )
+                self( Dialog.Modal, params["drawer"], ("0px","0px",f"{size}%","0px"),radius=0 )
         elif "toast" in params:
-            self._toasts.clear( UI.Toast( self, params["toast"], params["time"] ))
+            self._toasts.clear( Dialog.Toast( self, params["toast"], params["time"] ))
         else:
-            self.go( UI.Empty )
+            self( Dialog.Empty )
```

### Comparing `htagui-0.0.1/pyproject.toml` & `htagui-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.0.1" # auto-updated
+version = "0.0.2" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
@@ -15,16 +15,16 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.7"
-htag = ">= 0.100"
+htag = ">= 0.101"
 
 [tool.poetry.dev-dependencies]
-pytest = "^3.0"
+pytest = "^6"
 pytest-cov = "^2.6"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

