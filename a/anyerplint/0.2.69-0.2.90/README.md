# Comparing `tmp/anyerplint-0.2.69.tar.gz` & `tmp/anyerplint-0.2.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyerplint-0.2.69.tar", last modified: Tue Mar 19 14:38:36 2024, max compression
+gzip compressed data, was "anyerplint-0.2.90.tar", last modified: Thu Apr 11 05:37:03 2024, max compression
```

## Comparing `anyerplint-0.2.69.tar` & `anyerplint-0.2.90.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 14:38:36.169130 anyerplint-0.2.69/
--rw-rw-rw-   0        0        0      628 2024-03-19 14:38:36.167027 anyerplint-0.2.69/PKG-INFO
--rw-rw-rw-   0        0        0       91 2023-11-03 12:54:20.000000 anyerplint-0.2.69/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 14:38:36.120219 anyerplint-0.2.69/anyerplint/
--rw-rw-rw-   0        0        0      233 2023-09-20 08:47:10.000000 anyerplint-0.2.69/anyerplint/__init__.py
--rw-rw-rw-   0        0        0       80 2023-09-20 08:47:10.000000 anyerplint-0.2.69/anyerplint/__main__.py
--rw-rw-rw-   0        0        0      280 2024-03-01 20:38:38.000000 anyerplint-0.2.69/anyerplint/ast.py
--rw-rw-rw-   0        0        0    20288 2024-02-01 12:48:23.000000 anyerplint-0.2.69/anyerplint/business_logic.py
-drwxrwxrwx   0        0        0        0 2024-03-19 14:38:36.151042 anyerplint-0.2.69/anyerplint/cli/
--rw-rw-rw-   0        0        0        0 2023-09-20 08:47:10.000000 anyerplint-0.2.69/anyerplint/cli/__init__.py
--rw-rw-rw-   0        0        0     1107 2024-03-01 20:38:32.000000 anyerplint-0.2.69/anyerplint/cli/check.py
--rw-rw-rw-   0        0        0     1577 2024-01-03 11:53:45.000000 anyerplint-0.2.69/anyerplint/cli/importcmd.py
--rw-rw-rw-   0        0        0     1717 2023-12-13 14:41:26.000000 anyerplint-0.2.69/anyerplint/cli/initcmd.py
--rw-rw-rw-   0        0        0     1017 2024-03-19 14:16:59.000000 anyerplint-0.2.69/anyerplint/cli/main.py
--rw-rw-rw-   0        0        0     5424 2024-03-01 20:38:38.000000 anyerplint-0.2.69/anyerplint/cli/parsecmd.py
--rw-rw-rw-   0        0        0     2492 2024-01-17 11:49:24.000000 anyerplint-0.2.69/anyerplint/preprocessor.py
--rw-rw-rw-   0        0        0      107 2023-12-21 14:28:43.000000 anyerplint-0.2.69/anyerplint/recursive_list.py
--rw-rw-rw-   0        0        0     4847 2024-03-01 20:38:38.000000 anyerplint-0.2.69/anyerplint/tnex.py
--rw-rw-rw-   0        0        0     7460 2024-03-19 14:15:50.000000 anyerplint-0.2.69/anyerplint/translate.py
--rw-rw-rw-   0        0        0     2676 2024-01-09 08:12:37.000000 anyerplint-0.2.69/anyerplint/util.py
--rw-rw-rw-   0        0        0        8 2024-03-19 14:38:13.000000 anyerplint-0.2.69/anyerplint/version.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 14:38:36.164911 anyerplint-0.2.69/anyerplint.egg-info/
--rw-rw-rw-   0        0        0      628 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 14:38:36.000000 anyerplint-0.2.69/anyerplint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1621 2024-03-19 14:25:12.000000 anyerplint-0.2.69/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-19 14:38:36.169130 anyerplint-0.2.69/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-19 14:38:36.160598 anyerplint-0.2.69/test/
--rw-rw-rw-   0        0        0     2692 2024-01-17 11:49:24.000000 anyerplint-0.2.69/test/test_business_logic.py
--rw-rw-rw-   0        0        0      589 2024-01-17 11:49:24.000000 anyerplint-0.2.69/test/test_preprocess.py
--rw-rw-rw-   0        0        0     3497 2024-03-01 20:38:38.000000 anyerplint-0.2.69/test/test_tnex.py
--rw-rw-rw-   0        0        0      674 2024-03-19 13:26:43.000000 anyerplint-0.2.69/test/test_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.559095 anyerplint-0.2.90/
+-rw-rw-rw-   0        0        0      628 2024-04-11 05:37:03.558066 anyerplint-0.2.90/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2023-11-03 12:54:20.000000 anyerplint-0.2.90/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.531374 anyerplint-0.2.90/anyerplint/
+-rw-rw-rw-   0        0        0      233 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/__main__.py
+-rw-rw-rw-   0        0        0      391 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/ast.py
+-rw-rw-rw-   0        0        0    19517 2024-04-11 05:36:25.000000 anyerplint-0.2.90/anyerplint/business_logic.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.548651 anyerplint-0.2.90/anyerplint/cli/
+-rw-rw-rw-   0        0        0        0 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/cli/__init__.py
+-rw-rw-rw-   0        0        0     1107 2024-03-01 20:38:32.000000 anyerplint-0.2.90/anyerplint/cli/check.py
+-rw-rw-rw-   0        0        0     1594 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/importcmd.py
+-rw-rw-rw-   0        0        0     1718 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/initcmd.py
+-rw-rw-rw-   0        0        0     1015 2024-03-20 13:30:28.000000 anyerplint-0.2.90/anyerplint/cli/main.py
+-rw-rw-rw-   0        0        0     5390 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/parsecmd.py
+-rw-rw-rw-   0        0        0     2493 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/preprocessor.py
+-rw-rw-rw-   0        0        0      107 2023-12-21 14:28:43.000000 anyerplint-0.2.90/anyerplint/recursive_list.py
+-rw-rw-rw-   0        0        0     4852 2024-03-20 14:24:28.000000 anyerplint-0.2.90/anyerplint/tnex.py
+-rw-rw-rw-   0        0        0     7531 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/translate.py
+-rw-rw-rw-   0        0        0     2676 2024-01-09 08:12:37.000000 anyerplint-0.2.90/anyerplint/util.py
+-rw-rw-rw-   0        0        0        8 2024-04-11 05:36:43.000000 anyerplint-0.2.90/anyerplint/version.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.557033 anyerplint-0.2.90/anyerplint.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2024-03-20 14:24:28.000000 anyerplint-0.2.90/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 05:37:03.560127 anyerplint-0.2.90/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.554652 anyerplint-0.2.90/test/
+-rw-rw-rw-   0        0        0     2617 2024-04-11 05:36:25.000000 anyerplint-0.2.90/test/test_business_logic.py
+-rw-rw-rw-   0        0        0      589 2024-01-17 11:49:24.000000 anyerplint-0.2.90/test/test_preprocess.py
+-rw-rw-rw-   0        0        0     3507 2024-03-20 13:30:36.000000 anyerplint-0.2.90/test/test_tnex.py
+-rw-rw-rw-   0        0        0      674 2024-03-19 13:26:43.000000 anyerplint-0.2.90/test/test_translate.py
```

### Comparing `anyerplint-0.2.69/PKG-INFO` & `anyerplint-0.2.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyerplint
-Version: 0.2.69
+Version: 0.2.90
 Summary: anyerplint
 Project-URL: Homepage, https://github.com/Basware/anyerplint
 Project-URL: Repository, https://github.com/Basware/anyerplint
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyerplint-0.2.69/anyerplint/business_logic.py` & `anyerplint-0.2.90/anyerplint/business_logic.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,53 +18,53 @@
 
 
 ReportData = TypedDict(
     "ReportData",
     {
         "Unknown variables": list[str],
         "Unknown calls": list[str],
-        "Unknown functions": list[str],
         "Unknown jumps": list[str],
         "Unknown tags": list[str],
         "Other errors": list[str],
         "Expression errors": list[dict[str, str | list[str]]],
         "Unknown loop variables": list[str],
     },
     total=False,
 )
 
 
 @dataclass
 class Library:
+    """Stores known symbols from the 'standard library'."""
+
     variables: set[str]
     loopvariables: set[str]
     calls: set[str]
-    functions: set[str]
     jumps: set[str]
     tags: set[str]
     # if true, accumulate everything found to library
     teaching: bool
 
 
 # ruff lead this alone man
 emit = print
 
 
 def do_check(
     libs: list[str],
     targets: list[str],
     teaching: bool,
+    *,
     nostdlib: bool = False,
 ) -> dict[str, str | ReportData]:
     emit(f"AnyErpLintVersion: {__version__.strip()}")
 
     lib_vars = Library(
         variables=set(),
         calls=set(),
-        functions=set(),
         jumps=set(),
         tags=set(),
         teaching=teaching,
         loopvariables=set(),
     )
 
     # always feed the "standard library, except when unit testing (nostdlib)
@@ -88,15 +88,15 @@
     if lib_vars.teaching:
         write_lib(lib_vars)
 
     if has_errors:
         emit("Errors found: >")
         error_counts = {
             f: (
-                sum(len(l) for l in e.values() if isinstance(l, list))
+                sum(len(prop) for prop in e.values() if isinstance(prop, list))
                 if not isinstance(e, str)
                 else -1
             )
             for f, e in all_errors.items()
         }
         rep = sorted((k, v) for (k, v) in error_counts.items())
         for line in rep:
@@ -104,64 +104,59 @@
 
     return all_errors
 
 
 def write_lib(lib_vars: Library) -> None:
     def write_file(fname: Path, lines: list[str]) -> None:
         emit("  - ", fname)
-        f = open(fname, "wb")
-        for line in lines:
-            try:
-                if not line.strip().isascii():
+        with fname.open("wb") as f:
+            for line in lines:
+                try:
+                    if not line.strip().isascii():
+                        continue
+                    enc = line.strip().encode()
+                except UnicodeEncodeError:
+                    # skip bad lines for now
                     continue
-                enc = line.strip().encode()
-            except UnicodeEncodeError:
-                # skip bad lines for now
-                continue
-            f.write(enc)
-            f.write(b"\n")
+                f.write(enc)
+                f.write(b"\n")
 
     emit("Writing found function to:")
 
     stdlib = util.get_app_local_dir()
     calls_file = stdlib / "builtin_calls.txt"
     write_file(
         calls_file,
         sorted(call for call in lib_vars.calls if is_valid_call(call)),
     )
 
-    functions_file = stdlib / "builtin_functions.txt"
-    write_file(functions_file, sorted(lib_vars.functions))
-
     jumps_file = stdlib / "builtin_jumps.txt"
     write_file(jumps_file, sorted(lib_vars.jumps))
 
     tags_file = stdlib / "builtin_tags.txt"
     write_file(tags_file, sorted(lib_vars.tags))
 
     vars_file = stdlib / "builtin_vars.txt"
     write_file(vars_file, sorted(lib_vars.variables))
 
     loopvars_file = stdlib / "builtin_loopvars.txt"
     write_file(loopvars_file, sorted({lv.lower() for lv in lib_vars.loopvariables}))
 
 
-def is_valid_call(call: str) -> bool:
+def is_valid_call(_call: str) -> bool:
     return True
 
 
 def feed_lib(lib_vars: Library, libdir: Path) -> None:
-    def feed_set(set: set[str], fobj: IO[bytes]) -> None:
-        set.update(line.decode().strip() for line in fobj.readlines())
+    def feed_set(dest: set[str], fobj: IO[bytes]) -> None:
+        dest.update(line.decode().strip() for line in fobj.readlines())
 
     def visit_file(fname: str, fobj: IO[bytes]) -> None:
         if fname.endswith("_calls.txt"):
             feed_set(lib_vars.calls, fobj)
-        elif fname.endswith("_functions.txt"):
-            feed_set(lib_vars.functions, fobj)
         elif fname.endswith("_jumps.txt"):
             feed_set(lib_vars.jumps, fobj)
         elif fname.endswith("_tags.txt"):
             feed_set(lib_vars.tags, fobj)
         elif fname.endswith("_vars.txt"):
             feed_set(lib_vars.variables, fobj)
         elif fname.endswith("_loopvars.txt"):
@@ -197,15 +192,15 @@
 
 
 def check_file(lib_vars: Library, file: Path) -> str | ReportData | None:
     try:
         if should_skip_file(file):
             emit(f"{file}: SKIP nontemplate")
             return None
-        r = parse_file(file, lib_vars.teaching)
+        r = parse_file(file, teaching=lib_vars.teaching)
     except (
         ElementTree.ParseError,
         PermissionError,
         UnicodeDecodeError,
         preprocessor.PreprocessError,
     ) as e:
         return report_fatal(file, e)
@@ -223,34 +218,37 @@
             errs[str(f)] = errlist
 
     return errs
 
 
 @dataclass
 class ExprError:
+    """Represents an error in an expression."""
+
     summary: str
     translated: str
     messages: list[str]
 
     def render(self) -> dict[str, str | list[str]]:
-        """Render yaml compatible object"""
+        """Render yaml compatible object."""
         return {"Error": self.summary, "Simple": self.translated, "Msg": self.messages}
 
 
 @dataclass
 class Parsed:
+    """The things found while parsing a file."""
+
     var_decl: set[str]
     var_used: set[str]
     alltags: set[str]
     calls: set[str]
     jumps: set[str]
     syntax_errors: list[str]
     loop_var_decl: set[str]
     loop_var_use: set[str]
-    used_functions: set[str]
     expression_errors: list[ExprError]
     full_content: str
 
 
 def report(lib_vars: Library, fname: str, p: Parsed) -> ReportData:
     undeclared_vars = p.var_used - p.var_decl
     undeclared_vars.difference_update(lib_vars.variables)
@@ -259,15 +257,14 @@
         for lv in p.loop_var_use
         if lv.lower() not in p.loop_var_decl
         and lv.lower() not in lib_vars.loopvariables
     }
 
     if lib_vars.teaching:
         lib_vars.calls.update(p.calls)
-        lib_vars.functions.update(f for f in p.used_functions if f.isupper())
         lib_vars.jumps.update(p.jumps)
         lib_vars.tags.update(p.alltags)
         lib_vars.variables.update(undeclared_vars)
         lib_vars.loopvariables.update(lv.lower() for lv in unknown_loop_variables)
 
     errors: ReportData = {}
 
@@ -278,22 +275,14 @@
         )
 
     unknown_calls = p.calls
     unknown_calls.difference_update(lib_vars.calls)
     if unknown_calls:
         errors["Unknown calls"] = sorted(unknown_calls)
 
-    unknown_functions = p.used_functions
-    unknown_functions.difference_update(lib_vars.functions)
-    if unknown_functions:
-        errors["Unknown functions"] = util.add_linenumbers(
-            p.full_content,
-            sorted(unknown_functions),
-        )
-
     unknown_jumps = p.jumps
     unknown_jumps.difference_update(lib_vars.jumps)
     if unknown_jumps:
         errors["Unknown jumps"] = sorted(unknown_jumps)
 
     unknown_tags = p.alltags
     unknown_tags.difference_update(lib_vars.tags)
@@ -336,18 +325,18 @@
         suboperation = params.get(suboperation_param_name, "UNK")
         full += "." + suboperation
 
     return (full + " - " + ",".join(sorted(params))).strip()
 
 
 def summarize_output(node: Element) -> str:
-    type = node.attrib.get("type", "NOTYPE")
+    output_type = node.attrib.get("type", "NOTYPE")
     params = {p.attrib.get("name", "NONAME") for p in node.iter("parameter")}
 
-    return ("Output " + type + " - " + ",".join(sorted(params))).strip()
+    return ("Output " + output_type + " - " + ",".join(sorted(params))).strip()
 
 
 def summarize_tag(node: Element) -> str:
     at = " " + " ".join(sorted(node.attrib.keys())) if node.attrib else ""
     return "<" + node.tag + at + ">"
 
 
@@ -386,25 +375,21 @@
                         f"Expected brace {expected}, got {ch} at line {lnum} col {cnum}: {line.strip()}",
                     )
                     flush_stack = True
                     break
         if flush_stack:
             stack = []
     if stack:
-        pretty_stack = ", ".join(f"{ch} {l}" for ch, l in stack)
+        pretty_stack = ", ".join(f"{ch} {lnum}" for ch, lnum in stack)
         errors.append(
             f"File ended with mismatched braces, remaining in stack (char, linenum): {pretty_stack}",
         )
     return errors
 
 
-# xxx not really needed due to new logic
-MAGIC_VAR_NAMES = {"error", "return", "response", "invoice.i"}
-
-
 def describe_node(n: Element) -> str:
     return "<" + n.tag + str(n.attrib) + ">"
 
 
 def describe_jump(n: Element) -> str:
     params = sorted(
         child.attrib.get("name", "NONAME").strip() for child in n.iter("parameter")
@@ -530,15 +515,15 @@
                     translated=translated,
                     messages=errors,
                 )
             )
     return res
 
 
-def parse_file(fname: str | Path, teaching: bool = False) -> Parsed:
+def parse_file(fname: str | Path, *, teaching: bool = False) -> Parsed:
     tree = ElementTree.parse(fname)
     raw_cont = util.open_text_file(fname).read()
     comments_removed = util.replace_commented_xml_with_empty_lines(raw_cont)
 
     vardecl = {
         v.attrib.get("name", "unknown_var"): (v.text or "")
         for v in tree.iter("variable")
@@ -554,23 +539,17 @@
 
     propaccess = {
         (match.group(1), match.group(2))
         for expr, line in expressions
         for match in re.finditer(prop_regex, expr)
     }
     varuse = {name for expr_type, name in propaccess if expr_type.lower() == "v"}
-    used_functions = {
-        expr_type + "," + name
-        for expr_type, name in propaccess
-        if expr_type.lower() == "f"
-    }
 
     # what to do with p params?
     otherpropaccess = {k for k, v in propaccess if k.lower() not in ["v", "f", "p"]}
-    otherpropaccess.difference_update(MAGIC_VAR_NAMES)
     calls = {summarize_call(v) for v in tree.iter("builtInMethodParameterList")}
     outputs = {summarize_output(v) for v in tree.iter("output")}
     calls.update(outputs)
     alltags = {summarize_tag(t) for t in tree.iter()}
     loop_data_source_attribs = {n.attrib.get("loopDataSource") for n in tree.iter()}
     loop_data_sources = {
         ls.split(";")[0].lower() for ls in loop_data_source_attribs if ls
@@ -623,14 +602,13 @@
 
     return Parsed(
         var_decl=set(vardecl),
         var_used=varuse,
         alltags=alltags,
         calls=calls,
         jumps=jumps,
-        used_functions=used_functions,
         syntax_errors=errors,
         loop_var_decl=loop_data_sources,
         loop_var_use=otherpropaccess,
         full_content=comments_removed,
         expression_errors=expr_errors,
     )
```

### Comparing `anyerplint-0.2.69/anyerplint/cli/check.py` & `anyerplint-0.2.90/anyerplint/cli/check.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.69/anyerplint/cli/importcmd.py` & `anyerplint-0.2.90/anyerplint/cli/importcmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import os
 import shutil
 import urllib.error
 import urllib.request
 from pathlib import Path
 
 from anyerplint import util
 
@@ -25,27 +24,27 @@
 
 
 emit = print
 
 
 def do_import(fnames: list[str]) -> None:
     target_dir = util.get_app_local_dir()
-    if not os.path.isdir(target_dir):
-        os.makedirs(target_dir)
+    if not target_dir.is_dir():
+        target_dir.mkdir(parents=True)
     for f in fnames:
-        if f.startswith("http"):
+        if f.startswith(("http:", "https:")):
             lastpart = f.split("/")[-1]
             emit(lastpart)
 
             if not lastpart.endswith(".zip"):
                 lastpart = "downloaded.zip"
             tfile = Path(target_dir) / lastpart
             emit("Fething:", f, "->", tfile)
             try:
-                urllib.request.urlretrieve(f, tfile)
+                urllib.request.urlretrieve(f, tfile)  # noqa: S310
             except urllib.error.URLError:
                 emit(
                     "Failed to download, ensure your VPN is operational and the target file exists!"
                 )
         elif f.endswith(".zip"):
             emit("Copying:", f, "->", target_dir)
             shutil.copy(f, target_dir)
```

### Comparing `anyerplint-0.2.69/anyerplint/cli/initcmd.py` & `anyerplint-0.2.90/anyerplint/cli/initcmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   ]
 }
 """
 
 emit = print
 
 
-def handle_init(args: argparse.Namespace) -> None:
+def handle_init(_args: argparse.Namespace) -> None:
     init_vscode()
 
 
 def init_parser(parser: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """Declare arguments you need here."""
     parser.set_defaults(func=handle_init)
     return parser
```

### Comparing `anyerplint-0.2.69/anyerplint/cli/main.py` & `anyerplint-0.2.90/anyerplint/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,10 +29,9 @@
         subparsers.add_parser("init", help="Initialize vscode integration")
     )
 
     parsecmd.init_parser(
         subparsers.add_parser("parse", help="Parse and check expressions in templates")
     )
 
-
     args = main_parser.parse_args()
     args.func(args)
```

### Comparing `anyerplint-0.2.69/anyerplint/cli/parsecmd.py` & `anyerplint-0.2.90/anyerplint/cli/parsecmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         parsed = parse(exp[0])
         if not isinstance(parsed, FuncCall):
             continue
         hits = search_calls(parsed, func_name=func_name)
         for hit in hits:
             printed = pretty_flat_call(hit)
             with contextlib.suppress(UnicodeEncodeError):
-                print(str(fname) + " ; " + printed)
+                emit(str(fname) + " ; " + printed)
 
 
 def print_formatted_expression(
     exp: str, linenum: int, errors_only: bool, log_all: bool
 ) -> None:
     try:
         parsed = parse(exp)
@@ -130,17 +130,15 @@
 
 
 def handle_parse(args: argparse.Namespace) -> None:
     errors_only = args.errors
     console.no_color = args.no_color
     if args.fun:
         if not args.filename:
-            print(
-                "With 'parse --fun' mode, you must specify file or directory to check"
-            )
+            emit("With 'parse --fun' mode, you must specify file or directory to check")
             return
         for pat in args.filename:
             fnames = glob_plus(pat)
             for f in fnames:
                 with contextlib.suppress(
                     PreprocessError, ParseError, UnicodeDecodeError, PermissionError
                 ):
```

### Comparing `anyerplint-0.2.69/anyerplint/preprocessor.py` & `anyerplint-0.2.90/anyerplint/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from collections.abc import Iterable
 
 from anyerplint import util
 
 
 class PreprocessError(Exception):
-    """Raised by preprocessor"""
+    """Raised by preprocessor."""
 
 
 def tokenize(cont: str) -> list[str]:
     return re.split(r"([{}\"])", cont)
 
 
 def walk_tokens(toks: list[str]) -> Iterable[tuple[str, int]]:
```

### Comparing `anyerplint-0.2.69/anyerplint/tnex.py` & `anyerplint-0.2.90/anyerplint/tnex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """tnex - Trivial Nested EXpressions.
 
 Easier to read/write than s-expr's I guess
 
 """
+
 import re
 
 from anyerplint import util
 from anyerplint.ast import Expression, FuncCall, SpecialToken
 
 
 def tokenize(s: str) -> list[str]:
@@ -120,15 +121,15 @@
                 add_empty_arg = False
                 res.append(it.strip())
                 i += 1
 
     return (res, i + 1)
 
 
-def parse(s: str, expand_entities: bool = True) -> Expression:
+def parse(s: str, *, expand_entities: bool = True) -> Expression:
     if expand_entities:
         s = expand_xml_entities(s)
     tokens = tokenize(s)
     parsed, _ = emit_nested_sequence(tokens, top_level=True)
     if not parsed:
         msg = f"Empty parse result for expression: '{s}'"
         raise ParseError(msg)
```

### Comparing `anyerplint-0.2.69/anyerplint/translate.py` & `anyerplint-0.2.90/anyerplint/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from anyerplint.ast import Expression, FuncCall, SpecialToken
+from anyerplint.ast import Expression, SpecialToken
 from anyerplint.tnex import ParseError, parse
 
 
 def removequote(s: str) -> str:
     return s.removeprefix('"').removesuffix('"')
 
 
@@ -28,15 +28,14 @@
 
 # some 'trivial' translations
 nullary_funcs = {
     "F,GUID",
     "F,NOW",
 }
 # these will be translated to name(arg1; arg2)
-# xxx remove the mixed case variants
 nnary_funcs: dict[str, int | tuple[int, int]] = {
     "F,ADDXMLNS": 3,
     "F,CSV": (2, 3),
     "F,DATEADD": 3,
     "F,DATEDIFF": 3,
     "F,DBSELECT": (2, 999),
     "F,FLOOR": 1,
@@ -54,15 +53,18 @@
     "F,SAPSELECT": (6, 12),
     "F,SAPSELECTWS": (7, 12),
     "F,XMLENCODE": 1,
 }
 
 
 class Translator:
+    """Translates expressions into a simpler form."""
+
     def __init__(self) -> None:
+        """Initialize a translator with empty error list."""
         self.errors: list[str] = []
 
     def translate(self, tree: Expression) -> str:
         """Convert to pretty mostly-infix notation."""
         # only function calls are translated
         if tree == SpecialToken.EmptyArgument:
             return ""
```

### Comparing `anyerplint-0.2.69/anyerplint/util.py` & `anyerplint-0.2.90/anyerplint/util.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.69/anyerplint.egg-info/PKG-INFO` & `anyerplint-0.2.90/anyerplint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyerplint
-Version: 0.2.69
+Version: 0.2.90
 Summary: anyerplint
 Project-URL: Homepage, https://github.com/Basware/anyerplint
 Project-URL: Repository, https://github.com/Basware/anyerplint
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyerplint-0.2.69/anyerplint.egg-info/SOURCES.txt` & `anyerplint-0.2.90/anyerplint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.69/pyproject.toml` & `anyerplint-0.2.90/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -39,20 +39,25 @@
 Repository = "https://github.com/Basware/anyerplint"
 
 [project.scripts]
 anyerplint = "anyerplint.__main__:main"
 
 [tool.ruff]
 target-version = "py310"
+
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = [
+    "ANN101",  # Missing type annotation for self in method
     "COM812",  # Missing trailing comma
     "D100",  # Missing docstring in public module
-    "D104",  # Missing docstring in public package
     "D103",  # Missing docstring in public function
+    "D104",  # Missing docstring in public package
+    "D203",  # One blank line before class
+    "D213",  # Multi-line docstring summary should start at the second line
     "E501",  # Line too long
     "FBT001",  # Boolean-typed positional argument in function definition
     "ISC001",  # Single-line implicit string concatenation
 ]
 
 [tool.pytest.ini_options]
 filterwarnings = "ignore:.*:DeprecationWarning"
```

### Comparing `anyerplint-0.2.69/test/test_business_logic.py` & `anyerplint-0.2.90/test/test_business_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,14 @@
     assert errs == expected
 
 
 def test_check_expressions() -> None:
     input_file = root / "expressions.xml"
     res = business_logic.do_check([], [str(input_file)], teaching=False, nostdlib=True)
     expected = {
-        "Unknown functions": [
-            "F,NOW - line 4",
-        ],
         "Unknown tags": [
             "<erpConnector>",
             "<section name>",
             "<sections>",
             "<variable name>",
         ],
         "Expression errors": [
```

### Comparing `anyerplint-0.2.69/test/test_preprocess.py` & `anyerplint-0.2.90/test/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.69/test/test_tnex.py` & `anyerplint-0.2.90/test/test_tnex.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 
     assert parse(r'foo,"long / () accessor"') == 'foo,"long / () accessor"'
     assert parse(r'foo(F,NOW(),"yyyy")') == FuncCall(
         "foo", [FuncCall(',"yyyy"', [FuncCall("F,NOW", [])])]
     )
     assert parse(r'F,NOW(),"yyyy"') == FuncCall(',"yyyy"', [FuncCall("F,NOW", [])])
 
-    complex = parse(
+    complex_expr = parse(
         r'foo(f1;bar(b1;b2;"b3";"wide string");f2;baz(1;"some string with ) and ( and \" characters"))'
     )
-    assert complex == FuncCall(
+    assert complex_expr == FuncCall(
         "foo",
         [
             "f1",
             FuncCall("bar", ["b1", "b2", '"b3"', '"wide string"']),
             "f2",
             FuncCall("baz", ["1", '"some string with ) and ( and \\" characters"']),
         ],
```

### Comparing `anyerplint-0.2.69/test/test_translate.py` & `anyerplint-0.2.90/test/test_translate.py`

 * *Files identical despite different names*

