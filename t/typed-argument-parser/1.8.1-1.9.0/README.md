# Comparing `tmp/typed-argument-parser-1.8.1.tar.gz` & `tmp/typed-argument-parser-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-argument-parser-1.8.1.tar", last modified: Wed Jun 28 23:03:03 2023, max compression
+gzip compressed data, was "typed-argument-parser-1.9.0.tar", last modified: Sun Nov 12 04:51:46 2023, max compression
```

## Comparing `typed-argument-parser-1.8.1.tar` & `typed-argument-parser-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-28 23:03:03.367768 typed-argument-parser-1.8.1/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1073 2022-01-01 02:49:05.000000 typed-argument-parser-1.8.1/LICENSE.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)    25066 2023-06-28 23:03:03.367975 typed-argument-parser-1.8.1/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)    24190 2023-06-28 21:49:42.000000 typed-argument-parser-1.8.1/README.md
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-28 23:03:03.368576 typed-argument-parser-1.8.1/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1538 2023-06-28 21:47:33.000000 typed-argument-parser-1.8.1/setup.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-28 23:03:03.355752 typed-argument-parser-1.8.1/tap/
--rw-r--r--   0 kyleswanson   (501) staff       (20)      227 2023-06-28 21:48:51.000000 typed-argument-parser-1.8.1/tap/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      150 2023-06-28 23:01:55.000000 typed-argument-parser-1.8.1/tap/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)       27 2019-12-27 22:52:32.000000 typed-argument-parser-1.8.1/tap/py.typed
--rw-r--r--   0 kyleswanson   (501) staff       (20)    32453 2023-06-28 22:38:16.000000 typed-argument-parser-1.8.1/tap/tap.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3762 2023-06-28 21:48:41.000000 typed-argument-parser-1.8.1/tap/tapify.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)    18979 2023-06-28 21:45:52.000000 typed-argument-parser-1.8.1/tap/utils.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-28 23:03:03.364939 typed-argument-parser-1.8.1/tests/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     7765 2023-06-28 21:47:33.000000 typed-argument-parser-1.8.1/tests/test_actions.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)    59962 2023-06-28 22:49:47.000000 typed-argument-parser-1.8.1/tests/test_integration.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4672 2023-03-03 00:33:35.000000 typed-argument-parser-1.8.1/tests/test_load_config_files.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     7005 2023-06-28 21:47:33.000000 typed-argument-parser-1.8.1/tests/test_subparser.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)    19595 2023-03-06 19:46:10.000000 typed-argument-parser-1.8.1/tests/test_tapify.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)    20469 2023-06-28 21:47:33.000000 typed-argument-parser-1.8.1/tests/test_utils.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-28 23:03:03.367481 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)    25066 2023-06-28 23:03:03.000000 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      492 2023-06-28 23:03:03.000000 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-28 23:03:03.000000 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       45 2023-06-28 23:03:03.000000 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        4 2023-06-28 23:03:03.000000 typed-argument-parser-1.8.1/typed_argument_parser.egg-info/top_level.txt
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-11-12 04:51:46.115640 typed-argument-parser-1.9.0/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1073 2022-01-01 02:49:05.000000 typed-argument-parser-1.9.0/LICENSE.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    25117 2023-11-12 04:51:46.116024 typed-argument-parser-1.9.0/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    24190 2023-06-28 21:49:42.000000 typed-argument-parser-1.9.0/README.md
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-11-12 04:51:46.117456 typed-argument-parser-1.9.0/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1538 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-11-12 04:51:46.103912 typed-argument-parser-1.9.0/tap/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      227 2023-11-12 04:22:07.000000 typed-argument-parser-1.9.0/tap/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      150 2023-11-12 04:28:38.000000 typed-argument-parser-1.9.0/tap/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       27 2019-12-27 22:52:32.000000 typed-argument-parser-1.9.0/tap/py.typed
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    32275 2023-11-12 04:22:46.000000 typed-argument-parser-1.9.0/tap/tap.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4302 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tap/tapify.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    18875 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tap/utils.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-11-12 04:51:46.111175 typed-argument-parser-1.9.0/tests/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7630 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_actions.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    62968 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_integration.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4671 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_load_config_files.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7008 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_subparser.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    21818 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_tapify.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    20182 2023-11-12 04:19:59.000000 typed-argument-parser-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-11-12 04:51:46.115134 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)    25117 2023-11-12 04:51:46.000000 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      492 2023-11-12 04:51:46.000000 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-11-12 04:51:46.000000 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       45 2023-11-12 04:51:46.000000 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        4 2023-11-12 04:51:46.000000 typed-argument-parser-1.9.0/typed_argument_parser.egg-info/top_level.txt
```

### Comparing `typed-argument-parser-1.8.1/LICENSE.txt` & `typed-argument-parser-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `typed-argument-parser-1.8.1/PKG-INFO` & `typed-argument-parser-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: typed-argument-parser
-Version: 1.8.1
+Version: 1.9.0
 Summary: Typed Argument Parser
 Home-page: https://github.com/swansonk14/typed-argument-parser
-Download-URL: https://github.com/swansonk14/typed-argument-parser/archive/refs/tags/v_1.8.1.tar.gz
+Download-URL: https://github.com/swansonk14/typed-argument-parser/archive/refs/tags/v_1.9.0.tar.gz
 Author: Jesse Michel and Kyle Swanson
 Author-email: jessem.michel@gmail.com, swansonk.14@gmail.com
 License: MIT
 Keywords: typing,argument parser,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `typed-argument-parser-1.8.1/README.md` & `typed-argument-parser-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `typed-argument-parser-1.8.1/tap/tap.py` & `typed-argument-parser-1.9.0/tap/tap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import sys
 import time
 from argparse import ArgumentParser, ArgumentTypeError
-from collections import OrderedDict
 from copy import deepcopy
 from functools import partial
 from pathlib import Path
 from pprint import pformat
 from shlex import quote, split
 from types import MethodType
 from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Tuple, TypeVar, Union, get_type_hints
@@ -25,41 +24,43 @@
     get_literals,
     boolean_type,
     TupleTypeEnforcer,
     define_python_object_encoder,
     as_python_object,
     fix_py36_copy,
     enforce_reproducibility,
-    PathLike
+    PathLike,
 )
 
 if sys.version_info >= (3, 10):
     from types import UnionType
 
 
 # Constants
 EMPTY_TYPE = get_args(List)[0] if len(get_args(List)) > 0 else tuple()
 BOXED_COLLECTION_TYPES = {List, list, Set, set, Tuple, tuple}
 UNION_TYPES = {Union} | ({UnionType} if sys.version_info >= (3, 10) else set())
 OPTIONAL_TYPES = {Optional} | UNION_TYPES
 BOXED_TYPES = BOXED_COLLECTION_TYPES | OPTIONAL_TYPES
 
 
-TapType = TypeVar('TapType', bound='Tap')
+TapType = TypeVar("TapType", bound="Tap")
 
 
 class Tap(ArgumentParser):
     """Tap is a typed argument parser that wraps Python's built-in ArgumentParser."""
 
-    def __init__(self,
-                 *args,
-                 underscores_to_dashes: bool = False,
-                 explicit_bool: bool = False,
-                 config_files: Optional[List[PathLike]] = None,
-                 **kwargs):
+    def __init__(
+        self,
+        *args,
+        underscores_to_dashes: bool = False,
+        explicit_bool: bool = False,
+        config_files: Optional[List[PathLike]] = None,
+        **kwargs,
+    ):
         """Initializes the Tap instance.
 
         :param args: Arguments passed to the super class ArgumentParser.
         :param underscores_to_dashes: If True, convert underscores in flags to dashes.
         :param explicit_bool: Booleans can be specified on the command line as "--arg True" or "--arg False"
                               rather than "--arg". Additionally, booleans can be specified by prefixes of True and False
                               with any capitalization as well as 1 or 0.
@@ -81,27 +82,27 @@
         # Whether the arguments have been parsed (i.e. if parse_args has been called)
         self._parsed = False
 
         # Set extra arguments to empty list
         self.extra_args = []
 
         # Create argument buffer
-        self.argument_buffer = OrderedDict()
+        self.argument_buffer = {}
 
         # Create a place to put all of the subparsers
         self._subparser_buffer: List[Tuple[str, type, Dict[str, Any]]] = []
 
         # Get class variables help strings from the comments
         self.class_variables = self._get_class_variables()
 
         # Get annotations from self and all super classes up through tap
         self._annotations = self._get_annotations()
 
         # Set the default description to be the docstring
-        kwargs.setdefault('description', self.__doc__)
+        kwargs.setdefault("description", self.__doc__)
 
         # Initialize the super class, i.e. ArgumentParser
         super(Tap, self).__init__(*args, **kwargs)
 
         # Stores all of the subparsers
         self._subparsers = None
 
@@ -132,124 +133,131 @@
         # Set explicit bool
         explicit_bool = self._explicit_bool
 
         # Get variable name
         variable = get_argument_name(*name_or_flags)
 
         if self._underscores_to_dashes:
-            variable = variable.replace('-', '_')
+            variable = variable.replace("-", "_")
 
         # Get default if not specified
         if hasattr(self, variable):
-            kwargs['default'] = kwargs.get('default', getattr(self, variable))
+            kwargs["default"] = kwargs.get("default", getattr(self, variable))
 
         # Set required if option arg
         if (
             is_option_arg(*name_or_flags)
-            and variable != 'help'
-            and 'default' not in kwargs
-            and kwargs.get('action') != 'version'
+            and variable != "help"
+            and "default" not in kwargs
+            and kwargs.get("action") != "version"
         ):
-            kwargs['required'] = kwargs.get('required', not hasattr(self, variable))
+            kwargs["required"] = kwargs.get("required", not hasattr(self, variable))
 
         # Set help if necessary
-        if 'help' not in kwargs:
-            kwargs['help'] = '('
+        if "help" not in kwargs:
+            kwargs["help"] = "("
 
             # Type
             if variable in self._annotations:
-                kwargs['help'] += type_to_str(self._annotations[variable]) + ', '
+                kwargs["help"] += type_to_str(self._annotations[variable]) + ", "
 
             # Required/default
-            if kwargs.get('required', False) or is_positional_arg(*name_or_flags):
-                kwargs['help'] += 'required'
+            if kwargs.get("required", False) or is_positional_arg(*name_or_flags):
+                kwargs["help"] += "required"
             else:
-                kwargs['help'] += f'default={kwargs.get("default", None)}'
+                kwargs["help"] += f'default={kwargs.get("default", None)}'
 
-            kwargs['help'] += ')'
+            kwargs["help"] += ")"
 
             # Description
             if variable in self.class_variables:
-                kwargs['help'] += ' ' + self.class_variables[variable]['comment']
+                kwargs["help"] += " " + self.class_variables[variable]["comment"]
 
         # Set other kwargs where not provided
         if variable in self._annotations:
             # Get type annotation
             var_type = self._annotations[variable]
 
             # If type is not explicitly provided, set it if it's one of our supported default types
-            if 'type' not in kwargs:
+            if "type" not in kwargs:
                 # Unbox Union[type] (Optional[type]) and set var_type = type
                 if get_origin(var_type) in OPTIONAL_TYPES:
                     var_args = get_args(var_type)
 
                     # If type is Union or Optional without inner types, set type to equivalent of Optional[str]
                     if len(var_args) == 0:
                         var_args = (str, type(None))
 
                     # Raise error if type function is not explicitly provided for Union types (not including Optionals)
                     if get_origin(var_type) in UNION_TYPES and not (len(var_args) == 2 and var_args[1] == type(None)):
                         raise ArgumentTypeError(
-                            'For Union types, you must include an explicit type function in the configure method. '
-                            'For example,\n\n'
-                            'def to_number(string: str) -> Union[float, int]:\n'
-                            '    return float(string) if \'.\' in string else int(string)\n\n'
-                            'class Args(Tap):\n'
-                            '    arg: Union[float, int]\n'
-                            '\n'
-                            '    def configure(self) -> None:\n'
-                            '        self.add_argument(\'--arg\', type=to_number)'
+                            "For Union types, you must include an explicit type function in the configure method. "
+                            "For example,\n\n"
+                            "def to_number(string: str) -> Union[float, int]:\n"
+                            "    return float(string) if '.' in string else int(string)\n\n"
+                            "class Args(Tap):\n"
+                            "    arg: Union[float, int]\n"
+                            "\n"
+                            "    def configure(self) -> None:\n"
+                            "        self.add_argument('--arg', type=to_number)"
                         )
 
                     if len(var_args) > 0:
                         var_type = var_args[0]
 
                         # If var_type is tuple as in Python 3.6, change to a typing type
                         # (e.g., (typing.List, <class 'bool'>) ==> typing.List[bool])
                         if isinstance(var_type, tuple):
                             var_type = var_type[0][var_type[1:]]
 
                         explicit_bool = True
 
                 # First check whether it is a literal type or a boxed literal type
                 if is_literal_type(var_type):
-                    var_type, kwargs['choices'] = get_literals(var_type, variable)
+                    var_type, kwargs["choices"] = get_literals(var_type, variable)
 
-                elif (get_origin(var_type) in (List, list, Set, set)
-                      and len(get_args(var_type)) > 0
-                      and is_literal_type(get_args(var_type)[0])):
-                    var_type, kwargs['choices'] = get_literals(get_args(var_type)[0], variable)
-                    if kwargs.get('action') not in {'append', 'append_const'}:
-                        kwargs['nargs'] = kwargs.get('nargs', '*')
+                elif (
+                    get_origin(var_type) in (List, list, Set, set)
+                    and len(get_args(var_type)) > 0
+                    and is_literal_type(get_args(var_type)[0])
+                ):
+                    var_type, kwargs["choices"] = get_literals(get_args(var_type)[0], variable)
+                    if kwargs.get("action") not in {"append", "append_const"}:
+                        kwargs["nargs"] = kwargs.get("nargs", "*")
 
                 # Handle Tuple type (with type args) by extracting types of Tuple elements and enforcing them
                 elif get_origin(var_type) in (Tuple, tuple) and len(get_args(var_type)) > 0:
                     loop = False
                     types = get_args(var_type)
 
                     # Handle Tuple[type, ...]
                     if len(types) == 2 and types[1] == Ellipsis:
                         types = types[0:1]
                         loop = True
-                        kwargs['nargs'] = '*'
+                        kwargs["nargs"] = "*"
                     # Handle Tuple[()]
                     elif len(types) == 1 and types[0] == tuple():
                         types = [str]
                         loop = True
-                        kwargs['nargs'] = '*'
+                        kwargs["nargs"] = "*"
                     else:
-                        kwargs['nargs'] = len(types)
+                        kwargs["nargs"] = len(types)
+
+                    # Handle Literal types
+                    types = [get_literals(tp, variable)[0] if is_literal_type(tp) else tp for tp in types]
 
                     var_type = TupleTypeEnforcer(types=types, loop=loop)
 
                 if get_origin(var_type) in BOXED_TYPES:
                     # If List or Set or Tuple type, set nargs
-                    if (get_origin(var_type) in BOXED_COLLECTION_TYPES
-                            and kwargs.get('action') not in {'append', 'append_const'}):
-                        kwargs['nargs'] = kwargs.get('nargs', '*')
+                    if get_origin(var_type) in BOXED_COLLECTION_TYPES and kwargs.get("action") not in {
+                        "append",
+                        "append_const",
+                    }:
+                        kwargs["nargs"] = kwargs.get("nargs", "*")
 
                     # Extract boxed type for Optional, List, Set
                     arg_types = get_args(var_type)
 
                     # Set defaults type to str for Type and Type[()]
                     if len(arg_types) == 0 or arg_types[0] == EMPTY_TYPE:
                         var_type = str
@@ -259,67 +267,71 @@
                     # Handle the cases of List[bool], Set[bool], Tuple[bool]
                     if var_type == bool:
                         var_type = boolean_type
 
                 # If bool then set action, otherwise set type
                 if var_type == bool:
                     if explicit_bool:
-                        kwargs['type'] = boolean_type
-                        kwargs['choices'] = [True, False]  # this makes the help message more helpful
+                        kwargs["type"] = boolean_type
+                        kwargs["choices"] = [True, False]  # this makes the help message more helpful
                     else:
-                        action_cond = 'true' if kwargs.get('required', False) or not kwargs['default'] else 'false'
-                        kwargs['action'] = kwargs.get('action', f'store_{action_cond}')
-                elif kwargs.get('action') not in {'count', 'append_const'}:
-                    kwargs['type'] = var_type
+                        action_cond = "true" if kwargs.get("required", False) or not kwargs["default"] else "false"
+                        kwargs["action"] = kwargs.get("action", f"store_{action_cond}")
+                elif kwargs.get("action") not in {"count", "append_const"}:
+                    kwargs["type"] = var_type
 
         if self._underscores_to_dashes:
             # Replace "_" with "-" for arguments that aren't positional
-            name_or_flags = tuple(name_or_flag.replace('_', '-') if name_or_flag.startswith('-') else name_or_flag
-                                  for name_or_flag in name_or_flags)
+            name_or_flags = tuple(
+                name_or_flag.replace("_", "-") if name_or_flag.startswith("-") else name_or_flag
+                for name_or_flag in name_or_flags
+            )
 
         # Deepcopy default to prevent mutation of values
-        if 'default' in kwargs:
-            kwargs['default'] = deepcopy(kwargs['default'])
+        if "default" in kwargs:
+            kwargs["default"] = deepcopy(kwargs["default"])
 
         super(Tap, self).add_argument(*name_or_flags, **kwargs)
 
     def add_argument(self, *name_or_flags, **kwargs) -> None:
         """Adds an argument to the argument buffer, which will later be passed to _add_argument."""
         if self._initialized:
-            raise ValueError('add_argument cannot be called after initialization. '
-                             'Arguments must be added either as class variables or by overriding '
-                             'configure and including a self.add_argument call there.')
+            raise ValueError(
+                "add_argument cannot be called after initialization. "
+                "Arguments must be added either as class variables or by overriding "
+                "configure and including a self.add_argument call there."
+            )
 
-        variable = get_argument_name(*name_or_flags).replace('-', '_')
+        variable = get_argument_name(*name_or_flags).replace("-", "_")
         self.argument_buffer[variable] = (name_or_flags, kwargs)
 
     def _add_arguments(self) -> None:
         """Add arguments to self in the order they are defined as class variables (so the help string is in order)."""
         # Add class variables (in order)
         for variable in self.class_variables:
             if variable in self.argument_buffer:
                 name_or_flags, kwargs = self.argument_buffer[variable]
                 self._add_argument(*name_or_flags, **kwargs)
             else:
-                self._add_argument(f'--{variable}')
+                self._add_argument(f"--{variable}")
 
         # Add any arguments that were added manually in configure but aren't class variables (in order)
         for variable, (name_or_flags, kwargs) in self.argument_buffer.items():
             if variable not in self.class_variables:
                 self._add_argument(*name_or_flags, **kwargs)
 
     def process_args(self) -> None:
         """Perform additional argument processing and/or validation."""
         pass
 
     def add_subparser(self, flag: str, subparser_type: type, **kwargs) -> None:
         """Add a subparser to the collection of subparsers"""
-        help_desc = kwargs.get('help', subparser_type.__doc__)
-        kwargs['help'] = help_desc
-        
+        help_desc = kwargs.get("help", subparser_type.__doc__)
+        kwargs["help"] = help_desc
+
         self._subparser_buffer.append((flag, subparser_type, kwargs))
 
     def _add_subparsers(self) -> None:
         """Add each of the subparsers to the Tap object. """
         # Initialize the _subparsers object if not already created
         if self._subparsers is None and len(self._subparser_buffer) > 0:
             self._subparsers = super(Tap, self).add_subparsers()
@@ -376,54 +388,53 @@
         :return: A dictionary of reproducibility information.
         """
         # Get the path to the Python file that is being run
         if repo_path is None:
             repo_path = (Path.cwd() / Path(sys.argv[0]).parent).resolve()
 
         reproducibility = {
-            'command_line': f'python {" ".join(quote(arg) for arg in sys.argv)}',
-            'time': time.strftime('%c')
+            "command_line": f'python {" ".join(quote(arg) for arg in sys.argv)}',
+            "time": time.strftime("%c"),
         }
 
         git_info = GitInfo(repo_path=repo_path)
 
         if git_info.has_git():
-            reproducibility['git_root'] = git_info.get_git_root()
-            reproducibility['git_url'] = git_info.get_git_url(commit_hash=True)
-            reproducibility['git_has_uncommitted_changes'] = git_info.has_uncommitted_changes()
+            reproducibility["git_root"] = git_info.get_git_root()
+            reproducibility["git_url"] = git_info.get_git_url(commit_hash=True)
+            reproducibility["git_has_uncommitted_changes"] = git_info.has_uncommitted_changes()
 
         return reproducibility
 
     def _log_all(self, repo_path: Optional[PathLike] = None) -> Dict[str, Any]:
         """Gets all arguments along with reproducibility information.
 
         :param repo_path: Path to the git repo to examine for reproducibility info.
                           If None, uses the git repo of the Python file that is run.
         :return: A dictionary containing all arguments along with reproducibility information.
         """
         arg_log = self.as_dict()
-        arg_log['reproducibility'] = self.get_reproducibility_info(repo_path=repo_path)
+        arg_log["reproducibility"] = self.get_reproducibility_info(repo_path=repo_path)
 
         return arg_log
 
-    def parse_args(self: TapType,
-                   args: Optional[Sequence[str]] = None,
-                   known_only: bool = False,
-                   legacy_config_parsing = False) -> TapType:
+    def parse_args(
+        self: TapType, args: Optional[Sequence[str]] = None, known_only: bool = False, legacy_config_parsing=False
+    ) -> TapType:
         """Parses arguments, sets attributes of self equal to the parsed arguments, and processes arguments.
 
         :param args: List of strings to parse. The default is taken from `sys.argv`.
         :param known_only: If true, ignores extra arguments and only parses known arguments.
                            Unparsed arguments are saved to self.extra_args.
         :param legacy_config_parsing: If true, config files are parsed using `str.split` instead of `shlex.split`.
         :return: self, which is a Tap instance containing all of the parsed args.
         """
         # Prevent double parsing
         if self._parsed:
-            raise ValueError('parse_args can only be called once.')
+            raise ValueError("parse_args can only be called once.")
 
         # Collect arguments from all of the configs
 
         if legacy_config_parsing:
             splitter = lambda arg_string: arg_string.split()
         else:
             splitter = lambda arg_string: split(arg_string, comments=True)
@@ -468,33 +479,30 @@
 
         # Indicate that args have been parsed
         self._parsed = True
 
         return self
 
     @classmethod
-    def _get_from_self_and_super(cls,
-                                 extract_func: Callable[[type], dict],
-                                 dict_type: type = dict) -> Union[Dict[str, Any], OrderedDict]:
+    def _get_from_self_and_super(cls, extract_func: Callable[[type], dict]) -> Union[Dict[str, Any], Dict]:
         """Returns a dictionary mapping variable names to values.
 
         Variables and values are extracted from classes using key starting
         with this class and traversing up the super classes up through Tap.
 
-        If super class and sub class have the same key, the sub class value is used.
+        If super class and subclass have the same key, the subclass value is used.
 
         Super classes are traversed through breadth first search.
 
         :param extract_func: A function that extracts from a class a dictionary mapping variables to values.
-        :param dict_type: The type of dictionary to use (e.g. dict, OrderedDict, etc.)
         :return: A dictionary mapping variable names to values from the class dict.
         """
         visited = set()
         super_classes = [cls]
-        dictionary = dict_type()
+        dictionary = {}
 
         while len(super_classes) > 0:
             super_class = super_classes.pop(0)
 
             if super_class not in visited and issubclass(super_class, Tap):
                 super_dictionary = extract_func(super_class)
 
@@ -509,92 +517,90 @@
                 visited.add(super_class)
 
         return dictionary
 
     def _get_class_dict(self) -> Dict[str, Any]:
         """Returns a dictionary mapping class variable names to values from the class dict."""
         class_dict = self._get_from_self_and_super(
-            extract_func=lambda super_class: dict(getattr(super_class, '__dict__', dict()))
+            extract_func=lambda super_class: dict(getattr(super_class, "__dict__", dict()))
         )
         class_dict = {
             var: val
             for var, val in class_dict.items()
-            if not (var.startswith('_')
-                    or callable(val)
-                    or isinstance(val, staticmethod)
-                    or isinstance(val, classmethod)
-                    or isinstance(val, property))
+            if not (
+                var.startswith("_")
+                or callable(val)
+                or isinstance(val, staticmethod)
+                or isinstance(val, classmethod)
+                or isinstance(val, property)
+            )
         }
 
         return class_dict
 
     def _get_annotations(self) -> Dict[str, Any]:
         """Returns a dictionary mapping variable names to their type annotations."""
-        return self._get_from_self_and_super(
-            extract_func=lambda super_class: dict(get_type_hints(super_class))
-        )
+        return self._get_from_self_and_super(extract_func=lambda super_class: dict(get_type_hints(super_class)))
 
-    def _get_class_variables(self) -> OrderedDict:
-        """Returns an OrderedDict mapping class variables names to their additional information."""
-        class_variable_names = self._get_class_dict().keys() | self._get_annotations().keys()
+    def _get_class_variables(self) -> dict:
+        """Returns a dictionary mapping class variables names to their additional information."""
+        class_variable_names = {**self._get_annotations(), **self._get_class_dict()}.keys()
 
         try:
             class_variables = self._get_from_self_and_super(
-                extract_func=lambda super_class: get_class_variables(super_class),
-                dict_type=OrderedDict
+                extract_func=lambda super_class: get_class_variables(super_class)
             )
 
             # Handle edge-case of source code modification while code is running
             variables_to_add = class_variable_names - class_variables.keys()
             variables_to_remove = class_variables.keys() - class_variable_names
 
             for variable in variables_to_add:
-                class_variables[variable] = {'comment': ''}
+                class_variables[variable] = {"comment": ""}
 
             for variable in variables_to_remove:
                 class_variables.pop(variable)
         # Exception if inspect.getsource fails to extract the source code
         except Exception:
-            class_variables = OrderedDict()
+            class_variables = {}
             for variable in class_variable_names:
-                class_variables[variable] = {'comment': ''}
+                class_variables[variable] = {"comment": ""}
 
         return class_variables
 
     def _get_argument_names(self) -> Set[str]:
         """Returns a list of variable names corresponding to the arguments."""
-        return ({get_dest(*name_or_flags, **kwargs)
-                 for name_or_flags, kwargs in self.argument_buffer.values()} |
-                set(self._get_class_dict().keys()) |
-                set(self._annotations.keys())) - {'help'}
+        return (
+            {get_dest(*name_or_flags, **kwargs) for name_or_flags, kwargs in self.argument_buffer.values()}
+            | set(self._get_class_dict().keys())
+            | set(self._annotations.keys())
+        ) - {"help"}
 
     def as_dict(self) -> Dict[str, Any]:
         """Returns the member variables corresponding to the parsed arguments.
 
         Note: This does not include attributes set directly on an instance
         (e.g. arg is not included in MyTap().arg = "hi")
 
         :return: A dictionary mapping each argument's name to its value.
         """
         if not self._parsed:
-            raise ValueError('You should call `parse_args` before retrieving arguments.')
+            raise ValueError("You should call `parse_args` before retrieving arguments.")
 
         self_dict = self.__dict__
         class_dict = self._get_from_self_and_super(
-            extract_func=lambda super_class: dict(getattr(super_class, '__dict__', dict()))
+            extract_func=lambda super_class: dict(getattr(super_class, "__dict__", dict()))
         )
         class_dict = {key: val for key, val in class_dict.items() if key not in self_dict}
         stored_dict = {**self_dict, **class_dict}
 
         stored_dict = {
             var: getattr(self, var)
             for var, val in stored_dict.items()
-            if not (var.startswith('_')
-                    or isinstance(val, MethodType)
-                    or isinstance(val, staticmethod))
+            if not (var.startswith("_") or isinstance(val, MethodType) or isinstance(val, staticmethod))
         }
 
         tap_class_dict_keys = Tap().__dict__.keys() | Tap.__dict__.keys()
         stored_dict = {key: stored_dict[key] for key in stored_dict.keys() - tap_class_dict_keys}
 
         return stored_dict
 
@@ -608,54 +614,62 @@
         """
         # All of the required arguments must be provided or already set
         required_args = {a.dest for a in self._actions if a.required}
         unprovided_required_args = required_args - args_dict.keys()
         missing_required_args = [arg for arg in unprovided_required_args if not hasattr(self, arg)]
 
         if len(missing_required_args) > 0:
-            raise ValueError(f'Input dictionary "{args_dict}" does not include '
-                             f'all unset required arguments: "{missing_required_args}".')
+            raise ValueError(
+                f'Input dictionary "{args_dict}" does not include '
+                f'all unset required arguments: "{missing_required_args}".'
+            )
 
         # Load all arguments
         for key, value in args_dict.items():
             try:
                 setattr(self, key, value)
             except AttributeError:
                 if not skip_unsettable:
-                    raise AttributeError(f'Cannot set attribute "{key}" to "{value}". '
-                                         f'To skip arguments that cannot be set \n'
-                                         f'\t"skip_unsettable = True"')
+                    raise AttributeError(
+                        f'Cannot set attribute "{key}" to "{value}". '
+                        f"To skip arguments that cannot be set \n"
+                        f'\t"skip_unsettable = True"'
+                    )
 
         self._parsed = True
 
         return self
 
-    def save(self,
-             path: PathLike,
-             with_reproducibility: bool = True,
-             skip_unpicklable: bool = False,
-             repo_path: Optional[PathLike] = None) -> None:
+    def save(
+        self,
+        path: PathLike,
+        with_reproducibility: bool = True,
+        skip_unpicklable: bool = False,
+        repo_path: Optional[PathLike] = None,
+    ) -> None:
         """Saves the arguments and reproducibility information in JSON format, pickling what can't be encoded.
 
         :param path: Path to the JSON file where the arguments will be saved.
         :param with_reproducibility: If True, adds a "reproducibility" field with information (e.g. git hash)
                                      to the JSON file.
         :param repo_path: Path to the git repo to examine for reproducibility info.
                           If None, uses the git repo of the Python file that is run.
         :param skip_unpicklable: If True, does not save attributes whose values cannot be pickled.
         """
-        with open(path, 'w') as f:
+        with open(path, "w") as f:
             args = self._log_all(repo_path=repo_path) if with_reproducibility else self.as_dict()
             json.dump(args, f, indent=4, sort_keys=True, cls=define_python_object_encoder(skip_unpicklable))
 
-    def load(self,
-             path: PathLike,
-             check_reproducibility: bool = False,
-             skip_unsettable: bool = False,
-             repo_path: Optional[PathLike] = None) -> TapType:
+    def load(
+        self,
+        path: PathLike,
+        check_reproducibility: bool = False,
+        skip_unsettable: bool = False,
+        repo_path: Optional[PathLike] = None,
+    ) -> TapType:
         """Loads the arguments in JSON format. Note: Due to JSON, tuples are loaded as lists.
 
         :param path: Path to the JSON file where the arguments will be loaded from.
         :param check_reproducibility: When True, raises an error if the loaded reproducibility
                                       information doesn't match the current reproducibility information.
         :param skip_unsettable: When True, skips attributes that cannot be set in the Tap object,
                                 e.g. properties without setters.
@@ -663,15 +677,15 @@
                           If None, uses the git repo of the Python file that is run.
         :return: Returns self.
         """
         with open(path) as f:
             args_dict = json.load(f, object_hook=as_python_object)
 
         # Remove loaded reproducibility information since it is no longer valid
-        saved_reproducibility_data = args_dict.pop('reproducibility', None)
+        saved_reproducibility_data = args_dict.pop("reproducibility", None)
         if check_reproducibility:
             current_reproducibility_data = self.get_reproducibility_info(repo_path=repo_path)
             enforce_reproducibility(saved_reproducibility_data, current_reproducibility_data, path)
 
         self.from_dict(args_dict, skip_unsettable=skip_unsettable)
 
         return self
```

### Comparing `typed-argument-parser-1.8.1/tap/tapify.py` & `typed-argument-parser-1.9.0/tap/tapify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Tapify module, which can initialize a class or run a function by parsing arguments from the command line."""
 from inspect import signature, Parameter
-from typing import Any, Callable, List, Optional, TypeVar, Union
+from typing import Any, Callable, List, Optional, Type, TypeVar, Union
 
 from docstring_parser import parse
 
 from tap import Tap
 
-InputType = TypeVar('InputType')
-OutputType = TypeVar('OutputType')
+InputType = TypeVar("InputType")
+OutputType = TypeVar("OutputType")
 
 
-def tapify(class_or_function: Union[Callable[[InputType], OutputType], OutputType],
-           known_only: bool = False,
-           command_line_args: Optional[List[str]] = None,
-           **func_kwargs) -> OutputType:
+def tapify(
+    class_or_function: Union[Callable[[InputType], OutputType], Type[OutputType]],
+    known_only: bool = False,
+    command_line_args: Optional[List[str]] = None,
+    **func_kwargs,
+) -> OutputType:
     """Tapify initializes a class or runs a function by parsing arguments from the command line.
 
     :param class_or_function: The class or function to run with the provided arguments.
     :param known_only: If true, ignores extra arguments and only parses known arguments.
     :param command_line_args: A list of command line style arguments to parse (e.g., ['--arg', 'value']).
                               If None, arguments are parsed from the command line (default behavior).
     :param func_kwargs: Additional keyword arguments for the function. These act as default values when
@@ -36,50 +38,65 @@
     # Parse docstring
     docstring = parse(doc)
 
     # Get the description of each argument in the class init or function
     param_to_description = {param.arg_name: param.description for param in docstring.params}
 
     # Create a Tap object with a description from the docstring of the function or class
-    tap = Tap(description='\n'.join(filter(None, (docstring.short_description, docstring.long_description))))
+    tap = Tap(description="\n".join(filter(None, (docstring.short_description, docstring.long_description))))
+
+    # Keep track of whether **kwargs was provided
+    has_kwargs = False
 
     # Add arguments of class init or function to the Tap object
     for param_name, param in sig.parameters.items():
         tap_kwargs = {}
 
+        # Skip **kwargs
+        if param.kind == Parameter.VAR_KEYWORD:
+            has_kwargs = True
+            known_only = True
+            continue
+
         # Get type of the argument
         if param.annotation != Parameter.empty:
             # Any type defaults to str (needed for dataclasses where all non-default attributes must have a type)
             if param.annotation is Any:
                 tap._annotations[param.name] = str
             # Otherwise, get the type of the argument
             else:
                 tap._annotations[param.name] = param.annotation
 
         # Get the default or required of the argument
         if param.name in func_kwargs:
-            tap_kwargs['default'] = func_kwargs[param.name]
+            tap_kwargs["default"] = func_kwargs[param.name]
             del func_kwargs[param.name]
         elif param.default != Parameter.empty:
-            tap_kwargs['default'] = param.default
+            tap_kwargs["default"] = param.default
         else:
-            tap_kwargs['required'] = True
+            tap_kwargs["required"] = True
 
         # Get the help string of the argument
         if param.name in param_to_description:
-            tap.class_variables[param.name] = {'comment': param_to_description[param.name]}
+            tap.class_variables[param.name] = {"comment": param_to_description[param.name]}
 
         # Add the argument to the Tap object
-        tap._add_argument(f'--{param_name}', **tap_kwargs)
+        tap._add_argument(f"--{param_name}", **tap_kwargs)
 
     # If any func_kwargs remain, they are not used in the function, so raise an error
     if func_kwargs and not known_only:
-        raise ValueError(f'Unknown keyword arguments: {func_kwargs}')
+        raise ValueError(f"Unknown keyword arguments: {func_kwargs}")
 
     # Parse command line arguments
-    command_line_args = tap.parse_args(
-        args=command_line_args,
-        known_only=known_only
-    )
+    command_line_args = tap.parse_args(args=command_line_args, known_only=known_only)
+
+    # Get command line arguments as a dictionary
+    command_line_args_dict = command_line_args.as_dict()
+
+    # Get **kwargs from extra command line arguments
+    if has_kwargs:
+        kwargs = {tap.extra_args[i].lstrip("-"): tap.extra_args[i + 1] for i in range(0, len(tap.extra_args), 2)}
+
+        command_line_args_dict.update(kwargs)
 
     # Initialize the class or run the function with the parsed arguments
-    return class_or_function(**command_line_args.as_dict())
+    return class_or_function(**command_line_args_dict)
```

### Comparing `typed-argument-parser-1.8.1/tap/utils.py` & `typed-argument-parser-1.9.0/tap/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from argparse import ArgumentParser, ArgumentTypeError
 from base64 import b64encode, b64decode
-from collections import OrderedDict
 import copy
 from functools import wraps
 import inspect
 from io import StringIO
 from json import JSONEncoder
 import os
 import pickle
@@ -37,17 +36,17 @@
 def check_output(command: List[str], suppress_stderr: bool = True, **kwargs) -> str:
     """Runs subprocess.check_output and returns the result as a string.
 
     :param command: A list of strings representing the command to run on the command line.
     :param suppress_stderr: Whether to suppress anything written to standard error.
     :return: The output of the command, converted from bytes to string and stripped.
     """
-    with open(os.devnull, 'w') as devnull:
+    with open(os.devnull, "w") as devnull:
         devnull = devnull if suppress_stderr else None
-        output = subprocess.check_output(command, stderr=devnull, **kwargs).decode('utf-8').strip()
+        output = subprocess.check_output(command, stderr=devnull, **kwargs).decode("utf-8").strip()
     return output
 
 
 class GitInfo:
     """Class with helper methods for extracting information about a git repo."""
 
     def __init__(self, repo_path: PathLike):
@@ -55,69 +54,69 @@
 
     def has_git(self) -> bool:
         """Returns whether git is installed.
 
         :return: True if git is installed, False otherwise.
         """
         try:
-            output = check_output(['git', 'rev-parse', '--is-inside-work-tree'], cwd=self.repo_path)
-            return output == 'true'
+            output = check_output(["git", "rev-parse", "--is-inside-work-tree"], cwd=self.repo_path)
+            return output == "true"
         except (FileNotFoundError, subprocess.CalledProcessError):
             return False
 
     def get_git_root(self) -> str:
         """Gets the root directory of the git repo where the command is run.
 
         :return: The root directory of the current git repo.
         """
-        return check_output(['git', 'rev-parse', '--show-toplevel'], cwd=self.repo_path)
+        return check_output(["git", "rev-parse", "--show-toplevel"], cwd=self.repo_path)
 
     def get_git_url(self, commit_hash: bool = True) -> str:
         """Gets the https url of the git repo where the command is run.
 
         :param commit_hash: If True, the url links to the latest local git commit hash.
         If False, the url links to the general git url.
         :return: The https url of the current git repo.
         """
         # Get git url (either https or ssh)
         try:
-            url = check_output(['git', 'remote', 'get-url', 'origin'], cwd=self.repo_path)
+            url = check_output(["git", "remote", "get-url", "origin"], cwd=self.repo_path)
         except subprocess.CalledProcessError:
             # For git versions <2.0
-            url = check_output(['git', 'config', '--get', 'remote.origin.url'], cwd=self.repo_path)
+            url = check_output(["git", "config", "--get", "remote.origin.url"], cwd=self.repo_path)
 
         # Remove .git at end
-        url = url[:-len('.git')]
+        url = url[: -len(".git")]
 
         # Convert ssh url to https url
-        m = re.search('git@(.+):', url)
+        m = re.search("git@(.+):", url)
         if m is not None:
             domain = m.group(1)
-            path = url[m.span()[1]:]
-            url = f'https://{domain}/{path}'
+            path = url[m.span()[1] :]
+            url = f"https://{domain}/{path}"
 
         if commit_hash:
             # Add tree and hash of current commit
-            url = f'{url}/tree/{self.get_git_hash()}'
+            url = f"{url}/tree/{self.get_git_hash()}"
 
         return url
 
     def get_git_hash(self) -> str:
         """Gets the git hash of HEAD of the git repo where the command is run.
 
         :return: The git hash of HEAD of the current git repo.
         """
-        return check_output(['git', 'rev-parse', 'HEAD'], cwd=self.repo_path)
+        return check_output(["git", "rev-parse", "HEAD"], cwd=self.repo_path)
 
     def has_uncommitted_changes(self) -> bool:
         """Returns whether there are uncommitted changes in the git repo where the command is run.
 
         :return: True if there are uncommitted changes in the current git repo, False otherwise.
         """
-        status = check_output(['git', 'status'], cwd=self.repo_path)
+        status = check_output(["git", "status"], cwd=self.repo_path)
 
         return not status.endswith(NO_CHANGES_STATUS)
 
 
 def type_to_str(type_annotation: Union[type, Any]) -> str:
     """Gets a string representation of the provided type.
 
@@ -125,55 +124,55 @@
     :return: A string representation of the type annotation.
     """
     # Built-in type
     if type(type_annotation) == type:
         return type_annotation.__name__
 
     # Typing type
-    return str(type_annotation).replace('typing.', '')
+    return str(type_annotation).replace("typing.", "")
 
 
 def get_argument_name(*name_or_flags) -> str:
     """Gets the name of the argument.
 
     :param name_or_flags: Either a name or a list of option strings, e.g. foo or -f, --foo.
     :return: The name of the argument (extracted from name_or_flags).
     """
-    if '-h' in name_or_flags or '--help' in name_or_flags:
-        return 'help'
+    if "-h" in name_or_flags or "--help" in name_or_flags:
+        return "help"
 
     if len(name_or_flags) > 1:
-        name_or_flags = [n_or_f for n_or_f in name_or_flags if n_or_f.startswith('--')]
+        name_or_flags = [n_or_f for n_or_f in name_or_flags if n_or_f.startswith("--")]
 
     if len(name_or_flags) != 1:
-        raise ValueError(f'There should only be a single canonical name for argument {name_or_flags}!')
+        raise ValueError(f"There should only be a single canonical name for argument {name_or_flags}!")
 
-    return name_or_flags[0].lstrip('-')
+    return name_or_flags[0].lstrip("-")
 
 
 def get_dest(*name_or_flags, **kwargs) -> str:
     """Gets the name of the destination of the argument.
 
     :param name_or_flags: Either a name or a list of option strings, e.g. foo or -f, --foo.
     :param kwargs: Keyword arguments.
     :return: The name of the argument (extracted from name_or_flags).
     """
-    if '-h' in name_or_flags or '--help' in name_or_flags:
-        return 'help'
+    if "-h" in name_or_flags or "--help" in name_or_flags:
+        return "help"
 
     return ArgumentParser().add_argument(*name_or_flags, **kwargs).dest
 
 
 def is_option_arg(*name_or_flags) -> bool:
     """Returns whether the argument is an option arg (as opposed to a positional arg).
 
     :param name_or_flags: Either a name or a list of option strings, e.g. foo or -f, --foo.
     :return: True if the argument is an option arg, False otherwise.
     """
-    return any(name_or_flag.startswith('-') for name_or_flag in name_or_flags)
+    return any(name_or_flag.startswith("-") for name_or_flag in name_or_flags)
 
 
 def is_positional_arg(*name_or_flags) -> bool:
     """Returns whether the argument is a positional arg (as opposed to an optional arg).
 
     :param name_or_flags: Either a name or a list of option strings, e.g. foo or -f, --foo.
     :return: True if the argument is a positional arg, False otherwise.
@@ -189,120 +188,130 @@
     return token_generator
 
 
 def get_class_column(obj: type) -> int:
     """Determines the column number for class variables in a class."""
     first_line = 1
     for token_type, token, (start_line, start_column), (end_line, end_column), line in tokenize_source(obj):
-        if token.strip() == '@':
+        if token.strip() == "@":
             first_line += 1
-        if start_line <= first_line or token.strip() == '':
+        if start_line <= first_line or token.strip() == "":
             continue
 
         return start_column
 
 
 def source_line_to_tokens(obj: object) -> Dict[int, List[Dict[str, Union[str, int]]]]:
     """Gets a dictionary mapping from line number to a dictionary of tokens on that line for an object's source code."""
     line_to_tokens = {}
     for token_type, token, (start_line, start_column), (end_line, end_column), line in tokenize_source(obj):
-        line_to_tokens.setdefault(start_line, []).append({
-            'token_type': token_type,
-            'token': token,
-            'start_line': start_line,
-            'start_column': start_column,
-            'end_line': end_line,
-            'end_column': end_column,
-            'line': line
-        })
+        line_to_tokens.setdefault(start_line, []).append(
+            {
+                "token_type": token_type,
+                "token": token,
+                "start_line": start_line,
+                "start_column": start_column,
+                "end_line": end_line,
+                "end_column": end_column,
+                "line": line,
+            }
+        )
 
     return line_to_tokens
 
 
-def get_class_variables(cls: type) -> OrderedDict:
-    """Returns an OrderedDict mapping class variables to their additional information (currently just comments)."""
+def get_class_variables(cls: type) -> Dict[str, Dict[str, str]]:
+    """Returns a dictionary mapping class variables to their additional information (currently just comments)."""
     # Get mapping from line number to tokens
     line_to_tokens = source_line_to_tokens(cls)
 
     # Get class variable column number
     class_variable_column = get_class_column(cls)
 
     # Extract class variables
     class_variable = None
-    variable_to_comment = OrderedDict()
+    variable_to_comment = {}
     for tokens in line_to_tokens.values():
         for i, token in enumerate(tokens):
 
             # Skip whitespace
-            if token['token'].strip() == '':
+            if token["token"].strip() == "":
                 continue
 
             # Extract multiline comments
-            if (class_variable is not None
-                    and token['token_type'] == tokenize.STRING
-                    and token['token'][:1] in {'"', "'"}):
-                sep = ' ' if variable_to_comment[class_variable]['comment'] else ''
-                quote_char = token['token'][:1]
-                variable_to_comment[class_variable]['comment'] += sep + token['token'].strip(quote_char).strip()
+            if (
+                class_variable is not None
+                and token["token_type"] == tokenize.STRING
+                and token["token"][:1] in {'"', "'"}
+            ):
+                sep = " " if variable_to_comment[class_variable]["comment"] else ""
+                quote_char = token["token"][:1]
+                variable_to_comment[class_variable]["comment"] += sep + token["token"].strip(quote_char).strip()
 
             # Match class variable
             class_variable = None
-            if (token['token_type'] == tokenize.NAME and
-                    token['start_column'] == class_variable_column and
-                    len(tokens) > i and
-                    tokens[i + 1]['token'] in ['=', ':']):
+            if (
+                token["token_type"] == tokenize.NAME
+                and token["start_column"] == class_variable_column
+                and len(tokens) > i
+                and tokens[i + 1]["token"] in ["=", ":"]
+            ):
 
-                class_variable = token['token']
-                variable_to_comment[class_variable] = {'comment': ''}
+                class_variable = token["token"]
+                variable_to_comment[class_variable] = {"comment": ""}
 
                 # Find the comment (if it exists)
                 for j in range(i + 1, len(tokens)):
-                    if tokens[j]['token_type'] == tokenize.COMMENT:
+                    if tokens[j]["token_type"] == tokenize.COMMENT:
                         # Leave out "#" and whitespace from comment
-                        variable_to_comment[class_variable]['comment'] = tokens[j]['token'][1:].strip()
+                        variable_to_comment[class_variable]["comment"] = tokens[j]["token"][1:].strip()
                         break
 
             break
 
     return variable_to_comment
 
 
 def get_literals(literal: Literal, variable: str) -> Tuple[Callable[[str], Any], List[str]]:
     """Extracts the values from a Literal type and ensures that the values are all primitive types."""
     literals = list(get_args(literal))
 
     if not all(isinstance(literal, PRIMITIVES) for literal in literals):
         raise ArgumentTypeError(
             f'The type for variable "{variable}" contains a literal'
-            f'of a non-primitive type e.g. (str, int, float, bool).\n'
-            f'Currently only primitive-typed literals are supported.'
+            f"of a non-primitive type e.g. (str, int, float, bool).\n"
+            f"Currently only primitive-typed literals are supported."
         )
 
     str_to_literal = {str(literal): literal for literal in literals}
 
     if len(literals) != len(str_to_literal):
-        raise ArgumentTypeError('All literals must have unique string representations')
+        raise ArgumentTypeError("All literals must have unique string representations")
 
     def var_type(arg: str) -> Any:
-        return str_to_literal.get(arg, arg)
+        if arg not in str_to_literal:
+            raise ArgumentTypeError(f'Value for variable "{variable}" must be one of {literals}.')
+
+        return str_to_literal[arg]
 
     return var_type, literals
 
 
 def boolean_type(flag_value: str) -> bool:
     """Convert a string to a boolean if it is a prefix of 'True' or 'False' (case insensitive) or is '1' or '0'."""
-    if 'true'.startswith(flag_value.lower()) or flag_value == '1':
+    if "true".startswith(flag_value.lower()) or flag_value == "1":
         return True
-    if 'false'.startswith(flag_value.lower()) or flag_value == '0':
+    if "false".startswith(flag_value.lower()) or flag_value == "0":
         return False
     raise ArgumentTypeError('Value has to be a prefix of "True" or "False" (case insensitive) or "1" or "0".')
 
 
 class TupleTypeEnforcer:
     """The type argument to argparse for checking and applying types to Tuples."""
+
     def __init__(self, types: List[type], loop: bool = False):
         self.types = [boolean_type if t == bool else t for t in types]
         self.loop = loop
         self.index = 0
 
     def __call__(self, arg: str) -> Any:
         arg = self.types[self.index](arg)
@@ -312,14 +321,15 @@
             self.index %= len(self.types)
 
         return arg
 
 
 class MockTuple:
     """Mock of a tuple needed to prevent JSON encoding tuples as lists."""
+
     def __init__(self, _tuple: tuple) -> None:
         self.tuple = _tuple
 
 
 def _nested_replace_type(obj: Any, find_type: type, replace_type: type) -> Any:
     """Replaces any instance (including instances within lists, tuple, dict) of find_type with an instance of replace_type.
 
@@ -345,52 +355,45 @@
 
     if isinstance(obj, find_type):
         obj = replace_type(obj)
 
     return obj
 
 
-def define_python_object_encoder(skip_unpicklable: bool = False) -> 'PythonObjectEncoder':  # noqa F821
-
+def define_python_object_encoder(skip_unpicklable: bool = False) -> "PythonObjectEncoder":  # noqa F821
     class PythonObjectEncoder(JSONEncoder):
         """Stores parameters that are not JSON serializable as pickle dumps.
 
         See: https://stackoverflow.com/a/36252257
         """
+
         def iterencode(self, o: Any, _one_shot: bool = False) -> Iterator[str]:
             o = _nested_replace_type(o, tuple, MockTuple)
             return super(PythonObjectEncoder, self).iterencode(o, _one_shot)
 
         def default(self, obj: Any) -> Any:
             if isinstance(obj, set):
-                return {
-                    '_type': 'set',
-                    '_value': list(obj)
-                }
+                return {"_type": "set", "_value": list(obj)}
             elif isinstance(obj, MockTuple):
-                return {
-                    '_type': 'tuple',
-                    '_value': list(obj.tuple)
-                }
+                return {"_type": "tuple", "_value": list(obj.tuple)}
 
             try:
                 return {
-                    '_type': f'python_object (type = {obj.__class__.__name__})',
-                    '_value': b64encode(pickle.dumps(obj)).decode('utf-8')
+                    "_type": f"python_object (type = {obj.__class__.__name__})",
+                    "_value": b64encode(pickle.dumps(obj)).decode("utf-8"),
                 }
             except (pickle.PicklingError, TypeError, AttributeError) as e:
                 if not skip_unpicklable:
-                    raise ValueError(f'Could not pickle this object: Failed with exception {e}\n'
-                                     f'If you would like to ignore unpicklable attributes set '
-                                     f'skip_unpickleable = True in save.')
+                    raise ValueError(
+                        f"Could not pickle this object: Failed with exception {e}\n"
+                        f"If you would like to ignore unpicklable attributes set "
+                        f"skip_unpickleable = True in save."
+                    )
                 else:
-                    return {
-                        '_type': f'unpicklable_object {obj.__class__.__name__}',
-                        '_value': None
-                    }
+                    return {"_type": f"unpicklable_object {obj.__class__.__name__}", "_value": None}
 
     return PythonObjectEncoder
 
 
 class UnpicklableObject:
     """A class that serves as a placeholder for an object that could not be pickled. """
 
@@ -399,27 +402,27 @@
 
 
 def as_python_object(dct: Any) -> Any:
     """The hooks that allow a parameter that is not JSON serializable to be loaded.
 
     See: https://stackoverflow.com/a/36252257
     """
-    if '_type' in dct and '_value' in dct:
-        _type, value = dct['_type'], dct['_value']
+    if "_type" in dct and "_value" in dct:
+        _type, value = dct["_type"], dct["_value"]
 
-        if _type == 'tuple':
+        if _type == "tuple":
             return tuple(value)
 
-        elif _type == 'set':
+        elif _type == "set":
             return set(value)
 
-        elif _type.startswith('python_object'):
-            return pickle.loads(b64decode(value.encode('utf-8')))
+        elif _type.startswith("python_object"):
+            return pickle.loads(b64decode(value.encode("utf-8")))
 
-        elif _type.startswith('unpicklable_object'):
+        elif _type.startswith("unpicklable_object"):
             return UnpicklableObject()
 
         else:
             raise ArgumentTypeError(f'Special type "{_type}" not supported for JSON loading.')
 
     return dct
 
@@ -430,65 +433,65 @@
     Based on https://stackoverflow.com/questions/6279305/typeerror-cannot-deepcopy-this-pattern-object
     """
     if sys.version_info[:2] > (3, 6):
         return func
 
     @wraps(func)
     def wrapper(*args, **kwargs):
-        re_type = type(re.compile(''))
+        re_type = type(re.compile(""))
         has_prev_val = re_type in copy._deepcopy_dispatch
         prev_val = copy._deepcopy_dispatch.get(re_type, None)
-        copy._deepcopy_dispatch[type(re.compile(''))] = lambda r, _: r
+        copy._deepcopy_dispatch[type(re.compile(""))] = lambda r, _: r
 
         result = func(*args, **kwargs)
 
         if has_prev_val:
             copy._deepcopy_dispatch[re_type] = prev_val
         else:
             del copy._deepcopy_dispatch[re_type]
 
         return result
 
     return wrapper
 
 
-def enforce_reproducibility(saved_reproducibility_data: Optional[Dict[str, str]],
-                            current_reproducibility_data: Dict[str, str],
-                            path: PathLike) -> None:
+def enforce_reproducibility(
+    saved_reproducibility_data: Optional[Dict[str, str]], current_reproducibility_data: Dict[str, str], path: PathLike
+) -> None:
     """Checks if reproducibility has failed and raises the appropriate error.
 
     :param saved_reproducibility_data: Reproducibility information loaded from a saved file.
     :param current_reproducibility_data: Reproducibility information from the current object.
     :param path: The path name of the file that is being loaded.
     """
-    no_reproducibility_message = 'Reproducibility not guaranteed'
+    no_reproducibility_message = "Reproducibility not guaranteed"
 
     if saved_reproducibility_data is None:
-        raise ValueError(f'{no_reproducibility_message}: Could not find reproducibility '
-                         f'information in args loaded from "{path}".')
+        raise ValueError(
+            f"{no_reproducibility_message}: Could not find reproducibility "
+            f'information in args loaded from "{path}".'
+        )
+
+    if "git_url" not in saved_reproducibility_data:
+        raise ValueError(f"{no_reproducibility_message}: Could not find " f'git url in args loaded from "{path}".')
+
+    if "git_url" not in current_reproducibility_data:
+        raise ValueError(f"{no_reproducibility_message}: Could not find " f"git url in current args.")
+
+    if saved_reproducibility_data["git_url"] != current_reproducibility_data["git_url"]:
+        raise ValueError(
+            f"{no_reproducibility_message}: Differing git url/hash "
+            f'between current args and args loaded from "{path}".'
+        )
+
+    if saved_reproducibility_data["git_has_uncommitted_changes"]:
+        raise ValueError(f"{no_reproducibility_message}: Uncommitted changes " f'in args loaded from "{path}".')
 
-    if 'git_url' not in saved_reproducibility_data:
-        raise ValueError(f'{no_reproducibility_message}: Could not find '
-                         f'git url in args loaded from "{path}".')
-
-    if 'git_url' not in current_reproducibility_data:
-        raise ValueError(f'{no_reproducibility_message}: Could not find '
-                         f'git url in current args.')
-
-    if saved_reproducibility_data['git_url'] != current_reproducibility_data['git_url']:
-        raise ValueError(f'{no_reproducibility_message}: Differing git url/hash '
-                         f'between current args and args loaded from "{path}".')
-
-    if saved_reproducibility_data['git_has_uncommitted_changes']:
-        raise ValueError(f'{no_reproducibility_message}: Uncommitted changes '
-                         f'in args loaded from "{path}".')
-
-    if current_reproducibility_data['git_has_uncommitted_changes']:
-        raise ValueError(f'{no_reproducibility_message}: Uncommitted changes '
-                         f'in current args.')
+    if current_reproducibility_data["git_has_uncommitted_changes"]:
+        raise ValueError(f"{no_reproducibility_message}: Uncommitted changes " f"in current args.")
 
 
 # TODO: remove this once typing_inspect.get_origin is fixed for Python 3.8, 3.9, and 3.10
 # https://github.com/ilevkivskyi/typing_inspect/issues/64
 # https://github.com/ilevkivskyi/typing_inspect/issues/65
 def get_origin(tp: Any) -> Any:
     """Same as typing_inspect.get_origin but fixes unparameterized generic types like Set."""
```

### Comparing `typed-argument-parser-1.8.1/tests/test_actions.py` & `typed-argument-parser-1.9.0/tests/test_actions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,224 +3,221 @@
 import unittest
 from unittest import TestCase
 
 from tap import Tap
 
 
 class TestArgparseActions(TestCase):
-
     def test_actions_store_const(self):
         class StoreConstTap(Tap):
-
             def configure(self):
-                self.add_argument('--sum',
-                                  dest='accumulate',
-                                  action='store_const',
-                                  const=sum,
-                                  default=max)
+                self.add_argument("--sum", dest="accumulate", action="store_const", const=sum, default=max)
 
         args = StoreConstTap().parse_args([])
-        self.assertFalse(hasattr(args, 'sum'))
+        self.assertFalse(hasattr(args, "sum"))
         self.assertEqual(args.accumulate, max)
-        self.assertEqual(args.as_dict(), {'accumulate': max})
+        self.assertEqual(args.as_dict(), {"accumulate": max})
 
-        args = StoreConstTap().parse_args(['--sum'])
-        self.assertFalse(hasattr(args, 'sum'))
+        args = StoreConstTap().parse_args(["--sum"])
+        self.assertFalse(hasattr(args, "sum"))
         self.assertEqual(args.accumulate, sum)
-        self.assertEqual(args.as_dict(), {'accumulate': sum})
+        self.assertEqual(args.as_dict(), {"accumulate": sum})
 
     def test_actions_store_true_default_true(self):
         class StoreTrueDefaultTrueTap(Tap):
             foobar: bool = True
 
             def configure(self):
-                self.add_argument('--foobar', action='store_true')
+                self.add_argument("--foobar", action="store_true")
+
         args = StoreTrueDefaultTrueTap().parse_args([])
         self.assertTrue(args.foobar)
 
-        args = StoreTrueDefaultTrueTap().parse_args(['--foobar'])
+        args = StoreTrueDefaultTrueTap().parse_args(["--foobar"])
         self.assertTrue(args.foobar)
 
     def test_actions_store_true_default_false(self):
         class StoreTrueDefaultFalseTap(Tap):
             foobar: bool = False
 
             def configure(self):
-                self.add_argument('--foobar', action='store_true')
+                self.add_argument("--foobar", action="store_true")
+
         args = StoreTrueDefaultFalseTap().parse_args([])
         self.assertFalse(args.foobar)
 
-        args = StoreTrueDefaultFalseTap().parse_args(['--foobar'])
+        args = StoreTrueDefaultFalseTap().parse_args(["--foobar"])
         self.assertTrue(args.foobar)
 
     def test_actions_store_false_default_true(self):
         class StoreFalseDefaultTrueTap(Tap):
             foobar: bool = True
 
             def configure(self):
-                self.add_argument('--foobar', action='store_false')
+                self.add_argument("--foobar", action="store_false")
+
         args = StoreFalseDefaultTrueTap().parse_args([])
         self.assertTrue(args.foobar)
 
-        args = StoreFalseDefaultTrueTap().parse_args(['--foobar'])
+        args = StoreFalseDefaultTrueTap().parse_args(["--foobar"])
         self.assertFalse(args.foobar)
 
     def test_actions_store_false_default_false(self):
         class StoreFalseDefaultFalseTap(Tap):
             foobar: bool = False
 
             def configure(self):
-                self.add_argument('--foobar', action='store_false')
+                self.add_argument("--foobar", action="store_false")
+
         args = StoreFalseDefaultFalseTap().parse_args([])
         self.assertFalse(args.foobar)
 
-        args = StoreFalseDefaultFalseTap().parse_args(['--foobar'])
+        args = StoreFalseDefaultFalseTap().parse_args(["--foobar"])
         self.assertFalse(args.foobar)
 
     def test_actions_append_list(self):
         class AppendListTap(Tap):
-            arg: List = ['what', 'is']
+            arg: List = ["what", "is"]
 
             def configure(self):
-                self.add_argument('--arg', action='append')
+                self.add_argument("--arg", action="append")
 
         args = AppendListTap().parse_args([])
-        self.assertEqual(args.arg, ['what', 'is'])
+        self.assertEqual(args.arg, ["what", "is"])
 
-        args = AppendListTap().parse_args('--arg up --arg today'.split())
-        self.assertEqual(args.arg, 'what is up today'.split())
+        args = AppendListTap().parse_args("--arg up --arg today".split())
+        self.assertEqual(args.arg, "what is up today".split())
 
     def test_actions_append_list_int(self):
         class AppendListIntTap(Tap):
             arg: List[int] = [1, 2]
 
             def configure(self):
-                self.add_argument('--arg', action='append')
+                self.add_argument("--arg", action="append")
 
-        args = AppendListIntTap().parse_args('--arg 3 --arg 4'.split())
+        args = AppendListIntTap().parse_args("--arg 3 --arg 4".split())
         self.assertEqual(args.arg, [1, 2, 3, 4])
 
     def test_actions_append_list_literal(self):
         class AppendListLiteralTap(Tap):
-            arg: List[Literal['what', 'is', 'up', 'today']] = ['what', 'is']
+            arg: List[Literal["what", "is", "up", "today"]] = ["what", "is"]
 
             def configure(self):
-                self.add_argument('--arg', action='append')
+                self.add_argument("--arg", action="append")
 
-        args = AppendListLiteralTap().parse_args('--arg up --arg today'.split())
-        self.assertEqual(args.arg, 'what is up today'.split())
+        args = AppendListLiteralTap().parse_args("--arg up --arg today".split())
+        self.assertEqual(args.arg, "what is up today".split())
 
     def test_actions_append_untyped(self):
         class AppendListStrTap(Tap):
-            arg = ['what', 'is']
+            arg = ["what", "is"]
 
             def configure(self):
-                self.add_argument('--arg', action='append')
+                self.add_argument("--arg", action="append")
 
         args = AppendListStrTap().parse_args([])
-        self.assertEqual(args.arg, ['what', 'is'])
+        self.assertEqual(args.arg, ["what", "is"])
 
-        args = AppendListStrTap().parse_args('--arg up --arg today'.split())
-        self.assertEqual(args.arg, 'what is up today'.split())
+        args = AppendListStrTap().parse_args("--arg up --arg today".split())
+        self.assertEqual(args.arg, "what is up today".split())
 
     def test_actions_append_const(self):
         class AppendConstTap(Tap):
             arg: List[int] = [1, 2, 3]
 
             def configure(self):
-                self.add_argument('--arg', action='append_const', const=7)
+                self.add_argument("--arg", action="append_const", const=7)
 
         args = AppendConstTap().parse_args([])
         self.assertEqual(args.arg, [1, 2, 3])
 
-        args = AppendConstTap().parse_args('--arg --arg'.split())
+        args = AppendConstTap().parse_args("--arg --arg".split())
         self.assertEqual(args.arg, [1, 2, 3, 7, 7])
 
     def test_actions_count(self):
         class CountTap(Tap):
             arg = 7
 
             def configure(self):
-                self.add_argument('--arg', '-a', action='count')
+                self.add_argument("--arg", "-a", action="count")
 
         args = CountTap().parse_args([])
         self.assertEqual(args.arg, 7)
 
-        args = CountTap().parse_args('-aaa --arg'.split())
+        args = CountTap().parse_args("-aaa --arg".split())
         self.assertEqual(args.arg, 11)
 
     def test_actions_int_count(self):
         class CountIntTap(Tap):
             arg: int = 7
 
             def configure(self):
-                self.add_argument('--arg', '-a', action='count')
+                self.add_argument("--arg", "-a", action="count")
 
         args = CountIntTap().parse_args([])
         self.assertEqual(args.arg, 7)
 
-        args = CountIntTap().parse_args('-aaa --arg'.split())
+        args = CountIntTap().parse_args("-aaa --arg".split())
         self.assertEqual(args.arg, 11)
 
     def test_actions_version(self):
         class VersionTap(Tap):
-
             def configure(self):
-                self.add_argument('--version', action='version', version='2.0')
+                self.add_argument("--version", action="version", version="2.0")
 
         # Ensure that nothing breaks without version flag
         VersionTap().parse_args([])
 
         # TODO: With version flag testing fails, but manual tests work
         # tried redirecting stderr using unittest.mock.patch
         # VersionTap().parse_args(['--version'])
 
     @unittest.skipIf(sys.version_info < (3, 8), 'action="extend" introduced in argparse in Python 3.8')
     def test_actions_extend(self):
         class ExtendTap(Tap):
             arg = [1, 2]
 
             def configure(self):
-                self.add_argument('--arg', nargs="+", action='extend')
+                self.add_argument("--arg", nargs="+", action="extend")
 
         args = ExtendTap().parse_args([])
         self.assertEqual(args.arg, [1, 2])
 
-        args = ExtendTap().parse_args('--arg a b --arg a --arg c d'.split())
-        self.assertEqual(args.arg, [1, 2] + 'a b a c d'.split())
+        args = ExtendTap().parse_args("--arg a b --arg a --arg c d".split())
+        self.assertEqual(args.arg, [1, 2] + "a b a c d".split())
 
     @unittest.skipIf(sys.version_info < (3, 8), 'action="extend" introduced in argparse in Python 3.8')
     def test_actions_extend_list(self):
         class ExtendListTap(Tap):
-            arg: List = ['hi']
+            arg: List = ["hi"]
 
             def configure(self):
-                self.add_argument('--arg', action='extend')
+                self.add_argument("--arg", action="extend")
 
-        args = ExtendListTap().parse_args('--arg yo yo --arg yoyo --arg yo yo'.split())
-        self.assertEqual(args.arg, 'hi yo yo yoyo yo yo'.split())
+        args = ExtendListTap().parse_args("--arg yo yo --arg yoyo --arg yo yo".split())
+        self.assertEqual(args.arg, "hi yo yo yoyo yo yo".split())
 
     @unittest.skipIf(sys.version_info < (3, 8), 'action="extend" introduced in argparse in Python 3.8')
     def test_actions_extend_list_int(self):
         class ExtendListIntTap(Tap):
             arg: List[int] = [0]
 
             def configure(self):
-                self.add_argument('--arg', action='extend')
+                self.add_argument("--arg", action="extend")
 
-        args = ExtendListIntTap().parse_args('--arg 1 2 --arg 3 --arg 4 5'.split())
+        args = ExtendListIntTap().parse_args("--arg 1 2 --arg 3 --arg 4 5".split())
         self.assertEqual(args.arg, [0, 1, 2, 3, 4, 5])
 
     def test_positional_default(self):
         class PositionalDefault(Tap):
             arg: str
 
             def configure(self):
-                self.add_argument('arg')
+                self.add_argument("arg")
 
-        help_regex = r'.*positional arguments:\n.*arg\s*\(str, required\).*'
+        help_regex = r".*positional arguments:\n.*arg\s*\(str, required\).*"
         help_text = PositionalDefault().format_help()
         self.assertRegex(help_text, help_regex)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `typed-argument-parser-1.8.1/tests/test_integration.py` & `typed-argument-parser-1.9.0/tests/test_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,128 +37,131 @@
             pass
 
         EmptyTap().parse_args([])
 
     def test_empty_add_argument(self) -> None:
         class EmptyAddArgument(Tap):
             def configure(self) -> None:
-                self.add_argument('--hi')
+                self.add_argument("--hi")
 
-        hi = 'yo'
-        args = EmptyAddArgument().parse_args(['--hi', hi])
+        hi = "yo"
+        args = EmptyAddArgument().parse_args(["--hi", hi])
         self.assertEqual(args.hi, hi)
 
     def test_no_typed_args(self) -> None:
         class NoTypedTap(Tap):
             hi = 3
 
         args = NoTypedTap().parse_args([])
         self.assertEqual(args.hi, 3)
 
-        hi = 'yo'
-        args = NoTypedTap().parse_args(['--hi', hi])
+        hi = "yo"
+        args = NoTypedTap().parse_args(["--hi", hi])
         self.assertEqual(args.hi, hi)
 
     def test_only_typed_args(self) -> None:
         class OnlyTypedTap(Tap):
-            hi: str = 'sup'
+            hi: str = "sup"
 
         args = OnlyTypedTap().parse_args([])
-        self.assertEqual(args.hi, 'sup')
+        self.assertEqual(args.hi, "sup")
 
-        hi = 'yo'
-        args = OnlyTypedTap().parse_args(['--hi', hi])
+        hi = "yo"
+        args = OnlyTypedTap().parse_args(["--hi", hi])
         self.assertEqual(args.hi, hi)
 
     def test_type_as_string(self) -> None:
         class TypeAsString(Tap):
             a_number: "int" = 3
             a_list: "List[float]" = [3.7, 0.3]
 
         args = TypeAsString().parse_args([])
         self.assertEqual(args.a_number, 3)
         self.assertEqual(args.a_list, [3.7, 0.3])
 
         a_number = 42
         a_list = [3, 4, 0.7]
 
-        args = TypeAsString().parse_args(
-            ['--a_number', str(a_number), '--a_list'] + [str(i) for i in a_list]
-        )
+        args = TypeAsString().parse_args(["--a_number", str(a_number), "--a_list"] + [str(i) for i in a_list])
         self.assertEqual(args.a_number, a_number)
         self.assertEqual(args.a_list, a_list)
 
     def test_parse_twice(self) -> None:
         class ParseTwiceTap(Tap):
             a: int = 5
 
         with self.assertRaises(ValueError):
-            ParseTwiceTap().parse_args(['--a', '6']).parse_args(['--a', '7'])
+            ParseTwiceTap().parse_args(["--a", "6"]).parse_args(["--a", "7"])
 
 
 class RequiredClassVariableTests(TestCase):
-
     def setUp(self) -> None:
         class RequiredArgumentsParser(Tap):
             arg_str_required: str
             arg_list_str_required: List[str]
 
         self.tap = RequiredArgumentsParser()
 
     def test_arg_str_required(self):
         with self.assertRaises(SystemExit):
-            self.tap.parse_args([
-                '--arg_str_required', 'tappy',
-            ])
+            self.tap.parse_args(
+                ["--arg_str_required", "tappy",]
+            )
 
     def test_arg_list_str_required(self):
         with self.assertRaises(SystemExit):
-            self.tap.parse_args([
-                '--arg_list_str_required', 'hi', 'there',
-            ])
+            self.tap.parse_args(
+                ["--arg_list_str_required", "hi", "there",]
+            )
 
     def test_both_assigned_okay(self):
-        args = self.tap.parse_args([
-            '--arg_str_required', 'tappy',
-            '--arg_list_str_required', 'hi', 'there',
-        ])
-        self.assertEqual(args.arg_str_required, 'tappy')
-        self.assertEqual(args.arg_list_str_required, ['hi', 'there'])
+        args = self.tap.parse_args(["--arg_str_required", "tappy", "--arg_list_str_required", "hi", "there",])
+        self.assertEqual(args.arg_str_required, "tappy")
+        self.assertEqual(args.arg_list_str_required, ["hi", "there"])
 
 
 class ParameterizedStandardCollectionTests(TestCase):
-    @unittest.skipIf(sys.version_info < (3, 9),
-                     'Parameterized standard collections (e.g., list[int]) introduced in Python 3.9')
+    @unittest.skipIf(
+        sys.version_info < (3, 9), "Parameterized standard collections (e.g., list[int]) introduced in Python 3.9"
+    )
     def test_parameterized_standard_collection(self):
         class ParameterizedStandardCollectionTap(Tap):
             arg_list_str: list[str]
             arg_list_int: list[int]
             arg_list_int_default: list[int] = [1, 2, 5]
             arg_set_float: set[float]
-            arg_set_str_default: set[str] = {'one', 'two', 'five'}
+            arg_set_str_default: set[str] = {"one", "two", "five"}
             arg_tuple_int: tuple[int, ...]
             arg_tuple_float_default: tuple[float, float, float] = (1.0, 2.0, 5.0)
-            arg_tuple_str_override: tuple[str, str] = ('hi', 'there')
+            arg_tuple_str_override: tuple[str, str] = ("hi", "there")
             arg_optional_list_int: Optional[list[int]] = None
 
-        arg_list_str = ['a', 'b', 'pi']
+        arg_list_str = ["a", "b", "pi"]
         arg_list_int = [-2, -5, 10]
         arg_set_float = {3.54, 2.235}
         arg_tuple_int = (-4, 5, 9, 103)
-        arg_tuple_str_override = ('why', 'so')
+        arg_tuple_str_override = ("why", "so")
         arg_optional_list_int = [5, 4, 3]
 
-        args = ParameterizedStandardCollectionTap().parse_args([
-            '--arg_list_str', *arg_list_str,
-            '--arg_list_int', *[str(var) for var in arg_list_int],
-            '--arg_set_float', *[str(var) for var in arg_set_float],
-            '--arg_tuple_int', *[str(var) for var in arg_tuple_int],
-            '--arg_tuple_str_override', *arg_tuple_str_override,
-            '--arg_optional_list_int', *[str(var) for var in arg_optional_list_int]
-        ])
+        args = ParameterizedStandardCollectionTap().parse_args(
+            [
+                "--arg_list_str",
+                *arg_list_str,
+                "--arg_list_int",
+                *[str(var) for var in arg_list_int],
+                "--arg_set_float",
+                *[str(var) for var in arg_set_float],
+                "--arg_tuple_int",
+                *[str(var) for var in arg_tuple_int],
+                "--arg_tuple_str_override",
+                *arg_tuple_str_override,
+                "--arg_optional_list_int",
+                *[str(var) for var in arg_optional_list_int],
+            ]
+        )
 
         self.assertEqual(args.arg_list_str, arg_list_str)
         self.assertEqual(args.arg_list_int, arg_list_int)
         self.assertEqual(args.arg_list_int_default, ParameterizedStandardCollectionTap.arg_list_int_default)
         self.assertEqual(args.arg_set_float, arg_set_float)
         self.assertEqual(args.arg_set_str_default, ParameterizedStandardCollectionTap.arg_set_str_default)
         self.assertEqual(args.arg_tuple_int, arg_tuple_int)
@@ -183,51 +186,68 @@
     tuple_pair: Optional[Tuple[bool, str, int]]
     tuple_arbitrary_len_bool: Optional[Tuple[bool, ...]]
     tuple_arbitrary_len_int: Optional[Tuple[int, ...]]
     tuple_arbitrary_len_str: Optional[Tuple[str, ...]]
 
 
 class NestedOptionalTypeTests(TestCase):
-
     def test_nested_optional_types(self):
-        list_ = ['I', 'was', 'wondering']
+        list_ = ["I", "was", "wondering"]
         list_bool = [True, False]
         list_int = [0, 1, 2]
-        list_str = ['a', 'bee', 'cd', 'ee']
-        set_ = {'if', 'after', 'all'}
+        list_str = ["a", "bee", "cd", "ee"]
+        set_ = {"if", "after", "all"}
         set_bool = {True, False, True}
         set_int = {0, 1}
-        set_str = {'a', 'bee', 'cd'}
-        tuple_ = ('these', 'years')
+        set_str = {"a", "bee", "cd"}
+        tuple_ = ("these", "years")
         tuple_bool = (False,)
         tuple_int = (0,)
-        tuple_str = ('a',)
-        tuple_pair = (False, 'a', 1)
+        tuple_str = ("a",)
+        tuple_pair = (False, "a", 1)
         tuple_arbitrary_len_bool = (True, False, False)
         tuple_arbitrary_len_int = (1, 2, 3, 4)
-        tuple_arbitrary_len_str = ('a', 'b')
+        tuple_arbitrary_len_str = ("a", "b")
 
-        args = NestedOptionalTypesTap().parse_args([
-            '--list', *stringify(list_),
-            '--list_bool', *stringify(list_bool),
-            '--list_int', *stringify(list_int),
-            '--list_str', *stringify(list_str),
-            '--set', *stringify(set_),
-            '--set_bool', *stringify(set_bool),
-            '--set_int', *stringify(set_int),
-            '--set_str', *stringify(set_str),
-            '--tuple', *stringify(tuple_),
-            '--tuple_bool', *stringify(tuple_bool),
-            '--tuple_int', *stringify(tuple_int),
-            '--tuple_str', *stringify(tuple_str),
-            '--tuple_pair', *stringify(tuple_pair),
-            '--tuple_arbitrary_len_bool', *stringify(tuple_arbitrary_len_bool),
-            '--tuple_arbitrary_len_int', *stringify(tuple_arbitrary_len_int),
-            '--tuple_arbitrary_len_str', *stringify(tuple_arbitrary_len_str),
-        ])
+        args = NestedOptionalTypesTap().parse_args(
+            [
+                "--list",
+                *stringify(list_),
+                "--list_bool",
+                *stringify(list_bool),
+                "--list_int",
+                *stringify(list_int),
+                "--list_str",
+                *stringify(list_str),
+                "--set",
+                *stringify(set_),
+                "--set_bool",
+                *stringify(set_bool),
+                "--set_int",
+                *stringify(set_int),
+                "--set_str",
+                *stringify(set_str),
+                "--tuple",
+                *stringify(tuple_),
+                "--tuple_bool",
+                *stringify(tuple_bool),
+                "--tuple_int",
+                *stringify(tuple_int),
+                "--tuple_str",
+                *stringify(tuple_str),
+                "--tuple_pair",
+                *stringify(tuple_pair),
+                "--tuple_arbitrary_len_bool",
+                *stringify(tuple_arbitrary_len_bool),
+                "--tuple_arbitrary_len_int",
+                *stringify(tuple_arbitrary_len_int),
+                "--tuple_arbitrary_len_str",
+                *stringify(tuple_arbitrary_len_str),
+            ]
+        )
 
         self.assertEqual(args.list, list_)
         self.assertEqual(args.list_bool, list_bool)
         self.assertEqual(args.list_int, list_int)
         self.assertEqual(args.list_str, list_str)
 
         self.assertEqual(args.set, set_)
@@ -251,27 +271,34 @@
     list_path: List[Path]
     set_path: Set[Path]
     tuple_path: Tuple[Path, Path]
 
 
 class ComplexTypeTests(TestCase):
     def test_complex_types(self):
-        path = Path('/path/to/file.txt')
-        optional_path = Path('/path/to/optional/file.txt')
-        list_path = [Path('/path/to/list/file1.txt'), Path('/path/to/list/file2.txt')]
-        set_path = {Path('/path/to/set/file1.txt'), Path('/path/to/set/file2.txt')}
-        tuple_path = (Path('/path/to/tuple/file1.txt'), Path('/path/to/tuple/file2.txt'))
-
-        args = ComplexTypeTap().parse_args([
-            '--path', str(path),
-            '--optional_path', str(optional_path),
-            '--list_path', *[str(path) for path in list_path],
-            '--set_path', *[str(path) for path in set_path],
-            '--tuple_path', *[str(path) for path in tuple_path]
-        ])
+        path = Path("/path/to/file.txt")
+        optional_path = Path("/path/to/optional/file.txt")
+        list_path = [Path("/path/to/list/file1.txt"), Path("/path/to/list/file2.txt")]
+        set_path = {Path("/path/to/set/file1.txt"), Path("/path/to/set/file2.txt")}
+        tuple_path = (Path("/path/to/tuple/file1.txt"), Path("/path/to/tuple/file2.txt"))
+
+        args = ComplexTypeTap().parse_args(
+            [
+                "--path",
+                str(path),
+                "--optional_path",
+                str(optional_path),
+                "--list_path",
+                *[str(path) for path in list_path],
+                "--set_path",
+                *[str(path) for path in set_path],
+                "--tuple_path",
+                *[str(path) for path in tuple_path],
+            ]
+        )
 
         self.assertEqual(args.path, path)
         self.assertEqual(args.optional_path, optional_path)
         self.assertEqual(args.list_path, list_path)
         self.assertEqual(args.set_path, set_path)
         self.assertEqual(args.tuple_path, tuple_path)
 
@@ -282,206 +309,240 @@
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Person) and self.name == other.name
 
 
 class IntegrationDefaultTap(Tap):
     """Documentation is boring"""
+
     arg_untyped = 42
-    arg_str: str = 'hello there'
+    arg_str: str = "hello there"
     arg_int: int = -100
     arg_float: float = 77.3
     # TODO: how to handle untyped arguments?
     # users might accidentally think they should behave according to the inferred type
     # arg_bool_untyped_true = True
     # arg_bool_untyped_false = False
     arg_bool_true: bool = True
     arg_bool_false: bool = False
-    arg_literal: Literal['english', 'A', True, 88.9, 100] = 'A'
+    arg_literal: Literal["english", "A", True, 88.9, 100] = "A"
 
     arg_optional: Optional = None
     arg_optional_str: Optional[str] = None
     arg_optional_int: Optional[int] = None
     arg_optional_float: Optional[float] = None
     arg_optional_bool: Optional[bool] = None
-    arg_optional_literal: Optional[Literal['english', 'A', True, 88.9, 100]] = None
+    arg_optional_literal: Optional[Literal["english", "A", True, 88.9, 100]] = None
 
-    arg_list: List = ['these', 'are', 'strings']
-    arg_list_str: List[str] = ['hello', 'how are you']
+    arg_list: List = ["these", "are", "strings"]
+    arg_list_str: List[str] = ["hello", "how are you"]
     arg_list_int: List[int] = [10, -11]
     arg_list_float: List[float] = [3.14, 6.28]
     arg_list_bool: List[bool] = [True, False]
-    arg_list_literal: List[Literal['H', 1, 1.00784, False]] = ['H', False]
+    arg_list_literal: List[Literal["H", 1, 1.00784, False]] = ["H", False]
     arg_list_str_empty: List[str] = []
 
-    arg_set: Set = {'these', 'are', 'strings'}
-    arg_set_str: Set[str] = {'hello', 'how are you'}
+    arg_set: Set = {"these", "are", "strings"}
+    arg_set_str: Set[str] = {"hello", "how are you"}
     arg_set_int: Set[int] = {10, -11}
     arg_set_float: Set[float] = {3.14, 6.28}
     arg_set_bool: Set[bool] = {True, False}
-    arg_set_literal: Set[Literal['H', 1, 1.00784, False]] = {'H', False}
+    arg_set_literal: Set[Literal["H", 1, 1.00784, False]] = {"H", False}
     arg_set_str_empty: Set[str] = set()
 
-    arg_tuple: Tuple = ('these', 'are', 'strings')
-    arg_tuple_str: Tuple[str, ...] = ('hello', 'how are you')
+    arg_tuple: Tuple = ("these", "are", "strings")
+    arg_tuple_str: Tuple[str, ...] = ("hello", "how are you")
     arg_tuple_int: Tuple[int, ...] = (10, -11)
     arg_tuple_float: Tuple[float, ...] = (3.14, 6.28)
     arg_tuple_bool: Tuple[bool, ...] = (True, True, True, False)
-    arg_tuple_multi: Tuple[float, int, str, bool, float] = (1.2, 1, 'hi', True, 1.3)
+    arg_tuple_multi: Tuple[float, int, str, bool, float] = (1.2, 1, "hi", True, 1.3)
     # TODO: move these elsewhere since we don't support them as defaults
     # arg_other_type_required: Person
     # arg_other_type_default: Person = Person('tap')
 
 
 class SubclassTests(TestCase):
-
     def test_subclass(self) -> None:
         class IntegrationSubclassTap(IntegrationDefaultTap):
             arg_subclass_untyped = 33
-            arg_subclass_str: str = 'hello'
+            arg_subclass_str: str = "hello"
             arg_subclass_str_required: str
-            arg_subclass_str_set_me: str = 'goodbye'
+            arg_subclass_str_set_me: str = "goodbye"
             arg_float: float = -2.7
 
-        arg_subclass_str_required = 'subclassing is fun'
-        arg_subclass_str_set_me = 'all set!'
-        arg_int = '77'
-        self.args = IntegrationSubclassTap().parse_args([
-            '--arg_subclass_str_required', arg_subclass_str_required,
-            '--arg_subclass_str_set_me', arg_subclass_str_set_me,
-            '--arg_int', arg_int
-        ])
+        arg_subclass_str_required = "subclassing is fun"
+        arg_subclass_str_set_me = "all set!"
+        arg_int = "77"
+        self.args = IntegrationSubclassTap().parse_args(
+            [
+                "--arg_subclass_str_required",
+                arg_subclass_str_required,
+                "--arg_subclass_str_set_me",
+                arg_subclass_str_set_me,
+                "--arg_int",
+                arg_int,
+            ]
+        )
 
         arg_int = int(arg_int)
 
         self.assertEqual(self.args.arg_str, IntegrationDefaultTap.arg_str)
         self.assertEqual(self.args.arg_int, arg_int)
         self.assertEqual(self.args.arg_float, -2.7)
         self.assertEqual(self.args.arg_subclass_str_required, arg_subclass_str_required)
         self.assertEqual(self.args.arg_subclass_str_set_me, arg_subclass_str_set_me)
 
 
 class DefaultClassVariableTests(TestCase):
-
     def test_get_default_args(self) -> None:
         args = IntegrationDefaultTap().parse_args([])
 
         self.assertEqual(args.arg_untyped, 42)
-        self.assertEqual(args.arg_str, 'hello there')
+        self.assertEqual(args.arg_str, "hello there")
         self.assertEqual(args.arg_int, -100)
         self.assertEqual(args.arg_float, 77.3)
         self.assertEqual(args.arg_bool_true, True)
         self.assertEqual(args.arg_bool_false, False)
-        self.assertEqual(args.arg_literal, 'A')
+        self.assertEqual(args.arg_literal, "A")
 
         self.assertTrue(args.arg_optional is None)
         self.assertTrue(args.arg_optional_str is None)
         self.assertTrue(args.arg_optional_int is None)
         self.assertTrue(args.arg_optional_float is None)
         self.assertTrue(args.arg_optional_bool is None)
         self.assertTrue(args.arg_optional_literal is None)
 
-        self.assertEqual(args.arg_list, ['these', 'are', 'strings'])
-        self.assertEqual(args.arg_list_str, ['hello', 'how are you'])
+        self.assertEqual(args.arg_list, ["these", "are", "strings"])
+        self.assertEqual(args.arg_list_str, ["hello", "how are you"])
         self.assertEqual(args.arg_list_int, [10, -11])
         self.assertEqual(args.arg_list_float, [3.14, 6.28])
         self.assertEqual(args.arg_list_bool, [True, False])
-        self.assertEqual(args.arg_list_literal, ['H', False])
+        self.assertEqual(args.arg_list_literal, ["H", False])
         self.assertEqual(args.arg_list_str_empty, [])
 
-        self.assertEqual(args.arg_set, {'these', 'are', 'strings'})
-        self.assertEqual(args.arg_set_str, {'hello', 'how are you'})
+        self.assertEqual(args.arg_set, {"these", "are", "strings"})
+        self.assertEqual(args.arg_set_str, {"hello", "how are you"})
         self.assertEqual(args.arg_set_int, {10, -11})
         self.assertEqual(args.arg_set_float, {3.14, 6.28})
         self.assertEqual(args.arg_set_bool, {True, False})
-        self.assertEqual(args.arg_set_literal, {'H', False})
+        self.assertEqual(args.arg_set_literal, {"H", False})
         self.assertEqual(args.arg_set_str_empty, set())
 
-        self.assertEqual(args.arg_tuple, ('these', 'are', 'strings'))
-        self.assertEqual(args.arg_tuple_str, ('hello', 'how are you'))
+        self.assertEqual(args.arg_tuple, ("these", "are", "strings"))
+        self.assertEqual(args.arg_tuple_str, ("hello", "how are you"))
         self.assertEqual(args.arg_tuple_int, (10, -11))
         self.assertEqual(args.arg_tuple_float, (3.14, 6.28))
         self.assertEqual(args.arg_tuple_bool, (True, True, True, False))
-        self.assertEqual(args.arg_tuple_multi, (1.2, 1, 'hi', True, 1.3))
+        self.assertEqual(args.arg_tuple_multi, (1.2, 1, "hi", True, 1.3))
 
     def test_set_default_args(self) -> None:
-        arg_untyped = 'yes'
-        arg_str = 'goodbye'
-        arg_int = '2'
-        arg_float = '1e-2'
-        arg_literal = 'True'
-
-        arg_optional = 'yo'
-        arg_optional_str = 'hello'
-        arg_optional_int = '77'
-        arg_optional_float = '7.7'
-        arg_optional_bool = 'tru'
-        arg_optional_literal = '88.9'
-
-        arg_list = ['string', 'list']
-        arg_list_str = ['hi', 'there', 'how', 'are', 'you']
-        arg_list_int = ['1', '2', '3', '10', '-11']
-        arg_list_float = ['2.2', '-3.3', '2e20']
-        arg_list_bool = ['true', 'F']
+        arg_untyped = "yes"
+        arg_str = "goodbye"
+        arg_int = "2"
+        arg_float = "1e-2"
+        arg_literal = "True"
+
+        arg_optional = "yo"
+        arg_optional_str = "hello"
+        arg_optional_int = "77"
+        arg_optional_float = "7.7"
+        arg_optional_bool = "tru"
+        arg_optional_literal = "88.9"
+
+        arg_list = ["string", "list"]
+        arg_list_str = ["hi", "there", "how", "are", "you"]
+        arg_list_int = ["1", "2", "3", "10", "-11"]
+        arg_list_float = ["2.2", "-3.3", "2e20"]
+        arg_list_bool = ["true", "F"]
         arg_list_str_empty = []
-        arg_list_literal = ['H', '1']
+        arg_list_literal = ["H", "1"]
 
-        arg_set = ['hi', 'there']
-        arg_set_str = ['hi', 'hi', 'hi', 'how']
-        arg_set_int = ['1', '2', '2', '2', '3']
-        arg_set_float = ['1.23', '4.4', '1.23']
-        arg_set_bool = ['tru', 'fal']
+        arg_set = ["hi", "there"]
+        arg_set_str = ["hi", "hi", "hi", "how"]
+        arg_set_int = ["1", "2", "2", "2", "3"]
+        arg_set_float = ["1.23", "4.4", "1.23"]
+        arg_set_bool = ["tru", "fal"]
         arg_set_str_empty = []
-        arg_set_literal = ['False', '1.00784']
+        arg_set_literal = ["False", "1.00784"]
 
-        arg_tuple = ('hi', 'there')
-        arg_tuple_str = ('hi', 'hi', 'hi', 'how')
-        arg_tuple_int = ('1', '2', '2', '2', '3')
-        arg_tuple_float = ('1.23', '4.4', '1.23')
-        arg_tuple_bool = ('tru', 'fal')
-        arg_tuple_multi = ('1.2', '1', 'hi', 'T', '1.3')
-
-        args = IntegrationDefaultTap().parse_args([
-            '--arg_untyped', arg_untyped,
-            '--arg_str', arg_str,
-            '--arg_int', arg_int,
-            '--arg_float', arg_float,
-            '--arg_bool_true',
-            '--arg_bool_false',
-            '--arg_literal', arg_literal,
-
-            '--arg_optional', arg_optional,
-            '--arg_optional_str', arg_optional_str,
-            '--arg_optional_int', arg_optional_int,
-            '--arg_optional_float', arg_optional_float,
-            '--arg_optional_bool', arg_optional_bool,
-            '--arg_optional_literal', arg_optional_literal,
-
-            '--arg_list', *arg_list,
-            '--arg_list_str', *arg_list_str,
-            '--arg_list_int', *arg_list_int,
-            '--arg_list_float', *arg_list_float,
-            '--arg_list_bool', *arg_list_bool,
-            '--arg_list_str_empty', *arg_list_str_empty,
-            '--arg_list_literal', *arg_list_literal,
-            '--arg_set', *arg_set,
-            '--arg_set_str', *arg_set_str,
-            '--arg_set_int', *arg_set_int,
-            '--arg_set_float', *arg_set_float,
-            '--arg_set_bool', *arg_set_bool,
-            '--arg_set_str_empty', *arg_set_str_empty,
-            '--arg_set_literal', *arg_set_literal,
-
-            '--arg_tuple', *arg_tuple,
-            '--arg_tuple_str', *arg_tuple_str,
-            '--arg_tuple_int', *arg_tuple_int,
-            '--arg_tuple_float', *arg_tuple_float,
-            '--arg_tuple_bool', *arg_tuple_bool,
-            '--arg_tuple_multi', *arg_tuple_multi,
-        ])
+        arg_tuple = ("hi", "there")
+        arg_tuple_str = ("hi", "hi", "hi", "how")
+        arg_tuple_int = ("1", "2", "2", "2", "3")
+        arg_tuple_float = ("1.23", "4.4", "1.23")
+        arg_tuple_bool = ("tru", "fal")
+        arg_tuple_multi = ("1.2", "1", "hi", "T", "1.3")
+
+        args = IntegrationDefaultTap().parse_args(
+            [
+                "--arg_untyped",
+                arg_untyped,
+                "--arg_str",
+                arg_str,
+                "--arg_int",
+                arg_int,
+                "--arg_float",
+                arg_float,
+                "--arg_bool_true",
+                "--arg_bool_false",
+                "--arg_literal",
+                arg_literal,
+                "--arg_optional",
+                arg_optional,
+                "--arg_optional_str",
+                arg_optional_str,
+                "--arg_optional_int",
+                arg_optional_int,
+                "--arg_optional_float",
+                arg_optional_float,
+                "--arg_optional_bool",
+                arg_optional_bool,
+                "--arg_optional_literal",
+                arg_optional_literal,
+                "--arg_list",
+                *arg_list,
+                "--arg_list_str",
+                *arg_list_str,
+                "--arg_list_int",
+                *arg_list_int,
+                "--arg_list_float",
+                *arg_list_float,
+                "--arg_list_bool",
+                *arg_list_bool,
+                "--arg_list_str_empty",
+                *arg_list_str_empty,
+                "--arg_list_literal",
+                *arg_list_literal,
+                "--arg_set",
+                *arg_set,
+                "--arg_set_str",
+                *arg_set_str,
+                "--arg_set_int",
+                *arg_set_int,
+                "--arg_set_float",
+                *arg_set_float,
+                "--arg_set_bool",
+                *arg_set_bool,
+                "--arg_set_str_empty",
+                *arg_set_str_empty,
+                "--arg_set_literal",
+                *arg_set_literal,
+                "--arg_tuple",
+                *arg_tuple,
+                "--arg_tuple_str",
+                *arg_tuple_str,
+                "--arg_tuple_int",
+                *arg_tuple_int,
+                "--arg_tuple_float",
+                *arg_tuple_float,
+                "--arg_tuple_bool",
+                *arg_tuple_bool,
+                "--arg_tuple_multi",
+                *arg_tuple_multi,
+            ]
+        )
 
         arg_int = int(arg_int)
         arg_float = float(arg_float)
 
         arg_optional_int = float(arg_optional_int)
         arg_optional_float = float(arg_optional_float)
         arg_optional_bool = True
@@ -497,15 +558,15 @@
         arg_set_bool = {True, False}
         arg_set_str_empty = set()
         arg_set_literal = set(arg_set_literal)
 
         arg_tuple_int = tuple(int(arg) for arg in arg_tuple_int)
         arg_tuple_float = tuple(float(arg) for arg in arg_tuple_float)
         arg_tuple_bool = (True, False)
-        arg_tuple_multi = (1.2, 1, 'hi', True, 1.3)
+        arg_tuple_multi = (1.2, 1, "hi", True, 1.3)
 
         self.assertEqual(args.arg_untyped, arg_untyped)
         self.assertEqual(args.arg_str, arg_str)
         self.assertEqual(args.arg_int, arg_int)
         self.assertEqual(args.arg_float, arg_float)
 
         # Note: setting the bools as flags results in the opposite of their default
@@ -522,15 +583,15 @@
 
         self.assertEqual(args.arg_list, arg_list)
         self.assertEqual(args.arg_list_str, arg_list_str)
         self.assertEqual(args.arg_list_int, arg_list_int)
         self.assertEqual(args.arg_list_float, arg_list_float)
         self.assertEqual(args.arg_list_bool, arg_list_bool)
         self.assertEqual(args.arg_list_str_empty, arg_list_str_empty)
-        self.assertEqual(args.arg_list_literal, ['H', 1])
+        self.assertEqual(args.arg_list_literal, ["H", 1])
 
         self.assertEqual(args.arg_set, arg_set)
         self.assertEqual(args.arg_set_str, arg_set_str)
         self.assertEqual(args.arg_set_int, arg_set_int)
         self.assertEqual(args.arg_set_float, arg_set_float)
         self.assertEqual(args.arg_set_bool, arg_set_bool)
         self.assertEqual(args.arg_set_str_empty, arg_set_str_empty)
@@ -543,23 +604,23 @@
         self.assertEqual(args.arg_tuple_bool, arg_tuple_bool)
         self.assertEqual(args.arg_tuple_multi, arg_tuple_multi)
 
 
 class LiteralCrashTests(TestCase):
     def test_literal_crash(self) -> None:
         class LiteralCrashTap(Tap):
-            arg_lit: Literal['125', 'no, 3 sir']
+            arg_lit: Literal["125", "no, 3 sir"]
 
         # Suppress prints from SystemExit
         class DevNull:
             def write(self, msg):
                 pass
 
         with self.assertRaises(SystemExit):
-            LiteralCrashTap().parse_args(['--arg_lit', '123'])
+            LiteralCrashTap().parse_args(["--arg_lit", "123"])
 
 
 def convert_str_or_int(str_or_int: str) -> Union[str, int]:
     try:
         return int(str_or_int)
     except ValueError:
         return str_or_int
@@ -584,90 +645,101 @@
 
             return input_str
 
 
 # TODO: test crash if not specifying type function
 class UnionTypeTap(Tap):
     union_zero_required_arg: Union
-    union_zero_default_arg: Union = 'hi'
+    union_zero_default_arg: Union = "hi"
     union_one_required_arg: Union[str]
-    union_one_default_arg: Union[str] = 'there'
+    union_one_default_arg: Union[str] = "there"
     union_two_required_arg: Union[str, int]
     union_two_default_int_arg: Union[str, int] = 5
-    union_two_default_str_arg: Union[str, int] = 'year old'
+    union_two_default_str_arg: Union[str, int] = "year old"
     union_custom_required_arg: Union[Person, str]
     union_custom_required_flip_arg: Union[str, Person]
-    union_custom_default_arg: Union[Person, str] = Person('Jesse')
-    union_custom_default_flip_arg: Union[str, Person] = 'I want'
+    union_custom_default_arg: Union[Person, str] = Person("Jesse")
+    union_custom_default_flip_arg: Union[str, Person] = "I want"
     union_none_required_arg: Union[int, None]
     union_none_required_flip_arg: Union[None, int]
     union_many_required_arg: Union[int, float, Person, str]
     union_many_default_arg: Union[int, float, Person, str] = 3.14
 
     def configure(self) -> None:
-        self.add_argument('--union_two_required_arg', type=convert_str_or_int)
-        self.add_argument('--union_two_default_int_arg', type=convert_str_or_int)
-        self.add_argument('--union_two_default_str_arg', type=convert_str_or_int)
-        self.add_argument('--union_custom_required_arg', type=convert_person_or_str)
-        self.add_argument('--union_custom_required_flip_arg', type=convert_person_or_str)
-        self.add_argument('--union_custom_default_arg', type=convert_person_or_str)
-        self.add_argument('--union_custom_default_flip_arg', type=convert_person_or_str)
-        self.add_argument('--union_none_required_flip_arg', type=int)
-        self.add_argument('--union_many_required_arg', type=convert_many_types)
-        self.add_argument('--union_many_default_arg', type=convert_many_types)
+        self.add_argument("--union_two_required_arg", type=convert_str_or_int)
+        self.add_argument("--union_two_default_int_arg", type=convert_str_or_int)
+        self.add_argument("--union_two_default_str_arg", type=convert_str_or_int)
+        self.add_argument("--union_custom_required_arg", type=convert_person_or_str)
+        self.add_argument("--union_custom_required_flip_arg", type=convert_person_or_str)
+        self.add_argument("--union_custom_default_arg", type=convert_person_or_str)
+        self.add_argument("--union_custom_default_flip_arg", type=convert_person_or_str)
+        self.add_argument("--union_none_required_flip_arg", type=int)
+        self.add_argument("--union_many_required_arg", type=convert_many_types)
+        self.add_argument("--union_many_default_arg", type=convert_many_types)
 
 
 if sys.version_info >= (3, 10):
+
     class UnionType310Tap(Tap):
         union_two_required_arg: str | int
         union_two_default_int_arg: str | int = 10
-        union_two_default_str_arg: str | int = 'pieces of pie for'
+        union_two_default_str_arg: str | int = "pieces of pie for"
         union_custom_required_arg: Person | str
         union_custom_required_flip_arg: str | Person
-        union_custom_default_arg: Person | str = Person('Kyle')
-        union_custom_default_flip_arg: str | Person = 'making'
+        union_custom_default_arg: Person | str = Person("Kyle")
+        union_custom_default_flip_arg: str | Person = "making"
         union_none_required_arg: int | None
         union_none_required_flip_arg: None | int
         union_many_required_arg: int | float | Person | str
         union_many_default_arg: int | float | Person | str = 3.14 * 10 / 8
 
         def configure(self) -> None:
-            self.add_argument('--union_two_required_arg', type=convert_str_or_int)
-            self.add_argument('--union_two_default_int_arg', type=convert_str_or_int)
-            self.add_argument('--union_two_default_str_arg', type=convert_str_or_int)
-            self.add_argument('--union_custom_required_arg', type=convert_person_or_str)
-            self.add_argument('--union_custom_required_flip_arg', type=convert_person_or_str)
-            self.add_argument('--union_custom_default_arg', type=convert_person_or_str)
-            self.add_argument('--union_custom_default_flip_arg', type=convert_person_or_str)
-            self.add_argument('--union_none_required_flip_arg', type=int)
-            self.add_argument('--union_many_required_arg', type=convert_many_types)
-            self.add_argument('--union_many_default_arg', type=convert_many_types)
+            self.add_argument("--union_two_required_arg", type=convert_str_or_int)
+            self.add_argument("--union_two_default_int_arg", type=convert_str_or_int)
+            self.add_argument("--union_two_default_str_arg", type=convert_str_or_int)
+            self.add_argument("--union_custom_required_arg", type=convert_person_or_str)
+            self.add_argument("--union_custom_required_flip_arg", type=convert_person_or_str)
+            self.add_argument("--union_custom_default_arg", type=convert_person_or_str)
+            self.add_argument("--union_custom_default_flip_arg", type=convert_person_or_str)
+            self.add_argument("--union_none_required_flip_arg", type=int)
+            self.add_argument("--union_many_required_arg", type=convert_many_types)
+            self.add_argument("--union_many_default_arg", type=convert_many_types)
 
 
 class UnionTypeTests(TestCase):
     def test_union_types(self):
-        union_zero_required_arg = 'Kyle'
-        union_one_required_arg = 'ate'
-        union_two_required_arg = '2'
-        union_custom_required_arg = 'many'
-        union_custom_required_flip_arg = 'Jesse'
-        union_none_required_arg = '1'
-        union_none_required_flip_arg = '5'
-        union_many_required_arg = 'still hungry'
-
-        args = UnionTypeTap().parse_args([
-            '--union_zero_required_arg', union_zero_required_arg,
-            '--union_one_required_arg', union_one_required_arg,
-            '--union_two_required_arg', union_two_required_arg,
-            '--union_custom_required_arg', union_custom_required_arg,
-            '--union_custom_required_flip_arg', union_custom_required_flip_arg,
-            '--union_none_required_arg', union_none_required_arg,
-            '--union_none_required_flip_arg', union_none_required_flip_arg,
-            '--union_many_required_arg', union_many_required_arg
-        ])
+        union_zero_required_arg = "Kyle"
+        union_one_required_arg = "ate"
+        union_two_required_arg = "2"
+        union_custom_required_arg = "many"
+        union_custom_required_flip_arg = "Jesse"
+        union_none_required_arg = "1"
+        union_none_required_flip_arg = "5"
+        union_many_required_arg = "still hungry"
+
+        args = UnionTypeTap().parse_args(
+            [
+                "--union_zero_required_arg",
+                union_zero_required_arg,
+                "--union_one_required_arg",
+                union_one_required_arg,
+                "--union_two_required_arg",
+                union_two_required_arg,
+                "--union_custom_required_arg",
+                union_custom_required_arg,
+                "--union_custom_required_flip_arg",
+                union_custom_required_flip_arg,
+                "--union_none_required_arg",
+                union_none_required_arg,
+                "--union_none_required_flip_arg",
+                union_none_required_flip_arg,
+                "--union_many_required_arg",
+                union_many_required_arg,
+            ]
+        )
 
         union_two_required_arg = int(union_two_required_arg)
         union_custom_required_flip_arg = Person(union_custom_required_flip_arg)
         union_none_required_arg = int(union_none_required_arg)
         union_none_required_flip_arg = int(union_none_required_flip_arg)
 
         self.assertEqual(args.union_zero_required_arg, union_zero_required_arg)
@@ -691,29 +763,37 @@
             arg: Union[int, float]
 
         with self.assertRaises(ArgumentTypeError):
             UnionMissingTypeFunctionTap()
 
     @unittest.skipIf(sys.version_info < (3, 10), 'Union type operator "|" introduced in Python 3.10')
     def test_union_types_310(self):
-        union_two_required_arg = '1'  # int
-        union_custom_required_arg = 'hungry'  # str
-        union_custom_required_flip_arg = 'Loser'  # Person
-        union_none_required_arg = '8'  # int
-        union_none_required_flip_arg = '100'  # int
-        union_many_required_arg = '3.14'  # float
-
-        args = UnionType310Tap().parse_args([
-            '--union_two_required_arg', union_two_required_arg,
-            '--union_custom_required_arg', union_custom_required_arg,
-            '--union_custom_required_flip_arg', union_custom_required_flip_arg,
-            '--union_none_required_arg', union_none_required_arg,
-            '--union_none_required_flip_arg', union_none_required_flip_arg,
-            '--union_many_required_arg', union_many_required_arg
-        ])
+        union_two_required_arg = "1"  # int
+        union_custom_required_arg = "hungry"  # str
+        union_custom_required_flip_arg = "Loser"  # Person
+        union_none_required_arg = "8"  # int
+        union_none_required_flip_arg = "100"  # int
+        union_many_required_arg = "3.14"  # float
+
+        args = UnionType310Tap().parse_args(
+            [
+                "--union_two_required_arg",
+                union_two_required_arg,
+                "--union_custom_required_arg",
+                union_custom_required_arg,
+                "--union_custom_required_flip_arg",
+                union_custom_required_flip_arg,
+                "--union_none_required_arg",
+                union_none_required_arg,
+                "--union_none_required_flip_arg",
+                union_none_required_flip_arg,
+                "--union_many_required_arg",
+                union_many_required_arg,
+            ]
+        )
 
         union_two_required_arg = int(union_two_required_arg)
         union_custom_required_flip_arg = Person(union_custom_required_flip_arg)
         union_none_required_arg = int(union_none_required_arg)
         union_none_required_flip_arg = int(union_none_required_flip_arg)
         union_many_required_arg = float(union_many_required_arg)
 
@@ -738,317 +818,311 @@
             UnionMissingTypeFunctionTap()
 
 
 class AddArgumentTests(TestCase):
     def test_positional(self) -> None:
         class AddArgumentPositionalTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('arg_str')
+                self.add_argument("arg_str")
 
-        arg_str = 'positional'
+        arg_str = "positional"
         self.args = AddArgumentPositionalTap().parse_args([arg_str])
 
         self.assertEqual(self.args.arg_str, arg_str)
 
     def test_positional_ordering(self) -> None:
         class AddArgumentPositionalOrderingTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('arg_str')
-                self.add_argument('arg_int')
-                self.add_argument('arg_float')
-
-        arg_str = 'positional'
-        arg_int = '5'
-        arg_float = '1.1'
+                self.add_argument("arg_str")
+                self.add_argument("arg_int")
+                self.add_argument("arg_float")
+
+        arg_str = "positional"
+        arg_int = "5"
+        arg_float = "1.1"
         self.args = AddArgumentPositionalOrderingTap().parse_args([arg_str, arg_int, arg_float])
 
         arg_int = int(arg_int)
         arg_float = float(arg_float)
 
         self.assertEqual(self.args.arg_str, arg_str)
         self.assertEqual(self.args.arg_int, arg_int)
         self.assertEqual(self.args.arg_float, arg_float)
 
     def test_one_dash(self) -> None:
         class AddArgumentOneDashTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('-arg_str')
+                self.add_argument("-arg_str")
 
-        arg_str = 'one_dash'
-        self.args = AddArgumentOneDashTap().parse_args(['-arg_str', arg_str])
+        arg_str = "one_dash"
+        self.args = AddArgumentOneDashTap().parse_args(["-arg_str", arg_str])
 
         self.assertEqual(self.args.arg_str, arg_str)
 
     def test_two_dashes(self) -> None:
         class AddArgumentTwoDashesTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_str')
+                self.add_argument("--arg_str")
 
-        arg_str = 'two_dashes'
-        self.args = AddArgumentTwoDashesTap().parse_args(['--arg_str', arg_str])
+        arg_str = "two_dashes"
+        self.args = AddArgumentTwoDashesTap().parse_args(["--arg_str", arg_str])
 
         self.assertEqual(self.args.arg_str, arg_str)
 
     def test_one_and_two_dashes(self) -> None:
         class AddArgumentOneAndTwoDashesTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('-a', '--arg_str')
+                self.add_argument("-a", "--arg_str")
 
-        arg_str = 'one_or_two_dashes'
-        self.args = AddArgumentOneAndTwoDashesTap().parse_args(['-a', arg_str])
+        arg_str = "one_or_two_dashes"
+        self.args = AddArgumentOneAndTwoDashesTap().parse_args(["-a", arg_str])
 
         self.assertEqual(self.args.arg_str, arg_str)
 
-        self.args = AddArgumentOneAndTwoDashesTap().parse_args(['--arg_str', arg_str])
+        self.args = AddArgumentOneAndTwoDashesTap().parse_args(["--arg_str", arg_str])
 
         self.assertEqual(self.args.arg_str, arg_str)
 
     def test_not_class_variable(self) -> None:
         class AddArgumentNotClassVariableTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--non_class_arg')
+                self.add_argument("--non_class_arg")
 
-        arg_str = 'non_class_arg'
+        arg_str = "non_class_arg"
         self.tap = AddArgumentNotClassVariableTap()
-        self.assertTrue('non_class_arg' in self.tap._get_argument_names())
-        self.args = self.tap.parse_args(['--non_class_arg', arg_str])
+        self.assertTrue("non_class_arg" in self.tap._get_argument_names())
+        self.args = self.tap.parse_args(["--non_class_arg", arg_str])
 
         self.assertEqual(self.args.non_class_arg, arg_str)
 
     def test_complex_type(self) -> None:
         class AddArgumentComplexTypeTap(IntegrationDefaultTap):
-            arg_person: Person = Person('tap')
+            arg_person: Person = Person("tap")
             arg_person_required: Person
-            arg_person_untyped = Person('tap untyped')
+            arg_person_untyped = Person("tap untyped")
 
             def configure(self) -> None:
-                self.add_argument('--arg_person', type=Person)
-                self.add_argument('--arg_person_required', type=Person)
-                self.add_argument('--arg_person_untyped', type=Person)
+                self.add_argument("--arg_person", type=Person)
+                self.add_argument("--arg_person_required", type=Person)
+                self.add_argument("--arg_person_untyped", type=Person)
 
         arg_person_required = Person("hello, it's me")
 
-        args = AddArgumentComplexTypeTap().parse_args([
-            '--arg_person_required', arg_person_required.name,
-        ])
-        self.assertEqual(args.arg_person, Person('tap'))
+        args = AddArgumentComplexTypeTap().parse_args(["--arg_person_required", arg_person_required.name,])
+        self.assertEqual(args.arg_person, Person("tap"))
         self.assertEqual(args.arg_person_required, arg_person_required)
-        self.assertEqual(args.arg_person_untyped, Person('tap untyped'))
+        self.assertEqual(args.arg_person_untyped, Person("tap untyped"))
 
-        arg_person = Person('hi there')
-        arg_person_untyped = Person('heyyyy')
-        args = AddArgumentComplexTypeTap().parse_args([
-            '--arg_person', arg_person.name,
-            '--arg_person_required', arg_person_required.name,
-            '--arg_person_untyped', arg_person_untyped.name
-        ])
+        arg_person = Person("hi there")
+        arg_person_untyped = Person("heyyyy")
+        args = AddArgumentComplexTypeTap().parse_args(
+            [
+                "--arg_person",
+                arg_person.name,
+                "--arg_person_required",
+                arg_person_required.name,
+                "--arg_person_untyped",
+                arg_person_untyped.name,
+            ]
+        )
         self.assertEqual(args.arg_person, arg_person)
         self.assertEqual(args.arg_person_required, arg_person_required)
         self.assertEqual(args.arg_person_untyped, arg_person_untyped)
 
     def test_repeat_default(self) -> None:
         class AddArgumentRepeatDefaultTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_str', default=IntegrationDefaultTap.arg_str)
+                self.add_argument("--arg_str", default=IntegrationDefaultTap.arg_str)
 
         args = AddArgumentRepeatDefaultTap().parse_args([])
         self.assertEqual(args.arg_str, IntegrationDefaultTap.arg_str)
 
     def test_conflicting_default(self) -> None:
         class AddArgumentConflictingDefaultTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_str', default='yo dude')
+                self.add_argument("--arg_str", default="yo dude")
 
         args = AddArgumentConflictingDefaultTap().parse_args([])
-        self.assertEqual(args.arg_str, 'yo dude')
+        self.assertEqual(args.arg_str, "yo dude")
 
     # TODO: this
     def test_repeat_required(self) -> None:
         pass
 
     # TODO: this
     def test_conflicting_required(self) -> None:
         pass
 
     def test_repeat_type(self) -> None:
         class AddArgumentRepeatTypeTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_int', type=int)
+                self.add_argument("--arg_int", type=int)
 
         args = AddArgumentRepeatTypeTap().parse_args([])
         self.assertEqual(type(args.arg_int), int)
         self.assertEqual(args.arg_int, IntegrationDefaultTap.arg_int)
 
-        arg_int = '99'
-        args = AddArgumentRepeatTypeTap().parse_args(['--arg_int', arg_int])
+        arg_int = "99"
+        args = AddArgumentRepeatTypeTap().parse_args(["--arg_int", arg_int])
         arg_int = int(arg_int)
         self.assertEqual(type(args.arg_int), int)
         self.assertEqual(args.arg_int, arg_int)
 
     def test_conflicting_type(self) -> None:
         class AddArgumentConflictingTypeTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_int', type=str)
+                self.add_argument("--arg_int", type=str)
 
-        arg_int = 'yo dude'
-        args = AddArgumentConflictingTypeTap().parse_args(['--arg_int', arg_int])
+        arg_int = "yo dude"
+        args = AddArgumentConflictingTypeTap().parse_args(["--arg_int", arg_int])
         self.assertEqual(type(args.arg_int), str)
         self.assertEqual(args.arg_int, arg_int)
 
     # TODO
     def test_repeat_help(self) -> None:
         pass
 
     # TODO
     def test_conflicting_help(self) -> None:
         pass
 
     def test_repeat_nargs(self) -> None:
         class AddArgumentRepeatNargsTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_list_str', nargs='*')
+                self.add_argument("--arg_list_str", nargs="*")
 
-        arg_list_str = ['hi', 'there', 'person', '123']
-        args = AddArgumentRepeatNargsTap().parse_args(['--arg_list_str', *arg_list_str])
+        arg_list_str = ["hi", "there", "person", "123"]
+        args = AddArgumentRepeatNargsTap().parse_args(["--arg_list_str", *arg_list_str])
         self.assertEqual(args.arg_list_str, arg_list_str)
 
     def test_conflicting_nargs(self) -> None:
         class AddArgumentConflictingNargsTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_list_str', nargs=3)
+                self.add_argument("--arg_list_str", nargs=3)
 
-        arg_list_str = ['hi', 'there', 'person', '123']
+        arg_list_str = ["hi", "there", "person", "123"]
 
         with self.assertRaises(SystemExit):
-            AddArgumentConflictingNargsTap().parse_args(['--arg_list_str', *arg_list_str])
+            AddArgumentConflictingNargsTap().parse_args(["--arg_list_str", *arg_list_str])
 
     def test_repeat_action(self) -> None:
         class AddArgumentRepeatActionTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_bool_false', action='store_true', default=False)
+                self.add_argument("--arg_bool_false", action="store_true", default=False)
 
         args = AddArgumentRepeatActionTap().parse_args([])
         self.assertEqual(args.arg_bool_false, False)
 
-        args = AddArgumentRepeatActionTap().parse_args(['--arg_bool_false'])
+        args = AddArgumentRepeatActionTap().parse_args(["--arg_bool_false"])
         self.assertEqual(args.arg_bool_false, True)
 
     def test_conflicting_action(self) -> None:
         class AddArgumentConflictingActionTap(IntegrationDefaultTap):
             def configure(self) -> None:
-                self.add_argument('--arg_bool_false', action='store_false', default=True)
+                self.add_argument("--arg_bool_false", action="store_false", default=True)
 
         args = AddArgumentConflictingActionTap().parse_args([])
         self.assertEqual(args.arg_bool_false, True)
 
-        args = AddArgumentConflictingActionTap().parse_args(['--arg_bool_false'])
+        args = AddArgumentConflictingActionTap().parse_args(["--arg_bool_false"])
         self.assertEqual(args.arg_bool_false, False)
 
     def test_add_argument_post_initialization(self) -> None:
         args = IntegrationDefaultTap()
 
         with self.assertRaises(ValueError):
-            args.add_argument('--arg')
+            args.add_argument("--arg")
 
 
 class KnownTap(Tap):
     arg_int: int = 2
 
 
 class ParseKnownArgsTests(TestCase):
     arg_int = 3
     arg_float = 3.3
 
     def test_all_known(self) -> None:
-        args = KnownTap().parse_args([
-            '--arg_int', str(self.arg_int)
-        ], known_only=True)
+        args = KnownTap().parse_args(["--arg_int", str(self.arg_int)], known_only=True)
         self.assertEqual(args.arg_int, self.arg_int)
         self.assertEqual(args.extra_args, [])
 
     def test_some_known(self) -> None:
-        args = KnownTap().parse_args([
-            '--arg_int', str(self.arg_int),
-            '--arg_float', str(self.arg_float)
-        ], known_only=True)
+        args = KnownTap().parse_args(
+            ["--arg_int", str(self.arg_int), "--arg_float", str(self.arg_float)], known_only=True
+        )
         self.assertEqual(args.arg_int, self.arg_int)
-        self.assertEqual(args.extra_args, ['--arg_float', '3.3'])
+        self.assertEqual(args.extra_args, ["--arg_float", "3.3"])
 
     def test_none_known(self) -> None:
-        args = KnownTap().parse_args([
-            '--arg_float', str(self.arg_float)
-        ], known_only=True)
-        self.assertEqual(args.extra_args, ['--arg_float', '3.3'])
+        args = KnownTap().parse_args(["--arg_float", str(self.arg_float)], known_only=True)
+        self.assertEqual(args.extra_args, ["--arg_float", "3.3"])
 
 
 class DashedArgumentsTests(TestCase):
-
     def test_dashed_arguments(self) -> None:
         class DashedArgumentTap(Tap):
             arg: int = 10
             arg_u_ment: int = 10
             arg_you_mean_: int = 10
 
-        args = DashedArgumentTap(underscores_to_dashes=True).parse_args([
-            '--arg', '11',
-            '--arg-u-ment', '12',
-            '--arg-you-mean-', '13',
-        ])
+        args = DashedArgumentTap(underscores_to_dashes=True).parse_args(
+            ["--arg", "11", "--arg-u-ment", "12", "--arg-you-mean-", "13",]
+        )
         self.assertEqual(args.arg, 11)
         self.assertEqual(args.arg_u_ment, 12)
         self.assertEqual(args.arg_you_mean_, 13)
 
     def test_dashed_arguments_required_default(self) -> None:
-        class RequiredDashTap (Tap):
-            foo_arg: str = 'foo_arg'
+        class RequiredDashTap(Tap):
+            foo_arg: str = "foo_arg"
             foo_arg_2: Optional[int] = None
 
             def configure(self) -> None:
-                self.add_argument('-f', '--foo-arg')
-                self.add_argument('-f2', '--foo-arg-2')
+                self.add_argument("-f", "--foo-arg")
+                self.add_argument("-f2", "--foo-arg-2")
 
-        args = RequiredDashTap(underscores_to_dashes=True).parse_args(['-f', 'foo'])
-        self.assertEqual(args.foo_arg, 'foo')
+        args = RequiredDashTap(underscores_to_dashes=True).parse_args(["-f", "foo"])
+        self.assertEqual(args.foo_arg, "foo")
         self.assertEqual(args.foo_arg_2, None)
 
-        args = RequiredDashTap(underscores_to_dashes=True).parse_args(['-f2', '2'])
-        self.assertEqual(args.foo_arg, 'foo_arg')
+        args = RequiredDashTap(underscores_to_dashes=True).parse_args(["-f2", "2"])
+        self.assertEqual(args.foo_arg, "foo_arg")
         self.assertEqual(args.foo_arg_2, 2)
 
     def test_mismatch_dash_underscore_config_vs_annotations(self) -> None:
         class MismatchTap(Tap):
             arg_arg_arg: int
 
             def configure(self):
-                self.add_argument('--arg-arg_arg', '-arg', type=str)
+                self.add_argument("--arg-arg_arg", "-arg", type=str)
 
-        args = MismatchTap(underscores_to_dashes=True).parse_args('--arg-arg-arg aarg'.split())
-        self.assertEqual(args.arg_arg_arg, 'aarg')
+        args = MismatchTap(underscores_to_dashes=True).parse_args("--arg-arg-arg aarg".split())
+        self.assertEqual(args.arg_arg_arg, "aarg")
 
 
 class ParseExplicitBoolArgsTests(TestCase):
-
     def setUp(self) -> None:
         def test_bool_cases(cls):
-            for true in ['True', 'true', 'T', 't', '1']:
-                arg = cls(explicit_bool=True).parse_args(['--is_gpu', true])
+            for true in ["True", "true", "T", "t", "1"]:
+                arg = cls(explicit_bool=True).parse_args(["--is_gpu", true])
                 self.assertTrue(arg.is_gpu)
 
-            for false in ['False', 'false', 'F', 'f', '0']:
-                arg = cls(explicit_bool=True).parse_args(['--is_gpu', false])
+            for false in ["False", "false", "F", "f", "0"]:
+                arg = cls(explicit_bool=True).parse_args(["--is_gpu", false])
                 self.assertFalse(arg.is_gpu)
 
         self.test_bool_cases = test_bool_cases
 
     def test_explicit_bool(self):
         class ExplicitBoolTap(Tap):
             is_gpu: bool
 
         with self.assertRaises(SystemExit):
-            ExplicitBoolTap(explicit_bool=True).parse_args(['--is_gpu'])
+            ExplicitBoolTap(explicit_bool=True).parse_args(["--is_gpu"])
 
         with self.assertRaises(SystemExit):
             ExplicitBoolTap(explicit_bool=True).parse_args([])
 
         self.test_bool_cases(ExplicitBoolTap)
 
     def test_explicit_bool_false(self):
@@ -1073,267 +1147,308 @@
         args = SetNonSetTap().parse_args([])
         self.assertEqual(args.set_1, None)
         self.assertEqual(args.set_2, 3.7)
 
 
 class TupleTests(TestCase):
     def test_tuple_empty(self):
-        tup_arg = ('three', 'four', 'ten')
-        tup_default_arg = (1, 2, '5')
+        tup_arg = ("three", "four", "ten")
+        tup_default_arg = (1, 2, "5")
 
         class TupleEmptyTap(Tap):
             tup: Tuple
             tup_default: Tuple = tup_default_arg
 
-        args = TupleEmptyTap().parse_args([
-            '--tup', *tup_arg
-        ])
+        args = TupleEmptyTap().parse_args(["--tup", *tup_arg])
 
         self.assertEqual(args.tup, tup_arg)
         self.assertEqual(args.tup_default, tup_default_arg)
 
     def test_tuple_one(self):
         class TupleOneTap(Tap):
             tup_str: Tuple[str]
             tup_int: Tuple[int]
             tup_float: Tuple[float]
             tup_bool: Tuple[bool]
 
-        arg_str = 'hello'
+        arg_str = "hello"
         arg_int = 445
         arg_float = 7.9
-        arg_bool = 'tru'
+        arg_bool = "tru"
 
-        args = TupleOneTap().parse_args([
-            '--tup_str', arg_str,
-            '--tup_int', str(arg_int),
-            '--tup_float', str(arg_float),
-            '--tup_bool', arg_bool
-        ])
+        args = TupleOneTap().parse_args(
+            ["--tup_str", arg_str, "--tup_int", str(arg_int), "--tup_float", str(arg_float), "--tup_bool", arg_bool]
+        )
 
         self.assertEqual(args.tup_str, (arg_str,))
         self.assertEqual(args.tup_int, (arg_int,))
         self.assertEqual(args.tup_float, (arg_float,))
         self.assertEqual(args.tup_bool, (True,))
 
     def test_tuple_multi(self):
         class TupleMultiTap(Tap):
             tup: Tuple[str, int, float, bool, int, int, bool, bool, bool]
 
-        input_args = ('hi there', -1, -1.0, 'fAlS', 100, 1000, 'false', '0', '1')
-        true_args = ('hi there', -1, -1.0, False, 100, 1000, False, False, True)
+        input_args = ("hi there", -1, -1.0, "fAlS", 100, 1000, "false", "0", "1")
+        true_args = ("hi there", -1, -1.0, False, 100, 1000, False, False, True)
 
-        args = TupleMultiTap().parse_args([
-            '--tup', *[str(arg) for arg in input_args]
-        ])
+        args = TupleMultiTap().parse_args(["--tup", *[str(arg) for arg in input_args]])
 
         self.assertEqual(args.tup, true_args)
 
     def test_infinite_tuple(self):
         class UnboundedTupleTap(Tap):
             tup_str: Tuple[str, ...]
             tup_int: Tuple[int, ...]
             tup_float: Tuple[float, ...]
             tup_bool: Tuple[bool, ...]
 
-        arg_str = ('hi there', 'hello hi bye')
+        arg_str = ("hi there", "hello hi bye")
         arg_int = (2, 3, 4)
         arg_float = (-1.0, 0.0, 2.3, 4.7)
-        arg_bool = ('false', 'true', '0', '1', 'tru')
+        arg_bool = ("false", "true", "0", "1", "tru")
         arg_bool_true = (False, True, False, True, True)
 
-        args = UnboundedTupleTap().parse_args([
-            '--tup_str', *arg_str,
-            '--tup_int', *[str(arg) for arg in arg_int],
-            '--tup_float', *[str(arg) for arg in arg_float],
-            '--tup_bool', *arg_bool,
-        ])
+        args = UnboundedTupleTap().parse_args(
+            [
+                "--tup_str",
+                *arg_str,
+                "--tup_int",
+                *[str(arg) for arg in arg_int],
+                "--tup_float",
+                *[str(arg) for arg in arg_float],
+                "--tup_bool",
+                *arg_bool,
+            ]
+        )
 
         self.assertEqual(args.tup_str, arg_str)
         self.assertEqual(args.tup_int, arg_int)
         self.assertEqual(args.tup_float, arg_float)
         self.assertEqual(args.tup_bool, arg_bool_true)
 
     def test_tuple_class(self):
         class Dummy:
             def __init__(self, x):
                 self.x = x
 
-            def __eq__(self, other: 'Dummy'):
+            def __eq__(self, other: "Dummy"):
                 return isinstance(other, type(self)) and self.x == other.x
 
             def __str__(self):
-                return f'Dummy({self.x})'
+                return f"Dummy({self.x})"
 
         class TupleClassTap(Tap):
             tup: Tuple[int, str, Dummy, Dummy]
 
-        input_args = ('1', '2', '3', '4')
-        true_args = (1, '2', Dummy('3'), Dummy('4'))
+        input_args = ("1", "2", "3", "4")
+        true_args = (1, "2", Dummy("3"), Dummy("4"))
 
-        args = TupleClassTap().parse_args([
-            '--tup', *input_args
-        ])
+        args = TupleClassTap().parse_args(["--tup", *input_args])
 
         self.assertEqual(args.tup, true_args)
 
+    def test_tuple_literally_one(self):
+        class LiterallyOne(Tap):
+            tup: Tuple[Literal[1]]
+
+        input_args = ("1",)
+        true_args = (1,)
+
+        args = LiterallyOne().parse_args(["--tup", *input_args])
+
+        self.assertEqual(args.tup, true_args)
+
+        with self.assertRaises(SystemExit):
+            LiterallyOne().parse_args(["--tup", "2"])
+
+    def test_tuple_literally_two(self):
+        class LiterallyTwo(Tap):
+            tup: Tuple[Literal["two", 2], Literal[2, "too"]]
+
+        input_args = ("2", "too")
+        true_args = (2, "too")
+
+        args = LiterallyTwo().parse_args(["--tup", *input_args])
+
+        self.assertEqual(args.tup, true_args)
+
+        with self.assertRaises(SystemExit):
+            LiterallyTwo().parse_args(["--tup", "2"])
+
+        with self.assertRaises(SystemExit):
+            LiterallyTwo().parse_args(["--tup", "2", "3"])
+
+        with self.assertRaises(SystemExit):
+            LiterallyTwo().parse_args(["--tup", "too", "two"])
+
+    def test_tuple_literally_infinity(self):
+        class LiterallyInfinity(Tap):
+            tup: Tuple[Literal["infinity", "∞"], ...]
+
+        input_args = ("∞", "infinity", "∞")
+        true_args = input_args
+
+        args = LiterallyInfinity().parse_args(["--tup", *input_args])
+
+        self.assertEqual(args.tup, true_args)
+
+        with self.assertRaises(SystemExit):
+            LiterallyInfinity().parse_args(["--tup", "8"])
+
     def test_tuple_wrong_type_fails(self):
         class TupleTapTypeFails(Tap):
             tup: Tuple[int]
 
         with self.assertRaises(SystemExit):
-            TupleTapTypeFails().parse_args(['--tup', 'tomato'])
+            TupleTapTypeFails().parse_args(["--tup", "tomato"])
 
     def test_tuple_wrong_num_args_fails(self):
         class TupleTapArgsFails(Tap):
             tup: Tuple[int]
 
         with self.assertRaises(SystemExit):
-            TupleTapArgsFails().parse_args(['--tup', '1', '1'])
+            TupleTapArgsFails().parse_args(["--tup", "1", "1"])
 
     def test_tuple_wrong_order_fails(self):
         class TupleTapOrderFails(Tap):
             tup: Tuple[int, str]
 
         with self.assertRaises(SystemExit):
-            TupleTapOrderFails().parse_args(['--tup', 'seven', '1'])
+            TupleTapOrderFails().parse_args(["--tup", "seven", "1"])
 
     def test_empty_tuple_fails(self):
         class EmptyTupleTap(Tap):
             tup_str: Tuple[()]
 
-        arg_str = ('hi there', 'hello hi bye')
+        arg_str = ("hi there", "hello hi bye")
 
-        args = EmptyTupleTap().parse_args([
-            '--tup_str', *arg_str,
-        ])
+        args = EmptyTupleTap().parse_args(["--tup_str", *arg_str,])
 
         self.assertEqual(args.tup_str, arg_str)
 
     def test_tuple_non_tuple_default(self):
         class TupleNonTupleTap(Tap):
             tup_1: Tuple[int, str] = None
             tup_2: Tuple[str, int] = 3
 
         args = TupleNonTupleTap().parse_args([])
         self.assertEqual(args.tup_1, None)
         self.assertEqual(args.tup_2, 3)
 
 
 class TestAsDict(TestCase):
-
     def test_as_dict_simple(self):
         class SimpleTap(Tap):
             a: str
             b = 1
             c: bool = True
-            d: Tuple[str, ...] = ('hi', 'bob')
+            d: Tuple[str, ...] = ("hi", "bob")
             e: Optional[int] = None
             f: Set[int] = {1}
 
-        args = SimpleTap().parse_args(['--a', 'hi'])
-        as_dict_res = {'d': ('hi', 'bob'), 'b': 1, 'c': True, 'f': {1}, 'e': None, 'a': 'hi'}
+        args = SimpleTap().parse_args(["--a", "hi"])
+        as_dict_res = {"d": ("hi", "bob"), "b": 1, "c": True, "f": {1}, "e": None, "a": "hi"}
         self.assertEqual(args.as_dict(), as_dict_res)
 
     def test_as_dict_more_init_args(self):
         class InitArgsTap(Tap):
             a: str
             b = 1
 
             def __init__(self, g):
                 super(InitArgsTap, self).__init__()
                 self.g = g
 
-        args = InitArgsTap('GG').parse_args(['--a', 'hi'])
-        as_dict_res = {'b': 1, 'a': 'hi', 'g': 'GG'}
+        args = InitArgsTap("GG").parse_args(["--a", "hi"])
+        as_dict_res = {"b": 1, "a": "hi", "g": "GG"}
         self.assertEqual(args.as_dict(), as_dict_res)
 
     def test_as_dict_add_arguments(self):
         class AddArgumentsTap(Tap):
             a: str
             b = 1
 
             def configure(self):
-                self.add_argument('-arg_name', '--long_arg_name')
+                self.add_argument("-arg_name", "--long_arg_name")
 
-        args = AddArgumentsTap().parse_args(['--a', 'hi', '--long_arg_name', 'arg'])
+        args = AddArgumentsTap().parse_args(["--a", "hi", "--long_arg_name", "arg"])
 
-        as_dict_res = {'a': 'hi', 'b': 1, 'long_arg_name': 'arg'}
+        as_dict_res = {"a": "hi", "b": 1, "long_arg_name": "arg"}
         self.assertEqual(args.as_dict(), as_dict_res)
 
     def test_as_dict_manual_extra_args(self):
         class ManualExtraArgsTap(Tap):
             a: str
             b: int = 1
 
         args = ManualExtraArgsTap()
         args.c = 7
-        args = args.parse_args(['--a', 'hi'])
-        args.d = 'big'
+        args = args.parse_args(["--a", "hi"])
+        args.d = "big"
 
-        as_dict_res = {'a': 'hi', 'b': 1, 'c': 7, 'd': 'big'}
+        as_dict_res = {"a": "hi", "b": 1, "c": 7, "d": "big"}
         self.assertEqual(args.as_dict(), as_dict_res)
 
     def test_as_dict_property(self):
         class PropertyTap(Tap):
             a: str
             b: int = 1
 
             @property
             def pi(self):
                 return 3.14
 
         args = PropertyTap()
-        args = args.parse_args(['--a', 'hi'])
+        args = args.parse_args(["--a", "hi"])
 
-        as_dict_res = {'a': 'hi', 'b': 1, 'pi': 3.14}
+        as_dict_res = {"a": "hi", "b": 1, "pi": 3.14}
         self.assertEqual(args.as_dict(), as_dict_res)
 
     def test_as_dict_superclass_property(self):
         class SuperPropertyTap(Tap):
             a: str
 
             @property
             def pi(self):
                 return 3.14
 
         class SubPropertyTap(SuperPropertyTap):
             b: int = 1
 
         args = SubPropertyTap()
-        args = args.parse_args(['--a', 'hi'])
+        args = args.parse_args(["--a", "hi"])
 
-        as_dict_res = {'a': 'hi', 'b': 1, 'pi': 3.14}
+        as_dict_res = {"a": "hi", "b": 1, "pi": 3.14}
         self.assertEqual(args.as_dict(), as_dict_res)
 
 
 class TestFromDict(TestCase):
-
     def test_from_dict_simple(self):
         class SimpleFromDictTap(Tap):
             a: str
             d: Tuple[str, ...]
             b = 1
             c: bool = True
             e: Optional[int] = None
             f: Set[int] = {1}
 
-        args = SimpleFromDictTap().parse_args(['--a', 'hi', '--d', 'a', 'b', '--e', '7'])
+        args = SimpleFromDictTap().parse_args(["--a", "hi", "--d", "a", "b", "--e", "7"])
         d = args.as_dict()
 
         new_args = SimpleFromDictTap()
         new_args.from_dict(d)
 
         self.assertEqual(new_args.as_dict(), args.as_dict())
 
     def test_from_dict_returns_self(self):
         class FromDictReturnTap(Tap):
             a: str
 
-        args = FromDictReturnTap().parse_args(['--a', 'hi'])
+        args = FromDictReturnTap().parse_args(["--a", "hi"])
         d = args.as_dict()
 
         new_args = FromDictReturnTap().from_dict(d)
 
         self.assertEqual(new_args.as_dict(), args.as_dict())
 
     def test_from_dict_fails_without_required(self):
@@ -1341,89 +1456,88 @@
             a: str
             d: Tuple[str, ...]
             b = 1
             c: bool = True
             e: Optional[int] = None
             f: Set[int] = {1}
 
-        args = SimpleFromDictTap().parse_args(['--a', 'hi', '--d', 'a', 'b', '--e', '7'])
+        args = SimpleFromDictTap().parse_args(["--a", "hi", "--d", "a", "b", "--e", "7"])
         d = args.as_dict()
-        d.pop('a')
+        d.pop("a")
 
         new_args = SimpleFromDictTap()
 
         with self.assertRaises(ValueError):
             new_args.from_dict(d)
 
 
 class TestStoringTap(TestCase):
-
     def test_save_load_simple(self):
         class SimpleSaveLoadTap(Tap):
             a: str
             b = 1
             c: bool = True
 
-        args = SimpleSaveLoadTap().parse_args(['--a', 'hi'])
+        args = SimpleSaveLoadTap().parse_args(["--a", "hi"])
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'args.json')
+            fname = os.path.join(temp_dir, "args.json")
             args.save(fname)
             new_args = SimpleSaveLoadTap()
             new_args.load(fname)
 
-        output = {'a': 'hi', 'b': 1, 'c': True}
+        output = {"a": "hi", "b": 1, "c": True}
         self.assertEqual(output, new_args.as_dict())
 
     def test_save_load_return(self):
         class SaveLoadReturnTap(Tap):
             a: str
 
-        args = SaveLoadReturnTap().parse_args(['--a', 'hi'])
+        args = SaveLoadReturnTap().parse_args(["--a", "hi"])
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'args.json')
+            fname = os.path.join(temp_dir, "args.json")
             args.save(fname)
             new_args = SaveLoadReturnTap().load(fname)
 
-        output = {'a': 'hi'}
+        output = {"a": "hi"}
         self.assertEqual(output, new_args.as_dict())
 
     def test_save_load_complex(self):
         class ComplexSaveLoadTap(Tap):
             a: str
             d: Tuple[str, ...]
             b = 1
             c: bool = True
             e: Optional[int] = None
             f: Set[int] = {1}
-            g: Person = Person('tappy')
+            g: Person = Person("tappy")
 
             def configure(self) -> None:
-                self.add_argument('--g', type=Person)
+                self.add_argument("--g", type=Person)
 
-        args = ComplexSaveLoadTap().parse_args(['--a', 'hi', '--d', 'a', 'b', '--e', '7', '--g', 'tapper'])
+        args = ComplexSaveLoadTap().parse_args(["--a", "hi", "--d", "a", "b", "--e", "7", "--g", "tapper"])
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'args.json')
+            fname = os.path.join(temp_dir, "args.json")
             args.save(fname)
             new_args = ComplexSaveLoadTap()
             new_args.load(fname)
 
-        output = {'e': 7, 'f': {1}, 'd': ('a', 'b'), 'c': True, 'a': 'hi', 'b': 1, 'g': Person('tapper')}
+        output = {"e": 7, "f": {1}, "d": ("a", "b"), "c": True, "a": "hi", "b": 1, "g": Person("tapper")}
         self.assertEqual(output, new_args.as_dict())
 
     def test_save_load_property(self):
         class PropertySaveLoadTap(Tap):
-            a: str = 'hello'
+            a: str = "hello"
 
             def __init__(self):
                 super(PropertySaveLoadTap, self).__init__()
                 self._prop1 = 1
-                self._prop2 = 'hi'
+                self._prop2 = "hi"
 
             @property
             def prop1(self):
                 return self._prop1
 
             @property
             def prop2(self):
@@ -1431,61 +1545,60 @@
 
             @prop2.setter
             def prop2(self, prop2):
                 self._prop2 = prop2
 
             def process_args(self) -> None:
                 self._prop1 = 2
-                self.prop2 = 'bye'
+                self.prop2 = "bye"
 
         args = PropertySaveLoadTap().parse_args([])
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'args.json')
+            fname = os.path.join(temp_dir, "args.json")
             args.save(fname)
             new_args = PropertySaveLoadTap()
 
             with self.assertRaises(AttributeError):
                 new_args.load(fname)  # because trying to set unsettable prop1
 
             new_args.load(fname, skip_unsettable=True)
 
-        output = {'a': 'hello', 'prop1': 1, 'prop2': 'bye'}
+        output = {"a": "hello", "prop1": 1, "prop2": "bye"}
         self.assertEqual(output, new_args.as_dict())
 
 
 class TestDeepCopy(TestCase):
     def test_deep_copy(self):
         class DeepCopyTap(Tap):
             a: str
             d: Tuple[str, ...]
             b = 1
             c: bool = True
             e: Optional[int] = None
             f: Set[int] = {1}
-            g: Person = Person('tappy')
+            g: Person = Person("tappy")
 
             def configure(self) -> None:
-                self.add_argument('--g', type=Person)
+                self.add_argument("--g", type=Person)
 
             def __eq__(self, other):
                 return isinstance(other, DeepCopyTap) and self.as_dict() == other.as_dict()
 
-        args = DeepCopyTap().parse_args(['--a', 'hi', '--d', 'a', 'b', '--e', '7', '--g', 'tapper'])
+        args = DeepCopyTap().parse_args(["--a", "hi", "--d", "a", "b", "--e", "7", "--g", "tapper"])
 
         copied_args = deepcopy(args)
         self.assertEqual(args, copied_args)
 
         self.assertEqual(args.g, copied_args.g)
-        args.g.name = 'tap out'  # Ensure the deepcopy was recursive and deepcopied objects
+        args.g.name = "tap out"  # Ensure the deepcopy was recursive and deepcopied objects
         self.assertNotEqual(args.g, copied_args.g)
 
 
 class TestGetClassDict(TestCase):
-
     def test_get_class_dict(self):
         class GetClassDictTap(Tap):
             a: str
             b = 1
             d: Tuple[str, ...]
             c: bool = True
             e: Optional[int] = None
@@ -1500,40 +1613,39 @@
             def my_static_method(arg):
                 return arg
 
             @property
             def my_property(self):
                 return 1
 
-        args = GetClassDictTap().parse_args(['--a', 'hi', '--d', 'a', 'b', '--e', '7'])
-        result = {'b': 1, 'c': True, 'e': None, 'f': {1}}
+        args = GetClassDictTap().parse_args(["--a", "hi", "--d", "a", "b", "--e", "7"])
+        result = {"b": 1, "c": True, "e": None, "f": {1}}
         self.assertEqual(args._get_class_dict(), result)
 
 
 class TestPositionalArguments(TestCase):
-
     def test_underscores_to_dashes_does_not_modify_positional(self):
         class PositionalTap(Tap):
             under_score: int
 
             def configure(self):
-                self.add_argument('under_score')
+                self.add_argument("under_score")
 
-        args = PositionalTap(underscores_to_dashes=True).parse_args(['1'])
+        args = PositionalTap(underscores_to_dashes=True).parse_args(["1"])
 
         self.assertEqual(args.under_score, 1)
 
     def test_positional_maintains_types(self):
         class PositionalTap(Tap):
             a: int
 
             def configure(self) -> None:
-                self.add_argument('a')
+                self.add_argument("a")
 
-        args = PositionalTap().parse_args(['1'])
+        args = PositionalTap().parse_args(["1"])
 
         self.assertEqual(args.a, 1)
 
 
 class TestPickle(TestCase):
     def test_pickle(self):
         args = IntegrationDefaultTap().parse_args([])
@@ -1542,64 +1654,67 @@
         self.assertEqual(loaded_args.as_dict(), args.as_dict())
 
 
 class TestParserDescription(TestCase):
     def test_root_parser_description(self):
         class RootParser(Tap):
             """<Root Parser>"""
-            field: str = '1'
-        
+
+            field: str = "1"
+
         root_parser = RootParser()
         help_info = root_parser.format_help()
-        self.assertIn('<Root Parser>', help_info)
+        self.assertIn("<Root Parser>", help_info)
 
     def test_sub_parser_description(self):
-
         class SubParser(Tap):
             """<Sub Parser>"""
-            sub_field: str = '2'
-        
+
+            sub_field: str = "2"
+
         class RootParser(Tap):
             """<Root Parser>"""
-            field: str = '1'
+
+            field: str = "1"
 
             def configure(self):
-                self.add_subparsers(help='All sub parser')
-                self.add_subparser('sub', SubParser)
-        
+                self.add_subparsers(help="All sub parser")
+                self.add_subparser("sub", SubParser)
+
         help_desc = RootParser().format_help()
-        self.assertIn('<Sub Parser>', help_desc)
-        self.assertIn('<Root Parser>', help_desc)
+        self.assertIn("<Sub Parser>", help_desc)
+        self.assertIn("<Root Parser>", help_desc)
 
     def test_empty_docstring_should_be_empty(self):
         class NoDesc(Tap):
-            field: str = 'a'
+            field: str = "a"
 
         root_parser = NoDesc()
         help_info = root_parser.format_help()
-        help_flag = '[-h]'
+        help_flag = "[-h]"
         desc_start = help_info.index(help_flag) + len(help_flag)
-        desc_end = help_info.index('option')
-        desc = help_info[desc_start: desc_end].strip()
-        self.assertEqual(desc, '')
+        desc_end = help_info.index("option")
+        desc = help_info[desc_start:desc_end].strip()
+        self.assertEqual(desc, "")
 
     def test_manual_description_still_works(self):
         class NoDesc(Tap):
-            field: str = 'a'
+            field: str = "a"
 
-        expected_help_desc = 'I exist'
+        expected_help_desc = "I exist"
         help_desc = NoDesc(description=expected_help_desc).format_help()
         self.assertIn(expected_help_desc, help_desc)
 
     def test_manual_description_overwrites_docstring(self):
         class Desc(Tap):
             """I do not exist"""
-            field: str = 'a'
 
-        expected_help_desc = 'I exist'
+            field: str = "a"
+
+        expected_help_desc = "I exist"
         help_desc = Desc(description=expected_help_desc).format_help()
         self.assertIn(expected_help_desc, help_desc)
         self.assertNotIn("I do not exist", help_desc)
 
 
 class TestDefaultImmutability(TestCase):
     def test_default_immutability(self):
@@ -1617,18 +1732,18 @@
     def test_default_immutability_configure(self):
         holy_hand_grenada = [1, 2, 5]
 
         class DefaultImmutabilityTap(Tap):
             array: List[int]
 
             def configure(self) -> None:
-                self.add_argument('--array', default=holy_hand_grenada)
+                self.add_argument("--array", default=holy_hand_grenada)
 
         args = DefaultImmutabilityTap().parse_args([])
         self.assertEqual(args.array, holy_hand_grenada)
 
         holy_hand_grenada[2] = 3
         self.assertEqual(args.array, [1, 2, 5])
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typed-argument-parser-1.8.1/tests/test_load_config_files.py` & `typed-argument-parser-1.9.0/tests/test_load_config_files.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,140 +18,139 @@
 
 class LoadConfigFilesTests(TestCase):
     def test_file_does_not_exist(self) -> None:
         class EmptyTap(Tap):
             pass
 
         with self.assertRaises(FileNotFoundError):
-            EmptyTap(config_files=['nope']).parse_args([])
+            EmptyTap(config_files=["nope"]).parse_args([])
 
     def test_single_config(self) -> None:
         class SimpleTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
-                f.write('--a 1')
+            with open(fname, "w") as f:
+                f.write("--a 1")
 
             args = SimpleTap(config_files=[fname]).parse_args([])
 
         self.assertEqual(args.a, 1)
-        self.assertEqual(args.b, 'b')
+        self.assertEqual(args.b, "b")
 
     def test_single_config_overwriting(self) -> None:
         class SimpleOverwritingTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
-                f.write('--a 1 --b two')
+            with open(fname, "w") as f:
+                f.write("--a 1 --b two")
 
-            args = SimpleOverwritingTap(config_files=[fname]).parse_args('--a 2'.split())
+            args = SimpleOverwritingTap(config_files=[fname]).parse_args("--a 2".split())
 
         self.assertEqual(args.a, 2)
-        self.assertEqual(args.b, 'two')
+        self.assertEqual(args.b, "two")
 
     def test_single_config_known_only(self) -> None:
         class KnownOnlyTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
-                f.write('--a 1 --c seeNothing')
+            with open(fname, "w") as f:
+                f.write("--a 1 --c seeNothing")
 
             args = KnownOnlyTap(config_files=[fname]).parse_args([], known_only=True)
 
         self.assertEqual(args.a, 1)
-        self.assertEqual(args.b, 'b')
-        self.assertEqual(args.extra_args, ['--c', 'seeNothing'])
+        self.assertEqual(args.b, "b")
+        self.assertEqual(args.extra_args, ["--c", "seeNothing"])
 
     def test_single_config_required_still_required(self) -> None:
         class KnownOnlyTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir, self.assertRaises(SystemExit):
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
-                f.write('--b fore')
+            with open(fname, "w") as f:
+                f.write("--b fore")
 
             KnownOnlyTap(config_files=[fname]).parse_args([])
 
     def test_multiple_configs(self) -> None:
         class MultipleTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir:
-            fname1, fname2 = os.path.join(temp_dir, 'config1.txt'), os.path.join(temp_dir, 'config2.txt')
+            fname1, fname2 = os.path.join(temp_dir, "config1.txt"), os.path.join(temp_dir, "config2.txt")
 
-            with open(fname1, 'w') as f1, open(fname2, 'w') as f2:
-                f1.write('--b two')
-                f2.write('--a 1')
+            with open(fname1, "w") as f1, open(fname2, "w") as f2:
+                f1.write("--b two")
+                f2.write("--a 1")
 
             args = MultipleTap(config_files=[fname1, fname2]).parse_args([])
 
         self.assertEqual(args.a, 1)
-        self.assertEqual(args.b, 'two')
+        self.assertEqual(args.b, "two")
 
     def test_multiple_configs_overwriting(self) -> None:
         class MultipleOverwritingTap(Tap):
             a: int
-            b: str = 'b'
-            c: str = 'c'
+            b: str = "b"
+            c: str = "c"
 
         with TemporaryDirectory() as temp_dir:
-            fname1, fname2 = os.path.join(temp_dir, 'config1.txt'), os.path.join(temp_dir, 'config2.txt')
+            fname1, fname2 = os.path.join(temp_dir, "config1.txt"), os.path.join(temp_dir, "config2.txt")
 
-            with open(fname1, 'w') as f1, open(fname2, 'w') as f2:
-                f1.write('--a 1 --b two')
-                f2.write('--a 2 --c see')
+            with open(fname1, "w") as f1, open(fname2, "w") as f2:
+                f1.write("--a 1 --b two")
+                f2.write("--a 2 --c see")
 
-            args = MultipleOverwritingTap(config_files=[fname1, fname2]).parse_args('--b four'.split())
+            args = MultipleOverwritingTap(config_files=[fname1, fname2]).parse_args("--b four".split())
 
         self.assertEqual(args.a, 2)
-        self.assertEqual(args.b, 'four')
-        self.assertEqual(args.c, 'see')
+        self.assertEqual(args.b, "four")
+        self.assertEqual(args.c, "see")
 
     def test_junk_config(self) -> None:
         class JunkConfigTap(Tap):
             a: int
-            b: str = 'b'
+            b: str = "b"
 
         with TemporaryDirectory() as temp_dir, self.assertRaises(SystemExit):
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
-                f.write('is not a file that can reasonably be parsed')
+            with open(fname, "w") as f:
+                f.write("is not a file that can reasonably be parsed")
 
             JunkConfigTap(config_files=[fname]).parse_args([])
 
     def test_shlex_config(self) -> None:
         class ShlexConfigTap(Tap):
             a: int
             b: str
 
         with TemporaryDirectory() as temp_dir:
-            fname = os.path.join(temp_dir, 'config.txt')
+            fname = os.path.join(temp_dir, "config.txt")
 
-            with open(fname, 'w') as f:
+            with open(fname, "w") as f:
                 f.write('--a 21 # Important arg value\n\n# Multi-word quoted string\n--b "two three four"')
 
             args = ShlexConfigTap(config_files=[fname]).parse_args([])
 
         self.assertEqual(args.a, 21)
-        self.assertEqual(args.b, 'two three four')
+        self.assertEqual(args.b, "two three four")
 
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `typed-argument-parser-1.8.1/tests/test_subparser.py` & `typed-argument-parser-1.9.0/tests/test_subparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,211 +18,212 @@
 
 class TestSubparser(TestCase):
     def test_subparser_documentation_example(self):
         class SubparserA(Tap):
             bar: int  # bar help
 
         class SubparserB(Tap):
-            baz: Literal['X', 'Y', 'Z']  # baz help
+            baz: Literal["X", "Y", "Z"]  # baz help
 
         class Args(Tap):
             foo: bool = False  # foo help
 
             def configure(self):
-                self.add_subparsers(help='sub-command help')
-                self.add_subparser('a', SubparserA, help='a help')
-                self.add_subparser('b', SubparserB, help='b help')
+                self.add_subparsers(help="sub-command help")
+                self.add_subparser("a", SubparserA, help="a help")
+                self.add_subparser("b", SubparserB, help="b help")
 
         args = Args().parse_args([])
         self.assertFalse(args.foo)
-        self.assertFalse(hasattr(args, 'bar'))
-        self.assertFalse(hasattr(args, 'baz'))
+        self.assertFalse(hasattr(args, "bar"))
+        self.assertFalse(hasattr(args, "baz"))
 
-        args = Args().parse_args(['--foo'])
+        args = Args().parse_args(["--foo"])
         self.assertTrue(args.foo)
-        self.assertFalse(hasattr(args, 'bar'))
-        self.assertFalse(hasattr(args, 'baz'))
+        self.assertFalse(hasattr(args, "bar"))
+        self.assertFalse(hasattr(args, "baz"))
 
-        args = Args().parse_args('a --bar 1'.split())
+        args = Args().parse_args("a --bar 1".split())
         self.assertFalse(args.foo)
         self.assertEqual(args.bar, 1)
-        self.assertFalse(hasattr(args, 'baz'))
+        self.assertFalse(hasattr(args, "baz"))
 
-        args = Args().parse_args('--foo b --baz X'.split())
+        args = Args().parse_args("--foo b --baz X".split())
         self.assertTrue(args.foo)
-        self.assertFalse(hasattr(args, 'bar'))
-        self.assertEqual(args.baz, 'X')
+        self.assertFalse(hasattr(args, "bar"))
+        self.assertEqual(args.baz, "X")
 
         with self.assertRaises(SystemExit):
-            Args().parse_args('--baz X --foo b'.split())
+            Args().parse_args("--baz X --foo b".split())
 
         with self.assertRaises(SystemExit):
-            Args().parse_args('b --baz X --foo'.split())
+            Args().parse_args("b --baz X --foo".split())
 
         with self.assertRaises(SystemExit):
-            Args().parse_args('--foo a --bar 1 b --baz X'.split())
+            Args().parse_args("--foo a --bar 1 b --baz X".split())
 
     def test_name_collision(self):
         class SubparserA(Tap):
             a: int
 
         class Args(Tap):
             foo: bool = False
 
             def configure(self):
-                self.add_subparsers(help='sub-command help')
-                self.add_subparser('a', SubparserA, help='a help')
+                self.add_subparsers(help="sub-command help")
+                self.add_subparser("a", SubparserA, help="a help")
 
-        args = Args().parse_args('a --a 1'.split())
+        args = Args().parse_args("a --a 1".split())
         self.assertFalse(args.foo)
         self.assertEqual(args.a, 1)
 
     def test_name_overriding(self):
         class SubparserA(Tap):
             foo: int
 
         class Args(Tap):
             foo: bool = False
 
             def configure(self):
-                self.add_subparsers(help='sub-command help')
-                self.add_subparser('a', SubparserA)
+                self.add_subparsers(help="sub-command help")
+                self.add_subparser("a", SubparserA)
 
-        args = Args().parse_args(['--foo'])
+        args = Args().parse_args(["--foo"])
         self.assertTrue(args.foo)
 
-        args = Args().parse_args('a --foo 2'.split())
+        args = Args().parse_args("a --foo 2".split())
         self.assertEqual(args.foo, 2)
 
-        args = Args().parse_args('--foo a --foo 2'.split())
+        args = Args().parse_args("--foo a --foo 2".split())
         self.assertEqual(args.foo, 2)
 
     def test_add_subparser_twice(self):
         class SubparserA(Tap):
             bar: int
 
         class SubparserB(Tap):
             baz: int
 
         class Args(Tap):
             foo: bool = False
 
             def configure(self):
-                self.add_subparser('a', SubparserB)
-                self.add_subparser('a', SubparserA)
+                self.add_subparser("a", SubparserB)
+                self.add_subparser("a", SubparserA)
 
         if sys.version_info >= (3, 11):
             with self.assertRaises(ArgumentError):
                 Args().parse_args([])
         else:
-            args = Args().parse_args('a --bar 2'.split())
+            args = Args().parse_args("a --bar 2".split())
             self.assertFalse(args.foo)
             self.assertEqual(args.bar, 2)
-            self.assertFalse(hasattr(args, 'baz'))
+            self.assertFalse(hasattr(args, "baz"))
 
             with self.assertRaises(SystemExit):
-                Args().parse_args('a --baz 2'.split())
+                Args().parse_args("a --baz 2".split())
 
     def test_add_subparsers_twice(self):
         class SubparserA(Tap):
             a: int
 
         class Args(Tap):
             foo: bool = False
 
             def configure(self):
-                self.add_subparser('a', SubparserA)
-                self.add_subparsers(help='sub-command1 help')
-                self.add_subparsers(help='sub-command2 help')
+                self.add_subparser("a", SubparserA)
+                self.add_subparsers(help="sub-command1 help")
+                self.add_subparsers(help="sub-command2 help")
 
         with self.assertRaises(SystemExit):
             Args().parse_args([])
 
     def test_add_subparsers_with_add_argument(self):
         class SubparserA(Tap):
             for_sure: bool = False
 
         class Args(Tap):
             foo: bool = False
             bar: int = 1
 
             def configure(self):
-                self.add_argument('--bar', '-ib')
-                self.add_subparser('is_terrible', SubparserA)
-                self.add_argument('--foo', '-m')
+                self.add_argument("--bar", "-ib")
+                self.add_subparser("is_terrible", SubparserA)
+                self.add_argument("--foo", "-m")
 
-        args = Args().parse_args('-ib 0 -m is_terrible --for_sure'.split())
+        args = Args().parse_args("-ib 0 -m is_terrible --for_sure".split())
         self.assertTrue(args.foo)
         self.assertEqual(args.bar, 0)
         self.assertTrue(args.for_sure)
 
     def test_add_subsubparsers(self):
-
         class SubSubparserB(Tap):
             baz: bool = False
 
         class SubparserA(Tap):
             biz: bool = False
 
             def configure(self):
-                self.add_subparser('b', SubSubparserB)
+                self.add_subparser("b", SubSubparserB)
 
         class SubparserB(Tap):
             blaz: bool = False
 
         class Args(Tap):
             foo: bool = False
 
             def configure(self):
-                self.add_subparser('a', SubparserA)
-                self.add_subparser('b', SubparserB)
+                self.add_subparser("a", SubparserA)
+                self.add_subparser("b", SubparserB)
 
-        args = Args().parse_args('b --blaz'.split())
+        args = Args().parse_args("b --blaz".split())
         self.assertFalse(args.foo)
-        self.assertFalse(hasattr(args, 'baz'))
-        self.assertFalse(hasattr(args, 'biz'))
+        self.assertFalse(hasattr(args, "baz"))
+        self.assertFalse(hasattr(args, "biz"))
         self.assertTrue(args.blaz)
 
-        args = Args().parse_args('a --biz'.split())
+        args = Args().parse_args("a --biz".split())
         self.assertFalse(args.foo)
         self.assertTrue(args.biz)
-        self.assertFalse(hasattr(args, 'baz'))
-        self.assertFalse(hasattr(args, 'blaz'))
+        self.assertFalse(hasattr(args, "baz"))
+        self.assertFalse(hasattr(args, "blaz"))
 
-        args = Args().parse_args('a --biz b --baz'.split())
+        args = Args().parse_args("a --biz b --baz".split())
         self.assertFalse(args.foo)
         self.assertTrue(args.biz)
-        self.assertFalse(hasattr(args, 'blaz'))
+        self.assertFalse(hasattr(args, "blaz"))
         self.assertTrue(args.baz)
 
         with self.assertRaises(SystemExit):
-            Args().parse_args('b a'.split())
+            Args().parse_args("b a".split())
 
     def test_subparser_underscores_to_dashes(self):
         class AddProposal(Tap):
             proposal_id: int
 
         class Arguments(Tap):
             def configure(self) -> None:
                 self.add_subparsers(dest="subparser_name")
 
                 self.add_subparser(
-                    "add-proposal",
-                    AddProposal,
-                    help="Add a new proposal",
+                    "add-proposal", AddProposal, help="Add a new proposal",
                 )
 
-        args_underscores: Union[Arguments, AddProposal] = Arguments(underscores_to_dashes=False).parse_args('add-proposal --proposal_id 1'.split())
+        args_underscores: Union[Arguments, AddProposal] = Arguments(underscores_to_dashes=False).parse_args(
+            "add-proposal --proposal_id 1".split()
+        )
         self.assertEqual(args_underscores.proposal_id, 1)
 
-        args_dashes: Union[Arguments, AddProposal] = Arguments(underscores_to_dashes=True).parse_args('add-proposal --proposal-id 1'.split())
+        args_dashes: Union[Arguments, AddProposal] = Arguments(underscores_to_dashes=True).parse_args(
+            "add-proposal --proposal-id 1".split()
+        )
         self.assertEqual(args_dashes.proposal_id, 1)
 
         with self.assertRaises(SystemExit):
-            Arguments(underscores_to_dashes=False).parse_args('add-proposal --proposal-id 1'.split())
+            Arguments(underscores_to_dashes=False).parse_args("add-proposal --proposal-id 1".split())
 
         with self.assertRaises(SystemExit):
-            Arguments(underscores_to_dashes=True).parse_args('add-proposal --proposal_id 1'.split())
+            Arguments(underscores_to_dashes=True).parse_args("add-proposal --proposal_id 1".split())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `typed-argument-parser-1.8.1/tests/test_tapify.py` & `typed-argument-parser-1.9.0/tests/test_tapify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import contextlib
 from dataclasses import dataclass
 import io
 import sys
-from typing import List, Optional, Tuple, Any
+from typing import Dict, List, Optional, Tuple, Any
 import unittest
 from unittest import TestCase
 
 from tap import tapify
 
 
 # Suppress prints from SystemExit
@@ -19,24 +19,24 @@
 
 
 class Person:
     def __init__(self, name: str):
         self.name = name
 
     def __str__(self) -> str:
-        return f'Person({self.name})'
+        return f"Person({self.name})"
 
 
 class Problems:
     def __init__(self, problem_1: str, problem_2):
         self.problem_1 = problem_1
         self.problem_2 = problem_2
 
     def __str__(self) -> str:
-        return f'Problems({self.problem_1}, {self.problem_2})'
+        return f"Problems({self.problem_1}, {self.problem_2})"
 
 
 class TapifyTests(TestCase):
     def test_tapify_empty(self):
         def pie() -> float:
             return 3.14
 
@@ -50,19 +50,19 @@
                 return other == pie()
 
         for class_or_function in [pie, Pie, PieDataclass]:
             self.assertEqual(tapify(class_or_function, command_line_args=[]), 3.14)
 
     def test_tapify_simple_types(self):
         def concat(a: int, simple: str, test: float, of: float, types: bool) -> str:
-            return f'{a} {simple} {test} {of} {types}'
+            return f"{a} {simple} {test} {of} {types}"
 
         class Concat:
             def __init__(self, a: int, simple: str, test: float, of: float, types: bool):
-                self.kwargs = {'a': a, 'simple': simple, 'test': test, 'of': of, 'types': types}
+                self.kwargs = {"a": a, "simple": simple, "test": test, "of": of, "types": types}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             a: int
@@ -71,165 +71,189 @@
             of: float
             types: bool
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.a, self.simple, self.test, self.of, self.types)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--a', '1',
-                '--simple', 'simple',
-                '--test', '3.14',
-                '--of', '2.718',
-                '--types'
-            ])
+            output = tapify(
+                class_or_function,
+                command_line_args=["--a", "1", "--simple", "simple", "--test", "3.14", "--of", "2.718", "--types"],
+            )
 
-            self.assertEqual(output, '1 simple 3.14 2.718 True')
+            self.assertEqual(output, "1 simple 3.14 2.718 True")
 
     def test_tapify_simple_types_defaults(self):
-        def concat(a: int, simple: str, test: float, of: float = -.3, types: bool = False, wow: str = 'abc') -> str:
-            return f'{a} {simple} {test} {of} {types} {wow}'
+        def concat(a: int, simple: str, test: float, of: float = -0.3, types: bool = False, wow: str = "abc") -> str:
+            return f"{a} {simple} {test} {of} {types} {wow}"
 
         class Concat:
-            def __init__(self, a: int, simple: str, test: float, of: float = -.3, types: bool = False, wow: str = 'abc'):
-                self.kwargs = {'a': a, 'simple': simple, 'test': test, 'of': of, 'types': types, 'wow': wow}
+            def __init__(
+                self, a: int, simple: str, test: float, of: float = -0.3, types: bool = False, wow: str = "abc"
+            ):
+                self.kwargs = {"a": a, "simple": simple, "test": test, "of": of, "types": types, "wow": wow}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             a: int
             simple: str
             test: float
-            of: float = -.3
+            of: float = -0.3
             types: bool = False
-            wow: str = 'abc'
+            wow: str = "abc"
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.a, self.simple, self.test, self.of, self.types, self.wow)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--a', '1',
-                '--simple', 'simple',
-                '--test', '3.14',
-                '--types',
-                '--wow', 'wee'
-            ])
+            output = tapify(
+                class_or_function,
+                command_line_args=["--a", "1", "--simple", "simple", "--test", "3.14", "--types", "--wow", "wee"],
+            )
 
-            self.assertEqual(output, '1 simple 3.14 -0.3 True wee')
+            self.assertEqual(output, "1 simple 3.14 -0.3 True wee")
 
     def test_tapify_complex_types(self):
         def concat(complexity: List[str], requires: Tuple[int, int], intelligence: Person) -> str:
             return f'{" ".join(complexity)} {requires[0]} {requires[1]} {intelligence}'
 
         class Concat:
             def __init__(self, complexity: List[str], requires: Tuple[int, int], intelligence: Person):
-                self.kwargs = {'complexity': complexity, 'requires': requires, 'intelligence': intelligence}
+                self.kwargs = {"complexity": complexity, "requires": requires, "intelligence": intelligence}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             complexity: List[str]
             requires: Tuple[int, int]
             intelligence: Person
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.complexity, self.requires, self.intelligence)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--complexity', 'complex', 'things', 'require',
-                '--requires', '1', '0',
-                '--intelligence', 'jesse',
-            ])
-
-            self.assertEqual(output, 'complex things require 1 0 Person(jesse)')
-
-    @unittest.skipIf(sys.version_info < (3, 9),
-                     'Parameterized standard collections (e.g., list[int]) introduced in Python 3.9')
+            output = tapify(
+                class_or_function,
+                command_line_args=[
+                    "--complexity",
+                    "complex",
+                    "things",
+                    "require",
+                    "--requires",
+                    "1",
+                    "0",
+                    "--intelligence",
+                    "jesse",
+                ],
+            )
+
+            self.assertEqual(output, "complex things require 1 0 Person(jesse)")
+
+    @unittest.skipIf(
+        sys.version_info < (3, 9), "Parameterized standard collections (e.g., list[int]) introduced in Python 3.9"
+    )
     def test_tapify_complex_types_parameterized_standard(self):
         def concat(complexity: list[int], requires: tuple[int, int], intelligence: Person) -> str:
             return f'{" ".join(map(str, complexity))} {requires[0]} {requires[1]} {intelligence}'
 
         class Concat:
             def __init__(self, complexity: list[int], requires: tuple[int, int], intelligence: Person):
-                self.kwargs = {'complexity': complexity, 'requires': requires, 'intelligence': intelligence}
+                self.kwargs = {"complexity": complexity, "requires": requires, "intelligence": intelligence}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             complexity: list[int]
             requires: tuple[int, int]
             intelligence: Person
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.complexity, self.requires, self.intelligence)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--complexity', '1', '2', '3',
-                '--requires', '1', '0',
-                '--intelligence', 'jesse',
-            ])
+            output = tapify(
+                class_or_function,
+                command_line_args=["--complexity", "1", "2", "3", "--requires", "1", "0", "--intelligence", "jesse",],
+            )
 
-            self.assertEqual(output, '1 2 3 1 0 Person(jesse)')
+            self.assertEqual(output, "1 2 3 1 0 Person(jesse)")
 
     def test_tapify_complex_types_defaults(self):
-        def concat(complexity: List[str],
-                   requires: Tuple[int, int] = (2, 5),
-                   intelligence: Person = Person('kyle'),
-                   maybe: Optional[str] = None,
-                   possibly: Optional[str] = None) -> str:
+        def concat(
+            complexity: List[str],
+            requires: Tuple[int, int] = (2, 5),
+            intelligence: Person = Person("kyle"),
+            maybe: Optional[str] = None,
+            possibly: Optional[str] = None,
+        ) -> str:
             return f'{" ".join(complexity)} {requires[0]} {requires[1]} {intelligence} {maybe} {possibly}'
 
         class Concat:
-            def __init__(self, complexity: List[str],
-                         requires: Tuple[int, int] = (2, 5),
-                         intelligence: Person = Person('kyle'),
-                         maybe: Optional[str] = None,
-                         possibly: Optional[str] = None):
-                self.kwargs = {'complexity': complexity, 'requires': requires, 'intelligence': intelligence,
-                               'maybe': maybe, 'possibly': possibly}
+            def __init__(
+                self,
+                complexity: List[str],
+                requires: Tuple[int, int] = (2, 5),
+                intelligence: Person = Person("kyle"),
+                maybe: Optional[str] = None,
+                possibly: Optional[str] = None,
+            ):
+                self.kwargs = {
+                    "complexity": complexity,
+                    "requires": requires,
+                    "intelligence": intelligence,
+                    "maybe": maybe,
+                    "possibly": possibly,
+                }
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             complexity: List[str]
             requires: Tuple[int, int] = (2, 5)
-            intelligence: Person = Person('kyle')
+            intelligence: Person = Person("kyle")
             maybe: Optional[str] = None
             possibly: Optional[str] = None
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.complexity, self.requires, self.intelligence, self.maybe, self.possibly)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--complexity', 'complex', 'things', 'require',
-                '--requires', '-3', '12',
-                '--possibly', 'huh?'
-            ])
+            output = tapify(
+                class_or_function,
+                command_line_args=[
+                    "--complexity",
+                    "complex",
+                    "things",
+                    "require",
+                    "--requires",
+                    "-3",
+                    "12",
+                    "--possibly",
+                    "huh?",
+                ],
+            )
 
-            self.assertEqual(output, 'complex things require -3 12 Person(kyle) None huh?')
+            self.assertEqual(output, "complex things require -3 12 Person(kyle) None huh?")
 
     def test_tapify_too_few_args(self):
         def concat(so: int, many: float, args: str) -> str:
-            return f'{so} {many} {args}'
+            return f"{so} {many} {args}"
 
         class Concat:
             def __init__(self, so: int, many: float, args: str):
-                self.kwargs = {'so': so, 'many': many, 'args': args}
+                self.kwargs = {"so": so, "many": many, "args": args}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             so: int
@@ -237,140 +261,138 @@
             args: str
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.so, self.many, self.args)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
             with self.assertRaises(SystemExit):
-                tapify(class_or_function, command_line_args=[
-                    '--so', '23',
-                    '--many', '9.3'
-                ])
+                tapify(class_or_function, command_line_args=["--so", "23", "--many", "9.3"])
 
     def test_tapify_too_many_args(self):
         def concat(so: int, few: float) -> str:
-            return f'{so} {few}'
+            return f"{so} {few}"
 
         class Concat:
             def __init__(self, so: int, few: float):
-                self.kwargs = {'so': so, 'few': few}
+                self.kwargs = {"so": so, "few": few}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             so: int
             few: float
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.so, self.few)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
             with self.assertRaises(SystemExit):
-                tapify(class_or_function, command_line_args=[
-                    '--so', '23',
-                    '--few', '9.3',
-                    '--args', 'wow'
-                ])
+                tapify(class_or_function, command_line_args=["--so", "23", "--few", "9.3", "--args", "wow"])
 
     def test_tapify_too_many_args_known_only(self):
         def concat(so: int, few: float) -> str:
-            return f'{so} {few}'
+            return f"{so} {few}"
 
         class Concat:
             def __init__(self, so: int, few: float):
-                self.kwargs = {'so': so, 'few': few}
+                self.kwargs = {"so": so, "few": few}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             so: int
             few: float
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.so, self.few)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--so', '23',
-                '--few', '9.3',
-                '--args', 'wow'
-            ], known_only=True)
+            output = tapify(
+                class_or_function, command_line_args=["--so", "23", "--few", "9.3", "--args", "wow"], known_only=True
+            )
 
-            self.assertEqual(output, '23 9.3')
+            self.assertEqual(output, "23 9.3")
 
     def test_tapify_kwargs(self):
-        def concat(i: int, like: float, k: int, w: str = 'w', args: str = 'argy', always: bool = False) -> str:
-            return f'{i} {like} {k} {w} {args} {always}'
+        def concat(i: int, like: float, k: int, w: str = "w", args: str = "argy", always: bool = False) -> str:
+            return f"{i} {like} {k} {w} {args} {always}"
 
         class Concat:
-            def __init__(self, i: int, like: float, k: int, w: str = 'w', args: str = 'argy', always: bool = False):
-                self.kwargs = {'i': i, 'like': like, 'k': k, 'w': w, 'args': args, 'always': always}
+            def __init__(self, i: int, like: float, k: int, w: str = "w", args: str = "argy", always: bool = False):
+                self.kwargs = {"i": i, "like": like, "k": k, "w": w, "args": args, "always": always}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             i: int
             like: float
             k: int
-            w: str = 'w'
-            args: str = 'argy'
+            w: str = "w"
+            args: str = "argy"
             always: bool = False
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.i, self.like, self.k, self.w, self.args, self.always)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--i', '23',
-                '--args', 'wow',
-                '--like', '3.03',
-            ], known_only=True, w='hello', k=5, like=3.4, extra='arg')
+            output = tapify(
+                class_or_function,
+                command_line_args=["--i", "23", "--args", "wow", "--like", "3.03",],
+                known_only=True,
+                w="hello",
+                k=5,
+                like=3.4,
+                extra="arg",
+            )
 
-            self.assertEqual(output, '23 3.03 5 hello wow False')
+            self.assertEqual(output, "23 3.03 5 hello wow False")
 
     def test_tapify_kwargs_extra(self):
-        def concat(i: int, like: float, k: int, w: str = 'w', args: str = 'argy', always: bool = False) -> str:
-            return f'{i} {like} {k} {w} {args} {always}'
+        def concat(i: int, like: float, k: int, w: str = "w", args: str = "argy", always: bool = False) -> str:
+            return f"{i} {like} {k} {w} {args} {always}"
 
         class Concat:
-            def __init__(self, i: int, like: float, k: int, w: str = 'w', args: str = 'argy', always: bool = False):
-                self.kwargs = {'i': i, 'like': like, 'k': k, 'w': w, 'args': args, 'always': always}
+            def __init__(self, i: int, like: float, k: int, w: str = "w", args: str = "argy", always: bool = False):
+                self.kwargs = {"i": i, "like": like, "k": k, "w": w, "args": args, "always": always}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             i: int
             like: float
             k: int
-            w: str = 'w'
-            args: str = 'argy'
+            w: str = "w"
+            args: str = "argy"
             always: bool = False
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.i, self.like, self.k, self.w, self.args, self.always)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
             with self.assertRaises(ValueError):
-                tapify(class_or_function, command_line_args=[
-                    '--i', '23',
-                    '--args', 'wow',
-                    '--like', '3.03',
-                ], w='hello', k=5, like=3.4, mis='direction')
+                tapify(
+                    class_or_function,
+                    command_line_args=["--i", "23", "--args", "wow", "--like", "3.03",],
+                    w="hello",
+                    k=5,
+                    like=3.4,
+                    mis="direction",
+                )
 
     def test_tapify_unsupported_type(self):
         def concat(problems: Problems) -> str:
-            return f'{problems}'
+            return f"{problems}"
 
         class Concat:
             def __init__(self, problems: Problems):
                 self.problems = problems
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.problems)
@@ -379,73 +401,85 @@
         class ConcatDataclass:
             problems: Problems
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.problems)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[], problems=Problems('oh', 'no!'))
+            output = tapify(class_or_function, command_line_args=[], problems=Problems("oh", "no!"))
 
-            self.assertEqual(output, 'Problems(oh, no!)')
+            self.assertEqual(output, "Problems(oh, no!)")
 
             with self.assertRaises(SystemExit):
-                tapify(class_or_function, command_line_args=['--problems', '1', '2'])
+                tapify(class_or_function, command_line_args=["--problems", "1", "2"])
 
     def test_tapify_untyped(self):
-        def concat(untyped_1, typed_1: int,
-                   untyped_2=5, typed_2: str = 'now',
-                   untyped_3='hi', typed_3: bool = False) -> str:
-            return f'{untyped_1} {typed_1} {untyped_2} {typed_2} {untyped_3} {typed_3}'
-
-        class Concat:
-            def __init__(self, untyped_1, typed_1: int,
-                         untyped_2=5, typed_2: str = 'now',
-                         untyped_3='hi', typed_3: bool = False):
-                self.kwargs = {'untyped_1': untyped_1, 'typed_1': typed_1,
-                               'untyped_2': untyped_2, 'typed_2': typed_2,
-                               'untyped_3': untyped_3, 'typed_3': typed_3}
+        def concat(
+            untyped_1, typed_1: int, untyped_2=5, typed_2: str = "now", untyped_3="hi", typed_3: bool = False
+        ) -> str:
+            return f"{untyped_1} {typed_1} {untyped_2} {typed_2} {untyped_3} {typed_3}"
+
+        class Concat:
+            def __init__(
+                self, untyped_1, typed_1: int, untyped_2=5, typed_2: str = "now", untyped_3="hi", typed_3: bool = False
+            ):
+                self.kwargs = {
+                    "untyped_1": untyped_1,
+                    "typed_1": typed_1,
+                    "untyped_2": untyped_2,
+                    "typed_2": typed_2,
+                    "untyped_3": untyped_3,
+                    "typed_3": typed_3,
+                }
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             untyped_1: Any
             typed_1: int
             untyped_2: Any = 5
-            typed_2: str = 'now'
-            untyped_3: Any = 'hi'
+            typed_2: str = "now"
+            untyped_3: Any = "hi"
             typed_3: bool = False
 
             def __eq__(self, other: str) -> bool:
-                return other == concat(self.untyped_1, self.typed_1,
-                                       self.untyped_2, self.typed_2,
-                                       self.untyped_3, self.typed_3)
+                return other == concat(
+                    self.untyped_1, self.typed_1, self.untyped_2, self.typed_2, self.untyped_3, self.typed_3
+                )
+
+        for class_or_function in [concat, Concat, ConcatDataclass]:
+            output = tapify(
+                class_or_function,
+                command_line_args=[
+                    "--untyped_1",
+                    "why not type?",
+                    "--typed_1",
+                    "1",
+                    "--typed_2",
+                    "typing is great!",
+                    "--untyped_3",
+                    "bye",
+                ],
+            )
 
-        for class_or_function in [concat, Concat, ConcatDataclass]:
-            output = tapify(class_or_function, command_line_args=[
-                '--untyped_1', 'why not type?',
-                '--typed_1', '1',
-                '--typed_2', 'typing is great!',
-                '--untyped_3', 'bye'
-            ])
-
-            self.assertEqual(output, 'why not type? 1 5 typing is great! bye False')
+            self.assertEqual(output, "why not type? 1 5 typing is great! bye False")
 
     def test_double_tapify(self):
         def concat(a: int, b: int, c: int) -> str:
             """Concatenate three numbers."""
-            return f'{a} {b} {c}'
+            return f"{a} {b} {c}"
 
         class Concat:
             """Concatenate three numbers."""
 
             def __init__(self, a: int, b: int, c: int):
                 """Concatenate three numbers."""
-                self.kwargs = {'a': a, 'b': b, 'c': c}
+                self.kwargs = {"a": a, "b": b, "c": c}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             """Concatenate three numbers."""
@@ -454,83 +488,131 @@
             b: int
             c: int
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.a, self.b, self.c)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
-            output_1 = tapify(class_or_function, command_line_args=['--a', '1', '--b', '2', '--c', '3'])
-            output_2 = tapify(class_or_function, command_line_args=['--a', '4', '--b', '5', '--c', '6'])
+            output_1 = tapify(class_or_function, command_line_args=["--a", "1", "--b", "2", "--c", "3"])
+            output_2 = tapify(class_or_function, command_line_args=["--a", "4", "--b", "5", "--c", "6"])
 
-            self.assertEqual(output_1, '1 2 3')
-            self.assertEqual(output_2, '4 5 6')
+            self.assertEqual(output_1, "1 2 3")
+            self.assertEqual(output_2, "4 5 6")
 
     def test_tapify_args_kwargs(self):
         def concat(a: int, *args, b: int, **kwargs) -> str:
-            return f'{a} {args} {b} {kwargs}'
+            return f"{a} {args} {b} {kwargs}"
 
         class Concat:
             def __init__(self, a: int, *args, b: int, **kwargs):
                 self.a = a
                 self.args = args
                 self.b = b
                 self.kwargs = kwargs
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(a=self.a, *self.args, b=self.b, **self.kwargs)
 
         for class_or_function in [concat, Concat]:
             with self.assertRaises(SystemExit):
-                tapify(class_or_function, command_line_args=['--a', '1', '--b', '2'])
+                tapify(class_or_function, command_line_args=["--a", "1", "--b", "2"])
 
     def test_tapify_help(self):
         def concat(a: int, b: int, c: int) -> str:
             """Concatenate three numbers.
 
             :param a: The first number.
             :param b: The second number.
             :param c: The third number.
             """
-            return f'{a} {b} {c}'
+            return f"{a} {b} {c}"
 
         class Concat:
             def __init__(self, a: int, b: int, c: int):
                 """Concatenate three numbers.
 
                 :param a: The first number.
                 :param b: The second number.
                 :param c: The third number.
                 """
-                self.kwargs = {'a': a, 'b': b, 'c': c}
+                self.kwargs = {"a": a, "b": b, "c": c}
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(**self.kwargs)
 
         @dataclass
         class ConcatDataclass:
             """Concatenate three numbers.
 
             :param a: The first number.
             :param b: The second number.
             :param c: The third number.
             """
+
             a: int
             b: int
             c: int
 
             def __eq__(self, other: str) -> bool:
                 return other == concat(self.a, self.b, self.c)
 
         for class_or_function in [concat, Concat, ConcatDataclass]:
             f = io.StringIO()
             with contextlib.redirect_stdout(f):
                 with self.assertRaises(SystemExit):
-                    tapify(class_or_function, command_line_args=['-h'])
+                    tapify(class_or_function, command_line_args=["-h"])
+
+            self.assertIn("Concatenate three numbers.", f.getvalue())
+            self.assertIn("--a A       (int, required) The first number.", f.getvalue())
+            self.assertIn("--b B       (int, required) The second number.", f.getvalue())
+            self.assertIn("--c C       (int, required) The third number.", f.getvalue())
+
+
+class TestTapifyKwargs(unittest.TestCase):
+    def setUp(self) -> None:
+        def concat(a: int, b: int = 2, **kwargs) -> str:
+            """Concatenate three numbers.
+
+            :param a: The first number.
+            :param b: The second number.
+            """
+            return f'{a}_{b}_{"-".join(f"{k}={v}" for k, v in kwargs.items())}'
+
+        self.concat_function = concat
+
+        class Concat:
+            def __init__(self, a: int, b: int = 2, **kwargs: Dict[str, str]):
+                """Concatenate three numbers.
+
+                :param a: The first number.
+                :param b: The second number.
+                """
+                self.a = a
+                self.b = b
+                self.kwargs = kwargs
+
+            def __eq__(self, other: str) -> bool:
+                return other == concat(self.a, self.b, **self.kwargs)
+
+        self.concat_class = Concat
+
+    def test_tapify_empty_kwargs(self) -> None:
+        for class_or_function in [self.concat_function, self.concat_class]:
+            output = tapify(class_or_function, command_line_args=["--a", "1"])
+
+            self.assertEqual(output, "1_2_")
+
+    def test_tapify_has_kwargs(self) -> None:
+        for class_or_function in [self.concat_function, self.concat_class]:
+            output = tapify(class_or_function, command_line_args=["--a", "1", "--c", "3", "--d", "4"])
+
+            self.assertEqual(output, "1_2_c=3-d=4")
+
+    def test_tapify_has_kwargs_replace_default(self) -> None:
+        for class_or_function in [self.concat_function, self.concat_class]:
+            output = tapify(class_or_function, command_line_args=["--a", "1", "--c", "3", "--b", "5", "--d", "4"])
 
-            self.assertIn('Concatenate three numbers.', f.getvalue())
-            self.assertIn('--a A       (int, required) The first number.', f.getvalue())
-            self.assertIn('--b B       (int, required) The second number.', f.getvalue())
-            self.assertIn('--c C       (int, required) The third number.', f.getvalue())
+            self.assertEqual(output, "1_5_c=3-d=4")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `typed-argument-parser-1.8.1/tests/test_utils.py` & `typed-argument-parser-1.9.0/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from argparse import ArgumentTypeError
-from collections import OrderedDict
 import json
 import os
 import subprocess
 from tempfile import TemporaryDirectory
 from typing import Any, Callable, List, Literal, Dict, Set, Tuple, Union
 import unittest
 from unittest import TestCase
@@ -24,20 +23,20 @@
 
 
 class GitTests(TestCase):
     def setUp(self) -> None:
         self.temp_dir = TemporaryDirectory()
         self.prev_dir = os.getcwd()
         os.chdir(self.temp_dir.name)
-        subprocess.check_output(['git', 'init'])
-        self.url = 'https://github.com/test_account/test_repo'
-        subprocess.check_output(['git', 'remote', 'add', 'origin', f'{self.url}.git'])
-        subprocess.check_output(['touch', 'README.md'])
-        subprocess.check_output(['git', 'add', 'README.md'])
-        subprocess.check_output(['git', 'commit', '-m', 'Initial commit'])
+        subprocess.check_output(["git", "init"])
+        self.url = "https://github.com/test_account/test_repo"
+        subprocess.check_output(["git", "remote", "add", "origin", f"{self.url}.git"])
+        subprocess.check_output(["touch", "README.md"])
+        subprocess.check_output(["git", "add", "README.md"])
+        subprocess.check_output(["git", "commit", "-m", "Initial commit"])
         self.git_info = GitInfo(repo_path=self.temp_dir.name)
 
     def tearDown(self) -> None:
         os.chdir(self.prev_dir)
 
         # Add permissions to temporary directory to enable cleanup in Windows
         for root, dirs, files in os.walk(self.temp_dir.name):
@@ -55,478 +54,501 @@
             self.git_info.repo_path = temp_dir_no_git
             self.assertFalse(self.git_info.has_git())
             self.git_info.repo_path = self.temp_dir.name
             os.chdir(self.temp_dir.name)
 
     def test_get_git_root(self) -> None:
         # Ideally should be self.temp_dir.name == get_git_root() but the OS may add a prefix like /private
-        self.assertTrue(self.git_info.get_git_root().endswith(self.temp_dir.name.replace('\\', '/')))
+        self.assertTrue(self.git_info.get_git_root().endswith(self.temp_dir.name.replace("\\", "/")))
 
     def test_get_git_root_subdir(self) -> None:
-        subdir = os.path.join(self.temp_dir.name, 'subdir')
+        subdir = os.path.join(self.temp_dir.name, "subdir")
         os.makedirs(subdir)
         os.chdir(subdir)
 
         # Ideally should be self.temp_dir.name == get_git_root() but the OS may add a prefix like /private
-        self.assertTrue(self.git_info.get_git_root().endswith(self.temp_dir.name.replace('\\', '/')))
+        self.assertTrue(self.git_info.get_git_root().endswith(self.temp_dir.name.replace("\\", "/")))
 
         os.chdir(self.temp_dir.name)
 
     def test_get_git_url_https(self) -> None:
         self.assertEqual(self.git_info.get_git_url(commit_hash=False), self.url)
 
     def test_get_git_url_https_hash(self) -> None:
-        url = f'{self.url}/tree/'
-        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[:len(url)], url)
+        url = f"{self.url}/tree/"
+        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[: len(url)], url)
 
     def test_get_git_url_ssh(self) -> None:
-        subprocess.run(['git', 'remote', 'set-url', 'origin', 'git@github.com:test_account/test_repo.git'])
+        subprocess.run(["git", "remote", "set-url", "origin", "git@github.com:test_account/test_repo.git"])
         self.assertEqual(self.git_info.get_git_url(commit_hash=False), self.url)
 
     def test_get_git_url_ssh_hash(self) -> None:
-        subprocess.run(['git', 'remote', 'set-url', 'origin', 'git@github.com:test_account/test_repo.git'])
-        url = f'{self.url}/tree/'
-        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[:len(url)], url)
+        subprocess.run(["git", "remote", "set-url", "origin", "git@github.com:test_account/test_repo.git"])
+        url = f"{self.url}/tree/"
+        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[: len(url)], url)
 
     def test_get_git_url_https_enterprise(self) -> None:
-        true_url = 'https://github.tap.com/test_account/test_repo'
-        subprocess.run(['git', 'remote', 'set-url', 'origin', f'{true_url}.git'])
+        true_url = "https://github.tap.com/test_account/test_repo"
+        subprocess.run(["git", "remote", "set-url", "origin", f"{true_url}.git"])
         self.assertEqual(self.git_info.get_git_url(commit_hash=False), true_url)
 
     def test_get_git_url_https_hash_enterprise(self) -> None:
-        true_url = 'https://github.tap.com/test_account/test_repo'
-        subprocess.run(['git', 'remote', 'set-url', 'origin', f'{true_url}.git'])
-        url = f'{true_url}/tree/'
-        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[:len(url)], url)
+        true_url = "https://github.tap.com/test_account/test_repo"
+        subprocess.run(["git", "remote", "set-url", "origin", f"{true_url}.git"])
+        url = f"{true_url}/tree/"
+        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[: len(url)], url)
 
     def test_get_git_url_ssh_enterprise(self) -> None:
-        true_url = 'https://github.tap.com/test_account/test_repo'
-        subprocess.run(['git', 'remote', 'set-url', 'origin', 'git@github.tap.com:test_account/test_repo.git'])
+        true_url = "https://github.tap.com/test_account/test_repo"
+        subprocess.run(["git", "remote", "set-url", "origin", "git@github.tap.com:test_account/test_repo.git"])
         self.assertEqual(self.git_info.get_git_url(commit_hash=False), true_url)
 
     def test_get_git_url_ssh_hash_enterprise(self) -> None:
-        true_url = 'https://github.tap.com/test_account/test_repo'
-        subprocess.run(['git', 'remote', 'set-url', 'origin', 'git@github.tap.com:test_account/test_repo.git'])
-        url = f'{true_url}/tree/'
-        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[:len(url)], url)
+        true_url = "https://github.tap.com/test_account/test_repo"
+        subprocess.run(["git", "remote", "set-url", "origin", "git@github.tap.com:test_account/test_repo.git"])
+        url = f"{true_url}/tree/"
+        self.assertEqual(self.git_info.get_git_url(commit_hash=True)[: len(url)], url)
 
     def test_has_uncommitted_changes_false(self) -> None:
         self.assertFalse(self.git_info.has_uncommitted_changes())
 
     def test_has_uncommited_changes_true(self) -> None:
-        subprocess.run(['touch', 'main.py'])
+        subprocess.run(["touch", "main.py"])
         self.assertTrue(self.git_info.has_uncommitted_changes())
 
 
 class TypeToStrTests(TestCase):
     def test_type_to_str(self) -> None:
-        self.assertEqual(type_to_str(str), 'str')
-        self.assertEqual(type_to_str(int), 'int')
-        self.assertEqual(type_to_str(float), 'float')
-        self.assertEqual(type_to_str(bool), 'bool')
-        self.assertEqual(type_to_str(Any), 'Any')
-        self.assertEqual(type_to_str(Callable[[str], str]), 'Callable[[str], str]')
-        self.assertEqual(type_to_str(Callable[[str, int], Tuple[float, bool]]),
-                         'Callable[[str, int], Tuple[float, bool]]')
-        self.assertEqual(type_to_str(List[int]), 'List[int]')
-        self.assertEqual(type_to_str(List[str]), 'List[str]')
-        self.assertEqual(type_to_str(List[float]), 'List[float]')
-        self.assertEqual(type_to_str(List[bool]), 'List[bool]')
-        self.assertEqual(type_to_str(Set[int]), 'Set[int]')
-        self.assertEqual(type_to_str(Dict[str, int]), 'Dict[str, int]')
-        self.assertEqual(type_to_str(Union[List[int], Dict[float, bool]]), 'Union[List[int], Dict[float, bool]]')
+        self.assertEqual(type_to_str(str), "str")
+        self.assertEqual(type_to_str(int), "int")
+        self.assertEqual(type_to_str(float), "float")
+        self.assertEqual(type_to_str(bool), "bool")
+        self.assertEqual(type_to_str(Any), "Any")
+        self.assertEqual(type_to_str(Callable[[str], str]), "Callable[[str], str]")
+        self.assertEqual(
+            type_to_str(Callable[[str, int], Tuple[float, bool]]), "Callable[[str, int], Tuple[float, bool]]"
+        )
+        self.assertEqual(type_to_str(List[int]), "List[int]")
+        self.assertEqual(type_to_str(List[str]), "List[str]")
+        self.assertEqual(type_to_str(List[float]), "List[float]")
+        self.assertEqual(type_to_str(List[bool]), "List[bool]")
+        self.assertEqual(type_to_str(Set[int]), "Set[int]")
+        self.assertEqual(type_to_str(Dict[str, int]), "Dict[str, int]")
+        self.assertEqual(type_to_str(Union[List[int], Dict[float, bool]]), "Union[List[int], Dict[float, bool]]")
 
 
 def class_decorator(cls):
     return cls
 
 
 class ClassColumnTests(TestCase):
     def test_column_simple(self):
         class SimpleColumn:
             arg = 2
+
         self.assertEqual(get_class_column(SimpleColumn), 12)
 
     def test_column_comment(self):
         class CommentColumn:
             """hello
             there
 
 
             hi
             """
+
             arg = 2
+
         self.assertEqual(get_class_column(CommentColumn), 12)
 
     def test_column_space(self):
         class SpaceColumn:
 
             arg = 2
+
         self.assertEqual(get_class_column(SpaceColumn), 12)
 
     def test_column_method(self):
         class FuncColumn:
             def func(self):
                 pass
 
         self.assertEqual(get_class_column(FuncColumn), 12)
 
     def test_dataclass(self):
         @class_decorator
         class DataclassColumn:
             arg: int = 5
+
         self.assertEqual(get_class_column(DataclassColumn), 12)
 
     def test_dataclass_method(self):
         def wrapper(f):
             pass
 
         @class_decorator
         class DataclassColumn:
             @wrapper
             def func(self):
                 pass
+
         self.assertEqual(get_class_column(DataclassColumn), 12)
 
 
 class ClassVariableTests(TestCase):
     def test_no_variables(self):
         class NoVariables:
             pass
-        self.assertEqual(get_class_variables(NoVariables), OrderedDict())
+
+        self.assertEqual(get_class_variables(NoVariables), {})
 
     def test_one_variable(self):
         class OneVariable:
             arg = 2
-        class_variables = OrderedDict()
-        class_variables['arg'] = {'comment': ''}
+
+        class_variables = {"arg": {"comment": ""}}
         self.assertEqual(get_class_variables(OneVariable), class_variables)
 
     def test_multiple_variable(self):
         class MultiVariable:
             arg_1 = 2
             arg_2 = 3
-        class_variables = OrderedDict()
-        class_variables['arg_1'] = {'comment': ''}
-        class_variables['arg_2'] = {'comment': ''}
+
+        class_variables = {"arg_1": {"comment": ""}, "arg_2": {"comment": ""}}
         self.assertEqual(get_class_variables(MultiVariable), class_variables)
 
     def test_typed_variables(self):
         class TypedVariable:
             arg_1: str
             arg_2: int = 3
-        class_variables = OrderedDict()
-        class_variables['arg_1'] = {'comment': ''}
-        class_variables['arg_2'] = {'comment': ''}
+
+        class_variables = {"arg_1": {"comment": ""}, "arg_2": {"comment": ""}}
         self.assertEqual(get_class_variables(TypedVariable), class_variables)
 
     def test_separated_variables(self):
         class SeparatedVariable:
             """Comment
 
             """
+
             arg_1: str
 
             # Hello
             def func(self):
                 pass
 
             arg_2: int = 3
             """More comment"""
-        class_variables = OrderedDict()
-        class_variables['arg_1'] = {'comment': ''}
-        class_variables['arg_2'] = {'comment': 'More comment'}
+
+        class_variables = {"arg_1": {"comment": ""}, "arg_2": {"comment": "More comment"}}
         self.assertEqual(get_class_variables(SeparatedVariable), class_variables)
 
     def test_commented_variables(self):
         class CommentedVariable:
             """Comment
 
             """
+
             arg_1: str  # Arg 1 comment
 
             # Hello
             def func(self):
                 pass
 
             arg_2: int = 3  # Arg 2 comment
-            arg_3   :   Dict[str, int]      # noqa E203,E262   Poorly   formatted comment
+            arg_3: Dict[str, int]  # noqa E203,E262   Poorly   formatted comment
             """More comment"""
-        class_variables = OrderedDict()
-        class_variables['arg_1'] = {'comment': 'Arg 1 comment'}
-        class_variables['arg_2'] = {'comment': 'Arg 2 comment'}
-        class_variables['arg_3'] = {'comment': 'noqa E203,E262   Poorly   formatted comment More comment'}
+
+        class_variables = {
+            "arg_1": {"comment": "Arg 1 comment"},
+            "arg_2": {"comment": "Arg 2 comment"},
+            "arg_3": {"comment": "noqa E203,E262   Poorly   formatted comment More comment"},
+        }
         self.assertEqual(get_class_variables(CommentedVariable), class_variables)
 
     def test_bad_spacing_multiline(self):
         class TrickyMultiline:
             """   This is really difficult
 
         so
             so very difficult
             """
-            foo: str = 'my'  # Header line
+
+            foo: str = "my"  # Header line
 
             """    Footer
 T
         A
                 P
 
             multi
             line!!
                 """
 
-        class_variables = OrderedDict()
-        comment = 'Header line Footer\nT\n        A\n                P\n\n            multi\n            line!!'
-        class_variables['foo'] = {'comment': comment}
+        class_variables = {}
+        comment = "Header line Footer\nT\n        A\n                P\n\n            multi\n            line!!"
+        class_variables["foo"] = {"comment": comment}
         self.assertEqual(get_class_variables(TrickyMultiline), class_variables)
 
     def test_triple_quote_multiline(self):
         class TripleQuoteMultiline:
             bar: int = 0
-            '''biz baz'''
+            """biz baz"""
 
             hi: str
             """Hello there"""
 
-        class_variables = OrderedDict()
-        class_variables['bar'] = {'comment': 'biz baz'}
-        class_variables['hi'] = {'comment': 'Hello there'}
+        class_variables = {"bar": {"comment": "biz baz"}, "hi": {"comment": "Hello there"}}
         self.assertEqual(get_class_variables(TripleQuoteMultiline), class_variables)
 
     def test_single_quote_multiline(self):
         class SingleQuoteMultiline:
             bar: int = 0
-            'biz baz'
+            "biz baz"
 
             hi: str
             "Hello there"
 
-        class_variables = OrderedDict()
-        class_variables['bar'] = {'comment': 'biz baz'}
-        class_variables['hi'] = {'comment': 'Hello there'}
+        class_variables = {"bar": {"comment": "biz baz"}, "hi": {"comment": "Hello there"}}
         self.assertEqual(get_class_variables(SingleQuoteMultiline), class_variables)
 
     def test_functions_with_docs_multiline(self):
         class FunctionsWithDocs:
             i: int = 0
 
             def f(self):
                 """Function"""
-                a: str = 'hello'  # noqa F841
+                a: str = "hello"  # noqa F841
                 """with docs"""
 
-        class_variables = OrderedDict()
-        class_variables['i'] = {'comment': ''}
+        class_variables = {"i": {"comment": ""}}
         self.assertEqual(get_class_variables(FunctionsWithDocs), class_variables)
 
     def test_dataclass(self):
         @class_decorator
         class DataclassColumn:
             arg: int = 5
-        class_variables = OrderedDict()
-        class_variables['arg'] = {'comment': ''}
+
+        class_variables = {"arg": {"comment": ""}}
         self.assertEqual(get_class_variables(DataclassColumn), class_variables)
 
 
 class GetLiteralsTests(TestCase):
     def test_get_literals_string(self) -> None:
-        literal_f, shapes = get_literals(Literal['square', 'triangle', 'circle'], 'shape')
-        self.assertEqual(shapes, ['square', 'triangle', 'circle'])
-        self.assertEqual(literal_f('square'), 'square')
-        self.assertEqual(literal_f('triangle'), 'triangle')
-        self.assertEqual(literal_f('circle'), 'circle')
+        literal_f, shapes = get_literals(Literal["square", "triangle", "circle"], "shape")
+        self.assertEqual(shapes, ["square", "triangle", "circle"])
+        self.assertEqual(literal_f("square"), "square")
+        self.assertEqual(literal_f("triangle"), "triangle")
+        self.assertEqual(literal_f("circle"), "circle")
 
     def test_get_literals_primitives(self) -> None:
-        literals = [True, 'one', 2, 3.14]
-        literal_f, prims = get_literals(Literal[True, 'one', 2, 3.14], 'number')
+        literals = [True, "one", 2, 3.14]
+        literal_f, prims = get_literals(Literal[True, "one", 2, 3.14], "number")
         self.assertEqual(prims, literals)
         self.assertEqual([literal_f(str(p)) for p in prims], literals)
 
     def test_get_literals_uniqueness(self) -> None:
         with self.assertRaises(ArgumentTypeError):
-            get_literals(Literal['two', 2, '2'], 'number')
+            get_literals(Literal["two", 2, "2"], "number")
 
     def test_get_literals_empty(self) -> None:
-        literal_f, prims = get_literals(Literal, 'hi')
+        literal_f, prims = get_literals(Literal, "hi")
         self.assertEqual(prims, [])
 
 
 class TupleTypeEnforcerTests(TestCase):
     def test_tuple_type_enforcer_zero_types(self):
         enforcer = TupleTypeEnforcer(types=[])
         with self.assertRaises(IndexError):
-            enforcer('hi')
+            enforcer("hi")
 
     def test_tuple_type_enforcer_one_type_str(self):
         enforcer = TupleTypeEnforcer(types=[str])
-        self.assertEqual(enforcer('hi'), 'hi')
+        self.assertEqual(enforcer("hi"), "hi")
 
     def test_tuple_type_enforcer_one_type_int(self):
         enforcer = TupleTypeEnforcer(types=[int])
-        self.assertEqual(enforcer('123'), 123)
+        self.assertEqual(enforcer("123"), 123)
 
     def test_tuple_type_enforcer_one_type_float(self):
         enforcer = TupleTypeEnforcer(types=[float])
-        self.assertEqual(enforcer('3.14159'), 3.14159)
+        self.assertEqual(enforcer("3.14159"), 3.14159)
 
     def test_tuple_type_enforcer_one_type_bool(self):
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('True'), True)
+        self.assertEqual(enforcer("True"), True)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('true'), True)
+        self.assertEqual(enforcer("true"), True)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('False'), False)
+        self.assertEqual(enforcer("False"), False)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('false'), False)
+        self.assertEqual(enforcer("false"), False)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('tRu'), True)
+        self.assertEqual(enforcer("tRu"), True)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('faL'), False)
+        self.assertEqual(enforcer("faL"), False)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('1'), True)
+        self.assertEqual(enforcer("1"), True)
 
         enforcer = TupleTypeEnforcer(types=[bool])
-        self.assertEqual(enforcer('0'), False)
+        self.assertEqual(enforcer("0"), False)
 
     def test_tuple_type_enforcer_multi_types_same(self):
         enforcer = TupleTypeEnforcer(types=[str, str])
-        args = ['hi', 'bye']
+        args = ["hi", "bye"]
         output = [enforcer(arg) for arg in args]
         self.assertEqual(output, args)
 
         enforcer = TupleTypeEnforcer(types=[int, int, int])
         args = [123, 456, -789]
         output = [enforcer(str(arg)) for arg in args]
         self.assertEqual(output, args)
 
         enforcer = TupleTypeEnforcer(types=[float, float, float, float])
         args = [1.23, 4.56, -7.89, 3.14159]
         output = [enforcer(str(arg)) for arg in args]
         self.assertEqual(output, args)
 
         enforcer = TupleTypeEnforcer(types=[bool, bool, bool, bool, bool])
-        args = ['True', 'False', '1', '0', 'tru']
+        args = ["True", "False", "1", "0", "tru"]
         true_output = [True, False, True, False, True]
         output = [enforcer(str(arg)) for arg in args]
         self.assertEqual(output, true_output)
 
     def test_tuple_type_enforcer_multi_types_different(self):
         enforcer = TupleTypeEnforcer(types=[str, int, float, bool])
-        args = ['hello', 77, 0.2, 'tru']
-        true_output = ['hello', 77, 0.2, True]
+        args = ["hello", 77, 0.2, "tru"]
+        true_output = ["hello", 77, 0.2, True]
         output = [enforcer(str(arg)) for arg in args]
         self.assertEqual(output, true_output)
 
     def test_tuple_type_enforcer_infinite(self):
         enforcer = TupleTypeEnforcer(types=[int], loop=True)
         args = [1, 2, -5, 20]
         output = [enforcer(str(arg)) for arg in args]
         self.assertEqual(output, args)
 
 
 class NestedReplaceTypeTests(TestCase):
     def test_nested_replace_type_notype(self):
-        obj = ['123', 4, 5, ('hello', 4.4)]
+        obj = ["123", 4, 5, ("hello", 4.4)]
         replaced_obj = _nested_replace_type(obj, bool, int)
         self.assertEqual(obj, replaced_obj)
 
     def test_nested_replace_type_unnested(self):
-        obj = ['123', 4, 5, ('hello', 4.4), True, False, 'hi there']
+        obj = ["123", 4, 5, ("hello", 4.4), True, False, "hi there"]
         replaced_obj = _nested_replace_type(obj, tuple, list)
-        correct_obj = ['123', 4, 5, ['hello', 4.4], True, False, 'hi there']
+        correct_obj = ["123", 4, 5, ["hello", 4.4], True, False, "hi there"]
         self.assertNotEqual(obj, replaced_obj)
         self.assertEqual(correct_obj, replaced_obj)
 
     def test_nested_replace_type_nested(self):
-        obj = ['123', [4, (1, 2, (3, 4))], 5, ('hello', (4,), 4.4), {'1': [2, 3, [{'2': (3, 10)}, ' hi ']]}]
+        obj = ["123", [4, (1, 2, (3, 4))], 5, ("hello", (4,), 4.4), {"1": [2, 3, [{"2": (3, 10)}, " hi "]]}]
         replaced_obj = _nested_replace_type(obj, tuple, list)
-        correct_obj = ['123', [4, [1, 2, [3, 4]]], 5, ['hello', [4], 4.4], {'1': [2, 3, [{'2': [3, 10]}, ' hi ']]}]
+        correct_obj = ["123", [4, [1, 2, [3, 4]]], 5, ["hello", [4], 4.4], {"1": [2, 3, [{"2": [3, 10]}, " hi "]]}]
         self.assertNotEqual(obj, replaced_obj)
         self.assertEqual(correct_obj, replaced_obj)
 
 
 class Person:
     def __init__(self, name: str) -> None:
         self.name = name
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, Person) and self.name == other.name
 
 
 class PythonObjectEncoderTests(TestCase):
     def test_python_object_encoder_simple_types(self):
-        obj = [1, 2, 'hi', 'bye', 7.3, [1, 2, 'blarg'], True, False, None]
+        obj = [1, 2, "hi", "bye", 7.3, [1, 2, "blarg"], True, False, None]
         dumps = json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder())
         recreated_obj = json.loads(dumps, object_hook=as_python_object)
         self.assertEqual(recreated_obj, obj)
 
     def test_python_object_encoder_tuple(self):
-        obj = [1, 2, 'hi', 'bye', 7.3, (1, 2, 'blarg'), [('hi', 'bye'), 2], {'hi': {'bye': (3, 4)}}, True, False, None]
+        obj = [1, 2, "hi", "bye", 7.3, (1, 2, "blarg"), [("hi", "bye"), 2], {"hi": {"bye": (3, 4)}}, True, False, None]
         dumps = json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder())
         recreated_obj = json.loads(dumps, object_hook=as_python_object)
         self.assertEqual(recreated_obj, obj)
 
     def test_python_object_encoder_set(self):
-        obj = [1, 2, 'hi', 'bye', 7.3, {1, 2, 'blarg'}, [{'hi', 'bye'}, 2], {'hi': {'bye': {3, 4}}}, True, False, None]
+        obj = [1, 2, "hi", "bye", 7.3, {1, 2, "blarg"}, [{"hi", "bye"}, 2], {"hi": {"bye": {3, 4}}}, True, False, None]
         dumps = json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder())
         recreated_obj = json.loads(dumps, object_hook=as_python_object)
         self.assertEqual(recreated_obj, obj)
 
     def test_python_object_encoder_complex(self):
-        obj = [1, 2, 'hi', 'bye', 7.3, {1, 2, 'blarg'}, [('hi', 'bye'), 2], {'hi': {'bye': {3, 4}}}, True, False, None,
-               (Person('tappy'), Person('tapper'))]
+        obj = [
+            1,
+            2,
+            "hi",
+            "bye",
+            7.3,
+            {1, 2, "blarg"},
+            [("hi", "bye"), 2],
+            {"hi": {"bye": {3, 4}}},
+            True,
+            False,
+            None,
+            (Person("tappy"), Person("tapper")),
+        ]
         dumps = json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder())
         recreated_obj = json.loads(dumps, object_hook=as_python_object)
         self.assertEqual(recreated_obj, obj)
 
     def test_python_object_encoder_unpicklable(self):
         class CannotPickleThis:
             """Da na na na. Can't pickle this. """
+
             def __init__(self):
                 self.x = 1
 
         obj = [1, CannotPickleThis()]
         expected_obj = [1, UnpicklableObject()]
         with self.assertRaises(ValueError):
             json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder())
 
         dumps = json.dumps(obj, indent=4, sort_keys=True, cls=define_python_object_encoder(True))
         recreated_obj = json.loads(dumps, object_hook=as_python_object)
         self.assertEqual(recreated_obj, expected_obj)
 
 
 class EnforceReproducibilityTests(TestCase):
-
     def test_saved_reproducibility_data_is_none(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility(None, {}, 'here')
+            enforce_reproducibility(None, {}, "here")
 
     def test_git_url_not_in_saved_reproducibility_data(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility({}, {}, 'here')
+            enforce_reproducibility({}, {}, "here")
 
     def test_git_url_not_in_current_reproducibility_data(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility({'git_url': 'none'}, {}, 'here')
+            enforce_reproducibility({"git_url": "none"}, {}, "here")
 
     def test_git_urls_disagree(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility({'git_url': 'none'}, {'git_url': 'some'}, 'here')
+            enforce_reproducibility({"git_url": "none"}, {"git_url": "some"}, "here")
 
     def test_throw_error_for_saved_uncommitted_changes(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility({'git_url': 'none', 'git_has_uncommitted_changes': True}, {'git_url': 'some'}, 'here')
+            enforce_reproducibility(
+                {"git_url": "none", "git_has_uncommitted_changes": True}, {"git_url": "some"}, "here"
+            )
 
     def test_throw_error_for_uncommitted_changes(self):
         with self.assertRaises(ValueError):
-            enforce_reproducibility({'git_url': 'none', 'git_has_uncommitted_changes': False}, {'git_url': 'some', 'git_has_uncommitted_changes': True}, 'here')
+            enforce_reproducibility(
+                {"git_url": "none", "git_has_uncommitted_changes": False},
+                {"git_url": "some", "git_has_uncommitted_changes": True},
+                "here",
+            )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `typed-argument-parser-1.8.1/typed_argument_parser.egg-info/PKG-INFO` & `typed-argument-parser-1.9.0/typed_argument_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: typed-argument-parser
-Version: 1.8.1
+Version: 1.9.0
 Summary: Typed Argument Parser
 Home-page: https://github.com/swansonk14/typed-argument-parser
-Download-URL: https://github.com/swansonk14/typed-argument-parser/archive/refs/tags/v_1.8.1.tar.gz
+Download-URL: https://github.com/swansonk14/typed-argument-parser/archive/refs/tags/v_1.9.0.tar.gz
 Author: Jesse Michel and Kyle Swanson
 Author-email: jessem.michel@gmail.com, swansonk.14@gmail.com
 License: MIT
 Keywords: typing,argument parser,python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

