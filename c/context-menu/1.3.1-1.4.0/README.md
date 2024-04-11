# Comparing `tmp/context_menu-1.3.1.tar.gz` & `tmp/context_menu-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_menu-1.3.1.tar", last modified: Sun Jun  4 19:20:43 2023, max compression
+gzip compressed data, was "context_menu-1.4.0.tar", last modified: Thu Apr 11 06:25:12 2024, max compression
```

## Comparing `context_menu-1.3.1.tar` & `context_menu-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.256331 context_menu-1.3.1/
--rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.3.1/LICENSE
--rw-rw-rw-   0        0        0    14964 2023-06-04 19:20:43.254822 context_menu-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    14389 2023-06-02 19:46:16.000000 context_menu-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.237307 context_menu-1.3.1/context_menu/
--rw-rw-rw-   0        0        0       36 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/__init__.py
--rw-rw-rw-   0        0        0    11820 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/linux_menus.py
--rw-rw-rw-   0        0        0     5401 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/menus.py
--rw-rw-rw-   0        0        0    12508 2023-06-02 19:45:36.000000 context_menu-1.3.1/context_menu/windows_menus.py
-drwxrwxrwx   0        0        0        0 2023-06-04 19:20:43.254822 context_menu-1.3.1/context_menu.egg-info/
--rw-rw-rw-   0        0        0    14964 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-04 19:20:43.000000 context_menu-1.3.1/context_menu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 19:20:43.256331 context_menu-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-06-04 19:20:37.000000 context_menu-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.277140 context_menu-1.4.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    15187 2024-04-11 06:25:12.275141 context_menu-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14571 2024-04-11 06:18:32.000000 context_menu-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.239817 context_menu-1.4.0/context_menu/
+-rw-rw-rw-   0        0        0        0 2024-04-11 05:58:22.000000 context_menu-1.4.0/context_menu/__init__.py
+-rw-rw-rw-   0        0        0    12780 2024-04-11 05:58:22.000000 context_menu-1.4.0/context_menu/linux_menus.py
+-rw-rw-rw-   0        0        0     6325 2024-04-11 06:18:29.000000 context_menu-1.4.0/context_menu/menus.py
+-rw-rw-rw-   0        0        0     6319 2024-04-11 06:18:29.000000 context_menu-1.4.0/context_menu/pytest_plugin.py
+-rw-rw-rw-   0        0        0    15441 2024-04-11 06:18:32.000000 context_menu-1.4.0/context_menu/windows_menus.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.265329 context_menu-1.4.0/context_menu.egg-info/
+-rw-rw-rw-   0        0        0    15187 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 06:25:12.278142 context_menu-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      989 2024-04-11 06:18:58.000000 context_menu-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.273128 context_menu-1.4.0/tests/
+-rw-rw-rw-   0        0        0      157 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_imports.py
+-rw-rw-rw-   0        0        0     1493 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_linux.py
+-rw-rw-rw-   0        0        0      520 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_menus.py
+-rw-rw-rw-   0        0        0     5470 2024-04-11 06:18:32.000000 context_menu-1.4.0/tests/test_windows.py
```

### Comparing `context_menu-1.3.1/LICENSE` & `context_menu-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `context_menu-1.3.1/PKG-INFO` & `context_menu-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: context_menu
-Version: 1.3.1
+Version: 1.4.0
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest-html; extra == "test"
 
-# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://travis-ci.com/saleguas/context_menu.svg?token=STF1haAqx5Xq2x9zdkHH&branch=master)](https://app.travis-ci.com/github/saleguas/context_menu)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
+# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://github.com/saleguas/context_menu/actions/workflows/ci.yml/badge.svg)](https://github.com/saleguas/context_menu/actions/workflows/ci.yml)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
 
 ![logo](media/logo.png)
 
 💻 A Python library to create and deploy cross-platform native context menus. 💻
 
 
 Documentation available at: https://context-menu.readthedocs.io/en/latest/
@@ -82,15 +84,15 @@
 - Windows 7
 - Windows 10
 - Windows 11
 - Linux (Using Nautilus)
 
 ## 🐍 What Python versions are supported? 🐍
 
-**All python versions 3.1 and above** are supported.
+**All python versions 3.7 and above** are supported.
 
 # 💽 Installation 💽
 
 If you haven't installed Python, download and run an installer from the official
 website: https://www.python.org/downloads/
 
 Once you have Python, the rest is super simple. Simply just run the following command in a terminal to install the
@@ -182,19 +184,19 @@
 All context menus are **permanent** unless you remove them.
 
 # 🤖 Advanced Usage 🤖
 
 ## The `ContextMenu` Class
 
 The [ContextMenu](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu) object
-holds other context objects. It expects a name, and **the activation type** if it is the root menu(the first menu). Only
+holds other context objects. It expects a name, **the activation type** if it is the root menu(the first menu), and an optional icon path. Only
 compile the root menu.
 
 ```Python
-ContextMenu(name: str, type: str = None)
+ContextMenu(name: str, type: str = None, icon_path: str = None)
 ```
 
 Menus can be added to menus, creating cascading context menus. You can use
 the [{MENU}.add_items{ITEMS}](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu.add_items)
 function to add context elements together, for example:
 
 ```Python
@@ -348,14 +350,15 @@
 
 | Name                 | Location                                                           | Action                                   |
 | -------------------- | ------------------------------------------------------------------ | ---------------------------------------- |
 | FILES                | HKEY_CURRENT_USER\\Software\\Classes\\\*\\shell\\                  | Opens on a file                          |
 | DIRECTORY            | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\shell             | Opens on a directory                     |
 | DIRECTORY_BACKGROUND | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\Background\\shell | Opens on the background of the Directory |
 | DRIVE                | HKEY_CURRENT_USER\\Software\\Classes\\Drive\\shell                 | Opens on the drives(think USBs)          |
+| DESKTOP              | Software\\Classes\\DesktopBackground\\shell                        | Opens on the background of the desktop   |
 
 * * *
 
 I strongly recommend checking out the [examples folder](examples) for more complicated examples and usage.
 
 You can check out the official documentation [here](https://context-menu.readthedocs.io/en/latest/index.html).
```

### Comparing `context_menu-1.3.1/README.md` & `context_menu-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://travis-ci.com/saleguas/context_menu.svg?token=STF1haAqx5Xq2x9zdkHH&branch=master)](https://app.travis-ci.com/github/saleguas/context_menu)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
+# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://github.com/saleguas/context_menu/actions/workflows/ci.yml/badge.svg)](https://github.com/saleguas/context_menu/actions/workflows/ci.yml)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
 
 ![logo](media/logo.png)
 
 💻 A Python library to create and deploy cross-platform native context menus. 💻
 
 
 Documentation available at: https://context-menu.readthedocs.io/en/latest/
@@ -66,15 +66,15 @@
 - Windows 7
 - Windows 10
 - Windows 11
 - Linux (Using Nautilus)
 
 ## 🐍 What Python versions are supported? 🐍
 
-**All python versions 3.1 and above** are supported.
+**All python versions 3.7 and above** are supported.
 
 # 💽 Installation 💽
 
 If you haven't installed Python, download and run an installer from the official
 website: https://www.python.org/downloads/
 
 Once you have Python, the rest is super simple. Simply just run the following command in a terminal to install the
@@ -166,19 +166,19 @@
 All context menus are **permanent** unless you remove them.
 
 # 🤖 Advanced Usage 🤖
 
 ## The `ContextMenu` Class
 
 The [ContextMenu](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu) object
-holds other context objects. It expects a name, and **the activation type** if it is the root menu(the first menu). Only
+holds other context objects. It expects a name, **the activation type** if it is the root menu(the first menu), and an optional icon path. Only
 compile the root menu.
 
 ```Python
-ContextMenu(name: str, type: str = None)
+ContextMenu(name: str, type: str = None, icon_path: str = None)
 ```
 
 Menus can be added to menus, creating cascading context menus. You can use
 the [{MENU}.add_items{ITEMS}](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu.add_items)
 function to add context elements together, for example:
 
 ```Python
@@ -332,14 +332,15 @@
 
 | Name                 | Location                                                           | Action                                   |
 | -------------------- | ------------------------------------------------------------------ | ---------------------------------------- |
 | FILES                | HKEY_CURRENT_USER\\Software\\Classes\\\*\\shell\\                  | Opens on a file                          |
 | DIRECTORY            | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\shell             | Opens on a directory                     |
 | DIRECTORY_BACKGROUND | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\Background\\shell | Opens on the background of the Directory |
 | DRIVE                | HKEY_CURRENT_USER\\Software\\Classes\\Drive\\shell                 | Opens on the drives(think USBs)          |
+| DESKTOP              | Software\\Classes\\DesktopBackground\\shell                        | Opens on the background of the desktop   |
 
 * * *
 
 I strongly recommend checking out the [examples folder](examples) for more complicated examples and usage.
 
 You can check out the official documentation [here](https://context-menu.readthedocs.io/en/latest/index.html).
```

### Comparing `context_menu-1.3.1/context_menu/linux_menus.py` & `context_menu-1.4.0/context_menu/linux_menus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # imports -------------------------------------------------
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import os
 from enum import Enum
 
+if TYPE_CHECKING:
+    from context_menu.menus import ContextMenu, ItemType, ActivationType, CommandVar
+
 # code_preset.py -------------------------------------
 
 
 class ExistingCode(Enum):
-    '''
+    """
     Preset values important for metaprogramming.
-    '''
+    """
 
-    CODE_HEAD = '''
+    CODE_HEAD = """
 import gi
 import sys
 import os
 
 try:
 \tgi.require_version('Nautilus', '3.0')
 except:
@@ -24,346 +29,387 @@
 
 # -------------------------------------------- #
 
 try:
 \tfrom urllib import unquote
 except ImportError:
 \tfrom urllib.parse import unquote
-    '''
+    """
 
-    CLASS_TEMPLATE = '''
+    CLASS_TEMPLATE = """
 class {}MenuProvider(GObject.GObject, Nautilus.MenuProvider):
 \tdef __init__(self):
 \t\tpass
-'''
+"""
 
-    METHOD_HANDLER_TEMPLATE = '''
+    METHOD_HANDLER_TEMPLATE = """
 \tdef {}(self, menu, files):
 \t\tfilenames = [unquote(subFile.get_uri()[7:]) for subFile in files]
 \t\t{}.{}({}, "{}")
 
-'''
+"""
 
-    COMMAND_HANDLER_TEMPLATE = '''
+    COMMAND_HANDLER_TEMPLATE = """
 \tdef {}(self, menu, files):
 \t\tfilepath = [unquote(subFile.get_uri()[7:]) for subFile in files][0]
 \t\tos.system('{}'{})
 
-'''
+"""
 
-    FILE_ITEMS = '''\tdef get_file_items(self, *args):
-\t\tfiles = args[-1]'''
-    BACKGROUND_ITEMS = '''\tdef get_background_items(self, *args):
-\t\tfiles = args[-1]'''
-    SUB_MENU = 'submenu{} = Nautilus.Menu()'
+    FILE_ITEMS = """\tdef get_file_items(self, *args):
+\t\tfiles = args[-1]"""
+    BACKGROUND_ITEMS = """\tdef get_background_items(self, *args):
+\t\tfiles = args[-1]"""
+    SUB_MENU = "submenu{} = Nautilus.Menu()"
     MENU_ITEM = 'menuitem{} = Nautilus.MenuItem(name = "ExampleMenuProvider::{}", label="{}", tip = "{}", icon = "{}")'
 
+
 # code_builder.py ----------------------------------
 
 
 class CodeBuilder:
-    '''
+    """
     The CodeBuilder class is used for generating the final python file for the Linux menus.
-    '''
+    """
 
-    def __init__(self, name: str, body_commands: list, script_dirs: list, funcs: list, imports: list, type: str):
-        '''
+    def __init__(
+        self,
+        name: str,
+        body_commands: list[str],
+        script_dirs: list[str],
+        funcs: list[str],
+        imports: list[str],
+        type: ActivationType | str,
+    ) -> None:
+        """
         Pass the list of body_commands, the directories of all the scripts, the
         list of the function names, the list of the imports, and the type.
-        '''
+        """
         self.name = name
         self.body_commands = body_commands
         self.script_dirs = list(set(script_dirs))
         self.funcs = funcs
         self.imports = list(set(imports))
         self.type = type.upper()
 
-    def build_script_dirs(self):
-        '''
+    def build_script_dirs(self) -> str:
+        """
         Creates the header of necessary path configurations.
 
         Adds all the 'sys.path.appends' in order to immport the classes and functions.
 
         Handled automatically by compile.
-        '''
+        """
         compiled_dirs = [f'sys.path.append("{x}")' for x in self.script_dirs]
-        return '\n'.join(compiled_dirs)
+        return "\n".join(compiled_dirs)
 
-    def build_imports(self):
-        '''
+    def build_imports(self) -> str:
+        """
         Creates the header of necessary imports.
 
         Handled automatically by compile.
-        '''
-        compiled_imports = [f'import {x}' for x in self.imports]
-        return '\n'.join(compiled_imports)
+        """
+        compiled_imports = [f"import {x}" for x in self.imports]
+        return "\n".join(compiled_imports)
 
-    def compile(self):
-        '''
+    def compile(self) -> str:
+        """
         Creates the code file.
-        '''
+        """
         code_head = ExistingCode.CODE_HEAD.value
         script_dirs_code = self.build_script_dirs()
         imports_code = self.build_imports()
         class_dec = ExistingCode.CLASS_TEMPLATE.value.format(self.name)
-        class_funcs = '\n\n'.join(self.funcs)
+        class_funcs = "\n\n".join(self.funcs)
         class_type = ExistingCode.FILE_ITEMS.value
-        if self.type in ['DIRECTORY_BACKGROUND', 'DESKTOP_BACKGROUND']:
+        if self.type in ["DIRECTORY_BACKGROUND", "DESKTOP_BACKGROUND"]:
             class_type = ExistingCode.BACKGROUND_ITEMS.value
-        class_body = '\n'.join(map(lambda x: '\t\t' + x, self.body_commands))
+        class_body = "\n".join(map(lambda x: "\t\t" + x, self.body_commands))
 
-        code_skeleton = '''
+        code_skeleton = """
 {}
 {}
 {}
 {}
 {}
 {}
 {}
-    '''.format(code_head, script_dirs_code, imports_code, class_dec, class_funcs, class_type, class_body)
+    """.format(
+            code_head,
+            script_dirs_code,
+            imports_code,
+            class_dec,
+            class_funcs,
+            class_type,
+            class_body,
+        )
 
         return code_skeleton
 
 
 COMMAND_VARS = {
-    'FILENAME' : "filepath",
-    'DIR': "os.getcwd()",
-    'DIRECTORY': "os.getcwd()",
-    'PYTHONLOC' : 'sys.executable'
+    "FILENAME": "filepath",
+    "DIR": "os.getcwd()",
+    "DIRECTORY": "os.getcwd()",
+    "PYTHONLOC": "sys.executable",
 }
 
-def command_var_format(item: str):
-    '''
+
+def command_var_format(item: str) -> str:
+    """
     Converts a python string to a value for a command
 
-    '''
+    """
     return COMMAND_VARS[item.upper()]
 
 
 # code_builder.py ----------------------------------
 
+
 # Not necessary, but helps simplify the code.
 class Variable:
-    '''
+    """
     Very simple class with no methods to help simplify the code.
-    '''
+    """
 
-    def __init__(self, name: str, code: str):
+    def __init__(self, name: str, code: str) -> None:
         self.name = name
         self.code = code
 
 
 class NautilusMenu:
-
     # Constructor, automatically handeled by menus.py
-    def __init__(self, name: str, sub_items: list, type: str):
-        '''
+    def __init__(
+        self, name: str, sub_items: list[ItemType], type: ActivationType | str
+    ) -> None:
+        """
         Items required are the name of the top menu, the sub items, and the type.
-        '''
+        """
         # nautilus extensions doesn't work with filenames with spaces
         # Example menu item -> ExampleMenuItem
-        self.name = "".join([word.title() for word in name.split()]) if len(name.split()) > 0 else name
+        self.name = (
+            "".join([word.title() for word in name.split()])
+            if len(name.split()) > 0
+            else name
+        )
         self.sub_items = sub_items
         self.type = type
         self.counter = 0
 
-# Create all the necessary lists that will be used later on
-        self.commands = []
-        self.script_dirs = []
-        self.funcs = []
-        self.imports = []
-
-# Methods to create action code
-    def append_item(self, menu: str, item: str):
-        '''
-        Creates a necssary body_command.
-        '''
+        # Create all the necessary lists that will be used later on
+        self.commands: list[str] = []
+        self.script_dirs: list[str] = []
+        self.funcs: list[str] = []
+        self.imports: list[str] = []
+
+    # Methods to create action code
+    def append_item(self, menu: str, item: str) -> str:
+        """
+        Creates a necessary body_command.
+        """
         return "{}.append_item({})".format(menu, item)
 
-    def set_submenu(self, item: str, menu: str):
-        '''
-        Creates a necssary body_command.
-        '''
-        return '{}.set_submenu({})'.format(item, menu)
-
-    def connect(self, item: str, func: str):
-        '''
-        Creates a necssary body_command.
-        '''
+    def set_submenu(self, item: str, menu: str) -> str:
+        """
+        Creates a necessary body_command.
+        """
+        return "{}.set_submenu({})".format(item, menu)
+
+    def connect(self, item: str, func: str) -> str:
+        """
+        Creates a necessary body_command.
+        """
         return '{}.connect("activate", {}, files)'.format(item, func)
 
-# Methods to create variable declarations
+    # Methods to create variable declarations
 
-    def generate_menu(self):
-        '''
+    def generate_menu(self) -> Variable:
+        """
         Generates a nautilus menu variable.
-        '''
+        """
         base_menu = ExistingCode.SUB_MENU.value
         base_menu = base_menu.format(self.counter)
         self.counter += 1
 
-        return Variable(base_menu.split(' = ')[0], base_menu)
+        return Variable(base_menu.split(" = ")[0], base_menu)
 
-    def generate_item(self, name: str):
-        '''
+    def generate_item(self, name: str) -> Variable:
+        """
         Generates a nautilus command variable.
-        '''
+        """
         base_command = ExistingCode.MENU_ITEM.value
-        formatted_item = base_command.format(self.counter, name, name, '', '')
+        formatted_item = base_command.format(self.counter, name, name, "", "")
         self.counter += 1
 
-        return Variable(formatted_item.split(' = ')[0], formatted_item)
+        return Variable(formatted_item.split(" = ")[0], formatted_item)
 
-    def generate_python_func(self, class_origin: str, class_func: str, params: str):
-        '''
+    def generate_python_func(
+        self, class_origin: str, class_func: str, params: str
+    ) -> Variable:
+        """
         Generates a command attached to a python function
-        '''
-        func_name = 'method_handler{}'.format(self.counter)
+        """
+        func_name = "method_handler{}".format(self.counter)
         created_func = ExistingCode.METHOD_HANDLER_TEMPLATE.value.format(
-            func_name, class_origin, class_func, 'filenames', params)
+            func_name, class_origin, class_func, "filenames", params
+        )
 
         self.counter += 1
 
-        return Variable(f'self.{func_name}', created_func)
+        return Variable(f"self.{func_name}", created_func)
 
-    def generate_command_func(self, command: str):
-        '''
+    def generate_command_func(self, command: str) -> Variable:
+        """
         Generates a command attached to a python function
-        '''
-        func_name = 'method_handler{}'.format(self.counter)
+        """
+        func_name = "method_handler{}".format(self.counter)
         created_func = ExistingCode.COMMAND_HANDLER_TEMPLATE.value.format(
-            func_name, command, '')
+            func_name, command, ""
+        )
 
         self.counter += 1
 
-        return Variable(f'self.{func_name}', created_func)
+        return Variable(f"self.{func_name}", created_func)
 
-    def generate_mod_command_func(self, command: str, command_vars: list):
-        '''
+    def generate_mod_command_func(
+        self, command: str, command_vars: list[CommandVar]
+    ) -> Variable:
+        """
         Generates a command attached to a python function that allows special variables.
-        '''
-        new_command = command.replace('?',  '{}')
+        """
+        new_command = command.replace("?", "{}")
         modified_vars = [command_var_format(item) for item in command_vars]
-        final_str = ', '.join(modified_vars)
-        func_name = 'method_handler{}'.format(self.counter)
+        final_str = ", ".join(modified_vars)
+        func_name = "method_handler{}".format(self.counter)
         replace_func = """.format({})""".format(final_str)
         created_func = ExistingCode.COMMAND_HANDLER_TEMPLATE.value.format(
-            func_name, new_command, replace_func)
+            func_name, new_command, replace_func
+        )
 
         self.counter += 1
 
-        return Variable(f'self.{func_name}', created_func)
-
-
+        return Variable(f"self.{func_name}", created_func)
 
-# Other misc methods to help out
+    # Other misc methods to help out
 
-
-    def get_next_item(self):
-        '''
+    def get_next_item(self) -> str:
+        """
         Very niche, required in other methods.
-        '''
-        val = self.generate_item('')
+        """
+        val = self.generate_item("")
         self.counter -= 1
 
         return val.name
 
+    # Building the script body
 
-# Building the script body
-
-
-    def build_script_body(self, name: str, items: list):
-        '''
+    def build_script_body(self, name: str, items: list[ItemType]) -> None:
+        """
         Builds the body commands of the script.
-        '''
+        """
         top_item = self.generate_item(name)
         top_menu = self.generate_menu()
         submenu_com = self.set_submenu(top_item.name, top_menu.name)
         self.commands.append(top_item.code)
         self.commands.append(top_menu.code)
         self.commands.append(submenu_com)
 
         for item in items:
             if item.isMenu:
-                subsubmenu_con = self.append_item(
-                    top_menu.name, self.get_next_item())
+                subsubmenu_con = self.append_item(top_menu.name, self.get_next_item())
                 self.build_script_body(item.name, item.sub_items)
                 self.commands.append(subsubmenu_con)
+                continue
+
+            # if the item is a command
+            formatted_command = self.generate_item(item.name)
+            self.commands.append(formatted_command.code)
+
+            if item.python != None:
+                # if there is a python function
+                item_info = item.get_method_info()
+                connected_func = self.generate_python_func(
+                    item_info[1], item_info[0], item.params
+                )
+                self.script_dirs.append(item_info[2])
+                self.imports.append(item_info[1])
+            elif item.command_vars != None:
+                # if the command requries parameters
+                assert item.command is not None
+                assert item.command_vars is not None
+                connected_func = self.generate_mod_command_func(
+                    item.command, item.command_vars
+                )
             else:
-                # if the item is a command
-                formatted_command = self.generate_item(item.name)
-                self.commands.append(formatted_command.code)
-
-                connected_func = None
-
-                if item.python != None:
-                    # if there is a python function
-                    item_info = item.get_method_info()
-                    connected_func = self.generate_python_func(
-                        item_info[1], item_info[0], item.params)
-                    self.script_dirs.append(item_info[2])
-                    self.imports.append(item_info[1])
-                elif item.command_vars != None:
-                    # if the command requries parameters
-                    connected_func = self.generate_mod_command_func(item.command, item.command_vars)
-                else:
-                    # if the command is simply normal
-                    connected_func = self.generate_command_func(item.command)
-                    # connected_func = self.generate_func('os', 'system')
-
-                self.funcs.append(connected_func.code)
-
-                connected_command = self.connect(
-                    formatted_command.name, connected_func.name)
-                self.commands.append(connected_command)
-
-                formatted_command = self.append_item(
-                    top_menu.name, formatted_command.name)
-                self.commands.append(formatted_command)
+                # if the command is simply normal
+                assert item.command is not None
+                connected_func = self.generate_command_func(item.command)
+                # connected_func = self.generate_func('os', 'system')
+
+            self.funcs.append(connected_func.code)
+
+            connected_command = self.connect(
+                formatted_command.name, connected_func.name
+            )
+            self.commands.append(connected_command)
+
+            self.commands.append(
+                self.append_item(top_menu.name, formatted_command.name)
+            )
 
-    def build_script(self):
-        '''
+    def build_script(self) -> str:
+        """
         Finishes and returns the full code.
-        '''
+        """
         self.build_script_body(self.name, self.sub_items)
-        self.commands.append('return menuitem0,')
-        full_code = CodeBuilder(self.name,
-            self.commands, self.script_dirs, self.funcs, self.imports, self.type).compile()
+        self.commands.append("return menuitem0,")
+        full_code = CodeBuilder(
+            self.name,
+            self.commands,
+            self.script_dirs,
+            self.funcs,
+            self.imports,
+            self.type,
+        ).compile()
 
         return full_code
 
-    def create_path(self, path: str, dir: str):
-        '''
+    def create_path(self, path: str, dir: str) -> str:
+        """
         Creates a path to directory. Creates all sub-directories
-        '''
+        """
         new_dir = os.path.join(path, dir)
         if not os.path.exists(new_dir):
             os.makedirs(new_dir)
         return new_dir
 
-    def compile(self):
-        '''
+    def compile(self) -> None:
+        """
         Creates the code, creates a file, and moves it to the correct location.
-        '''
+        """
         code = self.build_script()
-        save_loc = os.path.join(os.path.expanduser('~'), '.local/share/')
+        save_loc = os.path.join(os.path.expanduser("~"), ".local/share/")
         print(save_loc)
-        save_loc = self.create_path(save_loc, 'nautilus-python')
-        save_loc = self.create_path(save_loc, 'extensions')
-        save_loc = os.path.join(save_loc, f'{self.name}.py')
-        py_file = open(save_loc, 'w')
+        save_loc = self.create_path(save_loc, "nautilus-python")
+        save_loc = self.create_path(save_loc, "extensions")
+        save_loc = os.path.join(save_loc, f"{self.name}.py")
+        py_file = open(save_loc, "w")
         py_file.write(code)
         py_file.close()
 
+
 # Testing section...
 
 try:
-    def remove_linux_menu(name):
-        save_loc = os.path.join(os.path.expanduser('~'), '.local/share/nautilus-python/extensions', name)
+
+    def remove_linux_menu(name) -> None:
+        save_loc = os.path.join(
+            os.path.expanduser("~"), ".local/share/nautilus-python/extensions", name
+        )
         try:
-            os.remove(save_loc + '.py')
-            os.remove(save_loc + '.pyc')
+            os.remove(save_loc + ".py")
+            os.remove(save_loc + ".pyc")
         except Exception as e:
             print(e)
 
-except:
+except Exception:
     pass
```

### Comparing `context_menu-1.3.1/context_menu/windows_menus.py` & `context_menu-1.4.0/context_menu/windows_menus.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,338 +1,455 @@
 # all imports ---------------
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import os
 import ctypes
 import sys
-from enum import Enum
+
+if TYPE_CHECKING:
+    from typing import Any
+    from types import FunctionType
+    from context_menu.menus import (
+        ItemType,
+        MethodInfo,
+        ActivationType,
+        CommandVar,
+        ContextMenu,
+    )
 
 
 # registry_shortcuts.py ----------------------------------------------------------------------------------------
 
 try:
     import winreg
 
     # ------------------------------------------------------------------
 
-    def is_admin():
-        '''
+    def is_admin() -> bool:
+        """
         Returns True if the current python instance has admin, and false otherwise.
-        '''
+        """
         try:
             return ctypes.windll.shell32.IsUserAnAdmin()
         except:
             return False
 
-    def run_admin(params=sys.argv[0], force=False):
-        '''
+    def run_admin(params: str = sys.argv[0], force: bool = False) -> None:
+        """
         If the python instance does not have admin priviledges, it stops the current execution and runs the program as admin.
 
         You can customize where it runs/Force it to run regardless.
-        '''
+        """
         if not is_admin() or force:
             ctypes.windll.shell32.ShellExecuteW(
-                None, "runas", sys.executable, params, None, 1)
+                None, "runas", sys.executable, params, None, 1
+            )
             sys.exit()
 
     # ------------------------------------------------------------------
 
-    def create_key(path: str, hive=winreg.HKEY_CURRENT_USER):
-        '''
+    def create_key(path: str, hive: int = winreg.HKEY_CURRENT_USER) -> None:
+        """
         Creates a key at the desired path.
-        '''
+        """
         winreg.CreateKey(hive, path)
 
-    def set_key_value(key_path: str, subkey_name: str, value: 'Value', hive=winreg.HKEY_CURRENT_USER):
-        '''
+    def set_key_value(
+        key_path: str,
+        subkey_name: str,
+        value: str | int,
+        hive: int = winreg.HKEY_CURRENT_USER,
+    ) -> None:
+        """
         Changes the value of a subkey. Creates the subkey if it doesn't exist.
-        '''
+        """
 
-        registry_key = winreg.OpenKey(hive, key_path, 0,
-                                      winreg.KEY_WRITE)
+        registry_key = winreg.OpenKey(hive, key_path, 0, winreg.KEY_WRITE)
         winreg.SetValueEx(registry_key, subkey_name, 0, winreg.REG_SZ, value)
         winreg.CloseKey(registry_key)
 
-    def list_keys(path: str, hive=winreg.HKEY_CURRENT_USER) -> 'List of keys':
-        '''
+    def get_key_value(
+        key_path: str,
+        subkey_name: str,
+        hive: int = winreg.HKEY_CURRENT_USER,
+    ) -> Any:
+        """
+        Gets the value of a subkey.
+        """
+        with winreg.OpenKey(hive, key_path, 0, winreg.KEY_READ) as open_key:
+            return winreg.QueryValueEx(open_key, subkey_name)[0]
+
+    def list_keys(path: str, hive: int = winreg.HKEY_CURRENT_USER) -> list[str]:
+        """
         Returns a list of all the keys at a given registry path.
-        '''
+        """
 
         open_key = winreg.OpenKey(hive, path)
         key_amt = winreg.QueryInfoKey(open_key)[0]
         keys = []
 
         for count in range(key_amt):
             subkey = winreg.EnumKey(open_key, count)
             keys.append(subkey)
 
         return keys
 
-    def delete_key(path: str, hive=winreg.HKEY_CURRENT_USER):
-        '''
+    def delete_key(path: str, hive: int = winreg.HKEY_CURRENT_USER) -> None:
+        """
         Deletes the desired key and all other subkeys at the given path.
-        '''
+        """
         open_key = winreg.OpenKey(hive, path)
         subkeys = list_keys(path)
 
         if len(subkeys) > 0:
             for key in subkeys:
-                delete_key(path + '\\' + key)
+                delete_key(path + "\\" + key)
         winreg.DeleteKey(open_key, "")
+
 except:
-    print('Not linux')
+
+    def create_key(path: str, hive: int = 0) -> None:
+        """
+        Creates a key at the desired path.
+        """
+        raise NotImplementedError("winreg is not available on this platform")
+
+    def set_key_value(
+        key_path: str, subkey_name: str, value: str | int, hive: int = 0
+    ) -> None:
+        """
+        Changes the value of a subkey. Creates the subkey if it doesn't exist.
+        """
+        raise NotImplementedError("winreg is not available on this platform")
+
+    def get_key_value(key_path: str, subkey_name: str, hive: int = 0) -> Any:
+        """
+        Gets the value of a subkey.
+        """
+        raise NotImplementedError("winreg is not available on this platform")
+
+    def list_keys(path: str, hive: int = 0) -> list[str]:
+        """
+        Returns a list of all the keys at a given registry path.
+        """
+        raise NotImplementedError("winreg is not available on this platform")
+
+    def delete_key(path: str, hive: int = 0) -> None:
+        """
+        Deletes the desired key and all other subkeys at the given path.
+        """
+        raise NotImplementedError("winreg is not available on this platform")
+
+    print("Not windows")
 
 
 # advanced_reg_config.py ----------------------------------------------------------------------------------------
 
 
 # These are the paths in the registry that correlate to when the context menu is fired.
 # For example, FILES is when a file is right clicked
 CONTEXT_SHORTCUTS = {
-    'FILELOC' : 'Software\\Classes\\',
-    'FILES': 'Software\\Classes\\*\\shell',
-    'DIRECTORY': 'Software\\Classes\\Directory\\shell',
-    'DIRECTORY_BACKGROUND': 'Software\\Classes\\Directory\\Background\\shell',
-    'DRIVE': 'Software\\Classes\\Drive\\shell'
+    "FILELOC": "Software\\Classes\\SystemFileAssociations",
+    "FILES": "Software\\Classes\\*\\shell",
+    "DIRECTORY": "Software\\Classes\\Directory\\shell",
+    "DIRECTORY_BACKGROUND": "Software\\Classes\\Directory\\Background\\shell",
+    "DRIVE": "Software\\Classes\\Drive\\shell",
+    "DESKTOP": "Software\\Classes\\DesktopBackground\\shell",
 }
 
 # Not used yet, but could be useful in the future
 COMMAND_PRESETS = {
-    'python': sys.executable,
-    'pythonw': os.path.join(os.path.dirname(sys.executable), 'pythonw.exe')
+    "python": sys.executable,
+    "pythonw": os.path.join(os.path.dirname(sys.executable), "pythonw.exe"),
 }
 
 COMMAND_VARS = {
-    'FILENAME' : "' '.join(sys.argv[1:]) ",
-    'DIR': 'os.getcwd()',
-    'DIRECTORY': 'os.getcwd()',
-    'PYTHONLOC' : 'sys.executable'
+    "FILENAME": "' '.join(sys.argv[1:]) ",
+    "DIR": "os.getcwd()",
+    "DIRECTORY": "os.getcwd()",
+    "PYTHONLOC": "sys.executable",
 }
 
-def context_registry_format(item: str) -> 'registry path to the desired type':
-    '''
+
+def join_keys(*keys: str) -> str:
+    """Joins parts of a registry path.
+
+    This joins the parts with \\ unlike os.path.join that would
+    use / on Linux and break tests.
+
+    :param keys: parts of the registry path
+    :return: complete registry path
+    """
+    return "\\".join(keys)
+
+
+def context_registry_format(item: str) -> str:
+    """
     Converts a verbose type into a registry path.
 
     For example, 'FILES' -> 'Software\\Classes\\*\\shell'
-    '''
+    """
     item = item.upper()
-    if '.' in item:
-        return os.path.join(CONTEXT_SHORTCUTS['FILELOC'], item.lower(), 'shell')
+    if "." in item:
+        return join_keys(CONTEXT_SHORTCUTS["FILELOC"], item.lower(), "shell")
     return CONTEXT_SHORTCUTS[item]
 
 
-def command_preset_format(item: str) -> 'Path to desired python type':
-    '''
+def command_preset_format(item: str) -> str:
+    """
     Converts a python string to an executable location.
 
     For example, 'python' -> sys.executable
-    '''
+    """
     return COMMAND_PRESETS[item.lower()]
 
-def command_var_format(item: str):
-    '''
+
+def command_var_format(item: str) -> str:
+    """
     Converts a python string to a value for a command
 
-    '''
+    """
     return COMMAND_VARS[item.upper()]
 
-def create_file_select_command(func_name: str, func_file_name: str, func_dir_path: str, params: str) -> 'Registry valid string to call python function':
-    '''
+
+def create_file_select_command(
+    func_name: str, func_file_name: str, func_dir_path: str, params: str
+) -> str:
+    """
     Creates a registry valid command to link a context menu entry to a funtion, specifically for file selection(FILES, DIRECTORY, DRIVE).
 
     Requires the name of the function, the name of the file, and the path to the directory of the file.
-    '''
+    """
     python_loc = sys.executable
-    sys_section = f'''import sys; sys.path.insert(0, '{func_dir_path}')'''.replace('\\', '/')
-    file_section = f'import {func_file_name}'
+    sys_section = f"""import sys; sys.path.insert(0, '{func_dir_path}')""".replace(
+        "\\", "/"
+    )
+    file_section = f"import {func_file_name}"
     dir_path = """' '.join(sys.argv[1:]) """
-    func_section = f'''{func_file_name}.{func_name}([{dir_path}],'{params}')'''
-    python_portion = f'''"{python_loc}" -c "{sys_section}; {file_section}; {func_section}"'''
+    func_section = f"""{func_file_name}.{func_name}([{dir_path}],'{params}')"""
+    python_portion = (
+        f'''"{python_loc}" -c "{sys_section}; {file_section}; {func_section}"'''
+    )
     full_command = f'''{python_portion} \"%1\"'''
 
     return full_command
 
 
-def create_directory_background_command(func_name: str, func_file_name: str, func_dir_path: str, params: str) -> 'Registry valid string to call python function':
-    '''
+def create_directory_background_command(
+    func_name: str, func_file_name: str, func_dir_path: str, params: str
+) -> str:
+    """
     Creates a registry valid command to link a context menu entry to a funtion, specifically for backgrounds(DIRECTORY_BACKGROUND, DESKTOP_BACKGROUND).
 
     Requires the name of the function, the name of the file, and the path to the directory of the file.
-    '''
+    """
     python_loc = sys.executable
-    sys_section = f'''import sys; import os; sys.path.insert(0, '{func_dir_path}')'''.replace('\\', '/')
-    file_section = f'import {func_file_name}'
-    dir_path = 'os.getcwd()'
-    func_section = f'''{func_file_name}.{func_name}([{dir_path}],'{params}')'''
-    full_command = f'''"{python_loc}" -c "{sys_section}; {file_section}; {func_section}"'''
+    sys_section = (
+        f"""import sys; import os; sys.path.insert(0, '{func_dir_path}')""".replace(
+            "\\", "/"
+        )
+    )
+    file_section = f"import {func_file_name}"
+    dir_path = "os.getcwd()"
+    func_section = f"""{func_file_name}.{func_name}([{dir_path}],'{params}')"""
+    full_command = (
+        f'''"{python_loc}" -c "{sys_section}; {file_section}; {func_section}"'''
+    )
 
     return full_command
 
 
-def create_shell_command(command: str, command_vars: list) -> 'Shell command':
-    '''
+def create_shell_command(command: str, command_vars: list[CommandVar]) -> str:
+    """
     Creates a shell command and replaces '?' with the command_vars list
-    '''
+    """
 
-    transformed_vars = ["' + " + command_var_format(item) + " + '" for item in command_vars]
-    new_command = command.replace("?", '{}').format(*transformed_vars)
-    python_section = '''import os; import sys; os.system('{}')'''.format(new_command)
-    full_command = '"{}" -c "{}" \"%1\""'.format(sys.executable, python_section)
+    transformed_vars = [
+        "' + " + command_var_format(item) + " + '" for item in command_vars
+    ]
+    new_command = command.replace("?", "{}").format(*transformed_vars)
+    python_section = """import os; import sys; os.system('{}')""".format(new_command)
+    full_command = '"{}" -c "{}" "%1"'.format(sys.executable, python_section)
     return full_command
 
 
-
 # windows_menus.py ----------------------------------------------------------------------------------------
 
 
 # Used to create a Registry entry
 class RegistryMenu:
-    '''
+    """
     Class to convert the general menu from menus.py to a Windows-specific menu.
-    '''
+    """
 
-    def __init__(self, name: str, sub_items: list, type: str):
-        '''
+    def __init__(self, name: str, sub_items: list[ItemType], type: str, icon_path: str = None) -> None:
+        """
         Handled automatically by menus.py, but requires a name, all the sub items, and a type
-        '''
+        """
         self.name = name
         self.sub_items = sub_items
         self.type = type.upper()
+        self.icon_path = icon_path
         self.path = context_registry_format(type)
 
-    def create_menu(self, name: str, path: str) -> 'Path to shell key of new menu':
-        '''
+    def create_menu(self, name: str, path: str, icon_path: str = None) -> str:
+        """
         Creates a menu with the given name and path.
 
         Used in the compile method.
-        '''
-        key_path = os.path.join(path, name)
+        """
+        key_path = join_keys(path, name)
         create_key(key_path)
 
-        set_key_value(key_path, 'MUIVerb', name)
-        set_key_value(key_path, 'subcommands', '')
+        set_key_value(key_path, "MUIVerb", name)
+        set_key_value(key_path, "subcommands", "")
+        if icon_path is not None:
+            set_key_value(key_path, 'Icon', icon_path)
 
-        key_shell_path = os.path.join(key_path, 'shell')
+        key_shell_path = join_keys(key_path, "shell")
         create_key(key_shell_path)
 
         return key_shell_path
 
-    def create_command(self, name: str, path: str, command: str):
-        '''
+    def create_command(self, name: str, path: str, command: str) -> None:
+        """
         Creates a key with a command subkey with the 'name' and 'command', at path 'path'.
-        '''
-        key_path = os.path.join(path, name)
+        """
+        key_path = join_keys(path, name)
         create_key(key_path)
-        set_key_value(key_path, '', name)
+        set_key_value(key_path, "", name)
 
-        command_path = os.path.join(key_path, 'command')
+        command_path = join_keys(key_path, "command")
         create_key(command_path)
-        set_key_value(command_path, '', command)
+        set_key_value(command_path, "", command)
 
-    def compile(self, items: list = None, path: str = None):
-        '''
+    def compile(
+        self, items: list[ItemType] | None = None, path: str | None = None
+    ) -> None:
+        """
         Used to create the menu. Recursively iterates through each element in the top level menu.
-        '''
+        """
         if items == None:
             # run_admin()
             items = self.sub_items
-            path = self.create_menu(self.name, self.path)
+            path = self.create_menu(self.name, self.path, self.icon_path)
 
+        assert items is not None
+        assert path is not None
         for item in items:
             if item.isMenu:
                 # if the item is a menu
-                submenu_path = self.create_menu(item.name, path)
+                submenu_path = self.create_menu(item.name, path, self.icon_path)
                 self.compile(items=item.sub_items, path=submenu_path)
-            else:
-                # Otherwise the item is  a command
-                if item.command == None:
-                    # If a Python function is defined
-                    func_name, func_file_name, func_dir_path = item.get_method_info()
-                    new_command = None
-                    if self.type in ['DIRECTORY_BACKGROUND', 'DESKTOP_BACKGROUND']:
-                        # If it requires a background command
-                        new_command = create_directory_background_command(
-                            func_name, func_file_name, func_dir_path, item.params)
-                    else:
-                        # If it requires a file command
-                        new_command = create_file_select_command(
-                            func_name, func_file_name, func_dir_path, item.params)
-                    self.create_command(item.name, path, new_command)
-                elif item.command_vars != None:
-                    # If the item has to be ran from os.system
+                continue
 
-                    new_command = create_shell_command(item.command, item.command_vars)
-                    self.create_command(item.name, path, new_command)
+            # Otherwise the item is  a command
+            if item.command == None:
+                # If a Python function is defined
+                func_name, func_file_name, func_dir_path = item.get_method_info()
+                new_command = None
+                if self.type in ["DIRECTORY_BACKGROUND", "DESKTOP_BACKGROUND"]:
+                    # If it requires a background command
+                    new_command = create_directory_background_command(
+                        func_name, func_file_name, func_dir_path, item.params
+                    )
                 else:
-                    # The item is just a plain old command
-                    self.create_command(item.name, path, item.command)
+                    # If it requires a file command
+                    new_command = create_file_select_command(
+                        func_name, func_file_name, func_dir_path, item.params
+                    )
+                self.create_command(item.name, path, new_command)
+            elif item.command_vars != None:
+                # If the item has to be ran from os.system
+                assert item.command is not None
+                assert item.command_vars is not None
+                new_command = create_shell_command(item.command, item.command_vars)
+                self.create_command(item.name, path, new_command)
+            else:
+                # The item is just a plain old command
+                assert item.command is not None
+                self.create_command(item.name, path, item.command)
 
 
 # Fast command class
 # Everything is identical to either the RegistryMenu class or code in the menus file
 class FastRegistryCommand:
-    '''
+    """
     Fast command class.
 
     Everything is identical to either the RegistryMenu class or code in the menus file
-    '''
+    """
 
-    def __init__(self, name: str, type: str, command: str, python: 'function', params: str, command_vars: list):
+    def __init__(
+        self,
+        name: str,
+        type: ActivationType | str,
+        command: str,
+        python: FunctionType,
+        params: str,
+        command_vars: list[CommandVar],
+    ) -> None:
         self.name = name
         self.type = type
         self.path = context_registry_format(type)
         self.command = command
         self.python = python
-        self.params=params
+        self.params = params
         self.command_vars = command_vars
 
-    def get_method_info(self):
+    def get_method_info(self) -> MethodInfo:
         import inspect
 
         func_file_path = os.path.abspath(inspect.getfile(self.python))
 
         func_dir_path = os.path.dirname(func_file_path)
         func_name = self.python.__name__
         func_file_name = os.path.splitext(os.path.basename(func_file_path))[0]
 
         return (func_name, func_file_name, func_dir_path)
 
-    def compile(self):
+    def compile(self) -> None:
         # run_admin()
 
-        key_path = os.path.join(self.path, self.name)
+        key_path = join_keys(self.path, self.name)
         create_key(key_path)
 
-        command_path = os.path.join(key_path, 'command')
+        command_path = join_keys(key_path, "command")
         create_key(command_path)
 
         new_command = self.command
 
         if self.command == None:
             # If a python function is defined
             func_name, func_file_name, func_dir_path = self.get_method_info()
-            if self.type in ['DIRECTORY_BACKGROUND', 'DESKTOP_BACKGROUND']:
+            if self.type in ["DIRECTORY_BACKGROUND", "DESKTOP_BACKGROUND"]:
                 # If it requires a background selection
                 new_command = create_directory_background_command(
-                    func_name, func_file_name, func_dir_path, self.params)
+                    func_name, func_file_name, func_dir_path, self.params
+                )
             else:
                 # If it requires a file selection
                 new_command = create_file_select_command(
-                    func_name, func_file_name, func_dir_path, self.params)
+                    func_name, func_file_name, func_dir_path, self.params
+                )
         elif self.command_vars != None:
             # If it has command_vars
             new_command = create_shell_command(self.command, self.command_vars)
 
-        set_key_value(command_path, '', new_command)
+        set_key_value(command_path, "", new_command)
 
 
 # Testing section...
 
 try:
-    def remove_windows_menu(name: str, type: str):
-        '''
+
+    def remove_windows_menu(name: str, type: ActivationType | str) -> None:
+        """
         Removes a context menu from the windows registry.
-        '''
+        """
         # run_admin()
-        menu_path = os.path.join(context_registry_format(type), name)
+        menu_path = join_keys(context_registry_format(type), name)
         delete_key(menu_path)
-except:
+
+except Exception:
     pass
     # for testing
```

### Comparing `context_menu-1.3.1/context_menu.egg-info/PKG-INFO` & `context_menu-1.4.0/context_menu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: context-menu
-Version: 1.3.1
+Version: 1.4.0
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest-html; extra == "test"
 
-# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://travis-ci.com/saleguas/context_menu.svg?token=STF1haAqx5Xq2x9zdkHH&branch=master)](https://app.travis-ci.com/github/saleguas/context_menu)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
+# 🗂️[context_menu](https://github.com/saleguas/context_menu) [![build passing](https://github.com/saleguas/context_menu/actions/workflows/ci.yml/badge.svg)](https://github.com/saleguas/context_menu/actions/workflows/ci.yml)   [![readthedocs](https://img.shields.io/readthedocs/context_menu)](https://context-menu.readthedocs.io/en/latest/) ![pip](https://img.shields.io/badge/pip-context__menu-blue) [![Downloads](https://pepy.tech/badge/context-menu)](https://pepy.tech/project/context-menu)
 
 ![logo](media/logo.png)
 
 💻 A Python library to create and deploy cross-platform native context menus. 💻
 
 
 Documentation available at: https://context-menu.readthedocs.io/en/latest/
@@ -82,15 +84,15 @@
 - Windows 7
 - Windows 10
 - Windows 11
 - Linux (Using Nautilus)
 
 ## 🐍 What Python versions are supported? 🐍
 
-**All python versions 3.1 and above** are supported.
+**All python versions 3.7 and above** are supported.
 
 # 💽 Installation 💽
 
 If you haven't installed Python, download and run an installer from the official
 website: https://www.python.org/downloads/
 
 Once you have Python, the rest is super simple. Simply just run the following command in a terminal to install the
@@ -182,19 +184,19 @@
 All context menus are **permanent** unless you remove them.
 
 # 🤖 Advanced Usage 🤖
 
 ## The `ContextMenu` Class
 
 The [ContextMenu](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu) object
-holds other context objects. It expects a name, and **the activation type** if it is the root menu(the first menu). Only
+holds other context objects. It expects a name, **the activation type** if it is the root menu(the first menu), and an optional icon path. Only
 compile the root menu.
 
 ```Python
-ContextMenu(name: str, type: str = None)
+ContextMenu(name: str, type: str = None, icon_path: str = None)
 ```
 
 Menus can be added to menus, creating cascading context menus. You can use
 the [{MENU}.add_items{ITEMS}](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextMenu.add_items)
 function to add context elements together, for example:
 
 ```Python
@@ -348,14 +350,15 @@
 
 | Name                 | Location                                                           | Action                                   |
 | -------------------- | ------------------------------------------------------------------ | ---------------------------------------- |
 | FILES                | HKEY_CURRENT_USER\\Software\\Classes\\\*\\shell\\                  | Opens on a file                          |
 | DIRECTORY            | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\shell             | Opens on a directory                     |
 | DIRECTORY_BACKGROUND | HKEY_CURRENT_USER\\Software\\Classes\\Directory\\Background\\shell | Opens on the background of the Directory |
 | DRIVE                | HKEY_CURRENT_USER\\Software\\Classes\\Drive\\shell                 | Opens on the drives(think USBs)          |
+| DESKTOP              | Software\\Classes\\DesktopBackground\\shell                        | Opens on the background of the desktop   |
 
 * * *
 
 I strongly recommend checking out the [examples folder](examples) for more complicated examples and usage.
 
 You can check out the official documentation [here](https://context-menu.readthedocs.io/en/latest/index.html).
```

### Comparing `context_menu-1.3.1/setup.py` & `context_menu-1.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import pathlib
 import setuptools
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
-README = (HERE / "README.md").read_text(encoding='utf-8')
+README = (HERE / "README.md").read_text(encoding="utf-8")
 
 # This call to setup() does all the work
 setuptools.setup(
     name="context_menu",
-    version="1.3.1",
+    version="1.4.0",
     description="Library to create cross-platform native context menus.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/saleguas/context_menu",
     author="Salvador Aleguas",
     author_email="salvador@aleguas.dev",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
-    packages=setuptools.find_packages(),
+    python_requires=">= 3.7",
+    packages=setuptools.find_packages(exclude=["tests*"]),
+    extras_require={"test": ["pytest-html"]},
 )
```

