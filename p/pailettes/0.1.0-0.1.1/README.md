# Comparing `tmp/pailettes-0.1.0.tar.gz` & `tmp/pailettes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pailettes-0.1.0.tar", max compression
+gzip compressed data, was "pailettes-0.1.1.tar", max compression
```

## Comparing `pailettes-0.1.0.tar` & `pailettes-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-03-27 18:50:12.067866 pailettes-0.1.0/LICENSE
--rw-r--r--   0        0        0     1040 2024-04-11 15:28:34.260155 pailettes-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-27 19:37:48.611302 pailettes-0.1.0/pailettes/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-11 15:33:15.361423 pailettes-0.1.0/pailettes/main.py
--rw-r--r--   0        0        0      403 2024-04-11 15:23:49.202931 pailettes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 pailettes-0.1.0/setup.py
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 pailettes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-27 18:50:12.067866 pailettes-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1040 2024-04-11 15:28:34.260155 pailettes-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 19:37:48.611302 pailettes-0.1.1/pailettes/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-11 15:33:15.361423 pailettes-0.1.1/pailettes/main.py
+-rw-r--r--   0        0        0      403 2024-04-11 15:41:25.014909 pailettes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 pailettes-0.1.1/setup.py
+-rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 pailettes-0.1.1/PKG-INFO
```

### Comparing `pailettes-0.1.0/LICENSE` & `pailettes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pailettes-0.1.0/README.md` & `pailettes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pailettes-0.1.0/pailettes/main.py` & `pailettes-0.1.1/pailettes/main.py`

 * *Files identical despite different names*

### Comparing `pailettes-0.1.0/setup.py` & `pailettes-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['openai>=1.14.3,<2.0.0', 'rich>=13.7.1,<14.0.0', 'typer[all]>=0.11.0,<0.12.0']
 
 entry_points = \
 {'console_scripts': ['pailettes = pailettes.main:app']}
 
 setup_kwargs = {
     'name': 'pailettes',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# Pailettes\n\nGenerate color palettes using artificial intelligence. The OpenAI API is used for this, so you will require an account.\n\n![Pailettes](https://raw.githubusercontent.com/psyonara/pailettes/master/imgs/headline.jpg)\n\n## Installation\n\n### Pipx\n\n```shell\npipx install pailettes\n```\n\n### Pip\n\n```shell\npip install pailettes\n```\n\n## Configuration\n\nTo configure your OpenAI API key, create an environment variable as follows.\n\n### Windows\nTODO\n\n### MacOS\nTODO\n\n### Linux\n```shell\nexport OPENAI_KEY="your-key-goes-here"\n```\n\nThis will set your OpenAI key for that terminal session. If you would like to permanently set the environment variable, consult the documentation of your OS/shell.\n\n## Usage\n\n### Quick Start\n\n```shell\npailettes retro\n```\n\nThis creates a color palette with a "retro" theme.\n\n### Number of colors\n\nTo specify the number of colors in your palette:\n\n```shell\npailettes retro --color-count=6\n```\n\n### Number of palettes\n\nTo specify the number of palettes to generate:\n\n```shell\npailettes retro --palette-count=3\n```\n',
     'author': 'Helmut Irle',
     'author_email': 'me@helmut.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.11,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pailettes-0.1.0/PKG-INFO` & `pailettes-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pailettes
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Helmut Irle
 Author-email: me@helmut.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: typer[all] (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Pailettes
```

