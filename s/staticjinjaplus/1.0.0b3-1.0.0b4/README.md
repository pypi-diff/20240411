# Comparing `tmp/staticjinjaplus-1.0.0b3.tar.gz` & `tmp/staticjinjaplus-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.0.0b3.tar", last modified: Mon Apr  8 16:12:14 2024, max compression
+gzip compressed data, was "staticjinjaplus-1.0.0b4.tar", last modified: Mon Apr  8 18:04:55 2024, max compression
```

## Comparing `staticjinjaplus-1.0.0b3.tar` & `staticjinjaplus-1.0.0b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.140244 staticjinjaplus-1.0.0b3/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b3/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b3/MANIFEST.in
--rw-rw-rw-   0        0        0    12082 2024-04-08 16:12:14.139245 staticjinjaplus-1.0.0b3/PKG-INFO
--rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 16:12:14.140244 staticjinjaplus-1.0.0b3/setup.cfg
--rw-rw-rw-   0        0        0     3598 2024-04-08 11:58:14.000000 staticjinjaplus-1.0.0b3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.121245 staticjinjaplus-1.0.0b3/staticjinjaplus/
--rw-rw-rw-   0        0        0     5799 2024-04-08 16:08:00.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       23 2024-04-08 16:10:32.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     1280 2024-04-07 14:43:00.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/jinja_helpers.py
--rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b3/staticjinjaplus/staticjinja_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:12:14.138244 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0    12082 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 16:12:14.000000 staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.942193 staticjinjaplus-1.0.0b4/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b4/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b4/MANIFEST.in
+-rw-rw-rw-   0        0        0    12082 2024-04-08 18:04:55.941194 staticjinjaplus-1.0.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:04:55.943193 staticjinjaplus-1.0.0b4/setup.cfg
+-rw-rw-rw-   0        0        0     3800 2024-04-08 18:01:44.000000 staticjinjaplus-1.0.0b4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.923193 staticjinjaplus-1.0.0b4/staticjinjaplus/
+-rw-rw-rw-   0        0        0     5720 2024-04-08 16:15:49.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       23 2024-04-08 16:16:48.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     1290 2024-04-08 16:15:31.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.940194 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    12082 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.0.0b3/LICENSE.md` & `staticjinjaplus-1.0.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b3/PKG-INFO` & `staticjinjaplus-1.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
```

### Comparing `staticjinjaplus-1.0.0b3/README.md` & `staticjinjaplus-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b3/setup.py` & `staticjinjaplus-1.0.0b4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Original setup.py template: https://github.com/kennethreitz/setup.py
 
 from setuptools import find_packages, setup, Command
+from importlib import util as importlib_util
+from subprocess import call
 from shutil import rmtree
-import io
-import os
+from os import path
 import sys
 
 NAME = 'staticjinjaplus'
 DESCRIPTION = 'An opinionated sweet spot between staticjinja and a full-blown static site generator.'
 URL = 'https://github.com/EpocDotFr/staticjinjaplus'
 EMAIL = 'contact.nospam@epoc.nospam.fr'
 AUTHOR = 'Maxime "Epoc" Gross'
@@ -44,66 +45,72 @@
 PROJECT_URLS = {
     'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage',
     'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
     'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
     'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
 }
 
-here = os.path.abspath(os.path.dirname(__file__))
+here = path.abspath(path.dirname(__file__))
 
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+    with open(path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 about = {}
 
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
 
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
+    spec = importlib_util.spec_from_file_location('__version__', path.join(here, project_slug, '__version__.py'))
+    module = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(module)
+
+    about['__version__'] = module.__version__
 else:
     about['__version__'] = VERSION
 
 
 class UploadCommand(Command):
     description = 'Build and publish the package.'
     user_options = []
 
     @staticmethod
     def status(s):
-        """Prints things in bold."""
         print('\033[1m{0}\033[0m'.format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
             self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+
+            rmtree(path.join(here, 'dist'))
         except OSError:
             pass
 
         self.status('Building Source and Wheel distribution…')
-        os.system('"{0}" -m build --sdist --wheel'.format(sys.executable))
+
+        call('"{0}" -m build --sdist --wheel'.format(sys.executable), shell=True)
 
         self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
+
+        call('twine upload dist/*', shell=True)
 
         self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
 
-        sys.exit()
+        call('git tag v{0}'.format(about['__version__']), shell=True)
+        call('git push --tags', shell=True)
+
+        exit()
 
 
 setup(
     name=NAME,
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
```

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus/__init__.py` & `staticjinjaplus-1.0.0b4/staticjinjaplus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,31 +136,30 @@
     if path.isdir(config['OUTPUT_DIR']):
         rmtree(config['OUTPUT_DIR'])
 
     makedirs(config['OUTPUT_DIR'], exist_ok=True)
 
 
 def publish(config: Dict) -> None:
-    """Publish the site (using `rsync` through SSH)"""
+    """Build and publish the site (using `rsync` through SSH)"""
     print('Overriding some configuration values from environment variables...')
 
     env = Env()
 
-    try:
-        config.update({
-            'BASE_URL': env.str('BASE_URL'),
-            'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
-            'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
-            'SSH_USER': env.str('SSH_USER'),
-            'SSH_HOST': env.str('SSH_HOST'),
-            'SSH_PORT': env.int('SSH_PORT', default=22),
-            'SSH_PATH': env.str('SSH_PATH'),
-        })
-    except ValueError as e:
-        print(e, file=sys.stderr)
+    config.update({
+        'BASE_URL': env.str('BASE_URL'),
+        'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
+        'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
+        'SSH_USER': env.str('SSH_USER'),
+        'SSH_HOST': env.str('SSH_HOST'),
+        'SSH_PORT': env.int('SSH_PORT', default=22),
+        'SSH_PATH': env.str('SSH_PATH'),
+    })
+
+    build(config)
 
     exit(call(
         'rsync --delete --exclude ".DS_Store" -pthrvz -c '
         '-e "ssh -p {SSH_PORT}" '
         '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
             config['OUTPUT_DIR'].rstrip('/') + '/', **config
         ),
```

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus/cli.py` & `staticjinjaplus-1.0.0b4/staticjinjaplus/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         '-w', '--watch',
         help='Automatically rebuild the site when templates are modified',
         action='store_true'
     )
 
     command_arg_parser.add_parser('clean', help='Delete and recreate the output directory')
 
-    command_arg_parser.add_parser('publish', help='Publish the site (using `rsync` through SSH)')
+    command_arg_parser.add_parser('publish', help='Build and publish the site (using `rsync` through SSH)')
 
     command_arg_parser.add_parser('serve', help='Serve the rendered site directory through HTTP')
 
     args = arg_parser.parse_args()
 
     config = staticjinjaplus.load_config()
```

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus/http.py` & `staticjinjaplus-1.0.0b4/staticjinjaplus/http.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-1.0.0b4/staticjinjaplus/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus/staticjinja_helpers.py` & `staticjinjaplus-1.0.0b4/staticjinjaplus/staticjinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b3/staticjinjaplus.egg-info/PKG-INFO` & `staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staticjinjaplus
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: An opinionated sweet spot between staticjinja and a full-blown static site generator.
 Home-page: https://github.com/EpocDotFr/staticjinjaplus
 Author: Maxime "Epoc" Gross
 Author-email: contact.nospam@epoc.nospam.fr
 License: DBAD
 Project-URL: Documentation, https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage
 Project-URL: Source, https://github.com/EpocDotFr/staticjinjaplus
```

