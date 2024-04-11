# Comparing `tmp/dkist-sphinx-theme-1.1.2.tar.gz` & `tmp/dkist-sphinx-theme-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-sphinx-theme-1.1.2.tar", last modified: Thu Aug  3 08:18:40 2023, max compression
+gzip compressed data, was "dkist-sphinx-theme-2.0.0rc1.tar", last modified: Thu Apr 11 09:52:23 2024, max compression
```

## Comparing `dkist-sphinx-theme-1.1.2.tar` & `dkist-sphinx-theme-2.0.0rc1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    19617 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/
--rw-rw-rw-   0 root         (0) root         (0)      288 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/
--rw-rw-rw-   0 root         (0) root         (0)     2441 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/module.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/autoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/core.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     2524 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/verify_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     6191 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_intersphinx_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_requirements_table.py
--rw-rw-rw-   0 root         (0) root         (0)     6662 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_workflow_diagram.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/
--rw-rw-rw-   0 root         (0) root         (0)     2589 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/layout.html
--rw-rw-rw-   0 root         (0) root         (0)     1949 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/navbar.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/dkist.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/
--rw-rw-rw-   0 root         (0) root         (0)   147435 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg
--rw-rw-rw-   0 root         (0) root         (0)    18231 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/NSOlogo.gif
--rw-rw-rw-   0 root         (0) root         (0)    41662 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/favico.ico
--rw-rw-rw-   0 root         (0) root         (0)    10027 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/forkme.png
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/pdf_icon.png
--rw-rw-rw-   0 root         (0) root         (0)      322 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/theme.conf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/tests/test_import.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-03 08:18:40.611033 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-08-03 08:18:40.000000 dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-03 08:18:40.615033 dkist-sphinx-theme-1.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-08-03 08:18:35.000000 dkist-sphinx-theme-1.1.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)    19617 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      987 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-11 09:52:23.746403 dkist-sphinx-theme-2.0.0rc1/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/
+-rw-rw-rw-   0 root         (0) root         (0)     3884 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/module.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/autoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/core.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/verify_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     6191 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_intersphinx_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_requirements_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_workflow_diagram.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/tests/test_import.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.738403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    46900 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png
+-rw-rw-rw-   0 root         (0) root         (0)    23107 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png
+-rw-rw-rw-   0 root         (0) root         (0)    41662 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-11 09:52:06.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/theme.conf
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 09:52:23.742403 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-04-11 09:52:23.000000 dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/top_level.txt
```

### Comparing `dkist-sphinx-theme-1.1.2/LICENSE.rst` & `dkist-sphinx-theme-2.0.0rc1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/bitbucket-pipelines.yml` & `dkist-sphinx-theme-2.0.0rc1/bitbucket-pipelines.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
         script:
           - pip install .[test]
           - pytest -v
 
     - step:
         script:
           - python --version
-          - pip install -U --force-reinstall twine
-          - python setup.py sdist
+          - pip install -U --force-reinstall twine build
+          - python -m build
           - python -m twine check dist/*
 
   tags:
     'v*':
       - step:
           script:
-            - python setup.py sdist
-            - pip install twine
+            - pip install twine build
+            - python -m build
             - twine upload dist/*
```

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/autoapi_templates/python/module.rst` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/autoapi.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/autoapi.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/core.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/core.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/conf/verify_requirements.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/conf/verify_requirements.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_intersphinx_mapping.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_intersphinx_mapping.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_requirements_table.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_requirements_table.py`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/create_workflow_diagram.py` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/create_workflow_diagram.py`

 * *Files 12% similar despite different names*

```diff
@@ -162,25 +162,27 @@
     image map.
     """
     # Create a mapping from fully-qualified class names to URLs.
     graphviz_output_format = self.builder.env.config.graphviz_output_format.upper()
     current_filename = self.builder.current_docname + self.builder.out_suffix
     urls = {}
     for child in node:
-        if child.get("refuri") is not None:
-            refuri = child.get("refuri")
-            if graphviz_output_format == "SVG" and not refuri.startswith("http"):
-                urls[child.astext()] = "../" + refuri
+        if child.get('refuri') is not None:
+            # Construct the name from the URI if the reference is external via intersphinx
+            if not child.get('internal', True):
+                refname = child['refuri'].rsplit('#', 1)[-1]
             else:
-                urls[child.astext()] = refuri
-        elif child.get("refid") is not None:
-            if graphviz_output_format == "SVG":
-                urls[child.astext()] = "../" + current_filename + "#" + child.get("refid")
+                refname = child['reftitle']
+
+            urls[refname] = child.get('refuri')
+        elif child.get('refid') is not None:
+            if graphviz_output_format == 'SVG':
+                urls[child['reftitle']] = current_filename + '#' + child.get('refid')
             else:
-                urls[child.astext()] = "#" + child.get("refid")
+                urls[child['reftitle']] = '#' + child.get('refid')
 
     dotcode = render_workflow(node["workflow"], urls=urls).source
     render_dot_html(self, node, dotcode, node["options"], filename=node.get("filename"))
     raise nodes.SkipNode
 
 
 def setup(app):
```

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme/dkist/static/img/favico.ico` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico`

 * *Files identical despite different names*

### Comparing `dkist-sphinx-theme-1.1.2/dkist_sphinx_theme.egg-info/SOURCES.txt` & `dkist-sphinx-theme-2.0.0rc1/src/dkist_sphinx_theme.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-.gitignore
 LICENSE.rst
 MANIFEST.in
 README.md
 bitbucket-pipelines.yml
-setup.py
-dkist_sphinx_theme/__init__.py
-dkist_sphinx_theme/create_intersphinx_mapping.py
-dkist_sphinx_theme/create_requirements_table.py
-dkist_sphinx_theme/create_workflow_diagram.py
-dkist_sphinx_theme.egg-info/PKG-INFO
-dkist_sphinx_theme.egg-info/SOURCES.txt
-dkist_sphinx_theme.egg-info/dependency_links.txt
-dkist_sphinx_theme.egg-info/requires.txt
-dkist_sphinx_theme.egg-info/top_level.txt
-dkist_sphinx_theme/autoapi_templates/python/module.rst
-dkist_sphinx_theme/conf/__init__.py
-dkist_sphinx_theme/conf/autoapi.py
-dkist_sphinx_theme/conf/core.py
-dkist_sphinx_theme/conf/theme.py
-dkist_sphinx_theme/conf/verify_requirements.py
-dkist_sphinx_theme/dkist/layout.html
-dkist_sphinx_theme/dkist/navbar.html
-dkist_sphinx_theme/dkist/theme.conf
-dkist_sphinx_theme/dkist/static/dkist.css
-dkist_sphinx_theme/dkist/static/img/DKISTLogo-Medium.jpg
-dkist_sphinx_theme/dkist/static/img/NSOlogo.gif
-dkist_sphinx_theme/dkist/static/img/favico.ico
-dkist_sphinx_theme/dkist/static/img/forkme.png
-dkist_sphinx_theme/dkist/static/img/pdf_icon.png
-dkist_sphinx_theme/tests/__init__.py
-dkist_sphinx_theme/tests/test_import.py
+pyproject.toml
+setup.cfg
+src/dkist_sphinx_theme/__init__.py
+src/dkist_sphinx_theme/create_intersphinx_mapping.py
+src/dkist_sphinx_theme/create_requirements_table.py
+src/dkist_sphinx_theme/create_workflow_diagram.py
+src/dkist_sphinx_theme.egg-info/PKG-INFO
+src/dkist_sphinx_theme.egg-info/SOURCES.txt
+src/dkist_sphinx_theme.egg-info/dependency_links.txt
+src/dkist_sphinx_theme.egg-info/entry_points.txt
+src/dkist_sphinx_theme.egg-info/requires.txt
+src/dkist_sphinx_theme.egg-info/top_level.txt
+src/dkist_sphinx_theme/autoapi_templates/python/module.rst
+src/dkist_sphinx_theme/conf/__init__.py
+src/dkist_sphinx_theme/conf/autoapi.py
+src/dkist_sphinx_theme/conf/core.py
+src/dkist_sphinx_theme/conf/theme.py
+src/dkist_sphinx_theme/conf/verify_requirements.py
+src/dkist_sphinx_theme/tests/__init__.py
+src/dkist_sphinx_theme/tests/test_import.py
+src/dkist_sphinx_theme/theme/dkist/theme.conf
+src/dkist_sphinx_theme/theme/dkist/static/css/dkist.css
+src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-blue-text.png
+src/dkist_sphinx_theme/theme/dkist/static/img/dkist-logo-v5-white-text.png
+src/dkist_sphinx_theme/theme/dkist/static/img/favico.ico
+src/dkist_sphinx_theme/theme/dkist/static/img/nso_logo.png
```

