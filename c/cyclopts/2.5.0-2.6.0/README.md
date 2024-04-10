# Comparing `tmp/cyclopts-2.5.0.tar.gz` & `tmp/cyclopts-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclopts-2.5.0.tar", max compression
+gzip compressed data, was "cyclopts-2.6.0.tar", max compression
```

## Comparing `cyclopts-2.5.0.tar` & `cyclopts-2.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-03-25 20:36:40.081176 cyclopts-2.5.0/LICENSE
--rw-r--r--   0        0        0    10910 2024-03-25 20:36:40.081176 cyclopts-2.5.0/README.md
--rw-r--r--   0        0        0      894 2024-03-25 20:36:53.913218 cyclopts-2.5.0/cyclopts/__init__.py
--rw-r--r--   0        0        0    10995 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/_convert.py
--rw-r--r--   0        0        0    13552 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/bind.py
--rw-r--r--   0        0        0    34060 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/core.py
--rw-r--r--   0        0        0     9637 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/exceptions.py
--rw-r--r--   0        0        0     4989 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/group.py
--rw-r--r--   0        0        0     2639 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/group_extractors.py
--rw-r--r--   0        0        0     9518 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/help.py
--rw-r--r--   0        0        0     7635 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/parameter.py
--rw-r--r--   0        0        0      190 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/protocols.py
--rw-r--r--   0        0        0        0 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/py.typed
--rw-r--r--   0        0        0     9265 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/resolve.py
--rw-r--r--   0        0        0     3851 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/types.py
--rw-r--r--   0        0        0     5425 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/utils.py
--rw-r--r--   0        0        0      205 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/validators/__init__.py
--rw-r--r--   0        0        0     1233 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/validators/_group.py
--rw-r--r--   0        0        0     1459 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/validators/_number.py
--rw-r--r--   0        0        0     1298 2024-03-25 20:36:40.089176 cyclopts-2.5.0/cyclopts/validators/_path.py
--rw-r--r--   0        0        0     4369 2024-03-25 20:36:53.913218 cyclopts-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 23:33:32.015391 cyclopts-2.6.0/LICENSE
+-rw-r--r--   0        0        0    10910 2024-04-10 23:33:32.015391 cyclopts-2.6.0/README.md
+-rw-r--r--   0        0        0      974 2024-04-10 23:33:47.123394 cyclopts-2.6.0/cyclopts/__init__.py
+-rw-r--r--   0        0        0    12220 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/_convert.py
+-rw-r--r--   0        0        0    13552 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/bind.py
+-rw-r--r--   0        0        0    34480 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/core.py
+-rw-r--r--   0        0        0     9637 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/exceptions.py
+-rw-r--r--   0        0        0     4989 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/group.py
+-rw-r--r--   0        0        0     2639 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/group_extractors.py
+-rw-r--r--   0        0        0     9704 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/help.py
+-rw-r--r--   0        0        0     7991 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/parameter.py
+-rw-r--r--   0        0        0      190 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/py.typed
+-rw-r--r--   0        0        0     9514 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/resolve.py
+-rw-r--r--   0        0        0     3851 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/types.py
+-rw-r--r--   0        0        0     6027 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/utils.py
+-rw-r--r--   0        0        0      205 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_group.py
+-rw-r--r--   0        0        0     1459 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_number.py
+-rw-r--r--   0        0        0     1298 2024-04-10 23:33:32.019391 cyclopts-2.6.0/cyclopts/validators/_path.py
+-rw-r--r--   0        0        0     4370 2024-04-10 23:33:47.123394 cyclopts-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11886 1970-01-01 00:00:00.000000 cyclopts-2.6.0/PKG-INFO
```

### Comparing `cyclopts-2.5.0/LICENSE` & `cyclopts-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/README.md` & `cyclopts-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/__init__.py` & `cyclopts-2.6.0/cyclopts/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning handle it.
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 
 __all__ = [
     "App",
     "CoercionError",
     "CommandCollisionError",
     "CycloptsError",
     "Dispatcher",
@@ -12,14 +12,15 @@
     "InvalidCommandError",
     "MissingArgumentError",
     "Parameter",
     "UnknownOptionError",
     "UnusedCliTokensError",
     "ValidationError",
     "convert",
+    "default_name_transform",
     "types",
     "validators",
 ]
 
 from cyclopts._convert import convert
 from cyclopts.core import App
 from cyclopts.exceptions import (
@@ -32,9 +33,10 @@
     UnknownOptionError,
     UnusedCliTokensError,
     ValidationError,
 )
 from cyclopts.group import Group
 from cyclopts.parameter import Parameter
 from cyclopts.protocols import Dispatcher
+from cyclopts.utils import default_name_transform
 
 from . import types, validators
```

### Comparing `cyclopts-2.5.0/cyclopts/_convert.py` & `cyclopts-2.6.0/cyclopts/_convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 if sys.version_info < (3, 9):
     from typing_extensions import Annotated  # pragma: no cover
 else:
     from typing import Annotated  # pragma: no cover
 
 
 from cyclopts.exceptions import CoercionError
-from cyclopts.utils import is_union
+from cyclopts.utils import default_name_transform, is_union
 
 if TYPE_CHECKING:
     from cyclopts.parameter import Parameter
 
 # from types import NoneType is available >=3.10
 NoneType = type(None)
 AnnotatedType = type(Annotated[int, 0])
@@ -79,15 +79,21 @@
     bool: _bool,
     int: _int,
     bytes: _bytes,
     bytearray: _bytearray,
 }
 
 
-def _convert_tuple(type_: Type[Any], *args: str, converter: Optional[Callable] = None) -> Tuple:
+def _convert_tuple(
+    type_: Type[Any],
+    *args: str,
+    converter: Optional[Callable[[Type, str], Any]],
+    name_transform: Callable[[str], str],
+) -> Tuple:
+    convert = partial(_convert, converter=converter, name_transform=name_transform)
     inner_types = tuple(x for x in get_args(type_) if x is not ...)
     inner_token_count, consume_all = token_count(type_)
     if consume_all:
         # variable-length tuple (list-like)
         remainder = len(args) % inner_token_count
         if remainder:
             raise CoercionError(
@@ -97,82 +103,95 @@
             inner_type = inner_types[0]
         elif len(inner_types) == 0:
             inner_type = str
         else:
             raise ValueError("A tuple must have 0 or 1 inner-types.")
 
         if inner_token_count == 1:
-            out = tuple(_convert(inner_type, x, converter=converter) for x in args)
+            out = tuple(convert(inner_type, x) for x in args)
         else:
             out = tuple(
-                _convert(inner_type, args[i : i + inner_token_count], converter=converter)
-                for i in range(0, len(args), inner_token_count)
+                convert(inner_type, args[i : i + inner_token_count]) for i in range(0, len(args), inner_token_count)
             )
         return out
     else:
         # Fixed-length tuple
         if inner_token_count != len(args):
             raise CoercionError(msg=f"Incorrect number of arguments: expected {inner_token_count} but got {len(args)}.")
         args_per_convert = [token_count(x)[0] for x in inner_types]
         it = iter(args)
         batched = [[next(it) for _ in range(size)] for size in args_per_convert]
         batched = [elem[0] if len(elem) == 1 else elem for elem in batched]
-        out = tuple(_convert(inner_type, arg, converter=converter) for inner_type, arg in zip(inner_types, batched))
+        out = tuple(convert(inner_type, arg) for inner_type, arg in zip(inner_types, batched))
     return out
 
 
-def _convert(type_, element, converter=None):
-    pconvert = partial(_convert, converter=converter)
+def _convert(
+    type_,
+    element,
+    *,
+    converter: Optional[Callable[[Type, str], Any]],
+    name_transform: Callable[[str], str],
+):
+    """Inner recursive conversion function for public ``convert``.
+
+    Parameters
+    ----------
+    converter: Callable
+    name_transform: Callable
+    """
+    convert = partial(_convert, converter=converter, name_transform=name_transform)
+    convert_tuple = partial(_convert_tuple, converter=converter, name_transform=name_transform)
     origin_type = get_origin(type_)
     inner_types = [resolve(x) for x in get_args(type_)]
 
     if type_ in _implicit_iterable_type_mapping:
-        return pconvert(_implicit_iterable_type_mapping[type_], element)
+        return convert(_implicit_iterable_type_mapping[type_], element)
 
     if origin_type is collections.abc.Iterable:
         assert len(inner_types) == 1
-        return pconvert(List[inner_types[0]], element)  # pyright: ignore[reportGeneralTypeIssues]
+        return convert(List[inner_types[0]], element)  # pyright: ignore[reportGeneralTypeIssues]
     elif is_union(origin_type):
         for t in inner_types:
             if t is NoneType:
                 continue
             try:
-                return pconvert(t, element)
+                return convert(t, element)
             except Exception:
                 pass
         else:
             raise CoercionError(input_value=element, target_type=type_)
     elif origin_type is Literal:
         for choice in get_args(type_):
             try:
-                res = pconvert(type(choice), (element))
+                res = convert(type(choice), (element))
             except Exception:
                 continue
             if res == choice:
                 return res
         else:
             raise CoercionError(input_value=element, target_type=type_)
     elif origin_type in _iterable_types:  # NOT including tuple
         count, _ = token_count(inner_types[0])
         if count > 1:
             gen = zip(*[iter(element)] * count)
         else:
             gen = element
-        return origin_type(pconvert(inner_types[0], e) for e in gen)  # pyright: ignore[reportOptionalCall]
+        return origin_type(convert(inner_types[0], e) for e in gen)  # pyright: ignore[reportOptionalCall]
     elif origin_type is tuple:
         if isinstance(element, str):
             # E.g. Tuple[str] (Annotation: tuple containing a single string)
-            return _convert_tuple(type_, element, converter=converter)
+            return convert_tuple(type_, element, converter=converter)
         else:
-            return _convert_tuple(type_, *element, converter=converter)
+            return convert_tuple(type_, *element, converter=converter)
     elif isclass(type_) and issubclass(type_, Enum):
         if converter is None:
-            element_lower = element.lower().replace("-", "_")
+            element_transformed = name_transform(element)
             for member in type_:
-                if member.name.lower().strip("_") == element_lower:
+                if name_transform(member.name) == element_transformed:
                     return member
             raise CoercionError(input_value=element, target_type=type_)
         else:
             return converter(type_, element)
     else:
         # The actual casting/converting of the underlying type is performed here.
         try:
@@ -236,15 +255,20 @@
 
 def resolve_annotated(type_: Type) -> Type:
     if type(type_) is AnnotatedType:
         type_ = get_args(type_)[0]
     return type_
 
 
-def convert(type_: Type, *args: str, converter: Optional[Callable] = None):
+def convert(
+    type_: Type,
+    *args: str,
+    converter: Optional[Callable[[Type, str], Any]] = None,
+    name_transform: Optional[Callable[[str], str]] = None,
+):
     """Coerce variables into a specified type.
 
     Internally used to coercing string CLI tokens into python builtin types.
     Externally, may be useful in a custom converter.
     See Cyclopt's automatic coercion rules :doc:`/rules`.
 
     If ``type_`` **is not** iterable, then each element of ``*args`` will be converted independently.
@@ -255,50 +279,68 @@
 
     Parameters
     ----------
     type_: Type
         A type hint/annotation to coerce ``*args`` into.
     `*args`: str
         String tokens to coerce.
-    converter: Optional[Callable]
-
+    converter: Optional[Callable[[Type, str], Any]]
         An optional function to convert tokens to the inner-most types.
         The converter should have signature:
 
         .. code-block:: python
 
             def converter(type_: type, value: str) -> Any:
                 ...
 
         This allows to use the :func:`convert` function to handle the the difficult task
         of traversing lists/tuples/unions/etc, while leaving the final conversion logic to
         the caller.
+    name_transform: Optional[Callable[[str], str]]
+        Currently only used for ``Enum`` type hints.
+        A function that transforms enum names and CLI values into a normalized format.
+
+        The function should have signature:
+
+        .. code-block:: python
+
+            def name_transform(s: str) -> str:
+                ...
+
+        where the returned value is the name to be used on the CLI.
+
+        If ``None``, defaults to ``cyclopts.default_name_transform``.
 
     Returns
     -------
     Any
         Coerced version of input ``*args``.
     """
+    if name_transform is None:
+        name_transform = default_name_transform
+
+    convert = partial(_convert, converter=converter, name_transform=name_transform)
+    convert_tuple = partial(_convert_tuple, converter=converter, name_transform=name_transform)
     type_ = resolve(type_)
 
     if type_ is Any:
         type_ = str
 
     type_ = _implicit_iterable_type_mapping.get(type_, type_)
 
     origin_type = get_origin_and_validate(type_)
 
     if origin_type is tuple:
-        return _convert_tuple(type_, *args, converter=converter)
+        return convert_tuple(type_, *args)
     elif (origin_type or type_) in _iterable_types or origin_type is collections.abc.Iterable:
-        return _convert(type_, args, converter=converter)
+        return convert(type_, args)
     elif len(args) == 1:
-        return _convert(type_, args[0], converter=converter)
+        return convert(type_, args[0])
     else:
-        return [_convert(type_, item, converter=converter) for item in args]
+        return [convert(type_, item) for item in args]
 
 
 def token_count(type_: Union[Type[Any], inspect.Parameter]) -> Tuple[int, bool]:
     """The number of tokens after a keyword the parameter should consume.
 
     Parameters
     ----------
```

### Comparing `cyclopts-2.5.0/cyclopts/bind.py` & `cyclopts-2.6.0/cyclopts/bind.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/core.py` & `cyclopts-2.6.0/cyclopts/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,25 +51,21 @@
     format_command_entries,
     format_doc,
     format_usage,
 )
 from cyclopts.parameter import Parameter, validate_command
 from cyclopts.protocols import Dispatcher
 from cyclopts.resolve import ResolvedCommand
-from cyclopts.utils import optional_to_tuple_converter, to_list_converter, to_tuple_converter
+from cyclopts.utils import default_name_transform, optional_to_tuple_converter, to_list_converter, to_tuple_converter
 
 with suppress(ImportError):
     # By importing, makes things like the arrow-keys work.
     import readline  # Not available on windows
 
 
-def _format_name(name: str):
-    return name.lower().replace("_", "-").strip("-")
-
-
 class _CannotDeriveCallingModuleNameError(Exception):
     pass
 
 
 def _get_root_module_name():
     """Get the calling package name from the call-stack."""
     for elem in inspect.stack():
@@ -220,14 +216,20 @@
         converter=GroupConverter(Group.create_default_commands()),
         kw_only=True,
     )
 
     converter: Optional[Callable] = field(default=None, kw_only=True)
     validator: List[Callable] = field(default=None, converter=to_list_converter, kw_only=True)
 
+    _name_transform: Optional[Callable[[str], str]] = field(
+        default=None,
+        alias="name_transform",
+        kw_only=True,
+    )
+
     ######################
     # Private Attributes #
     ######################
     # Maps CLI-name of a command to a function handle.
     _commands: Dict[str, "App"] = field(init=False, factory=dict)
 
     _parents: List["App"] = field(init=False, factory=list)
@@ -303,15 +305,15 @@
             return self._name  # pyright: ignore[reportGeneralTypeIssues]
         elif self.default_command is None:
             name = Path(sys.argv[0]).name
             if name == "__main__.py":
                 name = _get_root_module_name()
             return (name,)
         else:
-            return (_format_name(self.default_command.__name__),)
+            return (self.name_transform(self.default_command.__name__),)
 
     @property
     def help(self) -> str:
         if self._help is not None:
             return self._help
         elif self.default_command is None:
             # Try and fallback to a meta-app docstring.
@@ -324,14 +326,22 @@
         else:
             return self.default_command.__doc__
 
     @help.setter
     def help(self, value):
         self._help = value
 
+    @property
+    def name_transform(self):
+        return self._name_transform if self._name_transform else default_name_transform
+
+    @name_transform.setter
+    def name_transform(self, value):
+        self._name_transform = value
+
     def version_print(self) -> None:
         """Print the application version."""
         print(self.version() if callable(self.version) else self.version)
 
     def __getitem__(self, key: str) -> "App":
         """Get the subapp from a command string.
 
@@ -454,14 +464,17 @@
             if "group_parameters" not in kwargs:
                 kwargs["group_parameters"] = copy(self.group_parameters)
             if "group_arguments" not in kwargs:
                 kwargs["group_arguments"] = copy(self.group_arguments)
             app = App(default_command=obj, **kwargs)
             # app.name is handled below
 
+        if app._name_transform is None:
+            app.name_transform = self.name_transform
+
         if name is None:
             name = app.name
         else:
             app._name = name
 
         for n in to_tuple_converter(name):
             if n in self:
```

### Comparing `cyclopts-2.5.0/cyclopts/exceptions.py` & `cyclopts-2.6.0/cyclopts/exceptions.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/group.py` & `cyclopts-2.6.0/cyclopts/group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/group_extractors.py` & `cyclopts-2.6.0/cyclopts/group_extractors.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/help.py` & `cyclopts-2.6.0/cyclopts/help.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 from enum import Enum
-from functools import lru_cache
+from functools import lru_cache, partial
 from inspect import isclass
-from typing import TYPE_CHECKING, List, Literal, Tuple, Type, Union, get_args, get_origin
+from typing import TYPE_CHECKING, Callable, List, Literal, Tuple, Type, Union, get_args, get_origin
 
 import docstring_parser
 from attrs import define, field, frozen
 from rich import box, console
 from rich.panel import Panel
 from rich.table import Table
 from rich.text import Text
@@ -186,42 +186,44 @@
         from rich_rst import RestructuredText
 
         return RestructuredText("".join(x[0] for x in components))
     else:
         raise ValueError(f'Unknown help_format "{format}"')
 
 
-def _get_choices(type_: Type) -> str:
+def _get_choices(type_: Type, name_transform: Callable[[str], str]) -> str:
+    get_choices = partial(_get_choices, name_transform=name_transform)
     choices: str = ""
     _origin = get_origin(type_)
     if isclass(type_) and issubclass(type_, Enum):
-        choices = ",".join(x.name.lower().replace("_", "-") for x in type_)
+        choices = ",".join(name_transform(x.name) for x in type_)
     elif _origin is Union:
-        inner_choices = [_get_choices(inner) for inner in get_args(type_)]
+        inner_choices = [get_choices(inner) for inner in get_args(type_)]
         choices = ",".join(x for x in inner_choices if x)
     elif _origin is Literal:
         choices = ",".join(str(x) for x in get_args(type_))
     elif _origin in (list, set, tuple):
         args = get_args(type_)
         if len(args) == 1 or (_origin is tuple and len(args) == 2 and args[1] is Ellipsis):
-            choices = _get_choices(args[0])
+            choices = get_choices(args[0])
     return choices
 
 
 def create_parameter_help_panel(group: "Group", iparams, cparams: List[Parameter]) -> HelpPanel:
     help_panel = HelpPanel(format="parameter", title=group.name, description=group.help)
     icparams = [(ip, cp) for ip, cp in zip(iparams, cparams) if cp.show]
 
     if not icparams:
         return help_panel
 
     iparams, cparams = (list(x) for x in zip(*icparams))
 
     for iparam, cparam in icparams:
         assert cparam.name is not None
+        assert cparam.name_transform is not None
         type_ = get_hint_parameter(iparam)[0]
         options = list(cparam.name)
         options.extend(cparam.get_negatives(type_, *options))
 
         # Add an all-uppercase name if it's an argument
         if iparam.kind in (iparam.POSITIONAL_ONLY, iparam.POSITIONAL_OR_KEYWORD):
             arg_name = options[0].lstrip("-").upper()
@@ -237,28 +239,28 @@
 
         help_components = []
 
         if cparam.help:
             help_components.append(cparam.help)
 
         if cparam.show_choices:
-            choices = _get_choices(type_)
+            choices = _get_choices(type_, cparam.name_transform)
             if choices:
                 help_components.append(rf"[dim]\[choices: {choices}][/dim]")
 
         if cparam.show_env_var and cparam.env_var:
             env_vars = " ".join(cparam.env_var)
             help_components.append(rf"[dim]\[env var: {env_vars}][/dim]")
 
-        if not cparam.required and (
-            cparam.show_default or (cparam.show_default is None and iparam.default is not None)
+        if cparam.show_default or (
+            cparam.show_default is None and iparam.default not in {None, inspect.Parameter.empty}
         ):
             default = ""
             if isclass(type_) and issubclass(type_, Enum):
-                default = iparam.default.name.lower().replace("_", "-")
+                default = cparam.name_transform(iparam.default.name)
             else:
                 default = iparam.default
 
             help_components.append(rf"[dim]\[default: {default}][/dim]")
 
         if cparam.required:
             help_components.append(r"[red][dim]\[required][/dim][/red]")
```

### Comparing `cyclopts-2.5.0/cyclopts/parameter.py` & `cyclopts-2.6.0/cyclopts/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import inspect
+from functools import partial
 from typing import Any, Callable, Iterable, Optional, Tuple, Type, Union, cast, get_args, get_origin
 
 import attrs
 from attrs import field, frozen
 
 import cyclopts.utils
 from cyclopts._convert import (
     AnnotatedType,
     convert,
     get_origin_and_validate,
     resolve,
     resolve_optional,
 )
 from cyclopts.group import Group
-from cyclopts.utils import optional_to_tuple_converter, record_init, to_tuple_converter
+from cyclopts.utils import default_name_transform, optional_to_tuple_converter, record_init, to_tuple_converter
 
 
 def _double_hyphen_validator(instance, attribute, values):
     if not values:
         return
 
     for value in values:
@@ -44,15 +45,15 @@
 
     # This can ONLY ever be a Tuple[str, ...]
     name: Union[None, str, Iterable[str]] = field(
         default=None,
         converter=lambda x: cast(Tuple[str, ...], to_tuple_converter(x)),
     )
 
-    converter: Callable = field(default=None, converter=attrs.converters.default_if_none(convert))
+    _converter: Callable = field(default=None, alias="converter")
 
     # This can ONLY ever be a Tuple[Callable, ...]
     validator: Union[None, Callable, Iterable[Callable]] = field(
         default=(),
         converter=lambda x: cast(Tuple[Callable, ...], to_tuple_converter(x)),
     )
 
@@ -94,21 +95,31 @@
         validator=_double_hyphen_validator,
     )
 
     required: Optional[bool] = field(default=None)
 
     allow_leading_hyphen: bool = field(default=False)
 
+    name_transform: Optional[Callable[[str], str]] = field(
+        default=None,
+        converter=attrs.converters.default_if_none(default_name_transform),
+        kw_only=True,
+    )
+
     # Populated by the record_attrs_init_args decorator.
     _provided_args: Tuple[str] = field(default=(), init=False, eq=False)
 
     @property
     def show(self):
         return self._show if self._show is not None else self.parse
 
+    @property
+    def converter(self):
+        return self._converter if self._converter else partial(convert, name_transform=self.name_transform)
+
     def get_negatives(self, type_, *names: str) -> Tuple[str, ...]:
         type_ = get_origin(type_) or type_
 
         if self.negative is not None:
             return self.negative  # pyright: ignore
         elif type_ not in (bool, list, set):
             return ()
```

### Comparing `cyclopts-2.5.0/cyclopts/resolve.py` & `cyclopts-2.6.0/cyclopts/resolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,31 +165,34 @@
         )
 
         # Fully Resolve each Cyclopts Parameter
         self.iparam_to_cparam = ParameterDict()
         iparam_to_docstring_cparam = _resolve_docstring(f, signature) if parse_docstring else ParameterDict()
         empty_help_string_parameter = Parameter(help="")
         for iparam, groups in self.iparam_to_groups.items():
-            if iparam.kind in (iparam.POSITIONAL_ONLY, iparam.VAR_POSITIONAL):
-                # Name is only used for help-string
-                names = [iparam.name.upper()]
-            else:
-                names = ["--" + iparam.name.replace("_", "-")]
-
-            default_name_parameter = Parameter(name=names)
-
             cparam = get_hint_parameter(
                 iparam,
                 empty_help_string_parameter,
                 app_parameter,
                 *(x.default_parameter for x in groups),
                 iparam_to_docstring_cparam.get(iparam),
-                default_name_parameter,
                 Parameter(required=iparam.default is iparam.empty),
             )[1]
+
+            # Resolve name now that ``name_transform`` has been resolved.
+            if iparam.kind in (iparam.POSITIONAL_ONLY, iparam.VAR_POSITIONAL):
+                # Name is only used for help-string
+                names = [iparam.name.upper()]
+            else:
+                # cparam.name_transform cannot be None due to:
+                #     attrs.converters.default_if_none(default_name_transform)
+                assert cparam.name_transform is not None
+                names = ["--" + cparam.name_transform(iparam.name)]
+
+            cparam = Parameter.combine(Parameter(name=names), cparam)
             self.iparam_to_cparam[iparam] = cparam
 
         self.bind = signature.bind_partial if _has_unparsed_parameters(signature, app_parameter) else signature.bind
 
         # Create a convenient group-to-iparam structure
         self.groups_iparams = [
             (
```

### Comparing `cyclopts-2.5.0/cyclopts/types.py` & `cyclopts-2.6.0/cyclopts/types.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/utils.py` & `cyclopts-2.6.0/cyclopts/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -167,7 +167,31 @@
     if value is None:
         return None
 
     if not value:
         return ()
 
     return to_tuple_converter(value)
+
+
+def default_name_transform(s: str) -> str:
+    """Converts a python identifier into a CLI token.
+
+    Performs the following operations (in order):
+
+    1. Convert the string to all lowercase.
+    2. Replace ``_`` with ``-``.
+    3. Strip any leading/trailing ``-`` (also stripping ``_``, due to point 2).
+
+    Intended to be used with :attr:`App.name_transform` and :attr:`Parameter.name_transform`.
+
+    Parameters
+    ----------
+    s: str
+        Input python identifier string.
+
+    Returns
+    -------
+    str
+        Transformed name.
+    """
+    return s.lower().replace("_", "-").strip("-")
```

### Comparing `cyclopts-2.5.0/cyclopts/validators/_group.py` & `cyclopts-2.6.0/cyclopts/validators/_group.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/validators/_number.py` & `cyclopts-2.6.0/cyclopts/validators/_number.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/cyclopts/validators/_path.py` & `cyclopts-2.6.0/cyclopts/validators/_path.py`

 * *Files identical despite different names*

### Comparing `cyclopts-2.5.0/pyproject.toml` & `cyclopts-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "cyclopts"
-version = "2.5.0"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "2.6.0"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/cyclopts"
 repository = "https://github.com/BrianPugh/cyclopts"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.md"
 packages = [{include = "cyclopts"}]
@@ -44,15 +44,15 @@
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = ">=5.1"}
 pre_commit = ">=2.16.0"
 pytest = ">=7.1.2"
 pytest-cov = ">=3.0.0"
 pytest-mock = ">=3.7.0"
-typer = "0.9.0"
+typer = "0.12.0"
 arguably = "^1.2.5"
 fire = ">=0.5,<0.7"
 pydantic = "^2.5.3"
 
 [tool.poetry.group.debug]
 optional = true
```

### Comparing `cyclopts-2.5.0/PKG-INFO` & `cyclopts-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclopts
-Version: 2.5.0
+Version: 2.6.0
 Summary: 
 Home-page: https://github.com/BrianPugh/cyclopts
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

