# Comparing `tmp/django_typer-1.1.0.tar.gz` & `tmp/django_typer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_typer-1.1.0.tar", max compression
+gzip compressed data, was "django_typer-1.1.1.tar", max compression
```

## Comparing `django_typer-1.1.0.tar` & `django_typer-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2024-03-14 23:09:15.471852 django_typer-1.1.0/LICENSE
--rw-r--r--   0        0        0     8172 2024-04-03 22:32:47.609362 django_typer-1.1.0/README.md
--rw-r--r--   0        0        0    81834 2024-04-03 22:32:47.610140 django_typer-1.1.0/django_typer/__init__.py
--rw-r--r--   0        0        0     3268 2024-03-14 23:09:15.472335 django_typer-1.1.0/django_typer/apps.py
--rw-r--r--   0        0        0    16547 2024-03-14 23:09:15.472439 django_typer-1.1.0/django_typer/completers.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474628 django_typer-1.1.0/django_typer/management/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474707 django_typer-1.1.0/django_typer/management/commands/__init__.py
--rw-r--r--   0        0        0    26891 2024-04-03 18:21:16.067895 django_typer-1.1.0/django_typer/management/commands/shellcompletion.py
--rw-r--r--   0        0        0     7195 2024-03-14 23:09:15.474929 django_typer-1.1.0/django_typer/parsers.py
--rw-r--r--   0        0        0     5659 2024-04-03 18:21:16.068517 django_typer-1.1.0/django_typer/patch.py
--rw-r--r--   0        0        0        0 2024-03-14 23:09:15.475040 django_typer-1.1.0/django_typer/py.typed
--rw-r--r--   0        0        0     6055 2024-03-14 23:09:15.487659 django_typer-1.1.0/django_typer/types.py
--rw-r--r--   0        0        0     2828 2024-03-18 04:57:08.074572 django_typer-1.1.0/django_typer/utils.py
--rw-r--r--   0        0        0     5605 2024-04-03 22:32:47.614956 django_typer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9976 1970-01-01 00:00:00.000000 django_typer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-14 23:09:15.471852 django_typer-1.1.1/LICENSE
+-rw-r--r--   0        0        0     8170 2024-04-11 18:48:40.869937 django_typer-1.1.1/README.md
+-rw-r--r--   0        0        0    81850 2024-04-11 18:48:40.870985 django_typer-1.1.1/django_typer/__init__.py
+-rw-r--r--   0        0        0     3374 2024-04-11 18:48:40.871353 django_typer-1.1.1/django_typer/apps.py
+-rw-r--r--   0        0        0    16547 2024-03-14 23:09:15.472439 django_typer-1.1.1/django_typer/completers.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474628 django_typer-1.1.1/django_typer/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.474707 django_typer-1.1.1/django_typer/management/commands/__init__.py
+-rw-r--r--   0        0        0    26891 2024-04-03 18:21:16.067895 django_typer-1.1.1/django_typer/management/commands/shellcompletion.py
+-rw-r--r--   0        0        0     7195 2024-03-14 23:09:15.474929 django_typer-1.1.1/django_typer/parsers.py
+-rw-r--r--   0        0        0     5659 2024-04-03 18:21:16.068517 django_typer-1.1.1/django_typer/patch.py
+-rw-r--r--   0        0        0        0 2024-03-14 23:09:15.475040 django_typer-1.1.1/django_typer/py.typed
+-rw-r--r--   0        0        0     6055 2024-03-14 23:09:15.487659 django_typer-1.1.1/django_typer/types.py
+-rw-r--r--   0        0        0     2828 2024-03-18 04:57:08.074572 django_typer-1.1.1/django_typer/utils.py
+-rw-r--r--   0        0        0     5626 2024-04-11 18:48:40.872309 django_typer-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 django_typer-1.1.1/PKG-INFO
```

### Comparing `django_typer-1.1.0/LICENSE` & `django_typer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/README.md` & `django_typer-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # django-typer
 
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
 [![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
 [![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
```

### Comparing `django_typer-1.1.0/django_typer/__init__.py` & `django_typer-1.1.1/django_typer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
 
-VERSION = (1, 1, 0)
+VERSION = (1, 1, 1)
 
 __title__ = "Django Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-2024 Brian Kohan"
 
@@ -1206,16 +1206,16 @@
         exceptions - if rich is installed. This will default to the 'short' setting
         in the traceback configuration setting (off by default). This allows tracebacks
         to be configured by the user on a per deployment basis in the settings file. We
         therefore do not advise hardcoding this value.
     """
 
     style: ColorStyle
-    stdout: t.IO[str]
-    stderr: t.IO[str]
+    stdout: BaseOutputWrapper
+    stderr: BaseOutputWrapper
     requires_system_checks: t.Union[t.Sequence[str], str]
     suppressed_base_arguments: t.Optional[t.Iterable[str]]
     typer_app: Typer
     no_color: bool
     force_color: bool
     _num_commands: int = 0
     _has_callback: bool = False
```

### Comparing `django_typer-1.1.0/django_typer/apps.py` & `django_typer-1.1.1/django_typer/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,31 @@
 from django.utils.translation import gettext as _
 
 from django_typer import patch
 from django_typer.utils import traceback_config
 
 patch.apply()
 
-rich: t.Union[ModuleType, None] = None
+rich: t.Optional[ModuleType]
+traceback: t.Optional[ModuleType]
 
 try:
     import sys
 
     import rich
     from rich import traceback
     from typer import main as typer_main
 
     tb_config = traceback_config()
-    if rich and isinstance(tb_config, dict) and not tb_config.get("no_install", False):
+    if (
+        rich
+        and traceback
+        and isinstance(tb_config, dict)
+        and not tb_config.get("no_install", False)
+    ):
         # install rich tracebacks if we've been configured to do so (default)
         no_color = "NO_COLOR" in os.environ
         force_color = "FORCE_COLOR" in os.environ
         traceback.install(
             console=tb_config.pop(
                 "console",
                 (
@@ -56,15 +62,16 @@
             },
         )
         # typer installs its own exception hook and it falls back to the sys hook - depending
         # on when typer was imported it may have the original fallback system hook or our
         # installed rich one - we patch it here to make sure!
         typer_main._original_except_hook = sys.excepthook
 except ImportError:
-    pass
+    rich = None
+    traceback = None
 
 
 @register("settings")
 def check_traceback_config(app_configs, **kwargs) -> t.List[CheckMessage]:
     """
     A system check that validates that the traceback config is valid and
     contains only the expected parameters.
```

### Comparing `django_typer-1.1.0/django_typer/completers.py` & `django_typer-1.1.1/django_typer/completers.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/django_typer/management/commands/shellcompletion.py` & `django_typer-1.1.1/django_typer/management/commands/shellcompletion.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/django_typer/parsers.py` & `django_typer-1.1.1/django_typer/parsers.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/django_typer/patch.py` & `django_typer-1.1.1/django_typer/patch.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/django_typer/types.py` & `django_typer-1.1.1/django_typer/types.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/django_typer/utils.py` & `django_typer-1.1.1/django_typer/utils.py`

 * *Files identical despite different names*

### Comparing `django_typer-1.1.0/pyproject.toml` & `django_typer-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-typer"
-version = "1.1.0"
+version = "1.1.1"
 description = "Use Typer to define the CLI for your Django management commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bckohan/django-typer"
 homepage = "https://django-typer.readthedocs.io"
 keywords = ["django", "CLI", "management", "Typer", "commands"]
@@ -84,14 +84,15 @@
 ]
 scipy = [
     { version = ">=1.11", markers = "python_version > '3.8'" },
     { version = "<=1.10", markers = "python_version <= '3.8'" },
 ]
 django-stubs = "^4.2.7"
 pexpect = "^4.9.0"
+pyright = "^1.1.357"
 
 [tool.poetry.extras]
 rich = ["rich"]
 
 [tool.mypy]
 # The mypy configurations: http://bit.ly/2zEl9WI
 allow_redefinition = false
```

### Comparing `django_typer-1.1.0/PKG-INFO` & `django_typer-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use Typer to define the CLI for your Django management commands.
 Home-page: https://django-typer.readthedocs.io
 License: MIT
 Keywords: django,CLI,management,Typer,commands
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -40,15 +40,15 @@
 Requires-Dist: typing-extensions (>=3.7.4.3) ; python_version < "3.10"
 Project-URL: Repository, https://github.com/bckohan/django-typer
 Description-Content-Type: text/markdown
 
 # django-typer
 
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-typer.svg)](https://pypi.python.org/pypi/django-typer/)
 [![PyPI djversions](https://img.shields.io/pypi/djversions/django-typer.svg)](https://pypi.org/project/django-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/django-typer.svg)](https://pypi.python.org/pypi/django-typer)
 [![Documentation Status](https://readthedocs.org/projects/django-typer/badge/?version=latest)](http://django-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/bckohan/django-typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-typer)
 [![Test Status](https://github.com/bckohan/django-typer/workflows/test/badge.svg)](https://github.com/bckohan/django-typer/actions/workflows/test.yml)
```

