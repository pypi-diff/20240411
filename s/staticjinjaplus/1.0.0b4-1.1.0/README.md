# Comparing `tmp/staticjinjaplus-1.0.0b4.tar.gz` & `tmp/staticjinjaplus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticjinjaplus-1.0.0b4.tar", last modified: Mon Apr  8 18:04:55 2024, max compression
+gzip compressed data, was "staticjinjaplus-1.1.0.tar", last modified: Thu Apr 11 08:45:33 2024, max compression
```

## Comparing `staticjinjaplus-1.0.0b4.tar` & `staticjinjaplus-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.942193 staticjinjaplus-1.0.0b4/
--rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.0.0b4/LICENSE.md
--rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.0.0b4/MANIFEST.in
--rw-rw-rw-   0        0        0    12082 2024-04-08 18:04:55.941194 staticjinjaplus-1.0.0b4/PKG-INFO
--rw-rw-rw-   0        0        0    10664 2024-04-08 15:54:17.000000 staticjinjaplus-1.0.0b4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-08 18:04:55.943193 staticjinjaplus-1.0.0b4/setup.cfg
--rw-rw-rw-   0        0        0     3800 2024-04-08 18:01:44.000000 staticjinjaplus-1.0.0b4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.923193 staticjinjaplus-1.0.0b4/staticjinjaplus/
--rw-rw-rw-   0        0        0     5720 2024-04-08 16:15:49.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/__init__.py
--rw-rw-rw-   0        0        0       23 2024-04-08 16:16:48.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/__version__.py
--rw-rw-rw-   0        0        0     1290 2024-04-08 16:15:31.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/cli.py
--rw-rw-rw-   0        0        0     2407 2024-04-07 14:45:03.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/http.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/jinja_helpers.py
--rw-rw-rw-   0        0        0      712 2024-04-07 14:40:31.000000 staticjinjaplus-1.0.0b4/staticjinjaplus/staticjinja_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 18:04:55.940194 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/
--rw-rw-rw-   0        0        0    12082 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-08 18:04:55.000000 staticjinjaplus-1.0.0b4/staticjinjaplus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.370458 staticjinjaplus-1.1.0/
+-rw-rw-rw-   0        0        0     1161 2024-04-04 21:49:57.000000 staticjinjaplus-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2024-04-04 21:50:17.000000 staticjinjaplus-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20489 2024-04-11 08:45:33.369458 staticjinjaplus-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18804 2024-04-11 08:36:27.000000 staticjinjaplus-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 08:45:33.370458 staticjinjaplus-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4098 2024-04-11 08:37:09.000000 staticjinjaplus-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.348457 staticjinjaplus-1.1.0/staticjinjaplus/
+-rw-rw-rw-   0        0        0     6415 2024-04-11 08:42:19.000000 staticjinjaplus-1.1.0/staticjinjaplus/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-11 08:29:30.000000 staticjinjaplus-1.1.0/staticjinjaplus/__version__.py
+-rw-rw-rw-   0        0        0     1289 2024-04-08 22:09:51.000000 staticjinjaplus-1.1.0/staticjinjaplus/cli.py
+-rw-rw-rw-   0        0        0     2942 2024-04-11 08:42:04.000000 staticjinjaplus-1.1.0/staticjinjaplus/http.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 14:40:43.000000 staticjinjaplus-1.1.0/staticjinjaplus/jinja_helpers.py
+-rw-rw-rw-   0        0        0     1174 2024-04-09 21:15:15.000000 staticjinjaplus-1.1.0/staticjinjaplus/staticjinja_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-11 08:45:33.368458 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/
+-rw-rw-rw-   0        0        0    20489 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-11 08:45:33.000000 staticjinjaplus-1.1.0/staticjinjaplus.egg-info/top_level.txt
```

### Comparing `staticjinjaplus-1.0.0b4/LICENSE.md` & `staticjinjaplus-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b4/setup.py` & `staticjinjaplus-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 
 NAME = 'staticjinjaplus'
 DESCRIPTION = 'An opinionated sweet spot between staticjinja and a full-blown static site generator.'
 URL = 'https://github.com/EpocDotFr/staticjinjaplus'
 EMAIL = 'contact.nospam@epoc.nospam.fr'
 AUTHOR = 'Maxime "Epoc" Gross'
-REQUIRES_PYTHON = '>=3.12'
+REQUIRES_PYTHON = '>=3.9'
 VERSION = None  # Pulled from staticjinjaplus/__version__.py
 
 REQUIRED = [
     'staticjinja~=5.0',
     'webassets~=2.0',
     'htmlmin~=0.1',
     'cssutils~=2.10',
@@ -28,31 +28,37 @@
     'dev': {
         'build~=1.2',
         'twine~=5.0',
     }
 }
 
 CLASSIFIERS = [
-    'Development Status :: 4 - Beta',
+    'Development Status :: 5 - Production/Stable',
     'Operating System :: OS Independent',
+    'Environment :: Console',
     'Environment :: Web Environment',
-    'Topic :: Software Development :: Libraries',
+    'Topic :: Text Processing :: Markup :: XML',
     'Topic :: Text Processing :: Markup :: HTML',
     'Topic :: Text Processing :: Markup :: Markdown',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Intended Audience :: Developers',
 ]
 
 PROJECT_URLS = {
-    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#usage',
+    'Documentation': 'https://github.com/EpocDotFr/staticjinjaplus?tab=readme-ov-file#readme',
     'Source': 'https://github.com/EpocDotFr/staticjinjaplus',
     'Tracker': 'https://github.com/EpocDotFr/staticjinjaplus/issues',
     'Changelog': 'https://github.com/EpocDotFr/staticjinjaplus/releases',
 }
 
+KEYWORDS = ['static', 'website', 'site', 'generator', 'staticjinja', 'jinja', 'jinja2']
+
 here = path.abspath(path.dirname(__file__))
 
 try:
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
@@ -104,15 +110,14 @@
         self.status('Pushing git tags…')
 
         call('git tag v{0}'.format(about['__version__']), shell=True)
         call('git push --tags', shell=True)
 
         exit()
 
-
 setup(
     name=NAME,
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
@@ -129,9 +134,10 @@
             'staticjinjaplus = staticjinjaplus.cli:cli',
         ]
     },
     classifiers=CLASSIFIERS,
     cmdclass={
         'upload': UploadCommand,
     },
-    project_urls=PROJECT_URLS
-)
+    project_urls=PROJECT_URLS,
+    keywords=KEYWORDS
+)
```

### Comparing `staticjinjaplus-1.0.0b4/staticjinjaplus/__init__.py` & `staticjinjaplus-1.1.0/staticjinjaplus/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-from staticjinjaplus.http import ThreadingHTTPServerWithConfig, SimpleEnhancedHTTPRequestHandler
+from staticjinjaplus.http import EnhancedThreadingHTTPServer, SimpleEnhancedHTTPRequestHandler
+from staticjinjaplus import staticjinja_helpers, jinja_helpers
 from webassets import Environment as AssetsEnvironment
-from staticjinjaplus import staticjinja_helpers
 from importlib import util as importlib_util
-from staticjinjaplus import jinja_helpers
+from staticjinja import Site, logger
 from shutil import copytree, rmtree
 from os import makedirs, path
-from staticjinja import Site
 from subprocess import call
 from environs import Env
 from typing import Dict
 import locale
-import sys
 
 
 def load_config() -> Dict:
     """Load configuration from both `config.py` in the directory where staticjinjaplus is executed and environment
     variables, returning a dict representation of this configuration. Only uppercase variables are loaded"""
 
     # Set default config values
+    serve_port = 8080
+
     config = {
         'LOCALE': None,
-        'SERVE_PORT': 8080,
-        'BASE_URL': 'http://localhost:8080/',
+        'SERVE_PORT': serve_port,
+        'BASE_URL': f'http://localhost:{serve_port}/',
         'MINIFY_XML': False,
         'MINIFY_JSON': False,
         'TEMPLATES_DIR': 'templates',
         'OUTPUT_DIR': 'output',
         'STATIC_DIR': 'static',
         'ASSETS_DIR': 'assets',
         'ASSETS_BUNDLES': [],
         'CONTEXTS': [],
+        'GLOBALS': {},
+        'FILTERS': {},
+        'EXTENSIONS': [],
     }
 
     # Load and erase default config values from config.py, if the file exists
     try:
         spec = importlib_util.spec_from_file_location('config', 'config.py')
         actual_config = importlib_util.module_from_spec(spec)
         spec.loader.exec_module(actual_config)
@@ -56,63 +59,82 @@
 
     for code in config['LOCALE']:
         try:
             locale.setlocale(locale.LC_ALL, code)
 
             locale_successfully_set = True
 
-            print(f'System locale set to {code}')
+            logger.info(f'System locale set to {code}')
 
             break
         except locale.Error:
             pass
 
     if not locale_successfully_set:
-        print('Unable to set system locale', file=sys.stderr)
+        logger.error('Unable to set system locale')
 
 
 def build(config: Dict, watch: bool = False) -> None:
     """Build the site"""
     set_locale(config)
 
     webassets_cache = path.join(config['ASSETS_DIR'], '.webassets-cache')
 
     makedirs(webassets_cache, exist_ok=True)
     makedirs(config['STATIC_DIR'], exist_ok=True)
     makedirs(config['OUTPUT_DIR'], exist_ok=True)
     makedirs(config['ASSETS_DIR'], exist_ok=True)
 
-    print('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
+    logger.info('Copying static files from "{STATIC_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
 
     copytree(
         config['STATIC_DIR'],
         config['OUTPUT_DIR'],
         dirs_exist_ok=True
     )
 
-    print('Building from "{TEMPLATES_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
+    logger.info('Building from "{TEMPLATES_DIR}" to "{OUTPUT_DIR}"...'.format(**config))
+
+    rules = [
+        r for r in [
+            (r'.*\.(xml|html|rss|atom)', staticjinja_helpers.minify_xml_template) if config['MINIFY_XML'] else None,
+            (r'.*\.json', staticjinja_helpers.minify_json_template) if config['MINIFY_JSON'] else None,
+        ] if r is not None
+    ]
+
+    jinja_globals = {
+        'config': config,
+        'url': jinja_helpers.url(config),
+        'icon': jinja_helpers.icon(config),
+    }
+
+    jinja_globals.update(config['GLOBALS'])
+
+    jinja_filters = {
+        'tojsonm': jinja_helpers.tojsonm(config),
+        'dictmerge': jinja_helpers.dictmerge,
+    }
+
+    jinja_filters.update(config['FILTERS'])
+
+    jinja_extensions = [
+        'webassets.ext.jinja2.AssetsExtension',
+    ]
+
+    jinja_extensions.extend(config['EXTENSIONS'])
 
     site = Site.make_site(
         searchpath=config['TEMPLATES_DIR'],
         outpath=config['OUTPUT_DIR'],
         mergecontexts=True,
-        env_globals={
-            'config': config,
-            'url': jinja_helpers.url(config),
-            'icon': jinja_helpers.icon(config),
-        },
-        filters={
-            'tojsonm': jinja_helpers.tojsonm(config),
-            'dictmerge': jinja_helpers.dictmerge,
-        },
+        env_globals=jinja_globals,
+        filters=jinja_filters,
         contexts=config['CONTEXTS'] or None,
-        rules=[
-            (r'.*\.(html|xml)', staticjinja_helpers.minify_xml_template)
-        ] if config['MINIFY_XML'] else None,
-        extensions=['webassets.ext.jinja2.AssetsExtension'],
+        rules=rules or None,
+        extensions=jinja_extensions,
         env_kwargs={
             'trim_blocks': True,
             'lstrip_blocks': True,
         }
     )
 
     site.env.assets_environment = AssetsEnvironment(
@@ -127,56 +149,62 @@
         site.env.assets_environment.register(name, *args, **kwargs)
 
     site.render(watch)
 
 
 def clean(config: Dict) -> None:
     """Delete and recreate the output directory"""
-    print('Deleting and recreating "{OUTPUT_DIR}"...'.format(**config))
+    logger.info('Deleting and recreating "{OUTPUT_DIR}"...'.format(**config))
 
     if path.isdir(config['OUTPUT_DIR']):
         rmtree(config['OUTPUT_DIR'])
 
     makedirs(config['OUTPUT_DIR'], exist_ok=True)
 
 
 def publish(config: Dict) -> None:
     """Build and publish the site (using `rsync` through SSH)"""
-    print('Overriding some configuration values from environment variables...')
+    logger.info('Overriding some configuration values from environment variables...')
 
     env = Env()
 
     config.update({
         'BASE_URL': env.str('BASE_URL'),
         'MINIFY_XML': env.bool('MINIFY_XML', config['MINIFY_XML']),
         'MINIFY_JSON': env.bool('MINIFY_JSON', config['MINIFY_JSON']),
         'SSH_USER': env.str('SSH_USER'),
         'SSH_HOST': env.str('SSH_HOST'),
         'SSH_PORT': env.int('SSH_PORT', default=22),
         'SSH_PATH': env.str('SSH_PATH'),
     })
 
+    clean(config)
     build(config)
 
     exit(call(
         'rsync --delete --exclude ".DS_Store" -pthrvz -c '
         '-e "ssh -p {SSH_PORT}" '
         '{} {SSH_USER}@{SSH_HOST}:{SSH_PATH}'.format(
             config['OUTPUT_DIR'].rstrip('/') + '/', **config
         ),
         shell=True
     ))
 
 
 def serve(config: Dict) -> None:
     """Serve the rendered site directory through HTTP"""
-    print('Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config))
-
-    with ThreadingHTTPServerWithConfig(
-            ('127.0.0.1', config['SERVE_PORT']),
+    with EnhancedThreadingHTTPServer(
+            ('', config['SERVE_PORT']),
             SimpleEnhancedHTTPRequestHandler,
             directory=config['OUTPUT_DIR']
     ) as server:
+        msg = 'Serving "{OUTPUT_DIR}" on http://localhost:{SERVE_PORT}/'.format(**config)
+
+        if server.has_dualstack_ipv6:
+            msg += ' and http://[::1]:{SERVE_PORT}/'.format(**config)
+
+        logger.info(msg)
+
         try:
             server.serve_forever()
         except KeyboardInterrupt:
             pass
```

### Comparing `staticjinjaplus-1.0.0b4/staticjinjaplus/cli.py` & `staticjinjaplus-1.1.0/staticjinjaplus/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from argparse import ArgumentParser
 import staticjinjaplus
 
 
 def cli() -> None:
     arg_parser = ArgumentParser(
-        description='The staticjinjaplus CLI which should be your main and only entry point to staticjinjaplus.'
+        description='The staticjinjaplus CLI which should be your main and only way to interact with staticjinjaplus.'
     )
 
     command_arg_parser = arg_parser.add_subparsers(dest='command', required=True)
 
     build_arg_parser = command_arg_parser.add_parser('build', help='Build the site')
     build_arg_parser.add_argument(
         '-w', '--watch',
@@ -16,15 +16,15 @@
         action='store_true'
     )
 
     command_arg_parser.add_parser('clean', help='Delete and recreate the output directory')
 
     command_arg_parser.add_parser('publish', help='Build and publish the site (using `rsync` through SSH)')
 
-    command_arg_parser.add_parser('serve', help='Serve the rendered site directory through HTTP')
+    command_arg_parser.add_parser('serve', help='Serve the output directory through HTTP')
 
     args = arg_parser.parse_args()
 
     config = staticjinjaplus.load_config()
 
     if args.command == 'build':
         staticjinjaplus.build(config, args.watch)
```

### Comparing `staticjinjaplus-1.0.0b4/staticjinjaplus/http.py` & `staticjinjaplus-1.1.0/staticjinjaplus/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 from __future__ import annotations
 from http.server import ThreadingHTTPServer, SimpleHTTPRequestHandler
+from typing import Optional
 from http import HTTPStatus
 from os import fstat, path
+import socket
 
 
-class ThreadingHTTPServerWithConfig(ThreadingHTTPServer):
-    """Same as ThreadingHTTPServer but the directory to be served may be passed to its constructor"""
+class EnhancedThreadingHTTPServer(ThreadingHTTPServer):
+    """Same as ThreadingHTTPServer but the directory to be served may be passed to its constructor. It also tries to
+    listen to both IPv4 and IPv6 loopback addresses"""
     allow_reuse_address = True
     daemon_threads = True
+    has_dualstack_ipv6: bool
     directory: str
     RequestHandlerClass: SimpleEnhancedHTTPRequestHandler
 
     def __init__(self, *args, directory: str, **kvargs):
+        self.has_dualstack_ipv6 = socket.has_dualstack_ipv6()
+        self.address_family = socket.AF_INET6 if self.has_dualstack_ipv6 else socket.AF_INET
+        self.directory = directory
+
         super().__init__(*args, **kvargs)
 
-        self.directory = directory
+    def server_bind(self) -> None:
+        if self.has_dualstack_ipv6:
+            self.socket.setsockopt(socket.IPPROTO_IPV6, socket.IPV6_V6ONLY, 0)
+
+        super().server_bind()
 
     def finish_request(self, request, client_address) -> None:
         self.RequestHandlerClass(request, client_address, self, directory=self.directory)
 
 
 class SimpleEnhancedHTTPRequestHandler(SimpleHTTPRequestHandler):
     """A simple HTTP server handler which is meant to serve the output directory, with some enhancements (emulates URL
     rewrite for HTML files without .html extension; emulates custom 404 error page"""
     protocol_version = 'HTTP/1.1'
-    server: ThreadingHTTPServerWithConfig
+    server: EnhancedThreadingHTTPServer
 
     def __init__(self, *args, **kvargs):
         try:
             super().__init__(*args, **kvargs)
         except (ConnectionAbortedError, BrokenPipeError):
             pass
 
-    def translate_path(self, p) -> str:
+    def translate_path(self, p: str) -> str:
         p = super().translate_path(p)
 
         if not p.endswith(('\\', '/')):
             _, extension = path.splitext(p)
 
             if not extension:
                 p += '.html'
 
         return p
 
-    def send_error(self, code, message=None, explain=None) -> None:
-        if self.command != 'HEAD' and code == HTTPStatus.NOT_FOUND:
+    def send_error(self, code: int, message: Optional[str] = None, explain: Optional[str] = None) -> None:
+        status = HTTPStatus(code)
+
+        if self.command != 'HEAD' and (status.is_client_error or status.is_server_error):
             try:
-                f = open(path.join(self.directory, '404.html'), 'rb')
+                f = open(path.join(self.directory, f'{status.value}.html'), 'rb')
             except OSError:
                 return super().send_error(code, message=message, explain=explain)
 
             fs = fstat(f.fileno())
 
-            self.log_error("code %d, message %s", code, message)
             self.send_response(code, message)
             self.send_header('Connection', 'close')
 
             self.send_header('Content-Type', self.error_content_type)
             self.send_header('Content-Length', str(fs[6]))
             self.end_headers()
```

### Comparing `staticjinjaplus-1.0.0b4/staticjinjaplus/jinja_helpers.py` & `staticjinjaplus-1.1.0/staticjinjaplus/jinja_helpers.py`

 * *Files identical despite different names*

### Comparing `staticjinjaplus-1.0.0b4/staticjinjaplus/staticjinja_helpers.py` & `staticjinjaplus-1.1.0/staticjinjaplus/staticjinja_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 from htmlmin import minify as minify_xml
 from os import makedirs, path
 from staticjinja import Site
 from jinja2 import Template
+from jsmin import jsmin
 
 
 def minify_xml_template(site: Site, template: Template, **kwargs) -> None:
-    """Minify XML and HTML output from a rendered Jinja template"""
+    """Minify XML output (HTML/RSS/Atom) from a rendered Jinja template"""
     out = path.join(site.outpath, template.name)
 
     makedirs(path.dirname(out), exist_ok=True)
 
     with open(out, 'w', encoding=site.encoding) as f:
         f.write(
             minify_xml(
                 site.get_template(template.name).render(**kwargs),
                 remove_optional_attribute_quotes=False,
                 remove_empty_space=True,
                 remove_comments=True
             )
         )
+
+
+def minify_json_template(site: Site, template: Template, **kwargs) -> None:
+    """Minify JSON output from a rendered Jinja template"""
+    out = path.join(site.outpath, template.name)
+
+    makedirs(path.dirname(out), exist_ok=True)
+
+    with open(out, 'w', encoding=site.encoding) as f:
+        f.write(
+            jsmin(
+                site.get_template(template.name).render(**kwargs)
+            )
+        )
```

