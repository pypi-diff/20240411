# Comparing `tmp/shellplus-0.0.7a1.tar.gz` & `tmp/shellplus-0.0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellplus-0.0.7a1.tar", last modified: Tue Apr  2 09:53:04 2024, max compression
+gzip compressed data, was "shellplus-0.0.8b0.tar", last modified: Thu Apr 11 17:04:56 2024, max compression
```

## Comparing `shellplus-0.0.7a1.tar` & `shellplus-0.0.8b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.341572 shellplus-0.0.7a1/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:53:04.339570 shellplus-0.0.7a1/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.7a1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 09:53:04.341572 shellplus-0.0.7a1/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-04-02 09:52:47.000000 shellplus-0.0.7a1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.329785 shellplus-0.0.7a1/shellplus/
--rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.7a1/shellplus/__init__.py
--rw-rw-rw-   0        0        0      743 2024-04-02 09:16:37.000000 shellplus-0.0.7a1/shellplus/colors1.py
--rw-rw-rw-   0        0        0     1060 2024-04-02 09:11:30.000000 shellplus-0.0.7a1/shellplus/styles.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:53:04.338568 shellplus-0.0.7a1/shellplus.egg-info/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 09:53:04.000000 shellplus-0.0.7a1/shellplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.269070 shellplus-0.0.8b0/
+-rw-rw-rw-   0        0        0     1096 2024-04-11 17:04:56.267170 shellplus-0.0.8b0/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2024-01-26 16:03:46.000000 shellplus-0.0.8b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 17:04:56.269070 shellplus-0.0.8b0/setup.cfg
+-rw-rw-rw-   0        0        0      804 2024-04-11 17:04:23.000000 shellplus-0.0.8b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.258621 shellplus-0.0.8b0/shellplus/
+-rw-rw-rw-   0        0        0        0 2024-01-26 10:57:43.000000 shellplus-0.0.8b0/shellplus/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-04-02 09:16:37.000000 shellplus-0.0.8b0/shellplus/colors1.py
+-rw-rw-rw-   0        0        0     1046 2024-04-11 16:26:02.000000 shellplus-0.0.8b0/shellplus/styles.py
+drwxrwxrwx   0        0        0        0 2024-04-11 17:04:56.266169 shellplus-0.0.8b0/shellplus.egg-info/
+-rw-rw-rw-   0        0        0     1096 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 17:04:56.000000 shellplus-0.0.8b0/shellplus.egg-info/top_level.txt
```

### Comparing `shellplus-0.0.7a1/PKG-INFO` & `shellplus-0.0.8b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.7a1
-Classifier: Development Status :: 3 - Alpha
+Version: 0.0.8b0
+License: Unlicense
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: rich
 
 # ShellPlus
 
 ShellPlus is a Python package designed to streamline terminal text formatting, providing predefined styles and colors for efficient coding with colors and formatting in the terminal.
```

### Comparing `shellplus-0.0.7a1/README.md` & `shellplus-0.0.8b0/README.md`

 * *Files identical despite different names*

### Comparing `shellplus-0.0.7a1/setup.py` & `shellplus-0.0.8b0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='shellplus',
-    version='0.0.7a01',
+    version='0.0.8b0',
     packages=find_packages(),
     install_requires=[
         'rich',  # Add any other dependencies here
     ],
     setup_requires=['wheel'],  # Add 'wheel' to setup_requires
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: Public Domain',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     # Add the long_description field
     long_description=long_description,
     long_description_content_type='text/markdown',  # Assuming it's a Markdown file
+    license='Unlicense',
 )
```

### Comparing `shellplus-0.0.7a1/shellplus/colors1.py` & `shellplus-0.0.8b0/shellplus/colors1.py`

 * *Files identical despite different names*

### Comparing `shellplus-0.0.7a1/shellplus/styles.py` & `shellplus-0.0.8b0/shellplus/styles.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 
 styles = {
     'info': 'bold blue',
     'warn': 'italic yellow',
     'warning': 'italic yellow',
     'err': 'bold red',
     'error': 'bold red',
-    'serr': style.Style(color='#FA6E69', style='bold',),
-    'serror': style.Style(color='#FA6E69', style='bold',),
-    'softerr': style.Style(color='#FA6E69', style='bold',),
-    'softerror': style.Style(color='#FA6E69', style='bold',),
+    'serr': style.Style(color='#FA6E69', bold=True),
+    'serror': style.Style(color='#FA6E69', bold=True),
+    'softerr': style.Style(color='#FA6E69', bold=True),
+    'softerror': style.Style(color='#FA6E69', bold=True),
     'note': 'dim italic',
-    'worry': style.Style(color='#fdff8e',),
-    'invalid': style.Style(color='#ff3d3d', style='underline italic',),
+    'worry': style.Style(color='#fdff8e'),
+    'invalid': style.Style(color='#ff3d3d', underline=True, italic=True),
     'marked1': 'reverse yellow',
     'marked2': 'reverse green',
     'no_intr': 'strikethrough dim',
     'nointr': 'strikethrough dim',
     'no_interest': 'strikethrough dim',
     'nointerest': 'strikethrough dim',
     'unimportant': 'strikethrough dim',
-    'comment': style.Style(color='#186218', style='dim',),
+    'comment': style.Style(color='#186218', dim=True),
 }
 
-def print(message, style):
+def print_styled(message, style):
     shell = Console()
     stil = styles.get(style, '')
     shell.print(f'[{stil}]{message}[/{stil}]')
-
```

### Comparing `shellplus-0.0.7a1/shellplus.egg-info/PKG-INFO` & `shellplus-0.0.8b0/shellplus.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: shellplus
-Version: 0.0.7a1
-Classifier: Development Status :: 3 - Alpha
+Version: 0.0.8b0
+License: Unlicense
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: rich
 
 # ShellPlus
 
 ShellPlus is a Python package designed to streamline terminal text formatting, providing predefined styles and colors for efficient coding with colors and formatting in the terminal.
```

