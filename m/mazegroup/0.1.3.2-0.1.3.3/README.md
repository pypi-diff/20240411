# Comparing `tmp/mazegroup-0.1.3.2.tar.gz` & `tmp/mazegroup-0.1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mazegroup-0.1.3.2.tar", last modified: Wed Apr 10 19:50:19 2024, max compression
+gzip compressed data, was "mazegroup-0.1.3.3.tar", last modified: Thu Apr 11 07:21:09 2024, max compression
```

## Comparing `mazegroup-0.1.3.2.tar` & `mazegroup-0.1.3.3.tar`

### file list

```diff
@@ -1,22 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/echo/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/echo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup/saves/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/saves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/mazegroup/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/mazegroup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 19:50:19.000000 mazegroup-0.1.3.2/mazegroup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:50:19.238761 mazegroup-0.1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-10 19:50:14.000000 mazegroup-0.1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.269424 mazegroup-0.1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-11 07:21:09.269424 mazegroup-0.1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/echo/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/echo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/help/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/ls/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/ls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup/pyeval/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/pyeval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.269424 mazegroup-0.1.3.3/mazegroup/pyexec/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/pyexec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.269424 mazegroup-0.1.3.3/mazegroup/saves/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/saves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/mazegroup/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:21:09.265424 mazegroup-0.1.3.3/mazegroup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-11 07:21:09.000000 mazegroup-0.1.3.3/mazegroup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-11 07:21:09.000000 mazegroup-0.1.3.3/mazegroup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:21:09.000000 mazegroup-0.1.3.3/mazegroup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-11 07:21:09.000000 mazegroup-0.1.3.3/mazegroup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 07:21:09.000000 mazegroup-0.1.3.3/mazegroup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:21:09.269424 mazegroup-0.1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 07:21:04.000000 mazegroup-0.1.3.3/setup.py
```

### Comparing `mazegroup-0.1.3.2/PKG-INFO` & `mazegroup-0.1.3.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,28 @@
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
 # If there is a error, shows it (optional) :
 if type(returned) != utils.NoError:
-	print("Error :", returned)
+	print("Error :", returned.message)
 ```
 
+### Arguments
+
+You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
+
 ## Commands available :
 
-- `echo <...>``
+- `echo <...>`
 	- Print the textes in arguments.
+- `help <...>`
+	- Shows all commands available.
+- `ls <path>`
+	- Shows all directories and files from the selected path.
+- `pyexec <...>`
+	- Execute the Python code in arguments.
+- `pyeval <...>`
+	- Evaluate the Python expression in arguments.
```

### Comparing `mazegroup-0.1.3.2/README.md` & `mazegroup-0.1.3.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,26 @@
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
 # If there is a error, shows it (optional) :
 if type(returned) != utils.NoError:
-	print("Error :", returned)
+	print("Error :", returned.message)
 ```
 
+### Arguments
+
+You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
+
 ## Commands available :
 
-- `echo <...>``
+- `echo <...>`
 	- Print the textes in arguments.
+- `help <...>`
+	- Shows all commands available.
+- `ls <path>`
+	- Shows all directories and files from the selected path.
+- `pyexec <...>`
+	- Execute the Python code in arguments.
+- `pyeval <...>`
+	- Evaluate the Python expression in arguments.
```

### Comparing `mazegroup-0.1.3.2/mazegroup/commands.py` & `mazegroup-0.1.3.3/mazegroup/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,17 +66,20 @@
         for arg in self.args_:
             self.args[arg.name] = arg
         self.overflow = overflow
 
     def addArg(self, arg:Arg): self.args.append(arg)
 
     def tryArgs(self, args:list):
+        ag = []
+        for arg in self.args.values():
+            if arg.required: ag.append(arg)
         if len(args) > len(self.args) and not self.overflow:
             return utils.Error(f"Arguments overflow, {len(args)} was given but {len(self.args)} was waited")
-        elif len(args) < len(self.args):
+        elif len(args) < len(ag):
             return utils.Error(f"Missing arguments, {len(args)} was given but {len(self.args)} was waited")
         for arg_index, value in enumerate(args):
             if type(value) == dict:
                 try:
                     arg_index = value.keys()[0]
                 except:
                     return utils.Error()
@@ -134,15 +137,18 @@
         elif type(args) == dict:
             args = args.keys()
         else:
             return utils.Error(f"Bad arguments type on the '{self.name}' command execution")
         r = self.args.tryArgs(args)
         if type(r) != utils.NoError:
             _ = self.args.getArgsNames(); __ = ""
-            if not len(self.args.args_) < len(self.args.args):
+            args_ = []
+            for arg in self.args.args_:
+                if arg.required: args_.append(arg)
+            if not len(args_) < len(self.args.args):
                 for arg in _: __ += f"<{arg}>"
             else:
                 __ = f"<...>"
             return utils.Error(f"{r.message}\nUsage : mazegroup {self.name} {__}")
         try:
             if self.unique:
                 self.function(self.args.args)
```

### Comparing `mazegroup-0.1.3.2/mazegroup/utils.py` & `mazegroup-0.1.3.3/mazegroup/utils.py`

 * *Files identical despite different names*

### Comparing `mazegroup-0.1.3.2/mazegroup.egg-info/PKG-INFO` & `mazegroup-0.1.3.3/mazegroup.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazegroup
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: MazeGroup.py is an general prupose library for Python.
 Home-page: https://github.com/Geniusum/mazegroup.py
 Author: Genius_um
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -53,16 +53,28 @@
 import mazegroup.commands as commands
 import mazegroup.utils as utils  # For error checking
 
 returned = commands.executeCommand("echo", ["Hello,", "world!"])  # Echo "Hello, world!" by example
 
 # If there is a error, shows it (optional) :
 if type(returned) != utils.NoError:
-	print("Error :", returned)
+	print("Error :", returned.message)
 ```
 
+### Arguments
+
+You can evaluate Python expression in using `py:` in the argument (only the actual argument will be evaluate), by example the argument `"py:5 + 5"` will returns 10, we use `"` because we also use spaces on the expression.
+
 ## Commands available :
 
-- `echo <...>``
+- `echo <...>`
 	- Print the textes in arguments.
+- `help <...>`
+	- Shows all commands available.
+- `ls <path>`
+	- Shows all directories and files from the selected path.
+- `pyexec <...>`
+	- Execute the Python code in arguments.
+- `pyeval <...>`
+	- Evaluate the Python expression in arguments.
```

### Comparing `mazegroup-0.1.3.2/setup.py` & `mazegroup-0.1.3.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import setup, find_packages
 
-#
-
 setup(
     name="mazegroup",
-    version="0.1.3.2",
+    version="0.1.3.3",
     description="MazeGroup.py is an general prupose library for Python.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Genius_um",
     python_requires=">=3.9",
     url="https://github.com/Geniusum/mazegroup.py",
-    packages=["mazegroup", "mazegroup/cli", "mazegroup/echo", "mazegroup/saves"], # find_packages(),
+    packages=find_packages(),#["mazegroup", "mazegroup/cli", "mazegroup/echo", "mazegroup/saves"], # find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
```

