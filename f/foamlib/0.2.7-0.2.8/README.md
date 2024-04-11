# Comparing `tmp/foamlib-0.2.7.tar.gz` & `tmp/foamlib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foamlib-0.2.7.tar", last modified: Tue Apr  9 22:21:09 2024, max compression
+gzip compressed data, was "foamlib-0.2.8.tar", last modified: Thu Apr 11 16:25:11 2024, max compression
```

## Comparing `foamlib-0.2.7.tar` & `foamlib-0.2.8.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:09.252792 foamlib-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-09 22:21:04.000000 foamlib-0.2.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 22:21:09.252792 foamlib-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-09 22:21:04.000000 foamlib-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:09.248791 foamlib-0.2.7/foamlib/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:09.248791 foamlib-0.2.7/foamlib/_dictionaries/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_dictionaries/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12912 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_dictionaries/_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_dictionaries/_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_dictionaries/_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:04.000000 foamlib-0.2.7/foamlib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:09.248791 foamlib-0.2.7/foamlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-09 22:21:09.000000 foamlib-0.2.7/foamlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-09 22:21:09.000000 foamlib-0.2.7/foamlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:21:09.000000 foamlib-0.2.7/foamlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 22:21:09.000000 foamlib-0.2.7/foamlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 22:21:09.000000 foamlib-0.2.7/foamlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 22:21:04.000000 foamlib-0.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 22:21:09.252792 foamlib-0.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:21:09.248791 foamlib-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-09 22:21:04.000000 foamlib-0.2.7/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.893628 foamlib-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35131 2024-04-11 16:25:07.000000 foamlib-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-11 16:25:11.893628 foamlib-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-11 16:25:07.000000 foamlib-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20973 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib/_dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_dictionaries/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:07.000000 foamlib-0.2.8/foamlib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:25:11.889628 foamlib-0.2.8/foamlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:25:11.000000 foamlib-0.2.8/foamlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-11 16:25:07.000000 foamlib-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:25:11.893628 foamlib-0.2.8/setup.cfg
```

### Comparing `foamlib-0.2.7/LICENSE.txt` & `foamlib-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.7/PKG-INFO` & `foamlib-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.7/README.md` & `foamlib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.7/foamlib/_cases.py` & `foamlib-0.2.8/foamlib/_cases.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.7/foamlib/_dictionaries/_base.py` & `foamlib-0.2.8/foamlib/_dictionaries/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,22 +36,29 @@
         ] = ()
         name: Optional[str] = None
 
         def __post_init__(self) -> None:
             if not isinstance(self.dimensions, FoamDictionaryBase.DimensionSet):
                 self.dimensions = FoamDictionaryBase.DimensionSet(*self.dimensions)
 
-    Value = Union[str, int, float, bool, Dimensioned, DimensionSet, Sequence["Value"]]
+    Value = Union[
+        str,
+        int,
+        float,
+        bool,
+        Dimensioned,
+        DimensionSet,
+        Sequence["Value"],
+        Mapping[str, "Value"],
+    ]
     """
     A value that can be stored in an OpenFOAM dictionary.
     """
 
     _Dict = Dict[str, Union["Value", "_Dict"]]
 
     @abstractmethod
     def as_dict(self) -> _Dict:
         """Return a nested dict representation of the dictionary."""
         raise NotImplementedError
 
     _SetValue = Union[Value, "NDArray[np.generic]"]
-
-    _SetMapping = Mapping[str, Union["_SetValue", "_SetMapping"]]
```

### Comparing `foamlib-0.2.7/foamlib/_dictionaries/_files.py` & `foamlib-0.2.8/foamlib/_dictionaries/_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,19 +127,15 @@
             self._file._setitem(
                 (*self._keywords, keyword),
                 value,
                 assume_field=assume_field,
                 assume_dimensions=assume_dimensions,
             )
 
-        def __setitem__(
-            self,
-            keyword: str,
-            value: Union["FoamFile._SetValue", "FoamFile._SetMapping"],
-        ) -> None:
+        def __setitem__(self, keyword: str, value: "FoamFile._SetValue") -> None:
             self._setitem(keyword, value)
 
         def __delitem__(self, keyword: str) -> None:
             del self._file[(*self._keywords, keyword)]
 
         def __iter__(self) -> Iterator[str]:
             return self._file._iter(tuple(self._keywords))
@@ -187,15 +183,15 @@
             return FoamFile.Dictionary(self, keywords)
         else:
             return value
 
     def _setitem(
         self,
         keywords: Union[str, Tuple[str, ...]],
-        value: Union["FoamFile._SetValue", "FoamFile._SetMapping"],
+        value: "FoamFile._SetValue",
         *,
         assume_field: bool = False,
         assume_dimensions: bool = False,
     ) -> None:
         if not isinstance(keywords, tuple):
             keywords = (keywords,)
 
@@ -220,15 +216,15 @@
             self._write(
                 f"{contents[:start]}\n{serialize_entry(keywords[-1], value, assume_field=assume_field, assume_dimensions=assume_dimensions)}\n{contents[end:]}"
             )
 
     def __setitem__(
         self,
         keywords: Union[str, Tuple[str, ...]],
-        value: Union["FoamFile._SetValue", "FoamFile._SetMapping"],
+        value: "FoamFile._SetValue",
     ) -> None:
         self._setitem(keywords, value)
 
     def __delitem__(self, keywords: Union[str, Tuple[str, ...]]) -> None:
         if not isinstance(keywords, tuple):
             keywords = (keywords,)
 
@@ -280,23 +276,27 @@
 
 
 class FoamFieldFile(FoamFile):
     """An OpenFOAM dictionary file representing a field as a mutable mapping."""
 
     class BoundariesDictionary(FoamFile.Dictionary):
         def __getitem__(self, keyword: str) -> "FoamFieldFile.BoundaryDictionary":
-            return cast(FoamFieldFile.BoundaryDictionary, super().__getitem__(keyword))
+            value = super().__getitem__(keyword)
+            if not isinstance(value, FoamFieldFile.BoundaryDictionary):
+                assert not isinstance(value, FoamFile.Dictionary)
+                raise TypeError(f"boundary {keyword} is not a dictionary")
+            return value
 
     class BoundaryDictionary(FoamFile.Dictionary):
         """An OpenFOAM dictionary representing a boundary condition as a mutable mapping."""
 
         def __setitem__(
             self,
             key: str,
-            value: Union[FoamFile._SetValue, FoamFile._SetMapping],
+            value: FoamFile._SetValue,
         ) -> None:
             if key == "value":
                 self._setitem(key, value, assume_field=True)
             else:
                 self._setitem(key, value)
 
         @property
```

### Comparing `foamlib-0.2.7/foamlib/_dictionaries/_parsing.py` & `foamlib-0.2.8/foamlib/_dictionaries/_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import sys
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping, MutableMapping, Sequence
 else:
     from typing import Mapping, MutableMapping, Sequence
 
+if sys.version_info >= (3, 10):
+    from types import EllipsisType
+else:
+    from typing import Any as EllipsisType
+
 from pyparsing import (
     Dict,
     Forward,
     Group,
     Keyword,
     LineEnd,
     Literal,
@@ -52,43 +57,59 @@
         )
         | (
             common.integer + Literal("{").suppress() + elem + Literal("}").suppress()
         ).set_parse_action(lambda tks: [[tks[1]] * tks[0]])
     )
 
 
+def _dictionary_of(
+    keyword: ParserElement,
+    value: ParserElement,
+    *,
+    len: Union[int, EllipsisType] = ...,
+    located: bool = False,
+) -> ParserElement:
+    subdict = Forward()
+
+    entry = keyword + (
+        (Literal("{").suppress() + subdict + Literal("}").suppress())
+        | (value + Literal(";").suppress())
+    )
+
+    if located:
+        entry = Located(entry)
+
+    subdict <<= Dict(Group(entry)[...], asdict=not located)
+
+    return Dict(Group(entry)[len], asdict=not located)
+
+
 _TENSOR = _list_of(common.number) | common.number
 _IDENTIFIER = Word(identbodychars + "$", printables.replace(";", ""))
 _DIMENSIONED = (Opt(_IDENTIFIER) + _DIMENSIONS + _TENSOR).set_parse_action(
     lambda tks: FoamDictionaryBase.Dimensioned(*reversed(tks.as_list()))
 )
 _FIELD = (Keyword("uniform").suppress() + _TENSOR) | (
     Keyword("nonuniform").suppress() + _list_of(_TENSOR)
 )
 _TOKEN = QuotedString('"', unquote_results=False) | _IDENTIFIER
 _ITEM = Forward()
-_LIST = _list_of(_ITEM)
+_ENTRY = _dictionary_of(_IDENTIFIER, _ITEM, len=1)
+_LIST = _list_of(_ENTRY | _ITEM)
 _ITEM <<= _FIELD | _LIST | _DIMENSIONED | _DIMENSIONS | common.number | _SWITCH | _TOKEN
+
 _TOKENS = (
     QuotedString('"', unquote_results=False) | Word(printables.replace(";", ""))
 )[2, ...].set_parse_action(lambda tks: " ".join(tks))
 
 _VALUE = _ITEM ^ _TOKENS
 
-_ENTRY = Forward()
-_DICTIONARY = Dict(Group(_ENTRY)[...])
-_ENTRY <<= Located(
-    _TOKEN
-    + (
-        (Literal("{").suppress() + _DICTIONARY + Literal("}").suppress())
-        | (Opt(_VALUE, default="") + Literal(";").suppress())
-    )
-)
 _FILE = (
-    _DICTIONARY.ignore(c_style_comment)
+    _dictionary_of(_TOKEN, Opt(_VALUE, default=""), located=True)
+    .ignore(c_style_comment)
     .ignore(cpp_style_comment)
     .ignore(Literal("#include") + ... + LineEnd())  # type: ignore [no-untyped-call]
 )
 
 Parsed = Mapping[Sequence[str], Tuple[int, Optional[FoamDictionaryBase.Value], int]]
```

### Comparing `foamlib-0.2.7/foamlib/_dictionaries/_serialization.py` & `foamlib-0.2.8/foamlib/_dictionaries/_serialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import sys
 from contextlib import suppress
-from typing import Union
 
 if sys.version_info >= (3, 9):
     from collections.abc import Mapping
 else:
     from typing import Mapping
 
 from .._util import is_sequence
 from ._base import FoamDictionaryBase
 
 
-def _serialize_switch(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
-) -> str:
+def _serialize_switch(value: FoamDictionaryBase._SetValue) -> str:
     if value is True:
         return "yes"
     elif value is False:
         return "no"
     else:
         raise TypeError(f"Not a bool: {type(value)}")
 
 
 def _serialize_list(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
 ) -> str:
     if is_sequence(value):
         return f"({' '.join(_serialize_value(v) for v in value)})"
     else:
         raise TypeError(f"Not a valid sequence: {type(value)}")
 
 
 def _serialize_field(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
 ) -> str:
     if is_sequence(value):
         try:
             s = _serialize_list(value)
         except TypeError:
             raise TypeError(f"Not a valid field: {type(value)}") from None
         else:
@@ -57,36 +54,36 @@
                     )
                 return f"nonuniform List<{kind}> {len(value)}{s}"
     else:
         return f"uniform {value}"
 
 
 def _serialize_dimensions(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
 ) -> str:
     if is_sequence(value) and len(value) == 7:
         return f"[{' '.join(str(v) for v in value)}]"
     else:
         raise TypeError(f"Not a valid dimension set: {type(value)}")
 
 
 def _serialize_dimensioned(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
 ) -> str:
     if isinstance(value, FoamDictionaryBase.Dimensioned):
         if value.name is not None:
             return f"{value.name} {_serialize_dimensions(value.dimensions)} {_serialize_value(value.value)}"
         else:
             return f"{_serialize_dimensions(value.dimensions)} {_serialize_value(value.value)}"
     else:
         raise TypeError(f"Not a valid dimensioned value: {type(value)}")
 
 
 def _serialize_value(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
     *,
     assume_field: bool = False,
     assume_dimensions: bool = False,
 ) -> str:
     if isinstance(value, FoamDictionaryBase.DimensionSet) or assume_dimensions:
         with suppress(TypeError):
             return _serialize_dimensions(value)
@@ -100,29 +97,32 @@
 
     with suppress(TypeError):
         return _serialize_list(value)
 
     with suppress(TypeError):
         return _serialize_switch(value)
 
+    with suppress(TypeError):
+        return _serialize_dictionary(value)
+
     return str(value)
 
 
 def _serialize_dictionary(
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
 ) -> str:
     if isinstance(value, Mapping):
         return "\n".join(serialize_entry(k, v) for k, v in value.items())
     else:
         raise TypeError(f"Not a valid dictionary: {type(value)}")
 
 
 def serialize_entry(
     keyword: str,
-    value: Union[FoamDictionaryBase._SetValue, FoamDictionaryBase._SetMapping],
+    value: FoamDictionaryBase._SetValue,
     *,
     assume_field: bool = False,
     assume_dimensions: bool = False,
 ) -> str:
     try:
         return f"{keyword}\n{{\n{_serialize_dictionary(value)}\n}}"
     except TypeError:
```

### Comparing `foamlib-0.2.7/foamlib/_util.py` & `foamlib-0.2.8/foamlib/_util.py`

 * *Files identical despite different names*

### Comparing `foamlib-0.2.7/foamlib.egg-info/PKG-INFO` & `foamlib-0.2.8/foamlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foamlib
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python interface for interacting with OpenFOAM
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/foamlib
 Project-URL: Repository, https://github.com/gerlero/foamlib
 Project-URL: Documentation, https://foamlib.readthedocs.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

### Comparing `foamlib-0.2.7/pyproject.toml` & `foamlib-0.2.8/pyproject.toml`

 * *Files identical despite different names*

