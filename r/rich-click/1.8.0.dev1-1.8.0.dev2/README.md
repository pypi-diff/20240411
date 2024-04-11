# Comparing `tmp/rich-click-1.8.0.dev1.tar.gz` & `tmp/rich-click-1.8.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-click-1.8.0.dev1.tar", last modified: Tue Apr  9 13:13:34 2024, max compression
+gzip compressed data, was "rich-click-1.8.0.dev2.tar", last modified: Wed Apr 10 02:21:56 2024, max compression
```

## Comparing `rich-click-1.8.0.dev1.tar` & `rich-click-1.8.0.dev2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.008108 rich-click-1.8.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.012108 rich-click-1.8.0.dev1/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.016108 rich-click-1.8.0.dev1/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 13:13:34.000000 rich-click-1.8.0.dev1/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:13:34.012108 rich-click-1.8.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14716 2024-04-09 13:13:29.000000 rich-click-1.8.0.dev1/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.391591 rich-click-1.8.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.395591 rich-click-1.8.0.dev2/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.8.0.dev1/LICENSE` & `rich-click-1.8.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/PKG-INFO` & `rich-click-1.8.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev1
+Version: 1.8.0.dev2
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich-click-1.8.0.dev1/README.md` & `rich-click-1.8.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/pyproject.toml` & `rich-click-1.8.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/__init__.py` & `rich-click-1.8.0.dev2/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev1"
+__version__ = "1.8.0dev2"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich-click-1.8.0.dev1/src/rich_click/_compat_click.py` & `rich-click-1.8.0.dev2/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/cli.py` & `rich-click-1.8.0.dev2/src/rich_click/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -107,14 +107,22 @@
 @click.option(
     "--output",
     "-o",
     type=click.Choice(["html", "svg"], case_sensitive=False),
     help="Optionally render help text as HTML or SVG. By default, help text is rendered normally.",
 )
 @click.option(
+    "--suppress-warnings/--do-not-suppress-warnings",
+    is_flag=True,
+    default=False,
+    hidden=True,
+    help="Suppress warnings when there are conflicting entry_points."
+    " (This option is hidden because this situation is extremely rare).",
+)
+@click.option(
     # The rich-click CLI uses a special implementation of --help,
     # which is aware of the --rich-config object.
     "--help",
     "-h",
     "show_help",
     is_eager=True,
     is_flag=True,
@@ -128,14 +136,15 @@
         "errors_epilogue": "[d]Please run [yellow bold]rich-click --help[/] for usage information.[/]",
     }
 )
 def main(
     ctx: RichContext,
     script_and_args: List[str],
     output: Literal[None, "html", "svg"],
+    suppress_warnings: bool,
     rich_config: Optional[RichHelpConfiguration],
     show_help: bool,
 ) -> None:
     """
     The [link=https://github.com/ewels/rich-click]rich-click[/] CLI provides attractive help output from any
     tool using [link=https://click.palletsprojects.com/]click[/], formatted with
     [link=https://github.com/Textualize/rich]rich[/].
@@ -160,28 +169,58 @@
         if rich_config is not None:
             rich_config.use_markdown = False
             rich_config.use_rich_markup = True
             ctx.help_config = rich_config
         click.echo(ctx.get_help(), color=ctx.color)
         ctx.exit()
 
-    sys.path.append(".")
-
     script, *args = script_and_args
 
-    _from_entry_points = False
+    _selected: List[str] = []
+    module_path = ""
+    function_name = ""
+
+    for s in entry_points(group="console_scripts"):
+        if script == s.name:
+            if not _selected:
+                module_path, function_name = s.value.split(":", 1)
+            if suppress_warnings:
+                break
+            if s.value not in _selected:
+                _selected.append(s.value)
+
+    if len(_selected) > 1 and not suppress_warnings:
+        # This is an extremely rare edge case that comes up when the user sets the PYTHONPATH themselves.
+        if script in sys.argv:
+            _args = sys.argv.copy()
+            _args[_args.index(script)] = f"{module_path}:{function_name}"
+        else:
+            _args = ["rich-click", f"{module_path}:{function_name}"]
+
+        click.echo(
+            click.style(
+                f"WARNING: Multiple entry_points correspond with script '{script}': {_selected!r}."
+                "\nThis can happen when an 'egg-info' directory exists, you're using a virtualenv,"
+                " and you have set a custom PYTHONPATH."
+                f"\n\nThe selected script is '{module_path}:{function_name}', which is being executed now."
+                "\n\nIt is safer and recommended that you specify the MODULE:CLICK_COMMAND"
+                f" ('{module_path}:{function_name}') instead of the script ('{script}'), like this:"
+                f"\n\n>>> rich-click {' '.join(_args)}"
+                "\n\nAlternatively, you can pass --suppress-warnings to the rich-click CLI,"
+                " which will disable this message.",
+                fg="red",
+            ),
+            file=sys.stderr,
+        )
 
-    scripts = {script.name: script for script in entry_points(group="console_scripts")}
-    if script in scripts:
-        module_path, function_name = scripts[script].value.split(":", 1)
-        _from_entry_points = True
-    elif ":" in script:
+    if ":" in script and not module_path:
         # the path to a function was passed
         module_path, function_name = script.split(":", 1)
-    else:
+
+    if not module_path:
         raise click.ClickException(f"No such script: {script_and_args[0]}")
 
     prog = module_path.split(".", 1)[0]
     sys.argv = [prog, *args]
 
     # patch click before importing the program function
     _patch(rich_config=rich_config)
```

### Comparing `rich-click-1.8.0.dev1/src/rich_click/decorators.py` & `rich-click-1.8.0.dev2/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/patch.py` & `rich-click-1.8.0.dev2/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_click.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_command.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_context.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_help_configuration.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_help_configuration.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_help_formatter.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/rich_help_rendering.py` & `rich-click-1.8.0.dev2/src/rich_click/rich_help_rendering.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click/utils.py` & `rich-click-1.8.0.dev2/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/src/rich_click.egg-info/PKG-INFO` & `rich-click-1.8.0.dev2/src/rich_click.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev1
+Version: 1.8.0.dev2
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich-click-1.8.0.dev1/src/rich_click.egg-info/SOURCES.txt` & `rich-click-1.8.0.dev2/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/tests/test_config.py` & `rich-click-1.8.0.dev2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/tests/test_exit_code.py` & `rich-click-1.8.0.dev2/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/tests/test_help.py` & `rich-click-1.8.0.dev2/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev1/tests/test_rich_click_cli.py` & `rich-click-1.8.0.dev2/tests/test_rich_click_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         ["--", "mymodule:cli", "--help"],
     ],
 )
 def test_simple_rich_click_cli(simple_script: Path, assert_str: AssertStr, command: List[str]) -> None:
     res = subprocess.run(
         [sys.executable, "-m", "src.rich_click", "mymodule:cli", "--help"],
         stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
         env={**os.environ, "TERMINAL_WIDTH": "100", "FORCE_COLOR": "False"},
     )
     assert res.returncode == 0
 
     if CLICK_IS_BEFORE_VERSION_8X:
         usage = "mymodule"
     else:
```

