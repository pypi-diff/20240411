# Comparing `tmp/lenient_string_formatter-1.0.0.tar.gz` & `tmp/lenient_string_formatter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenient_string_formatter-1.0.0.tar", max compression
+gzip compressed data, was "lenient_string_formatter-1.0.1.tar", max compression
```

## Comparing `lenient_string_formatter-1.0.0.tar` & `lenient_string_formatter-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-04-10 14:07:44.723040 lenient_string_formatter-1.0.0/LICENSE
--rw-r--r--   0        0        0     3784 2024-04-10 14:07:44.723040 lenient_string_formatter-1.0.0/README.md
--rw-r--r--   0        0        0      226 2024-04-10 14:07:44.723040 lenient_string_formatter-1.0.0/lenient_string_formatter/__init__.py
--rw-r--r--   0        0        0     4737 2024-04-10 14:07:44.723040 lenient_string_formatter-1.0.0/lenient_string_formatter/lenient_formatter.py
--rw-r--r--   0        0        0        1 2024-04-10 14:07:44.723040 lenient_string_formatter-1.0.0/lenient_string_formatter/py.typed
--rw-r--r--   0        0        0      851 2024-04-10 14:07:52.398915 lenient_string_formatter-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 lenient_string_formatter-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 15:10:33.360262 lenient_string_formatter-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3784 2024-04-10 15:10:33.360262 lenient_string_formatter-1.0.1/README.md
+-rw-r--r--   0        0        0      226 2024-04-10 15:10:33.360262 lenient_string_formatter-1.0.1/lenient_string_formatter/__init__.py
+-rw-r--r--   0        0        0     4583 2024-04-10 15:10:33.360262 lenient_string_formatter-1.0.1/lenient_string_formatter/lenient_formatter.py
+-rw-r--r--   0        0        0        1 2024-04-10 15:10:33.360262 lenient_string_formatter-1.0.1/lenient_string_formatter/py.typed
+-rw-r--r--   0        0        0      851 2024-04-10 15:10:43.524389 lenient_string_formatter-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 lenient_string_formatter-1.0.1/PKG-INFO
```

### Comparing `lenient_string_formatter-1.0.0/LICENSE` & `lenient_string_formatter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lenient_string_formatter-1.0.0/README.md` & `lenient_string_formatter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lenient_string_formatter-1.0.0/lenient_string_formatter/lenient_formatter.py` & `lenient_string_formatter-1.0.1/lenient_string_formatter/lenient_formatter.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 
 class LenientFormatter(Formatter):
     """A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising exceptions.
 
     The following exceptions that are normally raised by the built-in string formatter are caught and handled as follows:
 
-        - KeyError and IndexError will not be raised if a field in the template is not matched by the arguments. Instead, the field will be left untouched in the output string.
-        - ValueError in case numbered and auto-numbered fields are mixed in the template (e.g. "{1} {}") will not be raised. Explicitly numbered fields will be matched according to their index (remaining untouched if the index is out of bounds), while auto-numbered fields will be matched according to their order in the arguments (again, remaining untouched if the index is out of bounds) independent of the explicit numbering.
-        - KeyError is not raised on unnumbered field with key/attribute access. (https://bugs.python.org/issue27307)
+    - KeyError and IndexError will not be raised if a field in the template is not matched by the arguments. Instead, the field will be left untouched in the output string.
+    - ValueError in case numbered and auto-numbered fields are mixed in the template (e.g. "{1} {}") will not be raised. Explicitly numbered fields will be matched according to their index (remaining untouched if the index is out of bounds), while auto-numbered fields will be matched according to their order in the arguments (again, remaining untouched if the index is out of bounds) independent of the explicit numbering.
+    - KeyError is not raised on unnumbered field with key/attribute access. (https://bugs.python.org/issue27307)
     """
 
     def vformat(
         self, format_string: str, args: Sequence[Any], kwargs: Mapping[str, Any]
     ) -> str:
         return _DisposableLenientFormatter().vformat(format_string, args, kwargs)
 
@@ -28,73 +28,72 @@
     Due to the stateful nature of this implementation (i.e. the auto-numbering is handled by an internal counter), this class should not be reused, and is therefore private and used only by the public LenientFormatter class.
     """
 
     def __init__(self) -> None:
         self.indexer = itertools.count()
         self._stale = False
         self.used_args = set()
-        self.recursion_depth = 2
 
     def vformat(
         self, format_string: str, args: Sequence[Any], kwargs: Mapping[str, Any]
     ) -> str:
         assert not self._stale, f"{type(self).__name__} must not be reused"
         self._stale = True
-        result, _ = self._vformat_lenient(format_string, args, kwargs)
+        result, _ = self._vformat_lenient(format_string, args, kwargs, 2)
         self.check_unused_args(self.used_args, args, kwargs)
         return result
 
     def get_value(
         self, key: str | int, args: Sequence[Any], kwargs: Mapping[str, Any]
     ) -> Any:
         try:
-            return super().get_value(key or next(self.indexer), args, kwargs)
+            return super().get_value(
+                key if key != "" else next(self.indexer), args, kwargs
+            )
         except (IndexError, KeyError):
             return _MISSING
 
     def _vformat_lenient(
-        self, format_string: str, args: Sequence[Any], kwargs: Mapping[str, Any]
+        self,
+        format_string: str,
+        args: Sequence[Any],
+        kwargs: Mapping[str, Any],
+        depth: int,
     ) -> tuple[str, bool]:
-        self._check_recursion()
+        if depth < 0:
+            raise ValueError("Max string recursion exceeded")
         result: list[tuple[str, bool]] = []
-        for literal_text, field_name, format_spec, conversion in self.parse(
-            format_string
-        ):
-            if literal_text:
-                result.append((literal_text, True))
+        for literal_text, field_name, spec, conversion in self.parse(format_string):
+            result.append((literal_text, True))
             if field_name is None:
                 continue
-            assert format_spec is not None
+            assert spec is not None
             result.append(
-                self._replace_field(field_name, conversion, format_spec, args, kwargs)
+                self._replace_field(field_name, conversion, spec, args, kwargs, depth)
             )
         return "".join(part for part, _ in result), all(known for _, known in result)
 
-    def _check_recursion(self) -> None:
-        if self.recursion_depth < 0:
-            raise ValueError("Max string recursion exceeded")
-        self.recursion_depth -= 1
-
     def _replace_field(
         self,
         field_name: str,
         conversion: str | None,
-        format_spec: str,
+        spec: str,
         args: Sequence[Any],
         kwargs: Mapping[str, Any],
+        depth: int,
     ) -> tuple[str, bool]:
         obj, arg_used = self.get_field(field_name, args, kwargs)
         if obj is _MISSING:
-            return str(_Unmatched(field_name, conversion, format_spec)), False
+            return str(_Unmatched(field_name, conversion, spec)), False
         obj = self.convert_field(obj, conversion)
-        new_format_spec, known = self._vformat_lenient(format_spec, args, kwargs)
+        new_spec, known = self._vformat_lenient(spec, args, kwargs, depth - 1)
         if not known:
-            return str(_Unmatched(field_name, conversion, format_spec)), False
+            return str(_Unmatched(field_name, conversion, spec)), False
         self.used_args.add(arg_used)
-        return self.format_field(obj, new_format_spec), True
+        return self.format_field(obj, new_spec), True
 
 
 class _Missing:
     """Objects representing a field that could not be matched by the arguments and are to be left untouched."""
 
     def __getitem__(self, key: object) -> Self:
         return self
```

### Comparing `lenient_string_formatter-1.0.0/pyproject.toml` & `lenient_string_formatter-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "lenient-string-formatter"
 # Version is overwritten at build time by CI based on git tag
-version = "1.0.0"
+version = "1.0.1"
 description = "A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising a KeyError."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-lenient-string-formatter"
 documentation = "https://abrahammurciano.github.io/python-lenient-string-formatter/lenient-string-formatter"
 keywords = []
```

### Comparing `lenient_string_formatter-1.0.0/PKG-INFO` & `lenient_string_formatter-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenient-string-formatter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising a KeyError.
 Home-page: https://github.com/abrahammurciano/python-lenient-string-formatter
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

