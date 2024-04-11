# Comparing `tmp/rich-click-1.8.0.dev2.tar.gz` & `tmp/rich-click-1.8.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-click-1.8.0.dev2.tar", last modified: Wed Apr 10 02:21:56 2024, max compression
+gzip compressed data, was "rich-click-1.8.0.dev3.tar", last modified: Thu Apr 11 00:37:11 2024, max compression
```

## Comparing `rich-click-1.8.0.dev2.tar` & `rich-click-1.8.0.dev3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.391591 rich-click-1.8.0.dev2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.395591 rich-click-1.8.0.dev2/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27385 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 02:21:56.000000 rich-click-1.8.0.dev2/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:21:56.399591 rich-click-1.8.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-10 02:21:47.000000 rich-click-1.8.0.dev2/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:37:11.189581 rich-click-1.8.0.dev3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27412 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-11 00:37:06.000000 rich-click-1.8.0.dev3/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 00:37:11.000000 rich-click-1.8.0.dev3/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:37:11.193581 rich-click-1.8.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-11 00:37:07.000000 rich-click-1.8.0.dev3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-11 00:37:07.000000 rich-click-1.8.0.dev3/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-11 00:37:07.000000 rich-click-1.8.0.dev3/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-11 00:37:07.000000 rich-click-1.8.0.dev3/tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.8.0.dev2/LICENSE` & `rich-click-1.8.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/PKG-INFO` & `rich-click-1.8.0.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev2
+Version: 1.8.0.dev3
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich-click-1.8.0.dev2/README.md` & `rich-click-1.8.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/pyproject.toml` & `rich-click-1.8.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/__init__.py` & `rich-click-1.8.0.dev3/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev2"
+__version__ = "1.8.0dev3"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich-click-1.8.0.dev2/src/rich_click/_compat_click.py` & `rich-click-1.8.0.dev3/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/cli.py` & `rich-click-1.8.0.dev3/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/decorators.py` & `rich-click-1.8.0.dev3/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/patch.py` & `rich-click-1.8.0.dev3/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_click.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_command.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_context.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_help_configuration.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_help_configuration.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_help_formatter.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click/rich_help_rendering.py` & `rich-click-1.8.0.dev3/src/rich_click/rich_help_rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         formatter: formatter object.
     """
     config = formatter.config
     # Print usage
     if getattr(self, "ctx", None) is not None:
         if TYPE_CHECKING:
             assert hasattr(self, "ctx")
-        self.ctx.get_usage()
+        self.ctx.command.get_usage(self.ctx, formatter)
     if config.errors_suggestion:
         formatter.write(
             Padding(
                 config.errors_suggestion,
                 (0, 1, 0, 1),
             ),
             style=config.style_errors_suggestion,
```

### Comparing `rich-click-1.8.0.dev2/src/rich_click/utils.py` & `rich-click-1.8.0.dev3/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/src/rich_click.egg-info/PKG-INFO` & `rich-click-1.8.0.dev3/src/rich_click.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev2
+Version: 1.8.0.dev3
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
```

### Comparing `rich-click-1.8.0.dev2/src/rich_click.egg-info/SOURCES.txt` & `rich-click-1.8.0.dev3/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/tests/test_config.py` & `rich-click-1.8.0.dev3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/tests/test_exit_code.py` & `rich-click-1.8.0.dev3/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/tests/test_help.py` & `rich-click-1.8.0.dev3/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev2/tests/test_rich_click_cli.py` & `rich-click-1.8.0.dev3/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

