# Comparing `tmp/sphinxcontrib_typer-0.2.0.tar.gz` & `tmp/sphinxcontrib_typer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.2.0.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.2.1.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.2.0.tar` & `sphinxcontrib_typer-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2024-04-03 19:52:41.798588 sphinxcontrib_typer-0.2.0/LICENSE
--rw-r--r--   0        0        0     5672 2024-04-03 19:52:41.799025 sphinxcontrib_typer-0.2.0/README.rst
--rw-r--r--   0        0        0     3120 2024-04-03 19:53:19.565537 sphinxcontrib_typer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    34776 2024-04-03 20:18:25.421226 sphinxcontrib_typer-0.2.0/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 19:06:12.851603 sphinxcontrib_typer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5272 2024-04-11 20:21:38.783615 sphinxcontrib_typer-0.2.1/README.md
+-rw-r--r--   0        0        0     3124 2024-04-11 20:23:05.351328 sphinxcontrib_typer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    34776 2024-04-11 20:22:02.389785 sphinxcontrib_typer-0.2.1/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     6912 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.1/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.2.0/LICENSE` & `sphinxcontrib_typer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.0/README.rst` & `sphinxcontrib_typer-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,138 +1,110 @@
-|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPI status| |Documentation Status|
-|Code Cov| |Test Status|
 
-.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-   :target: https://lbesson.mit-license.org/
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
+[![PyPI status](https://img.shields.io/pypi/status/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer)
+[![Documentation Status](https://readthedocs.org/projects/sphinxcontrib-typer/badge/?version=latest)](http://sphinxcontrib-typer.readthedocs.io/?badge=latest/)
+[![Code Cov](https://codecov.io/gh/sphinx-contrib/typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://app.codecov.io/gh/sphinx-contrib/typer)
+[![Test Status](https://github.com/sphinx-contrib/typer/workflows/test/badge.svg)](https://github.com/sphinx-contrib/typer/actions/workflows/test.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# sphinxcontrib-typer
+
+A Sphinx directive for auto generating docs for [Typer](https://typer.tiangolo.com/) 
+(and [Click](https://click.palletsprojects.com/) commands!) using the rich console
+formatting available in [Typer](https://typer.tiangolo.com/). This package generates
+concise command documentation in text, html or svg formats out of the box, but if your
+goal is to greatly customize the generated documentation
+[sphinx-click](https://sphinx-click.readthedocs.io/en/latest/) may be more appropriate
+and will also work for [Typer](https://typer.tiangolo.com/) commands.
 
-.. |PyPI version fury.io| image:: https://badge.fury.io/py/sphinxcontrib-typer.svg
-   :target: https://pypi.python.org/pypi/sphinxcontrib-typer/
-
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/sphinxcontrib-typer.svg
-   :target: https://pypi.python.org/pypi/sphinxcontrib-typer/
-
-.. |PyPI status| image:: https://img.shields.io/pypi/status/sphinxcontrib-typer.svg
-   :target: https://pypi.python.org/pypi/sphinxcontrib-typer
-
-.. |Documentation Status| image:: https://readthedocs.org/projects/sphinxcontrib-typer/badge/?version=latest
-   :target: http://sphinxcontrib-typer.readthedocs.io/?badge=latest/
-
-.. |Code Cov| image:: https://codecov.io/gh/sphinx-contrib/typer/branch/main/graph/badge.svg?token=0IZOKN2DYL
-   :target: https://app.codecov.io/gh/sphinx-contrib/typer
-
-.. |Test Status| image:: https://github.com/sphinx-contrib/typer/workflows/test/badge.svg
-   :target: https://github.com/sphinx-contrib/typer/actions
-
-
-===================
-sphinxcontrib-typer
-===================
-
-.. _Typer: https://typer.tiangolo.com/
-.. _Click: https://click.palletsprojects.com/
-.. _sphinx-click: https://sphinx-click.readthedocs.io/en/latest/
-
-A Sphinx directive for auto generating docs for Typer_ (and Click_ commands!)
-using the rich console formatting available in Typer_. This package generates
-concise command documentation in text, html or svg formats out of the box,
-but if your goal is to greatly customize the generated documentation 
-sphinx-click_ may be more appropriate and will also work for Typer_ commands.
-
-Installation
-============
+## Installation
 
 Install with pip::
 
     pip install sphinxcontrib-typer
 
 Add ``sphinxcontrib.typer`` to your ``conf.py`` file:
 
-.. code-block:: python
-
-    # be sure that the commands you want to document are importable
-    # from the python path when building the docs
-    import sys
-    from pathlib import Path
-    sys.path.insert(0, str(Path(__file__).parent / '../path/to/your/commands'))
-
-    extensions = [
-        ...
-        'sphinxcontrib.typer',
-        ...
-    ]
+```python
+# be sure that the commands you want to document are importable
+# from the python path when building the docs
+import sys
+from pathlib import Path
+sys.path.insert(0, str(Path(__file__).parent / '../path/to/your/commands'))
+
+extensions = [
+    ...
+    'sphinxcontrib.typer',
+    ...
+]
+```
 
-Usage
-=====
+## Usage
 
 Say you have a command in the file ``examples/example.py`` that looks like
 this:
 
-.. code-block:: python
-
-    import typer
-    import typing as t
-
-    app = typer.Typer(add_completion=False)
-
-    @app.callback()
-    def callback(
-        flag1: bool = typer.Option(False, help="Flag 1."),
-        flag2: bool = typer.Option(False, help="Flag 2.")
-    ):
-        """This is the callback function."""
-        pass
-
-
-    @app.command()
-    def foo(
-        name: str = typer.Option(..., help="The name of the item to foo.")
-    ):
-        """This is the foo command."""
-        pass
-
-
-    @app.command()
-    def bar(
-        names: t.List[str] = typer.Option(..., help="The names of the items to bar."),
-    ):
-        """This is the bar command."""
-        pass
-
-
-    if __name__ == "__main__":
-        app()
-
+```python
+import typer
+import typing as t
+
+app = typer.Typer(add_completion=False)
+
+@app.callback()
+def callback(
+    flag1: bool = typer.Option(False, help="Flag 1."),
+    flag2: bool = typer.Option(False, help="Flag 2.")
+):
+    """This is the callback function."""
+    pass
+
+
+@app.command()
+def foo(
+    name: str = typer.Option(..., help="The name of the item to foo.")
+):
+    """This is the foo command."""
+    pass
+
+
+@app.command()
+def bar(
+    names: t.List[str] = typer.Option(..., help="The names of the items to bar."),
+):
+    """This is the bar command."""
+    pass
+
+
+if __name__ == "__main__":
+    app()
+```
 
 You can generate documentation for this command using the ``typer`` directive
 like so:
 
-.. code-block:: rst
-
-    .. typer:: examples.example.app
-        :prog: example1
-        :width: 70
-        :preferred: html
-
+```rst
+.. typer:: examples.example.app
+    :prog: example1
+    :width: 70
+    :preferred: html
+```
 
 This would generate html that looks like this:
 
-.. image:: https://raw.githubusercontent.com/sphinx-contrib/typer/main/example.html.png
-   :width: 100%
-   :align: center
-
+![Example PNG](https://raw.githubusercontent.com/sphinx-contrib/typer/main/example.html.png)
 
 You could change ``:preferred:`` to svg, to generate svg instead:
 
-.. image:: https://raw.githubusercontent.com/sphinx-contrib/typer/main/example.svg
-   :width: 100%
-   :align: center
+![Example SVG](https://raw.githubusercontent.com/sphinx-contrib/typer/main/example.svg)
 
 |
 
-Or to text::
+Or to text
                                                                                             
     Usage: example [OPTIONS] COMMAND [ARGS]...                                                  
                                                                                                 
     This is the callback function.                                                              
                                                                                                 
     ╭─ Options ──────────────────────────────────────────────────────────╮
     │ --flag1    --no-flag1      Flag 1. [default: no-flag1]             │
```

### Comparing `sphinxcontrib_typer-0.2.0/pyproject.toml` & `sphinxcontrib_typer-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "sphinxcontrib-typer"
-version = "0.2.0"
+version = "0.2.1"
 description = "Auto generate docs for typer commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/sphinx-contrib/typer"
 homepage = "https://sphinxcontrib-typer.readthedocs.io"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Framework :: Sphinx :: Extension",
@@ -33,15 +33,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = ">=4.0.0"
 selenium = "^4.0.0"
 webdriver-manager = ">=3.0.0,<5.0.0"
 cairosvg = "^2.4.0"
 lxml = ">=4.2.0,<6.0.0"
-typer-slim = {extras = ["all"], version = ">=0.12.0,<1.0.0"}
+typer-slim = {extras = ["standard"], version = ">=0.12.0,<1.0.0"}
 pillow = ">=8.0.0"
 
 [tool.poetry.group.dev.dependencies]
 sphinx-rtd-theme = ">=1.0.0"
 ipdb = "^0.13.13"
 pytest = ">=7.4.3,<9.0.0"
 isort = "^5.13.2"
```

### Comparing `sphinxcontrib_typer-0.2.0/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.2.1/sphinxcontrib/typer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from sphinx.util import logging
 
 from typer import rich_utils as typer_rich_utils
 from typer.main import Typer, TyperGroup
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 2, 0)
+VERSION = (0, 2, 1)
 
 __title__ = 'SphinxContrib Typer'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Brian Kohan'
```

