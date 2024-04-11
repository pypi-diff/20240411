# Comparing `tmp/cappa-0.9.2.tar.gz` & `tmp/cappa-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cappa-0.9.2.tar", max compression
+gzip compressed data, was "cappa-0.9.3.tar", max compression
```

## Comparing `cappa-0.9.2.tar` & `cappa-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2240 2023-10-23 18:02:32.384993 cappa-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-10-23 18:02:32.384993 cappa-0.9.2/LICENSE
--rw-r--r--   0        0        0     4752 2023-10-23 18:02:32.384993 cappa-0.9.2/README.md
--rw-r--r--   0        0        0     1995 2023-10-23 18:02:32.388993 cappa-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      685 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/__init__.py
--rw-r--r--   0        0        0     4908 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/annotation.py
--rw-r--r--   0        0        0    12496 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/arg.py
--rw-r--r--   0        0        0     9731 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/argparse.py
--rw-r--r--   0        0        0     8682 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/base.py
--rw-r--r--   0        0        0     4608 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/class_inspect.py
--rw-r--r--   0        0        0     7658 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/command.py
--rw-r--r--   0        0        0        0 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/completion/__init__.py
--rw-r--r--   0        0        0     1890 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/completion/base.py
--rw-r--r--   0        0        0      288 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/completion/completers.py
--rw-r--r--   0        0        0     2080 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/completion/shells.py
--rw-r--r--   0        0        0      747 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/completion/types.py
--rw-r--r--   0        0        0      904 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/env.py
--rw-r--r--   0        0        0     4966 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/help.py
--rw-r--r--   0        0        0     6886 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/invoke.py
--rw-r--r--   0        0        0     2931 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/output.py
--rw-r--r--   0        0        0    16172 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/parser.py
--rw-r--r--   0        0        0        0 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/py.typed
--rw-r--r--   0        0        0     4503 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/subcommand.py
--rw-r--r--   0        0        0     2964 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/testing.py
--rw-r--r--   0        0        0     2547 2023-10-23 18:02:32.388993 cappa-0.9.2/src/cappa/typing.py
--rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 cappa-0.9.2/setup.py
--rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 cappa-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2429 2023-10-23 19:37:17.180878 cappa-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-10-23 19:37:17.180878 cappa-0.9.3/LICENSE
+-rw-r--r--   0        0        0     4752 2023-10-23 19:37:17.180878 cappa-0.9.3/README.md
+-rw-r--r--   0        0        0     1995 2023-10-23 19:37:17.184878 cappa-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/__init__.py
+-rw-r--r--   0        0        0     4908 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/annotation.py
+-rw-r--r--   0        0        0    12492 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/arg.py
+-rw-r--r--   0        0        0     9726 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/argparse.py
+-rw-r--r--   0        0        0     8682 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/base.py
+-rw-r--r--   0        0        0     4608 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/class_inspect.py
+-rw-r--r--   0        0        0     7658 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/command.py
+-rw-r--r--   0        0        0        0 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/completion/__init__.py
+-rw-r--r--   0        0        0     1890 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/completion/base.py
+-rw-r--r--   0        0        0      288 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/completion/completers.py
+-rw-r--r--   0        0        0     2080 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/completion/shells.py
+-rw-r--r--   0        0        0      747 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/completion/types.py
+-rw-r--r--   0        0        0      904 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/env.py
+-rw-r--r--   0        0        0     4966 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/help.py
+-rw-r--r--   0        0        0     6886 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/invoke.py
+-rw-r--r--   0        0        0     2931 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/output.py
+-rw-r--r--   0        0        0    16377 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/parser.py
+-rw-r--r--   0        0        0        0 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/py.typed
+-rw-r--r--   0        0        0     4503 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/subcommand.py
+-rw-r--r--   0        0        0     2964 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/testing.py
+-rw-r--r--   0        0        0     2547 2023-10-23 19:37:17.184878 cappa-0.9.3/src/cappa/typing.py
+-rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 cappa-0.9.3/setup.py
+-rw-r--r--   0        0        0     5648 1970-01-01 00:00:00.000000 cappa-0.9.3/PKG-INFO
```

### Comparing `cappa-0.9.2/CHANGELOG.md` & `cappa-0.9.3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 0.9.3
+
+- Ensure output of missing required options is deterministically ordered
+- Output all required options when listing out missing required options
+- Fix ignore num_args=0 override
+
 ## 0.9.2
 
 - Invoke the specific callable subcommand instance being targeted.
 
 ## 0.9.1
 
 - Supply the parsed Command instance as an invoke dependency.
```

### Comparing `cappa-0.9.2/LICENSE` & `cappa-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/README.md` & `cappa-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/pyproject.toml` & `cappa-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cappa"
-version = "0.9.2"
+version = "0.9.3"
 description = "Declarative CLI argument parser."
 
 repository = "https://github.com/dancardin/cappa"
 authors = ["DanCardin <ddcardin@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 keywords = [
```

### Comparing `cappa-0.9.2/src/cappa/__init__.py` & `cappa-0.9.3/src/cappa/__init__.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/annotation.py` & `cappa-0.9.3/src/cappa/annotation.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/arg.py` & `cappa-0.9.3/src/cappa/arg.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         annotation=NoneType,
         fallback_help: str | None = None,
         action: ArgAction | Callable | None = None,
         name: str | None = None,
     ) -> Arg:
         origin = typing.get_origin(annotation) or annotation
         type_args = typing.get_args(annotation)
-        required = infer_required(self, annotation, self.default)
+        required = infer_required(self, origin, self.default)
 
         name = typing.cast(str, name or self.name)
         short = infer_short(self, name)
         long = infer_long(self, origin, name)
         choices = infer_choices(self, origin, type_args)
         action = action or infer_action(self, origin, type_args, long, self.default)
         num_args = infer_num_args(self, origin, type_args, action, long)
```

### Comparing `cappa-0.9.2/src/cappa/argparse.py` & `cappa-0.9.3/src/cappa/argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import sys
 import typing
 from collections.abc import Callable
 
 from typing_extensions import assert_never
 
-from cappa.arg import Arg, ArgAction
+from cappa.arg import Arg, ArgAction, no_extra_arg_actions
 from cappa.command import Command, Subcommand
 from cappa.help import format_help, generate_arg_groups
 from cappa.invoke import fullfill_deps
 from cappa.output import Exit, HelpExit
 from cappa.parser import RawOption, Value
 from cappa.typing import assert_not_missing, assert_type, missing
 
@@ -237,17 +237,15 @@
 
     if arg.default is not missing:
         if arg.action and arg.action is ArgAction.append:
             kwargs["default"] = list(arg.default)  # type: ignore
         else:
             kwargs["default"] = arg.default
 
-    if num_args and (
-        arg.action and arg.action not in {ArgAction.store_true, ArgAction.store_false}
-    ):
+    if num_args is not None and (arg.action and arg.action not in no_extra_arg_actions):
         kwargs["nargs"] = num_args
     elif is_positional and not arg.required:
         kwargs["nargs"] = "?"
 
     if arg.choices:
         kwargs["choices"] = arg.choices
```

### Comparing `cappa-0.9.2/src/cappa/base.py` & `cappa-0.9.3/src/cappa/base.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/class_inspect.py` & `cappa-0.9.3/src/cappa/class_inspect.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/command.py` & `cappa-0.9.3/src/cappa/command.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/completion/base.py` & `cappa-0.9.3/src/cappa/completion/base.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/completion/shells.py` & `cappa-0.9.3/src/cappa/completion/shells.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/completion/types.py` & `cappa-0.9.3/src/cappa/completion/types.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/env.py` & `cappa-0.9.3/src/cappa/env.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/help.py` & `cappa-0.9.3/src/cappa/help.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/invoke.py` & `cappa-0.9.3/src/cappa/invoke.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/output.py` & `cappa-0.9.3/src/cappa/output.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/parser.py` & `cappa-0.9.3/src/cappa/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,25 +263,29 @@
                 parse_short_option(context, arg)
 
         parse_args(context)
 
         if not context.has_values():
             break
 
-    # Options are not explicitly iterated over because they can occur multi times non-contiguouesly.
+    # Options are not explicitly iterated over because they can occur multiple times non-contiguouesly.
     # So instead we check afterward, if there are any missing which we haven't yet fulfilled.
-    for opt_name in context.missing_options:
-        opt = context.options[opt_name]
-        if opt.required:
-            raise BadArgumentError(
-                f"The following arguments are required: {opt.names_str()}",
-                value="",
-                command=context.command,
-                arg=opt,
-            )
+    required_missing_options = [
+        context.options[opt_name]
+        for opt_name in sorted(context.missing_options)
+        if context.options[opt_name].required
+    ]
+    if required_missing_options:
+        names = ", ".join([opt.names_str("/") for opt in required_missing_options])
+        raise BadArgumentError(
+            f"The following arguments are required: {names}",
+            value="",
+            command=context.command,
+            arg=required_missing_options[0],
+        )
 
 
 def parse_option(context: ParseContext, raw: RawOption) -> None:
     if raw.name not in context.options:
         possible_values = [
             name for name in context.options if name.startswith(raw.name)
         ]
@@ -425,15 +429,15 @@
     name = typing.cast(str, arg.name)
     context.result[name] = nested_context.result
 
 
 def consume_arg(
     context: ParseContext, arg: Arg, option: RawOption | None = None
 ) -> typing.Any:
-    orig_num_args = arg.num_args or 1
+    orig_num_args = arg.num_args if arg.num_args is not None else 1
     num_args = orig_num_args
 
     if arg.action in no_extra_arg_actions:
         orig_num_args = 0
         num_args = 0
 
     result: list[str] | str
```

### Comparing `cappa-0.9.2/src/cappa/subcommand.py` & `cappa-0.9.3/src/cappa/subcommand.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/testing.py` & `cappa-0.9.3/src/cappa/testing.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/src/cappa/typing.py` & `cappa-0.9.3/src/cappa/typing.py`

 * *Files identical despite different names*

### Comparing `cappa-0.9.2/setup.py` & `cappa-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['docstring-parser>=0.15',
  'rich',
  'typing-extensions>=4.7.1',
  'typing-inspect>=0.9.0']
 
 setup_kwargs = {
     'name': 'cappa',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Declarative CLI argument parser.',
     'long_description': '# Cappa\n\n[![Actions Status](https://github.com/DanCardin/cappa/actions/workflows/test.yml/badge.svg)](https://github.com/dancardin/cappa/actions)\n[![Coverage Status](https://coveralls.io/repos/github/DanCardin/cappa/badge.svg?branch=main)](https://coveralls.io/github/DanCardin/cappa?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/cappa/badge/?version=latest)](https://cappa.readthedocs.io/en/latest/?badge=latest)\n\n- [Full documentation here](https://cappa.readthedocs.io/en/latest/).\n- [Comparison vs existing libraries.](https://cappa.readthedocs.io/en/latest/comparison.html).\n- [Annotation inference details](https://cappa.readthedocs.io/en/latest/annotation.html)\n- ["invoke" (click-like) details](https://cappa.readthedocs.io/en/latest/invoke.html)\n\nCappa is a declarative command line parsing library, taking much of its\ninspiration from the "Derive" API from the\n[Clap](https://docs.rs/clap/latest/clap/_derive/index.html) written in Rust.\n\n```python\nfrom dataclasses import dataclass, field\nimport cappa\nfrom typing import Literal\nfrom typing_extensions import Annotated\n\n\n@dataclass\nclass Example:\n    positional_arg: str = "optional"\n    boolean_flag: bool = False\n    single_option: Annotated[int | None, cappa.Arg(short=True, help="A number")] = None\n    multiple_option: Annotated[\n        list[Literal["one", "two", "three"]],\n        cappa.Arg(long=True, help="Pick one!"),\n    ] = field(default_factory=list)\n\n\nargs: Example = cappa.parse(Example, backend=cappa.backend)\nprint(args)\n```\n\nProduces the following CLI:\n\n![help text](./docs/source/_static/example.svg)\n\nIn this way, you can turn any dataclass-like object (with some additional\nannotations, depending on what you\'re looking for) into a CLI.\n\nYou\'ll note that `cappa.parse` returns an instance of the class. This API should\nfeel very familiar to `argparse`, except that you get the fully typed dataclass\ninstance back instead of a raw `Namespace`.\n\n## Invoke\n\n["invoke" documentation](https://cappa.readthedocs.io/en/latest/invoke.html)\n\nThe "invoke" API is meant to feel more like the experience you get when using\n`click` or `typer`. You can take the same dataclass, but register a function to\nbe called on successful parsing of the command.\n\n```python\nfrom dataclasses import dataclass\nimport cappa\nfrom typing_extensions import Annotated\n\ndef function(example: Example):\n    print(example)\n\n@cappa.command(invoke=function)\nclass Example:  # identical to original class\n    positional_arg: str\n    boolean_flag: bool\n    single_option: Annotated[int | None, cappa.Arg(long=True)]\n    multiple_option: Annotated[list[str], cappa.Arg(short=True)]\n\n\ncappa.invoke(Example)\n```\n\n(Note the lack of the dataclass decorator. You can optionally omit or include\nit, and it will be automatically inferred).\n\nAlternatively you can make your dataclass callable, as a shorthand for an\nexplcit invoke function:\n\n```python\n@dataclass\nclass Example:\n    ...   # identical to original class\n\n    def __call__(self):\n       print(self)\n```\n\nNote `invoke=function` can either be a reference to some callable, or a string\nmodule-reference to a function (which will get lazily imported and invoked).\n\nWith a single top-level command, the click-like API isn\'t particularly valuable\nby comparison. Click\'s command-centric API is primarily useful when composing a\nnumber of nested subcommands.\n\n## Subcommands\n\nThe useful aspect of click\'s functional composability is that you can define\nsome number of subcommands functions under a parent command, whichever\nsubcommand the function targets will be invoked.\n\n```python\nimport click\n\n@click.group(\'example\')\ndef example():\n    ...\n\n@example.command("print")\n@click.option(\'--loudly\', is_flag=True)\ndef print_cmd(loudly):\n    if loudly:\n      print("PRINTING!")\n    else:\n      print("printing!")\n\n@example.command("fail")\n@click.option(\'--code\', type: int)\ndef fail_cmd(code):\n    raise click.Exit(code=code)\n\n# Called like:\n# /example.py print\n# /example.py fail\n```\n\nWhereas with argparse, you\'d have had to manually match and call the funcitons\nyourself. This API does all of the hard parts of deciding which function to\ncall.\n\nSimilarly, you can achieve the same thing with cappa.\n\n```python\nfrom __future__ import annotations\nfrom dataclasses import dataclass\nimport cappa\n\n@dataclass\nclass Example:\n    cmd: cappa.Subcommands[Print | Fail]\n\n\ndef print_cmd(print: Print):\n    if print.loudly:\n        print("PRINTING!")\n    else:\n        print("printing!")\n\n@cappa.invoke(invoke=print_cmd)\nclass Print:\n    loudly: bool\n\n@dataclass\nclass Fail:\n    code: int\n\n    def __call__(self):  # again, __call__ is shorthand for the above explicit `invoke=` form.\n        raise cappa.Exit(code=code)\n\ncappa.invoke(Example)\n```\n',
     'author': 'DanCardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dancardin/cappa',
```

### Comparing `cappa-0.9.2/PKG-INFO` & `cappa-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cappa
-Version: 0.9.2
+Version: 0.9.3
 Summary: Declarative CLI argument parser.
 Home-page: https://github.com/dancardin/cappa
 License: Apache-2.0
 Keywords: CLI,argparse,parser
 Author: DanCardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.8,<4
```

