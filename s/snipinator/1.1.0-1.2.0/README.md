# Comparing `tmp/snipinator-1.1.0.tar.gz` & `tmp/snipinator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-oh2dlz6f/snipinator-1.1.0.tar", last modified: Wed Mar 27 14:52:27 2024, max compression
+gzip compressed data, was "/mnt/c/gdrive/code/snipinator.develop/develop/dist/.tmp-hup45qnf/snipinator-1.2.0.tar", last modified: Thu Apr 11 21:45:17 2024, max compression
```

## Comparing `snipinator-1.1.0.tar` & `snipinator-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-27 14:52:27.460740 snipinator-1.1.0/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-21 17:40:02.000000 snipinator-1.1.0/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    27385 2024-03-27 14:52:27.453722 snipinator-1.1.0/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)    20640 2024-03-27 14:51:50.000000 snipinator-1.1.0/README.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)     4146 2024-03-27 14:51:50.000000 snipinator-1.1.0/pyproject.toml
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-03-27 14:52:27.460740 snipinator-1.1.0/setup.cfg
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-27 14:52:27.345650 snipinator-1.1.0/snipinator/
--rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.1.0/snipinator/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    18213 2024-03-27 14:51:50.000000 snipinator-1.1.0/snipinator/cli.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    30775 2024-03-27 14:51:50.000000 snipinator-1.1.0/snipinator/snipinate.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.1.0/snipinator/snipinate_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-27 14:52:27.438760 snipinator-1.1.0/snipinator.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    27385 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/entry_points.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1785 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-03-27 14:52:27.000000 snipinator-1.1.0/snipinator.egg-info/top_level.txt
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.996852 snipinator-1.2.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-03-21 17:40:02.000000 snipinator-1.2.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    28191 2024-04-11 21:45:16.987808 snipinator-1.2.0/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    21315 2024-04-11 21:44:39.000000 snipinator-1.2.0/README.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4199 2024-04-11 21:44:39.000000 snipinator-1.2.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-11 21:45:16.998410 snipinator-1.2.0/setup.cfg
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.850839 snipinator-1.2.0/snipinator/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      514 2024-03-27 14:51:50.000000 snipinator-1.2.0/snipinator/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    18213 2024-03-27 14:51:50.000000 snipinator-1.2.0/snipinator/cli.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    31563 2024-04-11 21:44:39.000000 snipinator-1.2.0/snipinator/snipinate.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      866 2024-03-21 17:40:02.000000 snipinator-1.2.0/snipinator/snipinate_test.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-11 21:45:16.965862 snipinator-1.2.0/snipinator.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    28191 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      335 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       51 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/entry_points.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1820 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       11 2024-04-11 21:45:16.000000 snipinator-1.2.0/snipinator.egg-info/top_level.txt
```

### Comparing `snipinator-1.1.0/LICENSE.md` & `snipinator-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snipinator-1.1.0/PKG-INFO` & `snipinator-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -56,14 +56,15 @@
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
+Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: docutils==0.20.1; extra == "dev"
@@ -86,14 +87,15 @@
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.15; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: packaging==23.2; extra == "dev"
+Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
 Requires-Dist: pip-licenses==4.3.4; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pkginfo==1.9.6; extra == "dev"
 Requires-Dist: platformdirs==4.2.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: prettytable==3.10.0; extra == "dev"
@@ -108,18 +110,19 @@
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
-Requires-Dist: tomli==2.0.1; python_version < "3.11" and extra == "dev"
+Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.0; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: wheel==0.43.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
@@ -223,15 +226,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.1.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
 ```
 
 ### Use
 
 Example tempalte README:
 [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
 
@@ -281,33 +284,34 @@
 ````py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
-              decomentify: bool = False,
+              decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 ````
@@ -315,65 +319,67 @@
 ````py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
-                decomentify: bool = False,
+                decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
 ````
 
 ````py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
-               decomentify: bool = False,
+               decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -383,35 +389,36 @@
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
-            decomentify: bool = False,
+            decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimeters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -419,15 +426,15 @@
 
 ````py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
-          decomentify: bool = False,
+          decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
           rich_rows: int = 24,
           rich_cols: int = 80,
@@ -606,50 +613,55 @@
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## Release Process
 
 These instructions are for maintainers of the project.
 
-1. `develop` branch: Run `bash scripts/pre.sh` to ensure everything
-   is in order.
-2. `develop` branch: Bump the version in `pyproject.toml`, following
-   semantic versioning principles. Also modify the `last_unstable_release` and
-   `last_stable_release` in the `[tool.snipinator-project-metadata]` table as
-   appropriate.
-3. `develop` branch: Commit these changes with a message like "Prepare release
-   X.Y.Z". (See the contributions section [above](#commit-process)).
-4. `master` branch: Merge the `develop` branch into the `master` branch:
+1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+   everything is in order.
+2. In the `develop` branch, bump the version in `pyproject.toml`,
+   following semantic versioning principles. Also modify the
+   `last_unstable_release` and `last_stable_release` in the
+   `[tool.changeguard-project-metadata]` table as appropriate.
+3. In the `develop` branch, commit these changes with a message like
+   `"Prepare release X.Y.Z"`. (See the contributions section
+   [above](#commit-process)).
+4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
-7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
-   `git push --tags`.
+7. Push to GitHub: Push the commit and tags to GitHub with
+   `git push && git push --tags`.
+8. The `--no-ff` option adds a commit to the master branch for the merge, so
+   refork the develop branch from the master branch:
+   `git checkout develop && git merge master`.
+9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/snipinator
 [4]: https://img.shields.io/pypi/v/snipinator
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/master
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
 [8]: https://img.shields.io/pypi/pyversions/snipinator
 [9]:
   https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...master
+  https://github.com/realazthat/snipinator/compare/v1.2.0...master
 [11]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
```

### Comparing `snipinator-1.1.0/README.md` & `snipinator-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.1.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
 ```
 
 ### Use
 
 Example tempalte README:
 [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
 
@@ -153,33 +153,34 @@
 ````py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
-              decomentify: bool = False,
+              decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 ````
@@ -187,65 +188,67 @@
 ````py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
-                decomentify: bool = False,
+                decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
 ````
 
 ````py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
-               decomentify: bool = False,
+               decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -255,35 +258,36 @@
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
-            decomentify: bool = False,
+            decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimeters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -291,15 +295,15 @@
 
 ````py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
-          decomentify: bool = False,
+          decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
           rich_rows: int = 24,
           rich_cols: int = 80,
@@ -478,50 +482,55 @@
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## Release Process
 
 These instructions are for maintainers of the project.
 
-1. `develop` branch: Run `bash scripts/pre.sh` to ensure everything
-   is in order.
-2. `develop` branch: Bump the version in `pyproject.toml`, following
-   semantic versioning principles. Also modify the `last_unstable_release` and
-   `last_stable_release` in the `[tool.snipinator-project-metadata]` table as
-   appropriate.
-3. `develop` branch: Commit these changes with a message like "Prepare release
-   X.Y.Z". (See the contributions section [above](#commit-process)).
-4. `master` branch: Merge the `develop` branch into the `master` branch:
+1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+   everything is in order.
+2. In the `develop` branch, bump the version in `pyproject.toml`,
+   following semantic versioning principles. Also modify the
+   `last_unstable_release` and `last_stable_release` in the
+   `[tool.changeguard-project-metadata]` table as appropriate.
+3. In the `develop` branch, commit these changes with a message like
+   `"Prepare release X.Y.Z"`. (See the contributions section
+   [above](#commit-process)).
+4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
-7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
-   `git push --tags`.
+7. Push to GitHub: Push the commit and tags to GitHub with
+   `git push && git push --tags`.
+8. The `--no-ff` option adds a commit to the master branch for the merge, so
+   refork the develop branch from the master branch:
+   `git checkout develop && git merge master`.
+9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/snipinator
 [4]: https://img.shields.io/pypi/v/snipinator
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/master
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
 [8]: https://img.shields.io/pypi/pyversions/snipinator
 [9]:
   https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...master
+  https://github.com/realazthat/snipinator/compare/v1.2.0...master
 [11]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
```

### Comparing `snipinator-1.1.0/pyproject.toml` & `snipinator-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snipinator"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python code snippets for markdown files, e.g READMEs, from actual (testable) code."
 authors = [{name = "AYF", email = "realazthat@gmail.com"}]
 license = {file = "LICENSE.md"}
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Operating System :: OS Independent",
@@ -77,14 +77,15 @@
 dev = [
   "argcomplete==3.2.3",
   "autoflake==2.3.1",
   "build==1.0.3",
   "certifi==2024.2.2",
   "cffi==1.16.0",
   "cfgv==3.4.0",
+  "changeguard==0.3.1",
   "charset-normalizer==3.3.2",
   "click==8.1.7",
   "colorama==0.4.6",
   "cryptography==42.0.5",
   "defusedxml==0.7.1",
   "distlib==0.3.8",
   "docutils==0.20.1",
@@ -107,14 +108,15 @@
   "mdurl==0.1.2",
   "more-itertools==10.2.0",
   "mypy==1.8.0",
   "mypy-extensions==1.0.0",
   "nh3==0.2.15",
   "nodeenv==1.8.0",
   "packaging==23.2",
+  "pathspec==0.12.1",
   "pexpect==4.9.0",
   "pip-licenses==4.3.4",
   "pip-tools==7.3.0",
   "pkginfo==1.9.6",
   "platformdirs==4.2.0",
   "pre-commit==3.5.0",
   "prettytable==3.10.0",
@@ -129,18 +131,19 @@
   "requests==2.31.0",
   "requests-toolbelt==1.0.0",
   "rfc3986==2.0.0",
   "rich==13.7.1",
   "rich-argparse==1.4.0",
   "secretstorage==3.3.3",
   "toml-sort==0.23.1",
-  "tomli==2.0.1 ; python_version < \"3.11\"",
+  "tomli==2.0.1",
   "tomlkit==0.12.4",
   "twine==5.0.0",
   "types-colorama==0.4.15.20240311",
+  "types-pyyaml==6.0.12.20240311",
   "typing-extensions==4.10.0",
   "urllib3==2.2.1",
   "virtualenv==20.25.0",
   "wcwidth==0.2.13",
   "wheel==0.43.0",
   "xmltodict==0.13.0",
   "yapf==0.40.2",
@@ -156,11 +159,11 @@
 Documentation = "https://github.com/realazthat/snipinator"
 Repository = "https://github.com/realazthat/snipinator"
 
 [tool.setuptools]
 packages = ["snipinator"]
 
 [tool.snipinator-project-metadata]
-last_unstable_release = "1.1.0"
-last_stable_release = "1.1.0"
+last_unstable_release = "1.2.0"
+last_stable_release = "1.2.0"
 
 [tool.tomlsort]
```

### Comparing `snipinator-1.1.0/snipinator/__init__.py` & `snipinator-1.2.0/snipinator/__init__.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.1.0/snipinator/cli.py` & `snipinator-1.2.0/snipinator/cli.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.1.0/snipinator/snipinate.py` & `snipinator-1.2.0/snipinator/snipinate.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,34 +119,35 @@
 
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
-                decomentify: bool = False,
+                decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
   path_ = _CheckPath(path=path, cwd=_ctx.cwd)
@@ -164,33 +165,34 @@
 
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
-              decomentify: bool = False,
+              decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
   path_ = _CheckPath(path=path, cwd=_ctx.cwd)
@@ -210,31 +212,32 @@
 
 
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
-               decomentify: bool = False,
+               decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -252,35 +255,36 @@
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
-            decomentify: bool = False,
+            decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimeters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -309,35 +313,36 @@
 
 
 def path(path: str,
          *,
          escape: bool = False,
          indent: Union[str, int, None] = None,
          backtickify: Union[bool, str] = False,
-         decomentify: bool = False,
+         decomentify: Union[bool, Literal['nl']] = False,
          _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Verifies that `path` exists, and just returns `path`.
 
   Unfortunately, I don't know how to use this inside a link, because the
   formatters will destroy it, and it cannot be put into a code block (as the url
   section of a link in markdown does not allow code blocks).
 
   Args:
       path (str): The path to verify.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: Just returns the path. If the path doesn't exist,
         it will raise an error.
   """
@@ -463,15 +468,15 @@
 
 
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
-          decomentify: bool = False,
+          decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
           rich_rows: int = 24,
           rich_cols: int = 80,
@@ -604,34 +609,39 @@
       alt_attr = ''
       if rich_alt is not None:
         rich_alt_escaped = html.escape(rich_alt, quote=True)
         alt_attr = 'alt="' + rich_alt_escaped + '" '
 
       output = f'<img src="{str(template_rel_svg_path)}" {alt_attr}/>'
     else:
-      raise ValueError(f'Unsupported rich format: {json.dumps(rich)}')
+      raise ValueError(
+          f'Unsupported rich format: {json.dumps(rich)} it should'
+          ' be "raw", "svg", or "img+svg", or a file path ending with ".svg"')
   else:
     raise ValueError(
-        f'Unsupported rich format: {json.dumps(rich)}, it should be "raw", "svg", or "img+svg", or a file path ending with ".svg"'
-    )
+        f'Unsupported rich format: {json.dumps(rich)}, it should be "raw",'
+        ' "svg", or "img+svg", or a file path ending with ".svg"')
 
   output = _Backtickify(output, backtickify=backtickify)
   output = _Indent(output, indent=indent)
   output = _Decomentify(output, decomentify=decomentify)
   if not escape:
     return markupsafe.Markup(output)
   else:
     return output
 
 
 def _is_relative_to(path: Path, other: Path) -> bool:
   """Backport of Path.is_relative_to for Python < 3.9."""
-  absolute_path = path.resolve()
-  other_absolute = other.resolve()
-  return str(absolute_path).startswith(str(other_absolute))
+  if sys.version_info < (3, 9):
+    absolute_path = path.resolve()
+    other_absolute = other.resolve()
+    return str(absolute_path).startswith(str(other_absolute))
+  else:
+    return path.is_relative_to(other)
 
 
 def _CheckPath(*, path: str, cwd: Path) -> Path:
   path_ = Path(path)
 
   if path_.is_absolute():
     raise ValueError(
@@ -819,12 +829,13 @@
     return f'{bt_str}\n{text}\n{bt_str}'
   elif isinstance(backtickify, str):
     return f'{bt_str}{backtickify}\n{text}\n{bt_str}'
   else:
     return text
 
 
-def _Decomentify(text: str, *, decomentify: bool) -> str:
-  if decomentify:
-    return '-->' + text + '<!--'
-  else:
+def _Decomentify(text: str, *, decomentify: Union[bool, Literal['nl']]) -> str:
+  if decomentify is False:
     return text
+  if decomentify == 'nl':
+    text = f'\n{text}\n'
+  return '-->' + text + '<!--'
```

### Comparing `snipinator-1.1.0/snipinator/snipinate_test.py` & `snipinator-1.2.0/snipinator/snipinate_test.py`

 * *Files identical despite different names*

### Comparing `snipinator-1.1.0/snipinator.egg-info/PKG-INFO` & `snipinator-1.2.0/snipinator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snipinator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python code snippets for markdown files, e.g READMEs, from actual (testable) code.
 Author-email: AYF <realazthat@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Azriel Fasten.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -56,14 +56,15 @@
 Provides-Extra: dev
 Requires-Dist: argcomplete==3.2.3; extra == "dev"
 Requires-Dist: autoflake==2.3.1; extra == "dev"
 Requires-Dist: build==1.0.3; extra == "dev"
 Requires-Dist: certifi==2024.2.2; extra == "dev"
 Requires-Dist: cffi==1.16.0; extra == "dev"
 Requires-Dist: cfgv==3.4.0; extra == "dev"
+Requires-Dist: changeguard==0.3.1; extra == "dev"
 Requires-Dist: charset-normalizer==3.3.2; extra == "dev"
 Requires-Dist: click==8.1.7; extra == "dev"
 Requires-Dist: colorama==0.4.6; extra == "dev"
 Requires-Dist: cryptography==42.0.5; extra == "dev"
 Requires-Dist: defusedxml==0.7.1; extra == "dev"
 Requires-Dist: distlib==0.3.8; extra == "dev"
 Requires-Dist: docutils==0.20.1; extra == "dev"
@@ -86,14 +87,15 @@
 Requires-Dist: mdurl==0.1.2; extra == "dev"
 Requires-Dist: more-itertools==10.2.0; extra == "dev"
 Requires-Dist: mypy==1.8.0; extra == "dev"
 Requires-Dist: mypy-extensions==1.0.0; extra == "dev"
 Requires-Dist: nh3==0.2.15; extra == "dev"
 Requires-Dist: nodeenv==1.8.0; extra == "dev"
 Requires-Dist: packaging==23.2; extra == "dev"
+Requires-Dist: pathspec==0.12.1; extra == "dev"
 Requires-Dist: pexpect==4.9.0; extra == "dev"
 Requires-Dist: pip-licenses==4.3.4; extra == "dev"
 Requires-Dist: pip-tools==7.3.0; extra == "dev"
 Requires-Dist: pkginfo==1.9.6; extra == "dev"
 Requires-Dist: platformdirs==4.2.0; extra == "dev"
 Requires-Dist: pre-commit==3.5.0; extra == "dev"
 Requires-Dist: prettytable==3.10.0; extra == "dev"
@@ -108,18 +110,19 @@
 Requires-Dist: requests==2.31.0; extra == "dev"
 Requires-Dist: requests-toolbelt==1.0.0; extra == "dev"
 Requires-Dist: rfc3986==2.0.0; extra == "dev"
 Requires-Dist: rich==13.7.1; extra == "dev"
 Requires-Dist: rich-argparse==1.4.0; extra == "dev"
 Requires-Dist: secretstorage==3.3.3; extra == "dev"
 Requires-Dist: toml-sort==0.23.1; extra == "dev"
-Requires-Dist: tomli==2.0.1; python_version < "3.11" and extra == "dev"
+Requires-Dist: tomli==2.0.1; extra == "dev"
 Requires-Dist: tomlkit==0.12.4; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
 Requires-Dist: types-colorama==0.4.15.20240311; extra == "dev"
+Requires-Dist: types-pyyaml==6.0.12.20240311; extra == "dev"
 Requires-Dist: typing-extensions==4.10.0; extra == "dev"
 Requires-Dist: urllib3==2.2.1; extra == "dev"
 Requires-Dist: virtualenv==20.25.0; extra == "dev"
 Requires-Dist: wcwidth==0.2.13; extra == "dev"
 Requires-Dist: wheel==0.43.0; extra == "dev"
 Requires-Dist: xmltodict==0.13.0; extra == "dev"
 Requires-Dist: yapf==0.40.2; extra == "dev"
@@ -223,15 +226,15 @@
   - Why: Some dev dependencies require Python 3.8+.
 
 ```bash
 # Install from pypi (https://pypi.org/project/snipinator/)
 pip install snipinator
 
 # Install from git (https://github.com/realazthat/snipinator)
-pip install git+https://github.com/realazthat/snipinator.git@v1.1.0
+pip install git+https://github.com/realazthat/snipinator.git@v1.2.0
 ```
 
 ### Use
 
 Example tempalte README:
 [`snipinator/examples/EXAMPLE.md.jinja2`](./snipinator/examples/EXAMPLE.md.jinja2):
 
@@ -281,33 +284,34 @@
 ````py
 def pysnippet(path: str,
               symbol: Optional[str],
               *,
               escape: bool = False,
               indent: Union[str, int, None] = None,
               backtickify: Union[bool, str] = False,
-              decomentify: bool = False,
+              decomentify: Union[bool, Literal['nl']] = False,
               _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return a python snippet, allowing you to specify a class or function.
 
   Args:
       path (str): The path to the file.
       symbol (Optional[str]): The symbol to extract. If None, the entire file is
         returned. Defaults to None.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 ````
@@ -315,65 +319,67 @@
 ````py
 def pysignature(path: str,
                 symbol: str,
                 *,
                 escape: bool = False,
                 indent: Union[str, int, None] = None,
                 backtickify: Union[bool, str] = False,
-                decomentify: bool = False,
+                decomentify: Union[bool, Literal['nl']] = False,
                 _ctx: _Context) -> str:
   """Return the signature of a class or function in a python file.
 
   Returns the {class,function} signature and the docstring.
 
   Args:
       path (str): The path to the file.
       symbol (str): The symbol to extract.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       str: The signature and docstring.
   """
 ````
 
 ````py
 def rawsnippet(path: str,
                *,
                escape: bool = False,
                indent: Union[str, int, None] = None,
                backtickify: Union[bool, str] = False,
-               decomentify: bool = False,
+               decomentify: Union[bool, Literal['nl']] = False,
                _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Return an entire file as a snippet.
 
   Args:
       path (str): The path to the file.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -383,35 +389,36 @@
 def snippet(path: str,
             start: str,
             end: str,
             *,
             escape: bool = False,
             indent: Union[str, int, None] = None,
             backtickify: Union[bool, str] = False,
-            decomentify: bool = False,
+            decomentify: Union[bool, Literal['nl']] = False,
             _ctx: _Context) -> Union[str, markupsafe.Markup]:
   """Returns a _delimited_ snippet from a file.
 
   Does not return the delimeters themselves.
 
   Args:
       path (str): The path to the file.
       start (str): A string that indicates the start of the snippet.
       end (str): A string that indicates the end of the snippet.
       escape (bool, optional): Should use HTML entities escaping? Defaults to
         False.
-      indent (Union[str, int, None], optional): Should indent? By how much, or with
-        what prefix? Defaults to None.
-      backtickify (Union[bool, str], optional): Should surround with backticks? With
-        what language? Defaults to False.
-      decomentify (bool, optional): Assuming that you will be using HTML
-        comments around this call, setting this to true will add corresponding
-        comments to uncomment the output. This allows you to have the Jinja2
-        call unmolested by markdown formatters, because they will be inside of
-        a comment section. Defaults to False.
+      indent (Union[str, int, None], optional): Should indent? By how much, or
+        with what prefix? Defaults to None.
+      backtickify (Union[bool, str], optional): Should surround with backticks?
+        With what language? Defaults to False.
+      decomentify (Union[bool, Literal['nl']]): Assuming that you will be using
+        HTML comments around this call, setting this to true will add
+        correspondingcomments to uncomment the output. This allows you to have
+        the Jinja2 call unmolested by markdown formatters, because they will be
+        inside of a comment section. "nl" adds additional newlines after the
+        newline delimiters. Defaults to False.
       _ctx (_Context): This is used by the system and is not available as an
         argument.
 
   Returns:
       Union[str, markupsafe.Markup]: The snippet.
   """
 
@@ -419,15 +426,15 @@
 
 ````py
 def shell(args: str,
           *,
           escape: bool = False,
           indent: Union[str, int, None] = None,
           backtickify: Union[bool, str] = False,
-          decomentify: bool = False,
+          decomentify: Union[bool, Literal['nl']] = False,
           rich: Union[Literal['svg'], Literal['img+b64+svg'], Literal['raw'],
                       str] = 'raw',
           rich_alt: Optional[str] = None,
           rich_bg_color: Optional[str] = None,
           rich_term: Optional[str] = None,
           rich_rows: int = 24,
           rich_cols: int = 80,
@@ -606,50 +613,55 @@
 5. `git commit -m "..."`.
 6. Make a PR to `develop` (or push to develop if you have the rights).
 
 ## Release Process
 
 These instructions are for maintainers of the project.
 
-1. `develop` branch: Run `bash scripts/pre.sh` to ensure everything
-   is in order.
-2. `develop` branch: Bump the version in `pyproject.toml`, following
-   semantic versioning principles. Also modify the `last_unstable_release` and
-   `last_stable_release` in the `[tool.snipinator-project-metadata]` table as
-   appropriate.
-3. `develop` branch: Commit these changes with a message like "Prepare release
-   X.Y.Z". (See the contributions section [above](#commit-process)).
-4. `master` branch: Merge the `develop` branch into the `master` branch:
+1. In the `develop` branch, run `bash scripts/pre.sh` to ensure
+   everything is in order.
+2. In the `develop` branch, bump the version in `pyproject.toml`,
+   following semantic versioning principles. Also modify the
+   `last_unstable_release` and `last_stable_release` in the
+   `[tool.changeguard-project-metadata]` table as appropriate.
+3. In the `develop` branch, commit these changes with a message like
+   `"Prepare release X.Y.Z"`. (See the contributions section
+   [above](#commit-process)).
+4. Merge the `develop` branch into the `master` branch:
    `git checkout master && git merge develop --no-ff`.
 5. `master` branch: Tag the release: Create a git tag for the release with
    `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
 6. Publish to PyPI: Publish the release to PyPI with
    `bash scripts/deploy-to-pypi.sh`.
-7. Push to GitHub: Push the commit and tags to GitHub with `git push` and
-   `git push --tags`.
+7. Push to GitHub: Push the commit and tags to GitHub with
+   `git push && git push --tags`.
+8. The `--no-ff` option adds a commit to the master branch for the merge, so
+   refork the develop branch from the master branch:
+   `git checkout develop && git merge master`.
+9. Push the develop branch to GitHub: `git push origin develop`.
 
 [1]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=master
 [2]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml
 [3]: https://img.shields.io/github/license/realazthat/snipinator
 [4]: https://img.shields.io/pypi/v/snipinator
 [5]: https://pypi.org/project/snipinator/
 [6]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/master
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/master
 [7]: https://img.shields.io/github/last-commit/realazthat/snipinator/master
 [8]: https://img.shields.io/pypi/pyversions/snipinator
 [9]:
   https://img.shields.io/github/languages/top/realazthat/snipinator.svg?&cacheSeconds=28800
 [10]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...master
+  https://github.com/realazthat/snipinator/compare/v1.2.0...master
 [11]:
   https://github.com/realazthat/snipinator/actions/workflows/build-and-test.yml/badge.svg?branch=develop
 [12]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [13]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
 [14]: https://img.shields.io/github/last-commit/realazthat/snipinator/develop
 [15]:
-  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.1.0/develop
+  https://img.shields.io/github/commits-since/realazthat/snipinator/v1.2.0/develop
 [16]:
-  https://github.com/realazthat/snipinator/compare/v1.1.0...develop
+  https://github.com/realazthat/snipinator/compare/v1.2.0...develop
```

### Comparing `snipinator-1.1.0/snipinator.egg-info/requires.txt` & `snipinator-1.2.0/snipinator.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 [dev]
 argcomplete==3.2.3
 autoflake==2.3.1
 build==1.0.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
+changeguard==0.3.1
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
 cryptography==42.0.5
 defusedxml==0.7.1
 distlib==0.3.8
 docutils==0.20.1
@@ -47,14 +48,15 @@
 mdurl==0.1.2
 more-itertools==10.2.0
 mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.15
 nodeenv==1.8.0
 packaging==23.2
+pathspec==0.12.1
 pexpect==4.9.0
 pip-licenses==4.3.4
 pip-tools==7.3.0
 pkginfo==1.9.6
 platformdirs==4.2.0
 pre-commit==3.5.0
 prettytable==3.10.0
@@ -69,30 +71,29 @@
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 rich-argparse==1.4.0
 secretstorage==3.3.3
 toml-sort==0.23.1
+tomli==2.0.1
 tomlkit==0.12.4
 twine==5.0.0
 types-colorama==0.4.15.20240311
+types-pyyaml==6.0.12.20240311
 typing-extensions==4.10.0
 urllib3==2.2.1
 virtualenv==20.25.0
 wcwidth==0.2.13
 wheel==0.43.0
 xmltodict==0.13.0
 yapf==0.40.2
 yq==3.2.3
 zipp==3.17.0
 
-[dev:python_version < "3.11"]
-tomli==2.0.1
-
 [prod]
 colorama==0.4.6
 defusedxml==0.7.1
 jinja2==3.1.3
 markdown-it-py==3.0.0
 markupsafe==2.1.5
 mdurl==0.1.2
```

