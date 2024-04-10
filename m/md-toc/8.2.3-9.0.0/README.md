# Comparing `tmp/md_toc-8.2.3.tar.gz` & `tmp/md_toc-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md_toc-8.2.3.tar", last modified: Thu Feb 15 17:31:20 2024, max compression
+gzip compressed data, was "md_toc-9.0.0.tar", last modified: Wed Apr 10 22:11:23 2024, max compression
```

## Comparing `md_toc-8.2.3.tar` & `md_toc-9.0.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2024-02-15 17:31:20.964527 md_toc-8.2.3/
--rw-r--r--   0 vm        (1019) vm        (1019)       76 2024-02-15 17:19:19.000000 md_toc-8.2.3/CONTRIBUTING.md
--rw-r--r--   0 vm        (1019) vm        (1019)    35147 2024-02-15 17:19:19.000000 md_toc-8.2.3/LICENSE.txt
--rw-r--r--   0 vm        (1019) vm        (1019)      297 2024-02-15 17:19:23.000000 md_toc-8.2.3/MANIFEST.in
--rw-r--r--   0 vm        (1019) vm        (1019)     9871 2024-02-15 17:31:20.964527 md_toc-8.2.3/PKG-INFO
--rw-r--r--   0 vm        (1019) vm        (1019)     8094 2024-02-15 17:19:23.000000 md_toc-8.2.3/README.md
--rw-r--r--   0 vm        (1019) vm        (1019)      433 2024-02-15 17:19:23.000000 md_toc-8.2.3/SECURITY.md
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2024-02-15 17:31:20.960527 md_toc-8.2.3/md_toc/
--rw-r--r--   0 vm        (1019) vm        (1019)     1832 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/__init__.py
--rwxr-xr-x   0 vm        (1019) vm        (1019)     1335 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/__main__.py
--rw-r--r--   0 vm        (1019) vm        (1019)    58097 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/api.py
--rw-r--r--   0 vm        (1019) vm        (1019)    14790 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cli.py
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2024-02-15 17:31:20.964527 md_toc-8.2.3/md_toc/cmark/
--rw-r--r--   0 vm        (1019) vm        (1019)      758 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/__init__.py
--rw-r--r--   0 vm        (1019) vm        (1019)     9121 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/buffer_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1507 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/buffer_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2544 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/chunk_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1493 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/cmark_ctype_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2614 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/cmark_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1073 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/houdini_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     5615 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/houdini_html_u_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)    60365 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/inlines_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     8456 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/node_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     3810 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/node_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     4437 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/references_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1833 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/references_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     5135 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/scanners_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)     2158 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/scanners_h.py
--rw-r--r--   0 vm        (1019) vm        (1019)     4651 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/cmark/utf8_c.py
--rw-r--r--   0 vm        (1019) vm        (1019)    26183 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/constants.py
--rw-r--r--   0 vm        (1019) vm        (1019)     1561 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/exceptions.py
--rw-r--r--   0 vm        (1019) vm        (1019)     9412 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/generic.py
--rw-r--r--   0 vm        (1019) vm        (1019)     3352 2024-02-15 17:19:23.000000 md_toc-8.2.3/md_toc/types.py
-drwxr-xr-x   0 vm        (1019) vm        (1019)        0 2024-02-15 17:31:20.964527 md_toc-8.2.3/md_toc.egg-info/
--rw-r--r--   0 vm        (1019) vm        (1019)     9871 2024-02-15 17:31:20.000000 md_toc-8.2.3/md_toc.egg-info/PKG-INFO
--rw-r--r--   0 vm        (1019) vm        (1019)      680 2024-02-15 17:31:20.000000 md_toc-8.2.3/md_toc.egg-info/SOURCES.txt
--rw-r--r--   0 vm        (1019) vm        (1019)      151 2024-02-15 17:19:23.000000 md_toc-8.2.3/pyproject.toml
--rw-r--r--   0 vm        (1019) vm        (1019)     2224 2024-02-15 17:31:20.964527 md_toc-8.2.3/setup.cfg
--rw-r--r--   0 vm        (1019) vm        (1019)       56 2024-02-15 17:19:23.000000 md_toc-8.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:11:23.546063 md_toc-9.0.0/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-10 22:02:35.000000 md_toc-9.0.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35147 2024-04-10 22:02:35.000000 md_toc-9.0.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      320 2024-04-10 22:02:50.000000 md_toc-9.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9907 2024-04-10 22:11:23.546063 md_toc-9.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8130 2024-04-10 22:02:50.000000 md_toc-9.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-10 22:02:35.000000 md_toc-9.0.0/SECURITY.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:11:23.542063 md_toc-9.0.0/md_toc/
+-rw-r--r--   0 root         (0) root         (0)      801 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1335 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    58015 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/api.py
+-rw-r--r--   0 root         (0) root         (0)    14790 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:11:23.542063 md_toc-9.0.0/md_toc/cmark/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9121 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/buffer_c.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/buffer_h.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/chunk_h.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/cmark_ctype_c.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/cmark_h.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/houdini_h.py
+-rw-r--r--   0 root         (0) root         (0)     5615 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/houdini_html_u_c.py
+-rw-r--r--   0 root         (0) root         (0)    59278 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/inlines_c.py
+-rw-r--r--   0 root         (0) root         (0)     8456 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/node_c.py
+-rw-r--r--   0 root         (0) root         (0)     3305 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/node_h.py
+-rw-r--r--   0 root         (0) root         (0)     4437 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/references_c.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/references_h.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/scanners_c.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2024-04-10 22:02:35.000000 md_toc-9.0.0/md_toc/cmark/scanners_h.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/cmark/utf8_c.py
+-rw-r--r--   0 root         (0) root         (0)    10259 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1381 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9360 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/generic.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2024-04-10 22:02:50.000000 md_toc-9.0.0/md_toc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 22:11:23.542063 md_toc-9.0.0/md_toc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9907 2024-04-10 22:11:22.000000 md_toc-9.0.0/md_toc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      697 2024-04-10 22:11:23.000000 md_toc-9.0.0/md_toc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-10 22:02:35.000000 md_toc-9.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-10 22:02:35.000000 md_toc-9.0.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-10 22:11:23.546063 md_toc-9.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-10 22:02:35.000000 md_toc-9.0.0/setup.py
```

### Comparing `md_toc-8.2.3/LICENSE.txt` & `md_toc-9.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/PKG-INFO` & `md_toc-9.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_toc
-Version: 8.2.3
+Version: 9.0.0
 Summary: Automatically generate and add an accurate table of contents to markdown files
 Home-page: https://blog.franco.net.eu.org/software/#md-toc
 Author: Franco Masotti
 Author-email: franco.masotti@tutanota.com
 License: GPLv3+,
 Project-URL: Bug Tracker, https://github.com/frnmst/md-toc/issues
 Project-URL: Documentation, https://docs.franco.net.eu.org/md-toc/
@@ -148,15 +148,15 @@
 ### foo
 ## file
 
 ## bye
 
 # bye
 
-$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github -l6 foo.md
+$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github foo.md
 $ cat foo.md
 
 # Table of contents
 
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
@@ -208,14 +208,15 @@
 
 # bye
 >>> print(md_toc.build_toc('foo.md'), end='')
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 ```
 
 You can also write the TOC in place:
@@ -250,14 +251,15 @@
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 
 <!--TOC-->
```

### Comparing `md_toc-8.2.3/README.md` & `md_toc-9.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 ### foo
 ## file
 
 ## bye
 
 # bye
 
-$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github -l6 foo.md
+$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github foo.md
 $ cat foo.md
 
 # Table of contents
 
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
@@ -170,14 +170,15 @@
 
 # bye
 >>> print(md_toc.build_toc('foo.md'), end='')
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 ```
 
 You can also write the TOC in place:
@@ -212,14 +213,15 @@
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 
 <!--TOC-->
```

### Comparing `md_toc-8.2.3/md_toc/__main__.py` & `md_toc-9.0.0/md_toc/__main__.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/api.py` & `md_toc-9.0.0/md_toc/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # api.py
 #
-# Copyright (C) 2017-2023 Franco Masotti (see /README.md)
+# Copyright (C) 2017-2024 Franco Masotti (see /README.md)
 #
 # This file is part of md-toc.
 #
 # md-toc is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -66,15 +66,15 @@
     return tocs_equal
 
 
 def write_string_on_file_between_markers(
     filename: str,
     string: str,
     marker: str,
-    newline_string: str = common_defaults['newline string'],
+    newline_string: str = common_defaults['newline_string'],
 ) -> bool:
     r"""Write the table of contents on a single file.
 
     :parameter filename: the file that needs to be read or modified.
     :parameter string: the string that will be written on the file.
     :parameter marker: a marker that will identify the start
          and the end of the string.
@@ -132,15 +132,15 @@
     return equal
 
 
 def write_strings_on_files_between_markers(
     filenames: list[str],
     strings: list[str],
     marker: str,
-    newline_string: str = common_defaults['newline string'],
+    newline_string: str = common_defaults['newline_string'],
 ) -> bool:
     r"""Write the table of contents on multiple files.
 
     :parameter filenames: the files that needs to be read or modified.
     :parameter strings: the strings that will be written on the file. Each
          string is associated with one file.
     :parameter marker: a marker that will identify the start
@@ -176,15 +176,15 @@
     no_indentation: bool = False,
     no_list_coherence: bool = False,
     keep_header_levels: int = 3,
     parser: str = 'github',
     list_marker: str = '-',
     skip_lines: int = 0,
     constant_ordered_list: bool = False,
-    newline_string: str = common_defaults['newline string'],
+    newline_string: str = common_defaults['newline_string'],
 ) -> str:
     r"""Build the table of contents of a single file.
 
     :parameter filename: the file that needs to be read.
     :parameter ordered: decides whether to build an ordered list or not.
         Defaults to ``False``.
     :parameter no_links: disables the use of links.
@@ -224,24 +224,35 @@
     :type newline_string: str
     :returns: toc, the corresponding table of contents of the file.
     :rtype: str
     :raises: a built-in exception.
 
     .. warning:: In case of ordered TOCs you must explicitly pass one of the
         supported ordered list markers.
+
+    :Example:
+
+    >>> import md_toc # doctest: +SKIP
+    >>> with open('foo.md', 'w') as f: # doctest: +SKIP
+    ...     f.write('# This\n# Is an\n## Example\n') # doctest: +SKIP
+    26
+    >>> md_toc.api.build_toc('foo.md') # doctest: +SKIP
+    - [This](#this)
+    - [Is an](#is-an)
+      - [Example](#example)
     """
     if not skip_lines >= 0:
         raise ValueError
 
-    toc: list[str] = list()
-    header_type_counter: types.HeaderTypeCounter = dict()
+    toc: list[str] = []
+    header_type_counter: types.HeaderTypeCounter = {}
     header_type_curr: int = 0
     header_type_prev: int = 0
     header_type_first: int = 0
-    header_duplicate_counter: types.HeaderDuplicateCounter = dict()
+    header_duplicate_counter: types.HeaderDuplicateCounter = {}
 
     if filename == '-':
         f = sys.stdin
     else:
         # When reading input from the stream,
         # if newline is None, universal newlines mode is enabled.
         # Lines in the input can end in '\n', '\r', or '\r\n',
@@ -252,37 +263,41 @@
 
     # Help the developers: override the list_marker in case
     # this function is called with the default unordered list marker,
     # for example like this:
     # print(md_toc.build_toc('test.md', ordered=True))
     # This avoids an AssertionError later on.
     if (ordered and list_marker
-            == md_parser[parser]['list']['unordered']['default marker']):
+            == md_parser[parser]['list']['unordered']['default_marker']):
         list_marker = md_parser[parser]['list']['ordered'][
-            'default closing marker']
+            'default_closing_marker']
     if constant_ordered_list:
         ordered = True
     if ordered and (
             list_marker is None or list_marker
-            not in md_parser[parser]['list']['ordered']['closing markers']):
+            not in md_parser[parser]['list']['ordered']['closing_markers']):
         list_marker = md_parser[parser]['list']['ordered'][
-            'default closing marker']
+            'default_closing_marker']
 
     if skip_lines > 0:
         loop: bool = True
         line_counter = 1
         while loop:
             if line_counter > skip_lines or f.readline() == '':
                 loop = False
             line_counter += 1
 
-    line = f.readline()
-    indentation_log = init_indentation_log(parser, list_marker)
-    if not no_indentation and not no_list_coherence:
-        indentation_list: list[bool] = init_indentation_status_list(parser)
+    try:
+        line = f.readline()
+    except UnicodeDecodeError:
+        return ''.join(
+            ['<!--stop reading ', filename, ': probably a binary file-->'])
+
+    indentation_log: dict[types.IndentationLogElement] = init_indentation_log(
+        parser, list_marker)
     is_within_code_fence = False
     code_fence = None
     is_document_end = False
     while line:
         # Document ending detection.
         #
         # This changes the state of is_within_code_fence if the
@@ -291,16 +306,22 @@
         # however more semantically correct.
         #
         # See the unit tests (examples 95 and 96 of the github parser)
         # and the is_closing_code_fence function.
         if filename != '-':
             # stdin is not seekable.
             file_pointer_pos = f.tell()
-            if f.readline() == '':
-                is_document_end = True
+            try:
+                if f.readline() == '':
+                    is_document_end = True
+            except UnicodeDecodeError:
+                return ''.join([
+                    '<!--stop reading ', filename,
+                    ': probably a binary file-->'
+                ])
             f.seek(file_pointer_pos)
 
         # Code fence detection.
         if is_within_code_fence:
             is_within_code_fence = not is_closing_code_fence(
                 line,
                 code_fence,
@@ -326,59 +347,59 @@
 
             # We only need to get the first element since all the lines
             # have been already separated here.
             header: types.Header = headers[0]
 
             # Ignore invalid or to-be-invisible headers.
             if header is not None and header['visible']:
-                header_type_curr = header['type']
+                header_type_curr = header['header_type']
 
                 # Take care of the ordered TOC.
                 if ordered and not constant_ordered_list:
                     increase_index_ordered_list(
                         header_type_counter,
                         header_type_prev,
                         header_type_curr,
                         parser,
                     )
-                    index = header_type_counter[header_type_curr]
+                    index = header_type_counter['h' + str(header_type_curr)]
                 elif constant_ordered_list:
                     # This value should work on most parsers.
                     index = 1
                 else:
                     index = 1
 
                 # Take care of list indentations.
                 if no_indentation:
                     no_of_indentation_spaces_curr = 0
                     # TOC list coherence checks are not necessary
                     # without indentation.
                 else:
                     if not no_list_coherence:
+                        # In-place list coherence checks can be made using only
+                        # the first, current and previous header types.
                         if header_type_first == 0:
                             header_type_first = header_type_curr
-                        if not toc_renders_as_coherent_list(
-                                header_type_curr,
-                                header_type_first,
-                                indentation_list,
-                                parser,
-                        ):
+                        if header_type_prev == 0:
+                            header_type_prev = header_type_curr
+                        if (header_type_curr < header_type_first
+                                or header_type_curr > header_type_prev + 1):
                             raise TocDoesNotRenderAsCoherentList
 
                     compute_toc_line_indentation_spaces(
                         header_type_curr,
                         header_type_prev,
                         parser,
                         ordered,
                         list_marker,
                         indentation_log,
                         index,
                     )
                     no_of_indentation_spaces_curr = indentation_log[
-                        header_type_curr]['indentation spaces']
+                        header_type_curr]['indentation_spaces']
 
                 # endif
 
                 # Build a single TOC line.
                 toc_line_no_indent = build_toc_line_without_indentation(
                     header,
                     ordered,
@@ -398,15 +419,19 @@
 
                 header_type_prev = header_type_curr
 
             # endif
 
         # endif
 
-        line = f.readline()
+        try:
+            line = f.readline()
+        except UnicodeDecodeError:
+            return ''.join(
+                ['<!--stop reading ', filename, ': probably a binary file-->'])
 
     # endwhile
 
     f.close()
 
     return ''.join(toc)
 
@@ -418,15 +443,15 @@
     no_indentation: bool = False,
     no_list_coherence: bool = False,
     keep_header_levels: int = 3,
     parser: str = 'github',
     list_marker: str = '-',
     skip_lines: int = 0,
     constant_ordered_list: bool = False,
-    newline_string: str = common_defaults['newline string'],
+    newline_string: str = common_defaults['newline_string'],
 ) -> list[str]:
     r"""Parse files by line and build the table of contents of each file.
 
     :parameter filenames: the files that needs to be read.
     :parameter ordered: decides whether to build an ordered list or not.
          Defaults to ``False``.
     :parameter no_links: disables the use of links.
@@ -511,23 +536,23 @@
         raise ValueError
     if not header_type_curr >= 1:
         raise ValueError
 
     # Base cases for a new table of contents or a new index type.
     if header_type_prev == 0:
         header_type_prev = header_type_curr
-    if (header_type_curr not in header_type_count
+    if ('h' + str(header_type_curr) not in header_type_count
             or header_type_prev < header_type_curr):
-        header_type_count[header_type_curr] = 0
+        header_type_count['h' + str(header_type_curr)] = 0
 
-    header_type_count[header_type_curr] += 1
+    header_type_count['h' + str(header_type_curr)] += 1
 
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker']:
-        if header_type_count[header_type_curr] > md_parser['github']['list'][
-                'ordered']['max marker number']:
+        if header_type_count['h' + str(header_type_curr)] > md_parser[
+                'github']['list']['ordered']['max_marker_number']:
             raise GithubOverflowOrderedListMarker
 
 
 def init_indentation_log(
     parser: str = 'github',
     list_marker: str = '-',
 ) -> dict[types.IndentationLogElement]:
@@ -544,19 +569,19 @@
     :raises: a built-in exception.
 
     .. warning: this function does not make distinctions between ordered and unordered
          TOCs.
     """
     return {
         i: {
-            'index': md_parser[parser]['list']['ordered']['min marker number'],
-            'list marker': list_marker,
-            'indentation spaces': 0,
+            'index': md_parser[parser]['list']['ordered']['min_marker_number'],
+            'list_marker': list_marker,
+            'indentation_spaces': 0,
         }
-        for i in range(1, md_parser[parser]['header']['max levels'] + 1)
+        for i in range(1, md_parser[parser]['header']['max_levels'] + 1)
     }
 
 
 def compute_toc_line_indentation_spaces(
     header_type_curr: int = 1,
     header_type_prev: int = 0,
     parser: str = 'github',
@@ -601,30 +626,30 @@
     """
     if not header_type_curr >= 1:
         raise ValueError
     if not header_type_prev >= 0:
         raise ValueError
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
         if not len(indentation_log
-                   ) == md_parser['github']['header']['max levels']:
+                   ) == md_parser['github']['header']['max_levels']:
             raise ValueError
     if not index >= 1:
         raise ValueError
 
     if parser in [
             'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
             'redcarpet'
     ]:
         if ordered:
             if list_marker not in md_parser[parser]['list']['ordered'][
-                    'closing markers']:
+                    'closing_markers']:
                 raise ValueError
         else:
             if list_marker not in md_parser[parser]['list']['unordered'][
-                    'bullet markers']:
+                    'bullet_markers']:
                 raise ValueError
 
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
         index_length: int
         if ordered:
             if header_type_prev == 0:
                 index_length = 0
@@ -632,43 +657,43 @@
                 index_length = len(
                     str(indentation_log[header_type_prev]['index']), )
         else:
             index_length = 0
 
         if header_type_prev == 0:
             # Base case for the first toc line.
-            indentation_log[header_type_curr]['indentation spaces'] = 0
+            indentation_log[header_type_curr]['indentation_spaces'] = 0
         elif header_type_curr > header_type_prev:
             # More indentation.
-            indentation_log[header_type_curr]['indentation spaces'] = (
-                indentation_log[header_type_prev]['indentation spaces'] +
-                len(indentation_log[header_type_prev]['list marker'], ) +
+            indentation_log[header_type_curr]['indentation_spaces'] = (
+                indentation_log[header_type_prev]['indentation_spaces'] +
+                len(indentation_log[header_type_prev]['list_marker'], ) +
                 index_length + len(' '))
         elif header_type_curr < header_type_prev:
             # Less indentation. Since we went "back" we must reset
             # all the sublists in the data structure. The indentation spaces are the ones
             # computed before.
             for i in range(
                     header_type_curr + 1,
-                    md_parser['github']['header']['max levels'] + 1,
+                    md_parser['github']['header']['max_levels'] + 1,
             ):
                 indentation_log[i]['index'] = md_parser['github']['list'][
-                    'ordered']['min marker number']
-                indentation_log[i]['indentation spaces'] = 0
-                indentation_log[i]['list marker'] = list_marker
+                    'ordered']['min_marker_number']
+                indentation_log[i]['indentation_spaces'] = 0
+                indentation_log[i]['list_marker'] = list_marker
         # And finally, in case of same indentation we have: header_type_curr = header_type_prev
-        # so indentation_log[header_type_curr]['indentation spaces'] = indentation_log[header_type_prev]['indentation spaces']
+        # so indentation_log[header_type_curr]['indentation_spaces'] = indentation_log[header_type_prev]['indentation_spaces']
         # which is an identity.
 
         if ordered:
             indentation_log[header_type_curr]['index'] = index
-        indentation_log[header_type_curr]['list marker'] = list_marker
+        indentation_log[header_type_curr]['list_marker'] = list_marker
 
     elif parser in ['redcarpet']:
-        indentation_log[header_type_curr]['indentation spaces'] = 4 * (
+        indentation_log[header_type_curr]['indentation_spaces'] = 4 * (
             header_type_curr - 1)
 
 
 def build_toc_line_without_indentation(
     header: types.Header,
     ordered: bool = False,
     no_links: bool = False,
@@ -700,29 +725,29 @@
          without indentation.
     :rtype: str
     :raises: a built-in exception.
 
     .. warning:: In case of ordered TOCs you must explicitly pass one of the
         supported ordered list markers.
     """
-    if not header['type'] >= 1:
+    if not header['header_type'] >= 1:
         raise ValueError
     if not index >= 1:
         raise ValueError
     if parser in [
             'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
             'redcarpet'
     ]:
         if ordered:
             if list_marker not in md_parser[parser]['list']['ordered'][
-                    'closing markers']:
+                    'closing_markers']:
                 raise ValueError
         else:
             if list_marker not in md_parser[parser]['list']['unordered'][
-                    'bullet markers']:
+                    'bullet_markers']:
                 raise ValueError
 
     if parser in [
             'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
             'redcarpet'
     ]:
         if ordered:
@@ -754,14 +779,26 @@
     :parameter no_of_indentation_spaces: the number of indentation spaces.
          Defaults to ``0``.
     :type toc_line_no_indent: str
     :type no_of_indentation_spaces: int
     :returns: toc_line, a single line of the table of contents.
     :rtype: str
     :raises: a built-in exception.
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.build_toc_line('', 0)
+    ''
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.build_toc_line('my string', 10)
+    '          my string'
     """
     if not no_of_indentation_spaces >= 0:
         raise ValueError
 
     indentation: str = no_of_indentation_spaces * ' '
     return ''.join([indentation, toc_line_no_indent])
 
@@ -802,23 +839,33 @@
     :type line: str
     :type parser: str
     :returns: the input line without emphasis.
     :rtype: str
     :raises: a built-in exception.
 
     .. note:: Backslashes are preserved.
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.remove_emphasis('__my string__ *is this* one')
+    'my string is this one'
     """
     if parser in [
             'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
             'redcarpet'
     ]:
         mem = None
         refmap = references_h._cmarkCmarkReferenceMap()
 
         parent = node_h._cmarkCmarkNode()
+
+        # Remove NULL bytes.
+        line = line.replace('\x00', '')
+
         parent.data = line
         parent.length = len(line)
         parent.start_line = 0
         parent.start_column = 0
         parent.internal_offset = 1
 
         ignore: list[range] = inlines_c._cmark_cmark_parse_inlines(
@@ -848,14 +895,48 @@
 
     # Flatten list.
     rng_flat: list[int] = sorted([item for e in rng for item in e])
 
     return ''.join([line[i] for i in range(0, len(line)) if i not in rng_flat])
 
 
+def anchor_link_punctuation_filter(
+    input_string: str,
+    parser: str = 'github',
+) -> str:
+    r"""Remove punctuation and other unwanted characters from the anchor link string.
+
+    :parameter input_string: the unfiltered anchor link
+    :parameter parser: decides rules on how to generate anchor links.
+        Defaults to ``github``.
+    :type input_string: str
+    :type parser: str
+    :returns: a string without the unwanted characters.
+    :rtype: str
+    :raises: a built-in exception.
+
+    .. note: license B applies for the github part.
+        See docs/copyright_license.rst
+    """
+    # https://github.com/gjtorikian/html-pipeline/blob/7c7fad1f82f81ebf15dd81d59eed28d979b8e441/lib/html/pipeline/toc_filter.rb#L30
+    output_string: str
+    if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
+        # Remove punctuation: Keep spaces, hypens and "word characters" only.
+        # In other words, given the set:
+        # \w                alphanumeric
+        # \-                hyphen
+        #                   space
+        # remove its complementary set from the input_string. This is achieved
+        # using `^`.
+        pattern: str = r'[^\w\- ]'
+        replacement: str = ''
+        output_string = re.sub(pattern, replacement, input_string)
+    return output_string
+
+
 def build_anchor_link(
     header_text_trimmed: str,
     header_duplicate_counter: types.HeaderDuplicateCounter,
     parser: str = 'github',
 ) -> str:
     r"""Apply the specified slug rule to build the anchor link.
 
@@ -870,35 +951,39 @@
     :type header_duplicate_counter: types.HeaderDuplicateCounter
     :type parser: str
     :returns: None if the specified parser is not recognized, or the anchor
         link, otherwise.
     :rtype: str
     :raises: a built-in exception.
 
-    .. note: license B applies for the github part.
-        See docs/copyright_license.rst
-
     .. note: license A applies for the redcarpet part.
         See docs/copyright_license.rst
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.build_anchor_link('This is an example test       header', {}, 'gitlab')
+    'this-is-an-example-test-header'
     """
     # Check for newlines.
     if len(replace_and_split_newlines(header_text_trimmed)) > 1:
         raise StringCannotContainNewlines
 
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
         header_text_trimmed = header_text_trimmed.lower()
 
         # Filter HTML tags.
         header_text_trimmed = remove_html_tags(header_text_trimmed, parser)
 
         # Filter "emphasis and strong emphasis".
         header_text_trimmed = remove_emphasis(header_text_trimmed, parser)
 
-        # Remove punctuation: Keep spaces, hypens and "word characters" only.
-        header_text_trimmed = re.sub(r'[^\w\s\- ]', '', header_text_trimmed)
+        # Remove punctuation characters.
+        header_text_trimmed = anchor_link_punctuation_filter(
+            header_text_trimmed, parser)
 
         # Replace spaces with dash.
         header_text_trimmed = header_text_trimmed.replace(' ', '-')
 
         if parser in ['gitlab']:
             # See https://docs.gitlab.com/ee/user/markdown.html#header-ids-and-links
             # Two or more hyphens in a row are converted to one.
@@ -1038,50 +1123,50 @@
         raise ValueError
 
     struct: list[types.AtxHeadingStructElement] = list()
     line_visible: bool = True
 
     if len(line) == 0:
         return [{
-            'header type': None,
-            'header text trimmed': None,
+            'header_type': None,
+            'header_text_trimmed': None,
             'visible': False
         }]
 
     for subl in replace_and_split_newlines(line):
         current_headers = None
         final_line = None
 
         if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
 
             struct.append({
-                'header type': None,
-                'header text trimmed': None,
+                'header_type': None,
+                'header_text_trimmed': None,
                 'visible': False
             })
 
             # Empty substring or backslash.
             if len(subl) == 0 or subl[0] == '\u005c':
                 continue
 
             # Preceding.
             i: int = 0
             while i < len(subl) and subl[i] == ' ' and i <= md_parser[
-                    'github']['header']['max space indentation']:
+                    'github']['header']['max_space_indentation']:
                 i += 1
-            if i > md_parser['github']['header']['max space indentation']:
+            if i > md_parser['github']['header']['max_space_indentation']:
                 continue
 
             # ATX characters.
             offset = i
             while i < len(subl) and subl[i] == '#' and i <= md_parser[
-                    'github']['header']['max levels'] + offset:
+                    'github']['header']['max_levels'] + offset:
                 i += 1
 
-            if (i - offset > md_parser['github']['header']['max levels']
+            if (i - offset > md_parser['github']['header']['max_levels']
                     or i - offset == 0):
                 continue
 
             # We need to continue parsing to find possible duplicate headers
             # in other functions if we set keep_header_levels < max_levels.
             if i - offset > keep_header_levels:
                 line_visible: bool = False
@@ -1169,22 +1254,22 @@
                         hash_char_rounds += 1
 
             final_line = subl[cs_start:cs_end]
 
             # Add escaping.
             if not no_links:
                 if len(final_line) > 0 and final_line[-1] == '\u005c':
-                    final_line += ' '
+                    final_line = ''.join([final_line, ' '])
                 if len(
                         final_line.strip('\u0020').strip('\u0009').strip(
                             '\u000a').strip('\u000b').strip('\u000c').strip(
                                 '\u000d'), ) == 0:
                     raise GithubEmptyLinkLabel
                 if len(final_line,
-                       ) > md_parser['github']['link']['max chars label']:
+                       ) > md_parser['github']['link']['max_chars_label']:
                     raise GithubOverflowCharsLinkLabel
 
                 i = 0
                 while i < len(final_line):
                     # Escape square brackets if not already escaped.
                     if (final_line[i] == '[' or final_line[i] == ']'):
                         j = i - 1
@@ -1202,32 +1287,32 @@
                             [final_line[0:i], tmp, final_line[i:]])
                         i += 1 + len(tmp)
                     else:
                         i += 1
 
             # Overwrite the element with None as values.
             struct[-1] = {
-                'header type': current_headers,
-                'header text trimmed': final_line,
+                'header_type': current_headers,
+                'header_text_trimmed': final_line,
                 'visible': line_visible
             }
 
         elif parser in ['redcarpet']:
             struct.append({
-                'header type': None,
-                'header text trimmed': None,
+                'header_type': None,
+                'header_text_trimmed': None,
                 'visible': False
             })
 
             if len(subl) == 0 or subl[0] != '#':
                 continue
 
             i = 0
             while (i < len(subl)
-                   and i < md_parser['redcarpet']['header']['max levels']
+                   and i < md_parser['redcarpet']['header']['max_levels']
                    and subl[i] == '#'):
                 i += 1
             current_headers = i
 
             if i < len(subl) and subl[i] != ' ':
                 continue
 
@@ -1253,16 +1338,16 @@
                 final_line = final_line[i:end]
 
             if final_line is None:
                 current_headers = None
                 line_visible = False
 
             struct[-1] = {
-                'header type': current_headers,
-                'header text trimmed': final_line,
+                'header_type': current_headers,
+                'header_text_trimmed': final_line,
                 'visible': line_visible
             }
 
         # TODO: escape or remove '[', ']', '(', ')' in inline links for redcarpet,
         # TODO: check link label rules for redcarpet.
         # TODO: check live_visible
 
@@ -1303,22 +1388,22 @@
     :raises: a built-in exception.
 
     .. note::
          This works like a wrapper to other functions.
     """
     return [
         None if
-        (r['header type'] is None and r['header text trimmed'] is None) else {
-            'type':
-            r['header type'],
+        (r['header_type'] is None and r['header_text_trimmed'] is None) else {
+            'header_type':
+            r['header_type'],
             'text_original':
-            r['header text trimmed'],
+            r['header_text_trimmed'],
             'text_anchor_link':
             build_anchor_link(
-                r['header text trimmed'],
+                r['header_text_trimmed'],
                 header_duplicate_counter,
                 parser,
             ),
             'visible':
             r['visible'],
         } for r in get_atx_heading(
             header_text_line,
@@ -1340,15 +1425,15 @@
     :returns: True if the given line has valid indentation or False
          otherwise.
     :rtype: bool
     :raises: a built-in exception.
     """
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
         return len(line) - len(line.lstrip(
-            ' ')) <= md_parser['github']['code fence']['min marker characters']
+            ' ')) <= md_parser['github']['code_fence']['min_marker_characters']
     elif parser in ['redcarpet']:
         # TODO.
         return False
 
     return False
 
 
@@ -1363,17 +1448,17 @@
     :returns: None if the input line is not an opening code fence. Otherwise,
          returns the string which will identify the closing code fence
          according to the input parsers' rules.
     :rtype: typing.Optional[str]
     :raises: a built-in exception.
     """
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
-        markers = md_parser['github']['code fence']['marker']
-        marker_min_length = md_parser['github']['code fence'][
-            'min marker characters']
+        markers = md_parser['github']['code_fence']['marker']
+        marker_min_length = md_parser['github']['code_fence'][
+            'min_marker_characters']
 
         info_string: str
         info_string_start: int
 
         if not is_valid_code_fence_indent(line):
             return None
 
@@ -1448,19 +1533,31 @@
     :type line: str
     :type fence: str
     :type is_document_end: bool
     :type parser: str
     :returns: True if the line ends the current code block. False otherwise.
     :rtype: bool
     :raises: a built-in exception.
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.is_closing_code_fence('```', '```')
+    True
+
+    :Example:
+
+    >>> import md_toc
+    >>> md_toc.api.is_closing_code_fence('```', '~~~')
+    False
     """
     if parser in ['github', 'cmark', 'gitlab', 'commonmarker', 'goldmark']:
-        markers = md_parser['github']['code fence']['marker']
-        marker_min_length = md_parser['github']['code fence'][
-            'min marker characters']
+        markers = md_parser['github']['code_fence']['marker']
+        marker_min_length = md_parser['github']['code_fence'][
+            'min_marker_characters']
 
         if not is_valid_code_fence_indent(line):
             return False
 
         # Remove opening fence indentation after it is known to be valid.
         fence = fence.lstrip(' ')
         # Check if fence uses valid characters.
@@ -1520,97 +1617,9 @@
     elif parser in ['redcarpet']:
         # TODO.
         return False
 
     return False
 
 
-def init_indentation_status_list(parser: str = 'github') -> list[bool]:
-    r"""Create a data structure that holds the state of indentations.
-
-    :parameter parser: decides the length of the list.
-         Defaults to ``github``.
-    :type parser: str
-    :returns: indentation_list, a list that contains the state of
-         indentations given a header type.
-    :rtype: list
-    :raises: a built-in exception.
-    """
-    indentation_list: list[bool] = list()
-
-    if parser in [
-            'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
-            'redcarpet'
-    ]:
-        indentation_list = [
-            False for i in range(0, md_parser[parser]['header']['max levels'])
-        ]
-
-    return indentation_list
-
-
-def toc_renders_as_coherent_list(
-    header_type_curr: int = 1,
-    header_type_first: int = 1,
-    indentation_list: list[bool] = init_indentation_status_list('github'),
-    parser: str = 'github',
-) -> bool:
-    r"""Check if the TOC will render as a working list.
-
-    :parameter header_type_curr: the current type of header (h[1,...,Inf]).
-    :parameter header_type_first: the type of header first encountered (h[1,...,Inf]).
-         This must correspond to the one with the least indentation.
-    :parameter indentation_list: a list that holds the state of indentations.
-    :parameter parser: decides rules on how to generate ordered list markers.
-    :type header_type_curr: int
-    :type header_type_first: int
-    :type indentation_list: list
-    :type parser: str
-    :returns: renders_as_list
-    :rtype: bool
-    :raises: a built-in exception.
-
-    .. note: this function modifies the input list.
-    """
-    if not header_type_curr >= 1:
-        raise ValueError
-    if not header_type_first >= 1:
-        raise ValueError
-    if parser in [
-            'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
-            'redcarpet'
-    ]:
-        if not len(
-                indentation_list) == md_parser[parser]['header']['max levels']:
-            raise ValueError
-
-    renders_as_list: bool = True
-    if parser in [
-            'github', 'cmark', 'gitlab', 'commonmarker', 'goldmark',
-            'redcarpet'
-    ]:
-        # Update with current information.
-        indentation_list[header_type_curr - 1] = True
-
-        # Reset next cells to False, as a detection mechanism.
-        for i in range(
-                header_type_curr,
-                md_parser['github']['header']['max levels'],
-        ):
-            indentation_list[i] = False
-
-        # Check for previous False cells. If there is a "hole" in the list
-        # it means that the TOC will have "wrong" indentation spaces, thus
-        # either not rendering as an HTML list or not as the user intended.
-        i = header_type_curr - 1
-        while i >= header_type_first - 1 and indentation_list[i]:
-            i -= 1
-        if i >= header_type_first - 1:
-            renders_as_list = False
-        if header_type_curr < header_type_first:
-            renders_as_list = False
-
-    return renders_as_list
-
-
 if __name__ == '__main__':
     pass
```

### Comparing `md_toc-8.2.3/md_toc/cli.py` & `md_toc-9.0.0/md_toc/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # cli.py
 #
-# Copyright (C) 2017-2023 Franco Masotti (see /README.md)
+# Copyright (C) 2017-2024 Franco Masotti (see /README.md)
 #
 # This file is part of md-toc.
 #
 # md-toc is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -123,34 +123,34 @@
         )
 
     def _add_cmark_like_megroup_arguments(self, megroup, parser_name: str):
         megroup.add_argument(
             '-u',
             '--unordered-list-marker',
             choices=md_parser[parser_name]['list']['unordered']
-            ['bullet markers'],
+            ['bullet_markers'],
             nargs='?',
             const=md_parser[parser_name]['list']['unordered']
-            ['default marker'],
+            ['default_marker'],
             default=md_parser[parser_name]['list']['unordered']
-            ['default marker'],
+            ['default_marker'],
             help='set the marker and enables unordered list. Defaults to ' +
-            md_parser[parser_name]['list']['unordered']['default marker'],
+            md_parser[parser_name]['list']['unordered']['default_marker'],
         )
         megroup.add_argument(
             '-o',
             '--ordered-list-marker',
             choices=md_parser[parser_name]['list']['ordered']
-            ['closing markers'],
+            ['closing_markers'],
             nargs='?',
             const=md_parser[parser_name]['list']['ordered']
-            ['default closing marker'],
+            ['default_closing_marker'],
             help=('set the marker and enable ordered lists. Defaults to ' +
                   md_parser[parser_name]['list']['ordered']
-                  ['default closing marker']),
+                  ['default_closing_marker']),
         )
 
     def _add_cmark_like_arguments(self, parser, parser_name: str):
         parser.add_argument(
             '-c',
             '--constant-ordered-list',
             action='store_true',
@@ -158,20 +158,20 @@
                   list marker. This options enables ordered lists',
         )
         parser.add_argument(
             '-l',
             '--header-levels',
             type=int,
             choices=range(1,
-                          md_parser[parser_name]['header']['max levels'] + 1),
+                          md_parser[parser_name]['header']['max_levels'] + 1),
             nargs='?',
-            const=md_parser[parser_name]['header']['default keep levels'],
+            const=md_parser[parser_name]['header']['default_keep_levels'],
             help='set the maximum level of headers to be considered as part \
                   of the TOC. Defaults to ' +
-            str(md_parser[parser_name]['header']['default keep levels'], ),
+            str(md_parser[parser_name]['header']['default_keep_levels'], ),
         )
 
     def create_parser(self):
         """Create the CLI parser."""
         parser = argparse.ArgumentParser(
             description=PROGRAM_DESCRIPTION,
             formatter_class=argparse.RawDescriptionHelpFormatter,
@@ -200,15 +200,15 @@
                          as listed below',
         )
         self._add_filename_argument(github)
         megroup = github.add_mutually_exclusive_group()
         self._add_cmark_like_megroup_arguments(megroup, 'github')
         self._add_cmark_like_arguments(github, 'github')
         github.set_defaults(header_levels=md_parser['github']['header']
-                            ['default keep levels'], )
+                            ['default_keep_levels'], )
 
         ##########
         # gitlab #
         ##########
         gitlab = subparsers.add_parser(
             'gitlab',
             description='Use GitLab Flavored Markdown rules to generate an \
@@ -218,15 +218,15 @@
                          as listed below',
         )
         self._add_filename_argument(gitlab)
         megroup = gitlab.add_mutually_exclusive_group()
         self._add_cmark_like_megroup_arguments(megroup, 'gitlab')
         self._add_cmark_like_arguments(gitlab, 'gitlab')
         gitlab.set_defaults(header_levels=md_parser['gitlab']['header']
-                            ['default keep levels'], )
+                            ['default_keep_levels'], )
 
         ####################
         # cmark + Goldmark #
         ####################
         cmark = subparsers.add_parser(
             'cmark',
             aliases=['goldmark'],
@@ -236,15 +236,15 @@
                          as listed below',
         )
         self._add_filename_argument(cmark)
         megroup = cmark.add_mutually_exclusive_group()
         self._add_cmark_like_megroup_arguments(megroup, 'cmark')
         self._add_cmark_like_arguments(cmark, 'cmark')
         cmark.set_defaults(header_levels=md_parser['cmark']['header']
-                           ['default keep levels'], )
+                           ['default_keep_levels'], )
 
         #############
         # Redcarpet #
         #############
         redcarpet = subparsers.add_parser(
             'redcarpet',
             description='Use Redcarpet rules to generate an output. If no \
@@ -256,58 +256,58 @@
         )
         self._add_filename_argument(redcarpet)
         megroup = redcarpet.add_mutually_exclusive_group()
         megroup.add_argument(
             '-u',
             '--unordered-list-marker',
             choices=md_parser['redcarpet']['list']['unordered']
-            ['bullet markers'],
+            ['bullet_markers'],
             nargs='?',
             const=md_parser['redcarpet']['list']['unordered']
-            ['default marker'],
+            ['default_marker'],
             default=md_parser['redcarpet']['list']['unordered']
-            ['default marker'],
+            ['default_marker'],
             help='set the marker and enables unordered list. Defaults to ' +
-            md_parser['redcarpet']['list']['unordered']['default marker'],
+            md_parser['redcarpet']['list']['unordered']['default_marker'],
         )
         megroup.add_argument(
             '-o',
             '--ordered-list-marker',
             choices=md_parser['redcarpet']['list']['ordered']
-            ['closing markers'],
+            ['closing_markers'],
             nargs='?',
             const=md_parser['redcarpet']['list']['ordered']
-            ['default closing marker'],
+            ['default_closing_marker'],
             help='set the marker and enables ordered lists. Defaults to ' +
             md_parser['redcarpet']['list']['ordered']
-            ['default closing marker'],
+            ['default_closing_marker'],
         )
         redcarpet.add_argument(
             '-c',
             '--constant-ordered-list',
             action='store_true',
             help='intead of progressive numbers use a single integer as list \
                   marker. This options enables ordered lists',
         )
         redcarpet.add_argument(
             '-l',
             '--header-levels',
             type=int,
             choices=range(
                 1,
-                md_parser['redcarpet']['header']['max levels'] + 1,
+                md_parser['redcarpet']['header']['max_levels'] + 1,
             ),
             nargs='?',
-            const=md_parser['redcarpet']['header']['default keep levels'],
+            const=md_parser['redcarpet']['header']['default_keep_levels'],
             help='set the maximum level of headers to be considered as part \
                   of the TOC. Defaults to ' +
-            str(md_parser['redcarpet']['header']['default keep levels'], ),
+            str(md_parser['redcarpet']['header']['default_keep_levels'], ),
         )
         redcarpet.set_defaults(header_levels=md_parser['redcarpet']['header']
-                               ['default keep levels'], )
+                               ['default_keep_levels'], )
 
         ##########
         # Common #
         ##########
         no_list_coherence_or_no_indentation = parser.add_mutually_exclusive_group(
         )
         no_list_coherence_or_no_indentation.add_argument(
@@ -337,32 +337,32 @@
             action='store_true',
             help='avoids adding links to the TOC',
         )
         parser.add_argument(
             '-m',
             '--toc-marker',
             metavar='TOC_MARKER',
-            default=common_defaults['toc marker'],
+            default=common_defaults['toc_marker'],
             help=(
                 'set the string to be used as the marker for positioning the \
                 table of contents. Put this value between single quotes. \
-                Defaults to \'' + common_defaults['toc marker']) + '\'',
+                Defaults to \'' + common_defaults['toc_marker']) + '\'',
         )
         parser.add_argument(
             '-n',
             '--newline-string',
             choices=[r'\n', r'\r', r'\r\n'],
             metavar='NEWLINE_STRING',
             type=str,
-            default=common_defaults['newline string'],
+            default=common_defaults['newline_string'],
             help=('the string used to separate the lines of the TOC. \
                   Use single quotes to delimit the string. \
                   If you output in place all the newlines of the \
                   input file will be replaced with this value. \
-                  Defaults to ' + repr(common_defaults['newline string'])),
+                  Defaults to ' + repr(common_defaults['newline_string'])),
         )
         parser.add_argument(
             '-p',
             '--in-place',
             action='store_true',
             help='overwrite the input file',
         )
```

### Comparing `md_toc-8.2.3/md_toc/cmark/__init__.py` & `md_toc-9.0.0/md_toc/cmark/__init__.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/buffer_c.py` & `md_toc-9.0.0/md_toc/cmark/buffer_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/buffer_h.py` & `md_toc-9.0.0/md_toc/cmark/buffer_h.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,31 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
 r"""A cmark implementation file."""
 
+from dataclasses import dataclass
+from typing import Optional
+
 from .cmark_h import _cmarkCmarkMem
 
 # License E applies to this file except for non derivative code:
 # in that case the license header at the top of the file applies.
 # See docs/copyright_license.rst
 
 
 # 0.29, 0.30
+@dataclass
 class _cmarkCmarkStrbuf:
-    __slots__ = [
-        'mem',
-        'ptr',
-        'asize',
-        'size',
-    ]
-
-    def __init__(self):
-        self.mem: _cmarkCmarkMem = None
-        self.ptr: str = ''
-        self.asize: int = 0
-        self.size: int = 0
+    mem: Optional[_cmarkCmarkMem] = None
+    ptr: str = ''
+    asize: int = 0
+    size: int = 0
 
 
 # Should be equivalent to
 #     #define CMARK_BUF_INIT(mem) \
 #       { mem, cmark_strbuf__initbuf, 0, 0 }
 # 0.29, 0.30
 def _cmark_CMARK_BUF_INIT(mem: _cmarkCmarkMem):
```

### Comparing `md_toc-8.2.3/md_toc/cmark/chunk_h.py` & `md_toc-9.0.0/md_toc/cmark/chunk_h.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,37 +17,33 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
 r"""The cmark implementation file."""
 
 import copy
+from dataclasses import dataclass
 
 from ..constants import parser as md_parser
 from .cmark_ctype_c import _cmark_cmark_isspace
 
 # License E applies to this file except for non derivative code:
 # in that case the license header at the top of the file applies.
 # See docs/copyright_license.rst
 
 # Returns 1 if c is a "whitespace" character as defined by the spec.
 #   int cmark_isspace(char c) { return cmark_ctype_class[(uint8_t)c] == 1; }
 # The only defined whitespaces in the spec are Unicode whitespaces.
 
 
 # 0.30
+@dataclass
 class _cmarkCmarkChunk:
-    __slots__ = [
-        'data',
-        'length',
-    ]
-
-    def __init__(self, data: str = None, length: int = 0):
-        self.data: str = data
-        self.length: int = length
+    data: str = None
+    length: int = 0
 
 
 # 0.30
 def _cmark_cmark_chunk_free(c: _cmarkCmarkChunk):
     c.data = None
     c.length = 0
```

### Comparing `md_toc-8.2.3/md_toc/cmark/cmark_ctype_c.py` & `md_toc-9.0.0/md_toc/cmark/cmark_ctype_c.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,36 +16,35 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
 r"""The cmark implementation file."""
 
+import string
+import unicodedata
+
 from ..constants import parser as md_parser
 
 # License C applies to this file except for non derivative code:
 # in that case the license header at the top of the file applies.
 # See docs/copyright_license.rst
 
 
 # Return True if c is a "whitespace" character as defined by the spec.
 # 0.30
 def _cmark_cmark_isspace(char: int) -> bool:
-    value = False
-    if chr(char) in md_parser['cmark']['pseudo-re']['UWC']:
-        value = True
-
-    return value
+    # A Unicode whitespace character is any code point in the Unicode Zs
+    # general category, or a tab (U+0009), line feed (U+000A), form feed
+    # (U+000C), or carriage return (U+000D).
+    return (unicodedata.category(chr(char)) == 'Zs'
+            or chr(char) in ['\u0009', '\u000A', '\u000C', '\u000D'])
 
 
 # Return True if c is an ascii punctuation character.
 # 0.29, 0.30
 def _cmark_cmark_ispunct(char: int) -> bool:
-    value = False
-    if chr(char) in md_parser['cmark']['pseudo-re']['APC']:
-        value = True
-
-    return value
+    return chr(char) in string.punctuation
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `md_toc-8.2.3/md_toc/cmark/cmark_h.py` & `md_toc-9.0.0/md_toc/cmark/cmark_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/houdini_h.py` & `md_toc-9.0.0/md_toc/cmark/houdini_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/houdini_html_u_c.py` & `md_toc-9.0.0/md_toc/cmark/houdini_html_u_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/inlines_c.py` & `md_toc-9.0.0/md_toc/cmark/inlines_c.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # inlines_c.py
 #
-# Copyright (C) 2017-2022 Franco Masotti (see /README.md)
+# Copyright (C) 2017-2023 Franco Masotti (see /README.md)
 #
 # This file is part of md-toc.
 #
 # md-toc is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -146,40 +146,14 @@
         self.delim_char = ''
         self.can_open: bool = False
         self.can_close: bool = False
 
         # Extra attribute.
         self.offset: int = 0
 
-    def __str__(self):
-        if self.delim_char is not None:
-            if self.previous is None:
-                previous = 'None'
-            else:
-                previous = hex(id(self.previous))
-            if self.next is None:
-                next = 'None'
-            else:
-                next = hex(id(self.next))
-
-            el = '== element ' + hex(id(self)) + ' =='
-            it = 'inl_text = ' + str(self.inl_text)
-            de = 'delim_char = ' + self.delim_char
-            le = 'length = ' + str(self.length)
-            of = 'offset = ' + str(self.offset)
-            ac = 'active = ' + str(self.active)
-            pr = 'previous = ' + previous
-            ne = 'next = ' + next
-            co = 'can_open = ' + str(self.can_open)
-            cc = 'can_close = ' + str(self.can_close)
-
-            return (el + '\n' + it + '\n' + '\n' + de + '\n' + le + '\n' + of +
-                    '\n' + ac + '\n' + pr + '\n' + ne + '\n' + co + '\n' + cc +
-                    '\n')
-
 
 class _cmarkBracket:
     __slots__ = [
         'previous',
         'previous_delimiter',
         'inl_text',
         'position',
@@ -229,23 +203,14 @@
         self.last_bracket: _cmarkBracket = None
 
         # An integer list.
         self.backticks: list = list(range(0, MAXBACKTICKS + 1))
 
         self.scanned_for_backticks: bool = False
 
-    def scroll(self):
-        r"""Print the list."""
-        print(self.start)
-        print('===')
-        x = self.start
-        while x is not None:
-            print(x)
-            x = x.next
-
 
 # 0.30
 def _cmark_S_is_line_end_char(c: str) -> bool:
     return c == '\n' or c == '\r'
 
 
 # 0.30
@@ -421,14 +386,17 @@
 
     return backtick
 
 
 # 0.29, 0.30
 def _cmark_peek_char(subj: _cmarkSubject) -> int:
     # Instead of using assert just raise a ValueError
+    #
+    # NULL bytes should have been stripped out by now.  If they're
+    # present, it's a programming error:
     if subj.pos < subj.input.length and ord(subj.input.data[subj.pos]) == 0:
         raise ValueError
 
     if subj.pos < subj.input.length:
         return ord(subj.input.data[subj.pos])
     else:
         return 0
@@ -2069,24 +2037,22 @@
         0,
         0,
         0,
     ]
 
     n: int = subj.pos + 1
 
-    # Patch to avoid overflow problems.
-    # FIXME: this should not be needed!
-    if n > subj.input.length - 1:
-        return subj.input.length
-    if ord(subj.input.data[n]) > len(SPECIAL_CHARS) - 1 or ord(
-            subj.input.data[n]) > len(SMART_PUNCT_CHARS) - 1:
-        return n
-    # End patch.
-
     while n < subj.input.length:
+        # Patch to avoid overflow problems.
+        # FIXME: this should not be needed!
+        # These two are not present in the original C source code.
+        if (ord(subj.input.data[n]) > len(SPECIAL_CHARS)
+                or ord(subj.input.data[n]) > len(SMART_PUNCT_CHARS)):
+            return n
+
         if SPECIAL_CHARS[ord(subj.input.data[n])] == 1:
             return n
         if options & CMARK_OPT_SMART and SMART_PUNCT_CHARS[ord(
                 subj.input.data[n])]:
             return n
         n += 1
```

### Comparing `md_toc-8.2.3/md_toc/cmark/node_c.py` & `md_toc-9.0.0/md_toc/cmark/node_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/references_c.py` & `md_toc-9.0.0/md_toc/cmark/references_c.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     # A list of _cmarkCmarkReference
     ref: list = None
     r: _cmarkCmarkReference = None
     norm: str
 
     #     MAX_LINK_LABEL_LENGTH
     if label.length < 1 or label.length > md_parser['cmark']['link'][
-            'max chars label'] + 1:
+            'max_chars_label'] + 1:
         return None
 
     if maps is None or not maps.size:
         return None
 
     norm = _cmark_normalize_reference(maps.mem, label)
     if norm is None:
```

### Comparing `md_toc-8.2.3/md_toc/cmark/references_h.py` & `md_toc-9.0.0/md_toc/cmark/references_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/scanners_c.py` & `md_toc-9.0.0/md_toc/cmark/scanners_c.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/scanners_h.py` & `md_toc-9.0.0/md_toc/cmark/scanners_h.py`

 * *Files identical despite different names*

### Comparing `md_toc-8.2.3/md_toc/cmark/utf8_c.py` & `md_toc-9.0.0/md_toc/cmark/utf8_c.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,27 +164,20 @@
         # Reduce string length.
         length -= char_len
 
 
 # 0.29, 0.30
 def _cmark_cmark_utf8proc_is_space(char: int) -> bool:
     r"""Match anything in the Zs class, plus LF, CR, TAB, FF."""
-    value = False
-    if chr(char) in md_parser['cmark']['pseudo-re']['UWC']:
-        value = True
-
-    return value
+    return (unicodedata.category(chr(char)) == 'Zs'
+            or chr(char) in ['\u0009', '\u000A', '\u000C', '\u000D'])
 
 
 # 0.29, 0.30
 def _cmark_cmark_utf8proc_is_punctuation(char: int) -> bool:
     r"""Match anything in the P[cdefios] classes."""
-    value = False
-    if ((char < 128 and _cmark_cmark_ispunct(char))
-            or chr(char) in md_parser['cmark']['pseudo-re']['UPC']):
-        value = True
-
-    return value
+    return ((char < 128 and _cmark_cmark_ispunct(char))
+            or unicodedata.category(chr(char)).startswith('P'))
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `md_toc-8.2.3/md_toc/exceptions.py` & `md_toc-9.0.0/md_toc/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,7 @@
 
 class TocDoesNotRenderAsCoherentList(Exception):
     """TOC list indentations are either wrong or not what the user intended."""
 
 
 class StringCannotContainNewlines(Exception):
     """The specified string cannot contain newlines."""
-
-
-class CannotTreatUnicodeString(Exception):
-    """Cannot treat unicode string.
-
-    .. note:: This exception is deprecated and will be removed in the next major release.
-    """
```

### Comparing `md_toc-8.2.3/md_toc/generic.py` & `md_toc-9.0.0/md_toc/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # generic.py
 #
-# Copyright (C) 2017-2022 Franco Masotti (see /README.md)
+# Copyright (C) 2017-2023 Franco Masotti (see /README.md)
 #
 # This file is part of md-toc.
 #
 # md-toc is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -19,15 +19,14 @@
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Generic functions."""
 
 from __future__ import annotations
 
 import re
-import typing
 
 import fpyutils
 
 
 # _ctoi and _isascii taken from cpython source Lib/curses/ascii.py
 # See:
 # https://github.com/python/cpython/blob/283de2b9c18e38c9a573526d6c398ade7dd6f8e9/Lib/curses/ascii.py#L48
@@ -36,17 +35,17 @@
 # These two functions are released under the
 # PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
 # See https://directory.fsf.org/wiki/License:Python-2.0.1
 def _ctoi(c: str) -> int:
     if not len(c) == 1:
         raise ValueError
 
-    retval: str = c
+    retval: str | int = c
     if isinstance(c, str):
-        retval: int = ord(c)
+        retval = ord(c)
 
     return retval
 
 
 def _isascii(c) -> int:
     return 0 <= _ctoi(c) <= 127
 
@@ -66,16 +65,15 @@
                 lines.append(line)
             line = f.readline()
             line_counter += 1
 
     return ''.join(lines)
 
 
-def _remove_line_intervals(filename: str,
-                           line_intervals: list[list[typing.Sequence]]):
+def _remove_line_intervals(filename: str, line_intervals: list[list[int]]):
     # A nested list of integers divided in couples is expected.
     # Example: [[1, 4], [8, 9]]
     for interval in line_intervals:
         if len(interval) != 2 or interval[0] < 1 or interval[
                 1] < 1 or interval[0] > interval[1]:
             raise ValueError
```

### Comparing `md_toc-8.2.3/md_toc/types.py` & `md_toc-9.0.0/md_toc/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,71 +14,65 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with md-toc.  If not, see <http://www.gnu.org/licenses/>.
 #
-r"""Complex dict type definitions."""
+r"""Complex ``dict`` type definitions."""
 from typing import TypedDict
 
 
 class IndentationLogElement(TypedDict, total=False):
     r"""An ``indentation_log_element`` object.
 
     :parameter index: values: 1 -> md_parser['github']['header']['max levels'] + 1.
     :parameter list marker: ordered or undordered list marker.
     :parameter indentation spaces: number of indentation spaces.
     :type index: int
     :type list marker: str
     :type indentation spaces: int
     """
 
-    # index: 1 -> md_parser['github']['header']['max levels'] + 1
+    # index: 1 -> md_parser['github']['header']['max_levels'] + 1
     index: int
-    # FIXME
-    # Spaces are not allowed.
-
-
-#    list marker: str
-#    indentation spaces: int
+    list_marker: str
+    indentation_spaces: int
 
 
 class Header(TypedDict):
     r"""A ``header`` object.
 
-    :parameter type: h1 to h6 (``1`` -> ``6``).
+    :parameter header_type: h1 to h6 (``1`` -> ``6``).
     :parameter text_original: Raw text.
     :parameter text_anchor_link: Transformed text so it works as an anchor
        link.
     :parameter visible: if ``True`` the header needs to be visible, if
        ``False`` it will not.
-    :type type: int
+    :type header_type: int
     :type text_original: str
     :type text_anchor_link: str
     :type visible: bool
     """
 
-    type: int
+    header_type: int
     text_original: str
     text_anchor_link: str
     visible: bool
 
 
 class HeaderTypeCounter(TypedDict, total=False):
     r"""The number of headers for each type, from ``h1`` to ``h6``."""
 
-    # Should be something like:
-    # '1': int
-    # '2': int
-    # '3': int
-    # '4': int
-    # '5': int
-    # '6': int
-    pass
+    h1: int
+    h2: int
+    h3: int
+    h4: int
+    h5: int
+    h6: int
 
 
 class HeaderDuplicateCounter(TypedDict, total=False):
     r"""A ``header_duplicate_counter`` object.
 
     :parameter ``key``: a generic string corresponding to header links. Its
        value is the number of times ``key`` appears during the execution of
@@ -89,25 +83,25 @@
 
     key: int
 
 
 class AtxHeadingStructElement(TypedDict, total=False):
     """A single element of the list returned by the ``get_atx_heading`` function.
 
-    :parameter header type: h1 to h6 (``1`` -> ``6``).
-    :parameter header text trimmed: the link label.
+    :parameter header_type: h1 to h6 (``1`` -> ``6``).
+    :parameter header_text trimmed: the link label.
     :parameter visible: if the line has a smaller header that
        ``keep_header_levels``, then ``visible`` is set to ``False``.
-    :type header type: int
-    :type header text trimmed: str
+    :type header_type: int
+    :type header_text_trimmed: str
     :type visible: bool
 
-    .. note:: ``header type`` and ``header text trimmed`` are
+    .. note:: ``header_type`` and ``header_text_trimmed`` are
        set to ``None`` if the line does not contain header elements according
        to the rules of the selected markdown parser.
        ``visible`` is set to ``True`` if the line needs to be saved, ``False``
        if it just needed for duplicate counting.
     """
 
-    # header type: int
-    # header text trimmed: str
+    header_type: int
+    header_text_trimmed: str
     visible: bool
```

### Comparing `md_toc-8.2.3/md_toc.egg-info/PKG-INFO` & `md_toc-9.0.0/md_toc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md_toc
-Version: 8.2.3
+Version: 9.0.0
 Summary: Automatically generate and add an accurate table of contents to markdown files
 Home-page: https://blog.franco.net.eu.org/software/#md-toc
 Author: Franco Masotti
 Author-email: franco.masotti@tutanota.com
 License: GPLv3+,
 Project-URL: Bug Tracker, https://github.com/frnmst/md-toc/issues
 Project-URL: Documentation, https://docs.franco.net.eu.org/md-toc/
@@ -148,15 +148,15 @@
 ### foo
 ## file
 
 ## bye
 
 # bye
 
-$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github -l6 foo.md
+$ md_toc --in-place github --header-levels 6 foo.md        # or: md_toc -p github foo.md
 $ cat foo.md
 
 # Table of contents
 
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
@@ -208,14 +208,15 @@
 
 # bye
 >>> print(md_toc.build_toc('foo.md'), end='')
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 ```
 
 You can also write the TOC in place:
@@ -250,14 +251,15 @@
 <!--TOC-->
 
 - [Table of contents](#table-of-contents)
 - [this](#this)
   - [is](#is)
   - [a](#a)
     - [foo](#foo)
+      - [boo](#boo)
     - [foo](#foo-1)
   - [file](#file)
   - [bye](#bye)
 - [bye](#bye-1)
 
 <!--TOC-->
```

### Comparing `md_toc-8.2.3/md_toc.egg-info/SOURCES.txt` & `md_toc-9.0.0/md_toc.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.md
 SECURITY.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
 md_toc/__init__.py
 md_toc/__main__.py
 md_toc/api.py
 md_toc/cli.py
 md_toc/constants.py
```

### Comparing `md_toc-8.2.3/setup.cfg` & `md_toc-9.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md_toc
-version = 8.2.3
+version = 9.0.0
 license = GPLv3+,
 description = Automatically generate and add an accurate table of contents to markdown files
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Franco Masotti
 author_email = franco.masotti@tutanota.com
 keywords = 
@@ -39,16 +39,15 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: 3.13
 
 [options]
 python_requires = >=3.8
-install_requires = 
-	fpyutils >=4.0.1, <5
+install_requires = file: requirements.txt
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	md_toc = md_toc.__main__:main
 
 [options.packages.find]
@@ -81,15 +80,25 @@
 env_list = py{38,39,310,311,312,313}
 
 [testenv]
 description = run the tests with unittest
 package = wheel
 wheel_build_env = .pkg
 deps = 
-	pyfakefs>=5,<6
+	-r requirements.txt
+	-r requirements-dev.txt
 commands = 
-	python -m unittest md_toc.tests.tests --failfast --locals --verbose
+	python3 -m unittest md_toc.tests.tests --failfast --locals --verbose
+
+[testenv:fuzzer]
+description = run the fuzzer
+package = wheel
+wheel_build_env = .pkg
+deps = 
+	atheris>=2.3,<2.4
+commands = 
+	python3 -m md_toc.tests.fuzzer
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

