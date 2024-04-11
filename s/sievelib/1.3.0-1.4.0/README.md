# Comparing `tmp/sievelib-1.3.0.tar.gz` & `tmp/sievelib-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sievelib-1.3.0.tar", last modified: Thu Mar 28 14:10:07 2024, max compression
+gzip compressed data, was "sievelib-1.4.0.tar", last modified: Thu Apr 11 08:02:05 2024, max compression
```

## Comparing `sievelib-1.3.0.tar` & `sievelib-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.120573 sievelib-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-28 14:09:59.000000 sievelib-1.3.0/.github/workflows/sievelib.yml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-28 14:09:59.000000 sievelib-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-28 14:09:59.000000 sievelib-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-28 14:09:59.000000 sievelib-1.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 14:09:59.000000 sievelib-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-28 14:10:07.124573 sievelib-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-03-28 14:09:59.000000 sievelib-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-28 14:09:59.000000 sievelib-1.3.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 14:09:59.000000 sievelib-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-28 14:10:07.124573 sievelib-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-03-28 14:09:59.000000 sievelib-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/sievelib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/digest_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)    20037 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    23574 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/managesieve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19133 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/sievelib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/sievelib/tests/files/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tests/files/utf8_sieve.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tests/test_managesieve.py
--rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 14:09:59.000000 sievelib-1.3.0/sievelib/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:10:07.124573 sievelib-1.3.0/sievelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-28 14:10:07.000000 sievelib-1.3.0/sievelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 14:10:07.000000 sievelib-1.3.0/sievelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:10:07.000000 sievelib-1.3.0/sievelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 14:10:07.000000 sievelib-1.3.0/sievelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.269854 sievelib-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.265854 sievelib-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.265854 sievelib-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-11 08:02:01.000000 sievelib-1.4.0/.github/workflows/sievelib.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 08:02:01.000000 sievelib-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 08:02:01.000000 sievelib-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-11 08:02:01.000000 sievelib-1.4.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 08:02:01.000000 sievelib-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-11 08:02:05.269854 sievelib-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-11 08:02:01.000000 sievelib-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 08:02:01.000000 sievelib-1.4.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 08:02:01.000000 sievelib-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:02:05.269854 sievelib-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-11 08:02:01.000000 sievelib-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.265854 sievelib-1.4.0/sievelib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35086 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/digest_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21911 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/managesieve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19409 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.269854 sievelib-1.4.0/sievelib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.269854 sievelib-1.4.0/sievelib/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tests/files/utf8_sieve.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16265 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tests/test_managesieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25120 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 08:02:01.000000 sievelib-1.4.0/sievelib/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:02:05.269854 sievelib-1.4.0/sievelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-11 08:02:05.000000 sievelib-1.4.0/sievelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-11 08:02:05.000000 sievelib-1.4.0/sievelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:02:05.000000 sievelib-1.4.0/sievelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 08:02:05.000000 sievelib-1.4.0/sievelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 08:02:05.000000 sievelib-1.4.0/sievelib.egg-info/top_level.txt
```

### Comparing `sievelib-1.3.0/.github/workflows/sievelib.yml` & `sievelib-1.4.0/.github/workflows/sievelib.yml`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           pip install codecov pytest pytest-cov
+          pip install -e .
       - name: Run tests
         if: ${{ matrix.python-version != '3.11' }}
         run: |
           pytest
       - name: Run tests and coverage
         if: ${{ matrix.python-version == '3.11' }}
         run: |
```

### Comparing `sievelib-1.3.0/COPYING` & `sievelib-1.4.0/COPYING`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2011-2015 Antoine Nguyen <tonio@ngyn.org>
+Copyright (c) 2011-2024 Antoine Nguyen <tonio@ngyn.org>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sievelib-1.3.0/PKG-INFO` & `sievelib-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sievelib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Client-side SIEVE library
 Home-page: https://github.com/tonioo/sievelib
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: sieve,managesieve,parser,client
 Classifier: Programming Language :: Python
```

### Comparing `sievelib-1.3.0/README.rst` & `sievelib-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sievelib-1.3.0/setup.py` & `sievelib-1.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         include_package_data=True,
         description="Client-side SIEVE library",
         author="Antoine Nguyen",
         author_email="tonio@ngyn.org",
         url="https://github.com/tonioo/sievelib",
         license="MIT",
         keywords=["sieve", "managesieve", "parser", "client"],
-        install_requires=[],
+        install_requires=["typing-extensions"],
         setup_requires=["setuptools_scm"],
         use_scm_version={"local_scheme": local_scheme},
         classifiers=[
             "Programming Language :: Python",
             "Development Status :: 5 - Production/Stable",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
```

### Comparing `sievelib-1.3.0/sievelib/commands.py` & `sievelib-1.4.0/sievelib/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,30 @@
 provides extra information such as:
  * expected arguments,
  * completion callback,
  * etc.
 
 """
 
-import sys
 from collections.abc import Iterable
+import sys
+from typing import Any, Dict, Iterator, List, Optional, TypedDict, Union
+from typing_extensions import NotRequired
+
 from . import tools
 
 
 class CommandError(Exception):
     """Base command exception class."""
 
-    pass
-
 
 class UnknownCommand(CommandError):
     """Specific exception raised when an unknown command is encountered"""
 
-    def __init__(self, name):
+    def __init__(self, name: str):
         self.name = name
 
     def __str__(self):
         return "unknown command %s" % self.name
 
 
 class BadArgument(CommandError):
@@ -74,30 +75,50 @@
     def __init__(self, name):
         self.name = name
 
     def __str__(self):
         return "extension '{}' not loaded".format(self.name)
 
 
+class CommandExtraArg(TypedDict):
+    """Type definition for command extra argument."""
+
+    type: Union[str, List[str]]
+    values: NotRequired[List[str]]
+    valid_for: NotRequired[List[str]]
+
+
+class CommandArg(TypedDict):
+    """Type definition for command argument."""
+
+    name: str
+    type: List[str]
+    required: NotRequired[bool]
+    values: NotRequired[List[str]]
+    extra_arg: NotRequired[CommandExtraArg]
+    extension: NotRequired[str]
+    extension_values: NotRequired[Dict[str, str]]
+
+
 # Statement elements (see RFC, section 8.3)
 # They are used in different commands.
-comparator = {
+comparator: CommandArg = {
     "name": "comparator",
     "type": ["tag"],
     "values": [":comparator"],
     "extra_arg": {"type": "string", "values": ['"i;octet"', '"i;ascii-casemap"']},
     "required": False,
 }
-address_part = {
+address_part: CommandArg = {
     "name": "address-part",
     "values": [":localpart", ":domain", ":all"],
     "type": ["tag"],
     "required": False,
 }
-match_type = {
+match_type: CommandArg = {
     "name": "match-type",
     "values": [":is", ":contains", ":matches"],
     "extension_values": {
         ":count": "relational",
         ":value": "relational",
         ":regex": "regex",
     },
@@ -107,55 +128,58 @@
         "valid_for": [":count", ":value"],
     },
     "type": ["tag"],
     "required": False,
 }
 
 
-class Command(object):
+class Command:
     """Generic command representation.
 
     A command is described as follow:
      * A name
      * A type
      * A description of supported arguments
      * Does it accept an unknown quantity of arguments? (ex: anyof, allof)
      * Does it accept children? (ie. subcommands)
      * Is it an extension?
      * Must follow only certain commands
 
     """
 
-    _type = None
-    variable_args_nb = False
-    non_deterministic_args = False
-    accept_children = False
-    must_follow = None
-    extension = None
+    args_definition: List[CommandArg]
+    _type: str
+    variable_args_nb: bool = False
+    non_deterministic_args: bool = False
+    accept_children: bool = False
+    must_follow: Optional[List[str]] = None
+    extension: Optional[str] = None
 
-    def __init__(self, parent=None):
+    def __init__(self, parent: Optional["Command"] = None):
         self.parent = parent
-        self.arguments = {}
-        self.extra_arguments = {}  # to store tag arguments
-        self.children = []
+        self.arguments: Dict[str, Any] = {}
+        self.extra_arguments: Dict[str, Any] = {}  # to store tag arguments
+        self.children: List[Command] = []
 
         self.nextargpos = 0
         self.required_args = -1
         self.rargs_cnt = 0
-        self.curarg = None  # for arguments that expect an argument :p (ex: :comparator)
+        self.curarg: Union[CommandArg, None] = (
+            None  # for arguments that expect an argument :p (ex: :comparator)
+        )
 
-        self.name = self.__class__.__name__.replace("Command", "")
+        self.name: str = self.__class__.__name__.replace("Command", "")
         self.name = self.name.lower()
 
-        self.hash_comments = []
+        self.hash_comments: List[bytes] = []
 
     def __repr__(self):
         return "%s (type: %s)" % (self.name, self._type)
 
-    def tosieve(self, indentlevel=0, target=sys.stdout):
+    def tosieve(self, indentlevel: int = 0, target=sys.stdout):
         """Generate the sieve syntax corresponding to this command
 
         Recursive method.
 
         :param indentlevel: current indentation level
         :param target: opened file pointer where the content will be printed
         """
@@ -209,22 +233,24 @@
         if self.get_type() != "control":
             return
         target.write(" {\n")
         for ch in self.children:
             ch.tosieve(indentlevel + 4, target=target)
         self.__print("}", indentlevel, target=target)
 
-    def __print(self, data, indentlevel, nocr=False, target=sys.stdout):
+    def __print(
+        self, data: str, indentlevel: int, nocr: bool = False, target=sys.stdout
+    ):
         text = "%s%s" % (" " * indentlevel, data)
         if nocr:
             target.write(text)
         else:
             target.write(text + "\n")
 
-    def __get_arg_type(self, arg):
+    def __get_arg_type(self, arg: str) -> Optional[List[str]]:
         """Return the type corresponding to the given name.
 
         :param arg: a defined argument name
         """
         for a in self.args_definition:
             if a["name"] == arg:
                 return a["type"]
@@ -233,30 +259,30 @@
     def complete_cb(self):
         """Completion callback
 
         Called when a command is considered as complete by the parser.
         """
         pass
 
-    def get_expected_first(self):
+    def get_expected_first(self) -> Optional[List[str]]:
         """Return the first expected token for this command"""
         return None
 
-    def has_arguments(self):
+    def has_arguments(self) -> bool:
         return len(self.args_definition) != 0
 
     def reassign_arguments(self):
         """Reassign arguments to proper slots.
 
         Should be called when parsing of commands with non
         deterministic arguments is considered done.
         """
         raise NotImplementedError
 
-    def dump(self, indentlevel=0, target=sys.stdout):
+    def dump(self, indentlevel: int = 0, target=sys.stdout):
         """Display the command
 
         Pretty printing of this command and its eventual arguments and
         children. (recursively)
 
         :param indentlevel: integer that indicates indentation level to apply
         """
@@ -287,15 +313,15 @@
                 if isinstance(value, Command):
                     value.dump(indentlevel, target)
                     continue
                 self.__print(str(value), indentlevel, target=target)
         for ch in self.children:
             ch.dump(indentlevel, target)
 
-    def walk(self):
+    def walk(self) -> Iterator["Command"]:
         """Walk through commands."""
         yield self
         if self.has_arguments():
             for arg in self.args_definition:
                 if not arg["name"] in self.arguments:
                     continue
                 value = self.arguments[arg["name"]]
@@ -307,29 +333,31 @@
                 if isinstance(value, Command):
                     for node in value.walk():
                         yield node
         for ch in self.children:
             for node in ch.walk():
                 yield node
 
-    def addchild(self, child):
+    def addchild(self, child: "Command") -> bool:
         """Add a new child to the command
 
         A child corresponds to a command located into a block (this
         command's block). It can be either an action or a control.
 
         :param child: the new child
         :return: True on succes, False otherwise
         """
         if not self.accept_children:
             return False
         self.children += [child]
         return True
 
-    def iscomplete(self, atype=None, avalue=None):
+    def iscomplete(
+        self, atype: Optional[str] = None, avalue: Optional[str] = None
+    ) -> bool:
         """Check if the command is complete
 
         Check if all required arguments have been encountered. For
         commands that allow an undefined number of arguments, this
         method always returns False.
 
         :return: True if command is complete, False otherwise
@@ -338,38 +366,40 @@
             return False
         if self.required_args == -1:
             self.required_args = 0
             for arg in self.args_definition:
                 if arg.get("required", False):
                     self.required_args += 1
         return (
-            not self.curarg
+            self.curarg is None
             or "extra_arg" not in self.curarg
             or (
                 "valid_for" in self.curarg["extra_arg"]
                 and atype
                 and atype in self.curarg["extra_arg"]["type"]
                 and avalue not in self.curarg["extra_arg"]["valid_for"]
             )
         ) and (self.rargs_cnt == self.required_args)
 
-    def get_type(self):
+    def get_type(self) -> str:
         """Return the command's type"""
         if self._type is None:
             raise NotImplementedError
         return self._type
 
-    def __is_valid_value_for_arg(self, arg, value, check_extension=True):
+    def __is_valid_value_for_arg(
+        self, arg: CommandArg, value: str, check_extension: bool = True
+    ) -> bool:
         """Check if value is allowed for arg
 
         Some commands only allow a limited set of values. The method
         always returns True for methods that do not provide such a
         set.
 
-        :param arg: the argument's name
+        :param arg: the argument
         :param value: the value to check
         :param check_extension: check if value requires an extension
         :return: True on succes, False otherwise
         """
         if "values" not in arg and "extension_values" not in arg:
             return True
         if "values" in arg and value.lower() in arg["values"]:
@@ -382,28 +412,30 @@
                     and extension not in RequireCommand.loaded_extensions
                 )
                 if condition:
                     raise ExtensionNotLoaded(extension)
                 return True
         return False
 
-    def __is_valid_type(self, typ, typlist):
+    def __is_valid_type(self, typ: str, typlist: List[str]) -> bool:
         """Check if type is valid based on input type list
             "string" is special because it can be used for stringlist
 
         :param typ: the type to check
         :param typlist: the list of type to check
         :return: True on success, False otherwise
         """
         typ_is_str = typ == "string"
         str_list_in_typlist = "stringlist" in typlist
 
         return typ in typlist or (typ_is_str and str_list_in_typlist)
 
-    def check_next_arg(self, atype, avalue, add=True, check_extension=True):
+    def check_next_arg(
+        self, atype: str, avalue: str, add: bool = True, check_extension: bool = True
+    ) -> bool:
         """Argument validity checking
 
         This method is usually used by the parser to check if detected
         argument is allowed for this command.
 
         We make a distinction between required and optional
         arguments. Optional (or tagged) arguments can be provided
@@ -464,15 +496,15 @@
                     self.curarg = curarg
                     self.rargs_cnt += 1
                     self.nextargpos = pos + 1
                     if add:
                         self.arguments[curarg["name"]] = avalue
                 break
 
-            condition = atype in curarg["type"] and self.__is_valid_value_for_arg(
+            condition: bool = atype in curarg["type"] and self.__is_valid_value_for_arg(
                 curarg, avalue, check_extension
             )
             if condition:
                 ext = curarg.get("extension")
                 condition = (
                     check_extension
                     and ext
@@ -492,19 +524,19 @@
 
             pos += 1
 
         if failed:
             raise BadArgument(self.name, avalue, self.args_definition[pos]["type"])
         return True
 
-    def __contains__(self, name):
+    def __contains__(self, name: str) -> bool:
         """Check if argument is provided with command."""
         return name in self.arguments
 
-    def __getitem__(self, name):
+    def __getitem__(self, name: str) -> Any:
         """Shorcut to access a command argument
 
         :param name: the argument's name
         """
         found = False
         for ad in self.args_definition:
             if ad["name"] == name:
@@ -531,15 +563,15 @@
     unloaded extensions during the parsing)
     """
 
     args_definition = [
         {"name": "capabilities", "type": ["string", "stringlist"], "required": True}
     ]
 
-    loaded_extensions = []
+    loaded_extensions: List[str] = []
 
     def complete_cb(self):
         if type(self.arguments["capabilities"]) != list:
             exts = [self.arguments["capabilities"]]
         else:
             exts = self.arguments["capabilities"]
         for ext in exts:
@@ -549,24 +581,24 @@
 
 
 class IfCommand(ControlCommand):
     accept_children = True
 
     args_definition = [{"name": "test", "type": ["test"], "required": True}]
 
-    def get_expected_first(self):
+    def get_expected_first(self) -> List[str]:
         return ["identifier"]
 
 
 class ElsifCommand(ControlCommand):
     accept_children = True
     must_follow = ["if", "elsif"]
     args_definition = [{"name": "test", "type": ["test"], "required": True}]
 
-    def get_expected_first(self):
+    def get_expected_first(self) -> List[str]:
         return ["identifier"]
 
 
 class ElseCommand(ControlCommand):
     accept_children = True
     must_follow = ["if", "elsif"]
     args_definition = []
@@ -713,25 +745,25 @@
 
 class AllofCommand(TestCommand):
     accept_children = True
     variable_args_nb = True
 
     args_definition = [{"name": "tests", "type": ["testlist"], "required": True}]
 
-    def get_expected_first(self):
+    def get_expected_first(self) -> List[str]:
         return ["left_parenthesis"]
 
 
 class AnyofCommand(TestCommand):
     accept_children = True
     variable_args_nb = True
 
     args_definition = [{"name": "tests", "type": ["testlist"], "required": True}]
 
-    def get_expected_first(self):
+    def get_expected_first(self) -> List[str]:
         return ["left_parenthesis"]
 
 
 class EnvelopeCommand(TestCommand):
     args_definition = [
         comparator,
         address_part,
@@ -1040,15 +1072,17 @@
         cmds = [cmds]
 
     for command in cmds:
         if command.__name__.endswith("Command"):
             globals()[command.__name__] = command
 
 
-def get_command_instance(name, parent=None, checkexists=True):
+def get_command_instance(
+    name: str, parent: Optional[Command] = None, checkexists: bool = True
+) -> Command:
     """Try to guess and create the appropriate command instance
 
     Given a command name (encountered by the parser), construct the
     associated class name and, if known, return a new instance.
 
     If the command is not known or has not been loaded using require,
     an UnknownCommand exception is raised.
```

### Comparing `sievelib-1.3.0/sievelib/digest_md5.py` & `sievelib-1.4.0/sievelib/digest_md5.py`

 * *Files identical despite different names*

### Comparing `sievelib-1.3.0/sievelib/factory.py` & `sievelib-1.4.0/sievelib/factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,62 +6,78 @@
 
 Only commands (control/test/action) defined in the ``commands`` module
 are supported.
 """
 
 import io
 import sys
+from typing import List, Optional, TypedDict, Union
+from typing_extensions import NotRequired
 
 from sievelib import commands
 
 
-class FiltersSet(object):
+class FilterAlreadyExists(Exception):
+    pass
+
+
+class Filter(TypedDict):
+    """Type definition for filter."""
+
+    name: str
+    content: commands.Command
+    enabled: bool
+    description: NotRequired[str]
+
+
+class FiltersSet:
     """A set of filters."""
 
     def __init__(
         self,
-        name,
-        filter_name_pretext="# Filter: ",
-        filter_desc_pretext="# Description: ",
+        name: str,
+        filter_name_pretext: str = "# Filter: ",
+        filter_desc_pretext: str = "# Description: ",
     ):
-        """Represents a set of one or more filters
+        """
+        Represents a set of one or more filters.
 
         :param name: the filterset's name
         :param filter_name_pretext: the text that is used to mark a filter name
                                     (as comment preceding the filter)
         :param filter_desc_pretext: the text that is used to mark a filter
                                      description
         """
         self.name = name
         self.filter_name_pretext = filter_name_pretext
         self.filter_desc_pretext = filter_desc_pretext
-        self.requires = []
-        self.filters = []
+        self.requires: List[str] = []
+        self.filters: List[Filter] = []
 
     def __str__(self):
         target = io.StringIO()
         self.tosieve(target)
         ret = target.getvalue()
         target.close()
         return ret
 
-    def __isdisabled(self, fcontent):
+    def __isdisabled(self, fcontent: commands.Command) -> bool:
         """Tells if a filter is disabled or not
 
         Simply checks if the filter is surrounded by a "if false" test.
 
         :param fcontent: the filter's name
         """
         if not isinstance(fcontent, commands.IfCommand):
             return False
         if not isinstance(fcontent["test"], commands.FalseCommand):
             return False
         return True
 
-    def from_parser_result(self, parser):
+    def from_parser_result(self, parser: "sievelib.parser.Parser"):
         cpt = 1
         for f in parser.result:
             if isinstance(f, commands.RequireCommand):
                 if type(f.arguments["capabilities"]) == list:
                     [self.require(c) for c in f.arguments["capabilities"]]
                 else:
                     self.require(f.arguments["capabilities"])
@@ -82,51 +98,53 @@
                     "description": description,
                     "content": f,
                     "enabled": not self.__isdisabled(f),
                 }
             ]
             cpt += 1
 
-    def require(self, name):
+    def require(self, name: str):
         """Add a new extension to the requirements list
 
         :param name: the extension's name
         """
         name = name.strip('"')
         if name not in self.requires:
             self.requires += [name]
 
-    def check_if_arg_is_extension(self, arg):
+    def check_if_arg_is_extension(self, arg: str):
         """Include extension if arg requires one."""
         args_using_extensions = {":copy": "copy"}
         if arg in args_using_extensions:
             self.require(args_using_extensions[arg])
 
-    def __gen_require_command(self):
+    def __gen_require_command(self) -> Union[commands.Command, None]:
         """Internal method to create a RequireCommand based on requirements
 
         Called just before this object is going to be dumped.
         """
         if not len(self.requires):
             return None
         reqcmd = commands.get_command_instance("require")
         reqcmd.check_next_arg("stringlist", self.requires)
         return reqcmd
 
-    def __quote_if_necessary(self, value):
+    def __quote_if_necessary(self, value: str) -> str:
         """Add double quotes to the given string if necessary
 
         :param value: the string to check
         :return: the string between quotes
         """
         if not value.startswith(('"', "'")):
             return '"%s"' % value
         return value
 
-    def __build_condition(self, condition, parent, tag=None):
+    def __build_condition(
+        self, condition: List[str], parent: commands.Command, tag: Optional[str] = None
+    ) -> commands.Command:
         """Translate a condition to a valid sievelib Command.
 
         :param list condition: condition's definition
         :param ``Command`` parent: the parent
         :param str tag: tag to use instead of the one included into :keyword:`condition`
         :rtype: Command
         :return: the generated command
@@ -135,15 +153,20 @@
             tag = condition[1]
         cmd = commands.get_command_instance("header", parent)
         cmd.check_next_arg("tag", tag)
         cmd.check_next_arg("string", self.__quote_if_necessary(condition[0]))
         cmd.check_next_arg("string", self.__quote_if_necessary(condition[2]))
         return cmd
 
-    def __create_filter(self, conditions, actions, matchtype="anyof"):
+    def __create_filter(
+        self,
+        conditions: List[tuple],
+        actions: List[tuple],
+        matchtype: str = "anyof",
+    ) -> commands.Command:
         """Create a new filter
 
         A filter is composed of:
          * a name
          * one or more conditions (tests) combined together using ``matchtype``
          * one or more actions
 
@@ -263,109 +286,150 @@
                 else:
                     atype = "string"
                     arg = self.__quote_if_necessary(arg)
                 action.check_next_arg(atype, arg, check_extension=False)
             ifcontrol.addchild(action)
         return ifcontrol
 
-    def _unicode_filter_name(self, name):
+    def _unicode_filter_name(self, name) -> str:
         """Convert name to unicode if necessary."""
         return name.decode("utf-8") if isinstance(name, bytes) else name
 
-    def addfilter(self, name, conditions, actions, matchtype="anyof"):
+    def filter_exists(self, name: str) -> bool:
+        """Check if a filter with name already exists."""
+        for existing_filter in self.filters:
+            if existing_filter["name"] == name:
+                return True
+        return False
+
+    def addfilter(
+        self,
+        name: str,
+        conditions: List[tuple],
+        actions: List[tuple],
+        matchtype: str = "anyof",
+    ):
         """Add a new filter to this filters set
 
         :param name: the filter's name
         :param conditions: the list of conditions
         :param actions: the list of actions
         :param matchtype: "anyof" or "allof"
         """
+        name = self._unicode_filter_name(name)
+        if self.filter_exists(name):
+            raise FilterAlreadyExists
         ifcontrol = self.__create_filter(conditions, actions, matchtype)
         self.filters += [
             {
-                "name": self._unicode_filter_name(name),
+                "name": name,
                 "content": ifcontrol,
                 "enabled": True,
             }
         ]
 
-    def updatefilter(self, oldname, newname, conditions, actions, matchtype="anyof"):
+    def updatefilter(
+        self,
+        oldname: str,
+        newname: str,
+        conditions: List[tuple],
+        actions: List[tuple],
+        matchtype: str = "anyof",
+    ) -> bool:
         """Update a specific filter
 
         Instead of removing and re-creating the filter, we update the
         content in order to keep the original order between filters.
 
         :param oldname: the filter's current name
         :param newname: the filter's new name
         :param conditions: the list of conditions
         :param actions: the list of actions
         :param matchtype: "anyof" or "allof"
         """
+        filter_def = None
         oldname = self._unicode_filter_name(oldname)
-        newname = self._unicode_filter_name(newname)
         for f in self.filters:
             if f["name"] == oldname:
-                f["name"] = newname
-                f["content"] = self.__create_filter(conditions, actions, matchtype)
-                if not f["enabled"]:
-                    return self.disablefilter(newname)
-                return True
-        return False
+                filter_def = f
+                break
+        if not filter_def:
+            return False
+        newname = self._unicode_filter_name(newname)
+        if newname != oldname and self.filter_exists(newname):
+            raise FilterAlreadyExists
+        filter_def["name"] = newname
+        filter_def["content"] = self.__create_filter(conditions, actions, matchtype)
+        if not filter_def["enabled"]:
+            return self.disablefilter(newname)
+        return True
 
-    def replacefilter(self, oldname, sieve_filter, newname=None, description=None):
+    def replacefilter(
+        self,
+        oldname: str,
+        sieve_filter: commands.Command,
+        newname: Optional[str] = None,
+        description: Optional[str] = None,
+    ) -> bool:
         """replace a specific sieve_filter
 
         Instead of removing and re-creating the sieve_filter, we update the
         content in order to keep the original order between filters.
 
         :param oldname: the sieve_filter's current name
         :param newname: the sieve_filter's new name
         :param sieve_filter: the sieve_filter object as get from
                              FiltersSet.getfilter()
         """
+        filter_def = None
         oldname = self._unicode_filter_name(oldname)
-        newname = self._unicode_filter_name(newname)
-        if newname is None:
-            newname = oldname
         for f in self.filters:
             if f["name"] == oldname:
-                f["name"] = newname
-                f["content"] = sieve_filter
-                if description is not None:
-                    f["description"] = description
-                if not f["enabled"]:
-                    return self.disablefilter(newname)
-                return True
-        return False
+                filter_def = f
+                break
+        if not filter_def:
+            return False
+        if newname is None:
+            newname = oldname
+        newname = self._unicode_filter_name(newname)
+        if newname != oldname and self.filter_exists(newname):
+            raise FilterAlreadyExists
+        filter_def["name"] = newname
+        filter_def["content"] = sieve_filter
+        if description is not None:
+            filter_def["description"] = description
+        if not filter_def["enabled"]:
+            return self.disablefilter(newname)
+        return True
 
-    def getfilter(self, name):
+    def getfilter(self, name: str) -> Union[commands.Command, None]:
         """Search for a specific filter
 
         :param name: the filter's name
         :return: the Command object if found, None otherwise
         """
         name = self._unicode_filter_name(name)
         for f in self.filters:
             if f["name"] == name:
                 if not f["enabled"]:
                     return f["content"].children[0]
                 return f["content"]
         return None
 
-    def get_filter_matchtype(self, name):
+    def get_filter_matchtype(self, name: str) -> Union[str, None]:
         """Retrieve matchtype of the given filter."""
         flt = self.getfilter(name)
         if not flt:
             return None
         for node in flt.walk():
             if isinstance(node, (commands.AllofCommand, commands.AnyofCommand)):
                 return node.__class__.__name__.lower().replace("command", "")
         return None
 
-    def get_filter_conditions(self, name):
+    def get_filter_conditions(self, name: str) -> Union[List[str], None]:
         """Retrieve conditions of the given filter."""
         flt = self.getfilter(name)
         if not flt:
             return None
         conditions = []
         negate = False
         for node in flt.walk():
@@ -397,38 +461,38 @@
                         args = args[:3] + (":not{}".format(args[3][1:]),) + args[4:]
                     elif node.name == "exists":
                         args = ("not{}".format(args[0]),) + args[1:]
                     negate = False
                 conditions.append(args)
         return conditions
 
-    def get_filter_actions(self, name):
+    def get_filter_actions(self, name: str) -> Union[List[str], None]:
         """Retrieve actions of the given filter."""
         flt = self.getfilter(name)
         if not flt:
             return None
-        actions = []
+        actions: list = []
         for node in flt.walk():
             if isinstance(node, commands.ActionCommand):
                 actions.append(node.args_as_tuple())
         return actions
 
-    def removefilter(self, name):
+    def removefilter(self, name: str) -> bool:
         """Remove a specific filter
 
         :param name: the filter's name
         """
         name = self._unicode_filter_name(name)
         for f in self.filters:
             if f["name"] == name:
                 self.filters.remove(f)
                 return True
         return False
 
-    def enablefilter(self, name):
+    def enablefilter(self, name: str) -> bool:
         """Enable a filter
 
         Just removes the "if false" test surrouding this filter.
 
         :param name: the filter's name
         """
         name = self._unicode_filter_name(name)
@@ -438,26 +502,26 @@
             if not self.__isdisabled(f["content"]):
                 return False
             f["content"] = f["content"].children[0]
             f["enabled"] = True
             return True
         return False  # raise NotFound
 
-    def is_filter_disabled(self, name):
+    def is_filter_disabled(self, name: str) -> bool:
         """Tells if the filter is currently disabled or not
 
         :param name: the filter's name
         """
         name = self._unicode_filter_name(name)
         for f in self.filters:
             if f["name"] == name:
                 return self.__isdisabled(f["content"])
         return True
 
-    def disablefilter(self, name):
+    def disablefilter(self, name: str) -> bool:
         """Disable a filter
 
         Instead of commenting the filter, we just surround it with a
         "if false { }" test.
 
         :param name: the filter's name
         :return: True if filter was disabled, False otherwise
@@ -471,15 +535,15 @@
                 continue
             ifcontrol.addchild(f["content"])
             f["content"] = ifcontrol
             f["enabled"] = False
             return True
         return False
 
-    def movefilter(self, name, direction):
+    def movefilter(self, name: str, direction: str) -> bool:
         """Moves the filter up or down
 
         :param name: the filter's name
         :param direction: string "up" or "down"
         """
         name = self._unicode_filter_name(name)
         cpt = 0
```

### Comparing `sievelib-1.3.0/sievelib/managesieve.py` & `sievelib-1.4.0/sievelib/managesieve.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Implementation based on RFC 5804.
 """
 
 import base64
 import re
 import socket
 import ssl
+from typing import Any, List, Optional, Tuple
 
 from .digest_md5 import DigestMD5
 from . import tools
 
 
 CRLF = b"\r\n"
 
@@ -33,15 +34,15 @@
 
 
 class Error(Exception):
     pass
 
 
 class Response(Exception):
-    def __init__(self, code, data):
+    def __init__(self, code: bytes, data: bytes):
         self.code = code
         self.data = data
 
     def __str__(self):
         return "%s %s" % (self.code, self.data)
 
 
@@ -65,28 +66,29 @@
         if cls.authenticated:
             return meth(cls, *args, **kwargs)
         raise Error("Authentication required")
 
     return check
 
 
-class Client(object):
+class Client:
     read_size = 4096
     read_timeout = 5
 
-    def __init__(self, srvaddr, srvport=4190, debug=False):
+    def __init__(self, srvaddr: str, srvport: int = 4190, debug: bool = False):
         self.srvaddr = srvaddr
         self.srvport = srvport
         self.__debug = debug
-        self.sock = None
-        self.__read_buffer = b""
-        self.authenticated = False
-        self.errcode = None
+        self.sock: socket.socket = None
+        self.__read_buffer: bytes = b""
+        self.authenticated: bool = False
+        self.errcode: bytes = None
+        self.errmsg: bytes = b""
 
-        self.__capabilities = {}
+        self.__capabilities: dict[str, str] = {}
         self.__respcode_expr = re.compile(rb"(OK|NO|BYE)\s*(.+)?")
         self.__error_expr = re.compile(rb'(\([\w/-]+\))?\s*(".+")')
         self.__size_expr = re.compile(rb"\{(\d+)\+?\}")
         self.__active_expr = re.compile(rb"ACTIVE", re.IGNORECASE)
 
     def __del__(self):
         if self.sock is not None:
@@ -94,15 +96,15 @@
             self.sock = None
 
     def __dprint(self, message):
         if not self.__debug:
             return
         print("DEBUG: %s" % message)
 
-    def __read_block(self, size):
+    def __read_block(self, size: int) -> bytes:
         """Read a block of 'size' bytes from the server.
 
         An internal buffer is used to read data from the server. If
         enough data is available from it, we return that data.
 
         Eventually, we try to grab the missing part from the server
         for Client.read_timeout seconds. If no data can be
@@ -124,15 +126,15 @@
         try:
             buf += self.sock.recv(size)
         except (socket.timeout, ssl.SSLError):
             raise Error("Failed to read %d bytes from the server" % size)
         self.__dprint(buf)
         return buf
 
-    def __read_line(self):
+    def __read_line(self) -> bytes:
         """Read one line from the server.
 
         An internal buffer is used to read data from the server
         (blocks of Client.read_size bytes). If the buffer
         is not empty, we try to find an entire line to return.
 
         If we failed, we try to read new content from the server for
@@ -171,15 +173,15 @@
                 if m.group(1) == b"BYE":
                     raise Error("Connection closed by server")
                 if m.group(1) == b"NO":
                     self.__parse_error(m.group(2))
                 raise Response(m.group(1), m.group(2))
         return ret
 
-    def __read_response(self, nblines=-1):
+    def __read_response(self, nblines: int = -1) -> Tuple[bytes, bytes, bytes]:
         """Read a response from the server.
 
         In the usual case, we read lines until we find one that looks
         like a response (OK|NO|BYE\s*(.+)?).
 
         If *nblines* > 0, we read excactly nblines before returning.
 
@@ -207,15 +209,15 @@
             resp += line + CRLF
             cpt += 1
             if nblines != -1 and cpt == nblines:
                 break
 
         return (code, data, resp)
 
-    def __prepare_args(self, args):
+    def __prepare_args(self, args: List[Any]) -> List[bytes]:
         """Format command arguments before sending them.
 
         Command arguments of type string must be quoted, the only
         exception concerns size indication (of the form {\d\+?}).
 
         :param args: list of arguments
         :return: a list for transformed arguments
@@ -227,30 +229,34 @@
                     ret += [a]
                 else:
                     ret += [b'"' + a + b'"']
                 continue
             ret += [bytes(str(a).encode("utf-8"))]
         return ret
 
-    def __prepare_content(self, content):
+    def __prepare_content(self, content: str) -> bytes:
         """Format script content before sending it.
 
         Script length must be inserted before the content,
         enclosed in curly braces, separated by CRLF.
 
         :param content: script content as str or bytes
         :return: transformed script as bytes
         """
-        if isinstance(content, str):
-            content = content.encode("utf-8")
-        return b"{%d+}%s%s" % (len(content), CRLF, content)
+        bcontent: bytes = content.encode("utf-8")
+        return b"{%d+}%s%s" % (len(bcontent), CRLF, bcontent)
 
     def __send_command(
-        self, name, args=None, withcontent=False, extralines=None, nblines=-1
-    ):
+        self,
+        name: str,
+        args: Optional[List[bytes]] = None,
+        withcontent: bool = False,
+        extralines: Optional[List[bytes]] = None,
+        nblines: int = -1,
+    ) -> Tuple[str, str, bytes]:
         """Send a command to the server.
 
         If args is not empty, we concatenate the given command with
         the content of this list. If extralines is not empty, they are
         sent one by one to the server. (CLRF are automatically
         appended to them)
 
@@ -281,30 +287,30 @@
         if isinstance(data, bytes):
             data = data.decode("utf-8")
 
         if withcontent:
             return (code, data, content)
         return (code, data)
 
-    def __get_capabilities(self):
+    def __get_capabilities(self) -> bool:
         code, data, capabilities = self.__read_response()
         if code == "NO":
             return False
 
         for l in capabilities.splitlines():
             parts = l.split(None, 1)
             cname = parts[0].strip(b'"').decode("utf-8")
             if cname not in KNOWN_CAPABILITIES:
                 continue
             self.__capabilities[cname] = (
                 parts[1].strip(b'"').decode("utf-8") if len(parts) > 1 else None
             )
         return True
 
-    def __parse_error(self, text):
+    def __parse_error(self, text: bytes):
         """Parse an error received from the server.
 
         if text corresponds to a size indication, we grab the
         remaining content from the server.
 
         Otherwise, we try to match an error of the form \(\w+\)?\s*".+"
 
@@ -324,50 +330,52 @@
             raise Error("Bad error message")
         if m.group(1) is not None:
             self.errcode = m.group(1).strip(b"()")
         else:
             self.errcode = b""
         self.errmsg = m.group(2).strip(b'"')
 
-    def _plain_authentication(self, login, password, authz_id=b""):
+    def _plain_authentication(
+        self, login: bytes, password: bytes, authz_id: bytes = b""
+    ) -> bool:
         """SASL PLAIN authentication
 
         :param login: username
         :param password: clear password
         :return: True on success, False otherwise.
         """
-        if isinstance(login, str):
-            login = login.encode("utf-8")
-        if isinstance(password, str):
-            password = password.encode("utf-8")
         params = base64.b64encode(b"\0".join([authz_id, login, password]))
         code, data = self.__send_command("AUTHENTICATE", [b"PLAIN", params])
         if code == "OK":
             return True
         return False
 
-    def _login_authentication(self, login, password, authz_id=""):
+    def _login_authentication(
+        self, login: bytes, password: bytes, authz_id: bytes = ""
+    ) -> bool:
         """SASL LOGIN authentication
 
         :param login: username
         :param password: clear password
         :return: True on success, False otherwise.
         """
         extralines = [
-            b'"%s"' % base64.b64encode(login.encode("utf-8")),
-            b'"%s"' % base64.b64encode(password.encode("utf-8")),
+            b'"%s"' % base64.b64encode(login),
+            b'"%s"' % base64.b64encode(password),
         ]
         code, data = self.__send_command(
             "AUTHENTICATE", [b"LOGIN"], extralines=extralines
         )
         if code == "OK":
             return True
         return False
 
-    def _digest_md5_authentication(self, login, password, authz_id=""):
+    def _digest_md5_authentication(
+        self, login: bytes, password: bytes, authz_id: bytes = b""
+    ) -> bool:
         """SASL DIGEST-MD5 authentication
 
         :param login: username
         :param password: clear password
         :return: True on success, False otherwise.
         """
         code, data, challenge = self.__send_command(
@@ -386,15 +394,17 @@
             self.errmsg = "Bad challenge received from server"
             return False
         code, data = self.__send_command('""')
         if code == "OK":
             return True
         return False
 
-    def _oauthbearer_authentication(self, login, password, authz_id=""):
+    def _oauthbearer_authentication(
+        self, login: bytes, password: bytes, authz_id: bytes = b""
+    ) -> bool:
         """
         OAUTHBEARER authentication.
 
         :param login: username
         :param password: clear password
         :return: True on success, False otherwise.
         """
@@ -405,15 +415,21 @@
         token = b"n,a=" + login + b",\001auth=Bearer " + password + b"\001\001"
         token = base64.b64encode(token)
         code, data = self.__send_command("AUTHENTICATE", [b"OAUTHBEARER", token])
         if code == "OK":
             return True
         return False
 
-    def __authenticate(self, login, password, authz_id=b"", authmech=None):
+    def __authenticate(
+        self,
+        login: str,
+        password: str,
+        authz_id: str = "",
+        authmech: Optional[str] = None,
+    ) -> bool:
         """AUTHENTICATE command
 
         Actually, it is just a wrapper to the real commands (one by
         mechanism). We try all supported mechanisms (from the
         strongest to the weakest) until we find one supported by the
         server.
 
@@ -435,23 +451,27 @@
             mech_list = [authmech]
 
         for mech in mech_list:
             if mech not in srv_mechanisms:
                 continue
             mech = mech.lower().replace("-", "_")
             auth_method = getattr(self, "_%s_authentication" % mech)
-            if auth_method(login, password, authz_id):
+            if auth_method(
+                login.encode("utf-8"),
+                password.encode("utf-8"),
+                authz_id.encode("utf-8"),
+            ):
                 self.authenticated = True
                 return True
             return False
 
         self.errmsg = b"No suitable mechanism found"
         return False
 
-    def __starttls(self, keyfile=None, certfile=None):
+    def __starttls(self, keyfile=None, certfile=None) -> bool:
         """STARTTLS command
 
         See MANAGESIEVE specifications, section 2.2.
 
         :param keyfile: an eventual private key to use
         :param certfile: an eventual certificate to use
         :rtype: boolean
@@ -468,35 +488,35 @@
         except ssl.SSLError as e:
             raise Error("SSL error: %s" % str(e))
         self.sock = nsock
         self.__capabilities = {}
         self.__get_capabilities()
         return True
 
-    def get_implementation(self):
+    def get_implementation(self) -> str:
         """Returns the IMPLEMENTATION value.
 
         It is read from server capabilities. (see the CAPABILITY
         command)
 
         :rtype: string
         """
         return self.__capabilities["IMPLEMENTATION"]
 
-    def get_sasl_mechanisms(self):
+    def get_sasl_mechanisms(self) -> List[str]:
         """Returns the supported authentication mechanisms.
 
         They're read from server capabilities. (see the CAPABILITY
         command)
 
         :rtype: list of string
         """
         return self.__capabilities["SASL"].split()
 
-    def has_tls_support(self):
+    def has_tls_support(self) -> bool:
         """Tells if the server has STARTTLS support or not.
 
         It is read from server capabilities. (see the CAPABILITY
         command)
 
         :rtype: boolean
         """
@@ -510,15 +530,22 @@
 
         :rtype: string
         """
         if isinstance(self.__capabilities["SIEVE"], str):
             self.__capabilities["SIEVE"] = self.__capabilities["SIEVE"].split()
         return self.__capabilities["SIEVE"]
 
-    def connect(self, login, password, authz_id=b"", starttls=False, authmech=None):
+    def connect(
+        self,
+        login: str,
+        password: str,
+        authz_id: str = "",
+        starttls: bool = False,
+        authmech: Optional[str] = None,
+    ):
         """Establish a connection with the server.
 
         This function must be used. It read the server capabilities
         and wraps calls to STARTTLS and AUTHENTICATE commands.
 
         :param login: username
         :param password: clear password
@@ -574,26 +601,26 @@
             "HAVESPACE", [scriptname.encode("utf-8"), scriptsize]
         )
         if code == "OK":
             return True
         return False
 
     @authentication_required
-    def listscripts(self):
+    def listscripts(self) -> Tuple[str, List[str]]:
         """List available scripts.
 
         See MANAGESIEVE specifications, section 2.7
 
         :returns: a 2-uple (active script, [script1, ...])
         """
         code, data, listing = self.__send_command("LISTSCRIPTS", withcontent=True)
         if code == "NO":
             return None
-        ret = []
-        active_script = None
+        ret: List[str] = []
+        active_script: str = None
         for l in listing.splitlines():
             if self.__size_expr.match(l):
                 continue
             m = re.match(rb'"([^"]+)"\s*(.+)', l)
             if m is None:
                 ret += [l.strip(b'"').decode("utf-8")]
                 continue
@@ -632,16 +659,16 @@
 
         See MANAGESIEVE specifications, section 2.6
 
         :param name: script's name
         :param content: script's content
         :rtype: boolean
         """
-        content = self.__prepare_content(content)
-        code, data = self.__send_command("PUTSCRIPT", [name.encode("utf-8"), content])
+        bcontent = self.__prepare_content(content)
+        code, data = self.__send_command("PUTSCRIPT", [name.encode("utf-8"), bcontent])
         if code == "OK":
             return True
         return False
 
     @authentication_required
     def deletescript(self, name: str) -> bool:
         """Delete a script from the server
@@ -723,12 +750,12 @@
         See MANAGESIEVE specifications, section 2.12
 
         :param name: script's content
         :rtype: boolean
         """
         if "VERSION" not in self.__capabilities:
             raise NotImplementedError("server does not support CHECKSCRIPT command")
-        content = self.__prepare_content(content)
-        code, data = self.__send_command("CHECKSCRIPT", [content])
+        bcontent = self.__prepare_content(content)
+        code, data = self.__send_command("CHECKSCRIPT", [bcontent])
         if code == "OK":
             return True
         return False
```

### Comparing `sievelib-1.3.0/sievelib/parser.py` & `sievelib-1.4.0/sievelib/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 language used to filter emails.
 
 This implementation is based on RFC 5228 (http://tools.ietf.org/html/rfc5228)
 
 """
 import re
 import sys
+from typing import Iterator, Tuple
 
 from sievelib.commands import get_command_instance, CommandError, RequireCommand
 
 
 class ParseError(Exception):
     """Generic parsing error"""
 
-    def __init__(self, msg):
+    def __init__(self, msg: str):
         self.msg = msg
 
     def __str__(self):
-        return "parsing error: %s" % self.msg
+        return f"parsing error: {self.msg}"
 
 
 class Lexer:
     """
     The lexical analysis part.
 
     This class provides a simple way to define tokens (with patterns)
@@ -42,23 +43,23 @@
         for name, part in definitions:
             param = b"(?P<%s>%s)" % (name, part)
             parts.append(param)
         self.regexpString = b"|".join(parts)
         self.regexp = re.compile(self.regexpString, re.MULTILINE)
         self.wsregexp = re.compile(rb"\s+", re.M)
 
-    def curlineno(self):
+    def curlineno(self) -> int:
         """Return the current line number"""
         return self.text[: self.pos].count(b"\n") + 1
 
-    def curcolno(self):
+    def curcolno(self) -> int:
         """Return the current column number"""
         return self.pos - self.text.rfind(b"\n", 0, self.pos)
 
-    def scan(self, text):
+    def scan(self, text: bytes) -> Iterator[Tuple[str, bytes]]:
         """Analyse some data
 
         Analyse the passed content. Each time a token is recognized, a
         2-uple containing its name and parsed value is raised (via
         yield).
 
         On error, a ParseError exception is raised.
@@ -75,15 +76,15 @@
 
             m = self.regexp.match(text, self.pos)
             if m is None:
                 token = text[self.pos :]
                 m = self.wsregexp.search(token)
                 if m is not None:
                     token = token[: m.start()]
-                raise ParseError("unknown token %s" % token)
+                raise ParseError(f"unknown token {token}")
 
             yield (m.lastgroup, m.group(m.lastgroup))
             self.pos += len(m.group(0))
 
 
 class Parser:
     """The grammatical analysis part.
@@ -106,15 +107,15 @@
         (b"multiline", rb"text:[^$]*?[\r\n]+\.$"),
         (b"string", rb'"([^"\\]|\\.)*"'),
         (b"identifier", rb"[a-zA-Z_][\w]*"),
         (b"tag", rb":[a-zA-Z_][\w]*"),
         (b"number", rb"[0-9]+[KMGkmg]?"),
     ]
 
-    def __init__(self, debug=False):
+    def __init__(self, debug: bool = False):
         self.debug = debug
         self.lexer = Lexer(Parser.lrules)
 
     def __dprint(self, *msgs):
         if not self.debug:
             return
         for m in msgs:
@@ -140,37 +141,37 @@
         """Set the next expected token.
 
         One or more tokens can be provided. (they will represent the
         valid possibilities for the next token).
         """
         self.__expected = args
 
-    def __push_expected_bracket(self, ttype, tvalue):
+    def __push_expected_bracket(self, ttype: str, tvalue: bytes):
         """Append a new expected bracket.
 
         Next time a bracket is closed, it must match the one provided here.
         """
         self.__expected_brackets.append((ttype, tvalue))
 
-    def __pop_expected_bracket(self, ttype, tvalue):
+    def __pop_expected_bracket(self, ttype: str, tvalue):
         """Drop the last expected bracket.
 
         If the given bracket doesn't match the dropped expected bracket,
         or if no bracket is expected at all, a ParseError will be raised.
         """
         try:
             etype, evalue = self.__expected_brackets.pop()
         except IndexError:
             raise ParseError("unexpected closing bracket %s (none opened)" % (tvalue,))
         if ttype != etype:
             raise ParseError(
                 "unexpected closing bracket %s (expected %s)" % (tvalue, evalue)
             )
 
-    def __up(self, onlyrecord=False):
+    def __up(self, onlyrecord: bool = False):
         """Return to the current command's parent
 
         This method should be called each time a command is
         complete. In case of a top level command (no parent), it is
         recorded into a specific list for further usage.
 
         :param onlyrecord: tell to only record the new command into its parent.
@@ -221,15 +222,15 @@
                 self.__curcommand.get_type() == "test"
                 and self.__curcommand.variable_args_nb
             )
             if condition:
                 self.__set_expected("comma", "right_parenthesis")
             break
 
-    def __check_command_completion(self, testsemicolon=True):
+    def __check_command_completion(self, testsemicolon: bool = True) -> bool:
         """Check for command(s) completion
 
         This function should be called each time a new argument is
         seen by the parser in order to check a command is complete. As
         not only one command can be ended when receiving a new
         argument (nested commands case), we apply the same work to
         parent commands.
@@ -264,15 +265,15 @@
                     return False
                 if not self.__curcommand.iscomplete():
                     if self.__curcommand.variable_args_nb:
                         self.__set_expected("comma", "right_parenthesis")
                     break
         return True
 
-    def __stringlist(self, ttype, tvalue):
+    def __stringlist(self, ttype: str, tvalue: bytes) -> bool:
         """Specific method to parse the 'string-list' type
 
         Syntax:
             string-list = "[" string *("," string) "]" / string
                             ; if there is only a single string, the brackets
                             ; are optional
         """
@@ -286,15 +287,15 @@
         if ttype == "right_bracket":
             self.__pop_expected_bracket(ttype, tvalue)
             self.__curcommand.check_next_arg("stringlist", self.__curstringlist)
             self.__cstate = self.__arguments
             return self.__check_command_completion()
         return False
 
-    def __argument(self, ttype, tvalue):
+    def __argument(self, ttype: str, tvalue: bytes) -> bool:
         """Argument parsing method
 
         This method acts as an entry point for 'argument' parsing.
 
         Syntax:
             string-list / number / tag
 
@@ -323,15 +324,15 @@
             self.__curcommand.reassign_arguments()
             # rewind lexer
             self.lexer.pos -= 1
             return True
 
         return False
 
-    def __arguments(self, ttype, tvalue):
+    def __arguments(self, ttype: str, tvalue: bytes) -> bool:
         """Arguments parsing method
 
         Entry point for command arguments parsing. The parser must
         call this method for each parsed command (either a control,
         action or test).
 
         Syntax:
@@ -367,15 +368,15 @@
             return True
 
         if self.__argument(ttype, tvalue):
             return self.__check_command_completion(testsemicolon=False)
 
         return False
 
-    def __command(self, ttype, tvalue):
+    def __command(self, ttype: str, tvalue: bytes) -> bool:
         """Command parsing method
 
         Entry point for command parsing. Here is expected behaviour:
          * Handle command beginning if detected,
          * Call the appropriate sub-method (specified by __cstate) to
            handle the body,
          * Handle command ending or block opening if detected.
@@ -428,15 +429,15 @@
             if not self.__check_command_completion(testsemicolon=False):
                 return False
             self.__curcommand.complete_cb()
             self.__up()
             return True
         return False
 
-    def parse(self, text):
+    def parse(self, text: bytes) -> bool:
         """The parser entry point.
 
         Parse the provided text to check for its validity.
 
         On success, the parsing tree is available into the result
         attribute. It is a list of sievecommands.Command objects (see
         the module documentation for specific information).
@@ -448,15 +449,16 @@
         :return: True on success (no error detected), False otherwise
         """
         if isinstance(text, str):
             text = text.encode("utf-8")
 
         self.__reset_parser()
         try:
-            tvalue = ""
+            ttype: str
+            tvalue: bytes = b""
             for ttype, tvalue in self.lexer.scan(text):
                 if ttype == "hash_comment":
                     self.hash_comments += [tvalue.strip()]
                     continue
                 if ttype == "bracket_comment":
                     continue
                 if self.__expected is not None:
@@ -495,15 +497,15 @@
                 self.lexer.curcolno(),
                 len(tvalue),
             )
             self.error = "line %d: %s" % (self.error_pos[0], str(e))
             return False
         return True
 
-    def parse_file(self, name):
+    def parse_file(self, name: str) -> bool:
         """Parse the content of a file.
 
         See 'parse' method for information.
 
         :param name: the pathname of the file to parse
         :return: True on success (no error detected), False otherwise
         """
```

### Comparing `sievelib-1.3.0/sievelib/tests/test_factory.py` & `sievelib-1.4.0/sievelib/tests/test_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,132 @@
 import unittest
 import io
 
-from sievelib.factory import FiltersSet
+from sievelib.factory import FilterAlreadyExists, FiltersSet
 from .. import parser
 
 
 class FactoryTestCase(unittest.TestCase):
 
     def setUp(self):
         self.fs = FiltersSet("test")
 
+    def test_add_duplicate_filter(self):
+        """Try to add the same filter name twice, should fail."""
+        self.fs.addfilter(
+            "ruleX",
+            [
+                ("Sender", ":is", "toto@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Toto"),
+            ],
+        )
+        with self.assertRaises(FilterAlreadyExists):
+            self.fs.addfilter(
+                "ruleX",
+                [
+                    ("Sender", ":is", "toto@toto.com"),
+                ],
+                [
+                    ("fileinto", ":copy", "Toto"),
+                ],
+            )
+
+    def test_updatefilter(self):
+        self.fs.addfilter(
+            "ruleX",
+            [
+                ("Sender", ":is", "toto@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Toto"),
+            ],
+        )
+        result = self.fs.updatefilter(
+            "ruleY",
+            "ruleX",
+            [
+                ("Sender", ":is", "tata@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Tata"),
+            ],
+        )
+        self.assertFalse(result)
+        result = self.fs.updatefilter(
+            "ruleX",
+            "ruleY",
+            [
+                ("Sender", ":is", "tata@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Tata"),
+            ],
+        )
+        self.assertTrue(result)
+        self.assertIs(self.fs.getfilter("ruleX"), None)
+        self.assertIsNot(self.fs.getfilter("ruleY"), None)
+
+    def test_updatefilter_duplicate(self):
+        self.fs.addfilter(
+            "ruleX",
+            [
+                ("Sender", ":is", "toto@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Toto"),
+            ],
+        )
+        self.fs.addfilter(
+            "ruleY",
+            [
+                ("Sender", ":is", "toto@tota.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Tota"),
+            ],
+        )
+        with self.assertRaises(FilterAlreadyExists):
+            self.fs.updatefilter(
+                "ruleX",
+                "ruleY",
+                [
+                    ("Sender", ":is", "toto@toti.com"),
+                ],
+                [
+                    ("fileinto", ":copy", "Toti"),
+                ],
+            )
+
+    def test_replacefilter(self):
+        self.fs.addfilter(
+            "ruleX",
+            [
+                ("Sender", ":is", "toto@toto.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Toto"),
+            ],
+        )
+        self.fs.addfilter(
+            "ruleY",
+            [
+                ("Sender", ":is", "toto@tota.com"),
+            ],
+            [
+                ("fileinto", ":copy", "Tota"),
+            ],
+        )
+        content = self.fs.getfilter("ruleX")
+        result = self.fs.replacefilter("ruleZ", content)
+        self.assertFalse(result)
+        result = self.fs.replacefilter("ruleY", content)
+        self.assertTrue(result)
+
     def test_get_filter_conditions(self):
         """Test get_filter_conditions method."""
         orig_conditions = [("Sender", ":is", "toto@toto.com")]
         self.fs.addfilter(
             "ruleX",
             orig_conditions,
             [
```

### Comparing `sievelib-1.3.0/sievelib/tests/test_managesieve.py` & `sievelib-1.4.0/sievelib/tests/test_managesieve.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,27 @@
     def setUp(self):
         """Create client."""
         self.client = managesieve.Client("127.0.0.1")
 
     def authenticate(self, mock_socket):
         """Authenticate client."""
         mock_socket.return_value.recv.side_effect = (AUTHENTICATION,)
-        self.client.connect(b"user", b"password")
+        self.client.connect("user", "password")
 
     def test_connection(self, mock_socket):
         """Test connection."""
         self.authenticate(mock_socket)
         self.assertEqual(self.client.get_sieve_capabilities(), ["fileinto", "vacation"])
         mock_socket.return_value.recv.side_effect = (b"OK test\r\n",)
         self.client.logout()
 
     def test_auth_oauthbearer(self, mock_socket):
         """Test OAUTHBEARER mechanism."""
         mock_socket.return_value.recv.side_effect = (AUTHENTICATION,)
-        self.assertTrue(self.client.connect(b"user", b"token", authmech="OAUTHBEARER"))
+        self.assertTrue(self.client.connect("user", "token", authmech="OAUTHBEARER"))
 
     def test_capabilities(self, mock_socket):
         """Test capabilities command."""
         self.authenticate(mock_socket)
         mock_socket.return_value.recv.side_effect = (
             CAPABILITIES + b'OK "Capability completed."\r\n',
         )
@@ -141,15 +141,15 @@
 
     def test_renamescript_simulated(self, mock_socket):
         """Test renamescript command simulation."""
         mock_socket.return_value.recv.side_effect = (
             CAPABILITIES_WITHOUT_VERSION + b'OK "Dovecot ready."\r\n'
             b'OK "Logged in."\r\n',
         )
-        self.client.connect(b"user", b"password")
+        self.client.connect("user", "password")
         mock_socket.return_value.recv.side_effect = (
             LISTSCRIPTS,
             GETSCRIPT,
             b'OK "putscript completed."\r\n',
             b'OK "setactive completed."\r\n',
             b'OK "deletescript completed."\r\n',
         )
```

### Comparing `sievelib-1.3.0/sievelib/tests/test_parser.py` & `sievelib-1.4.0/sievelib/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sievelib-1.3.0/sievelib.egg-info/PKG-INFO` & `sievelib-1.4.0/sievelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sievelib
-Version: 1.3.0
+Version: 1.4.0
 Summary: Client-side SIEVE library
 Home-page: https://github.com/tonioo/sievelib
 Author: Antoine Nguyen
 Author-email: tonio@ngyn.org
 License: MIT
 Keywords: sieve,managesieve,parser,client
 Classifier: Programming Language :: Python
```

### Comparing `sievelib-1.3.0/sievelib.egg-info/SOURCES.txt` & `sievelib-1.4.0/sievelib.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 sievelib/factory.py
 sievelib/managesieve.py
 sievelib/parser.py
 sievelib/tools.py
 sievelib.egg-info/PKG-INFO
 sievelib.egg-info/SOURCES.txt
 sievelib.egg-info/dependency_links.txt
+sievelib.egg-info/requires.txt
 sievelib.egg-info/top_level.txt
 sievelib/tests/__init__.py
 sievelib/tests/test_factory.py
 sievelib/tests/test_managesieve.py
 sievelib/tests/test_parser.py
 sievelib/tests/files/utf8_sieve.txt
```

