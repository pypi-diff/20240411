# Comparing `tmp/webdomains-1.0.0b2.tar.gz` & `tmp/webdomains-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdomains-1.0.0b2.tar", last modified: Wed Jul 14 14:08:29 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `webdomains-1.0.0b2.tar` & `webdomains-1.0.0b3.tar`

### file list

```diff
@@ -1,28 +1,15 @@
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      307 2020-12-04 15:37:35.000000 webdomains-1.0.0b2/.editorconfig
--rw-r--r--   0 jerome    (1000) jerome    (1000)      205 2021-07-14 14:05:01.000000 webdomains-1.0.0b2/.gitignore
--rw-r--r--   0 jerome    (1000) jerome    (1000)      643 2021-07-14 14:05:01.000000 webdomains-1.0.0b2/CHANGELOG.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)    35149 2017-09-30 07:16:26.000000 webdomains-1.0.0b2/LICENSE
--rw-r--r--   0 jerome    (1000) jerome    (1000)       75 2020-12-07 08:09:34.000000 webdomains-1.0.0b2/MANIFEST.in
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1287 2021-07-14 14:05:01.000000 webdomains-1.0.0b2/Makefile
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3302 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1842 2021-07-14 13:53:59.000000 webdomains-1.0.0b2/README.md
--rw-r--r--   0 jerome    (1000) jerome    (1000)      510 2021-07-14 13:51:33.000000 webdomains-1.0.0b2/pyproject.toml
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1262 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/setup.cfg
--rw-r--r--   0 jerome    (1000) jerome    (1000)       38 2021-07-14 13:50:13.000000 webdomains-1.0.0b2/setup.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-07-14 14:08:29.120081 webdomains-1.0.0b2/tests/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     2390 2021-01-19 15:07:58.000000 webdomains-1.0.0b2/tests/test_core.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/webdomains/
--rw-r--r--   0 jerome    (1000) jerome    (1000)      213 2021-07-14 13:57:33.000000 webdomains-1.0.0b2/webdomains/__init__.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)     9793 2021-01-06 18:14:25.000000 webdomains-1.0.0b2/webdomains/cli.py
--rw-r--r--   0 jerome    (1000) jerome    (1000)    12791 2021-01-06 18:15:17.000000 webdomains-1.0.0b2/webdomains/core.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/webdomains/templates/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     1453 2021-03-19 17:55:34.000000 webdomains-1.0.0b2/webdomains/templates/server.conf
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3966 2020-12-07 08:58:05.000000 webdomains-1.0.0b2/webdomains/utils.py
-drwxr-xr-x   0 jerome    (1000) jerome    (1000)        0 2021-07-14 14:08:29.124081 webdomains-1.0.0b2/webdomains.egg-info/
--rw-r--r--   0 jerome    (1000) jerome    (1000)     3302 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/PKG-INFO
--rw-r--r--   0 jerome    (1000) jerome    (1000)      448 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/SOURCES.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)        1 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/dependency_links.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       51 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/entry_points.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)      105 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/requires.txt
--rw-r--r--   0 jerome    (1000) jerome    (1000)       11 2021-07-14 14:08:29.000000 webdomains-1.0.0b2/webdomains.egg-info/top_level.txt
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/.editorconfig
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/CHANGELOG.md
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/Makefile
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/tests/test_core.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/webdomains/__init__.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/webdomains/cli.py
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/webdomains/core.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/webdomains/utils.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/webdomains/templates/server.conf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/README.md
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 webdomains-1.0.0b3/PKG-INFO
```

### Comparing `webdomains-1.0.0b2/CHANGELOG.md` & `webdomains-1.0.0b3/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## 1.0.0-beta3 - 2024-04-11
+### Added
+- Set and retrieve proxied server to which root location of a domain will be
+  mapped (Closes #3)
+
 ## 1.0.0-beta2 - 2021-07-14
 ### Changed
 - Remove `root` and `index` directives from the default template
 
 ## 1.0.0-beta1 - 2021-01-19
 ### Added
 - Base class to define different kind of domains in `webdomains.core`
```

### Comparing `webdomains-1.0.0b2/LICENSE` & `webdomains-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `webdomains-1.0.0b2/Makefile` & `webdomains-1.0.0b3/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 	@$(PYTHON) -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
 
 clean: ## remove all build, test, coverage and Python artifacts
 	rm -rf build dist .eggs *.egg-info
 	find webdomains/ \
 	  \( -name '*.py[co]' -o -name '__pycache__' \) -exec rm -rf {} +
 
-tests: ## run tests quickly with the current Python
+test: ## run tests quickly with the current Python
 	$(PYTHON) -m pytest --cov --cov-report=term:skip-covered
 
 coverage: tests ## check code coverage quickly with the current Python
 	$(PYTHON) -m coverage html
 	@echo open htmlcov/index.html
 
 lint: ## check the Python code syntax and style
-	$(PYTHON) -m flake8 webdomains tests
+	@$(PYTHON) -m ruff check
+	@$(PYTHON) -m ruff format --check --quiet
 
-format: ## fix the Python code syntax and imports order
-	$(PYTHON) -m isort webdomains tests
-	$(PYTHON) -m black webdomains tests
+format: ## format and fix the Python code syntax
+	$(PYTHON) -m ruff check --fix
+	$(PYTHON) -m ruff format
 
 release: dist ## package and upload a release
-	twine upload dist/*
+	$(PYTHON) -m twine upload dist/*
 
 dist: clean ## builds source and wheel package
-	$(PYTHON) setup.py sdist
-	$(PYTHON) setup.py bdist_wheel
-	ls -l dist
+	$(PYTHON) -m build
```

### Comparing `webdomains-1.0.0b2/PKG-INFO` & `webdomains-1.0.0b3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,87 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: webdomains
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: Manage your Web domains served by NGINX
-Home-page: UNKNOWN
-Author: Cliss XXI
-Author-email: contact@cliss21.com
-License: GPLv3
-Project-URL: Bug Tracker, https://forge.cliss21.org/cliss21/webdomains/issues
-Project-URL: Source Code, https://forge.cliss21.org/cliss21/webdomains
-Description: # webdomains
-        
-        Manage your Web domains served by NGINX.
-        
-        ## Installation
-        ### Requirements
-        
-        On a Debian-based host, you will need an already configured and running
-        [NGINX server](https://nginx.net/). You may also install the following
-        packages to satisfy the Python dependencies:
-        - `python3-click`
-        - `python3-jinja2`
-        
-        To generate the SSL/TLS certificates for the domains, you will also have to
-        install and configure [dehydrated](https://dehydrated.io/). It is recommended
-        to use a recent version - i.e. from `buster-backports`. To serve the ACME
-        challenge, the default NGINX configuration of a domain is looking for
-        `/etc/nginx/snippets/acme-challenge.conf` - which can just contain:
-        
-        ```nginx
-        location /.well-known/acme-challenge {
-            default_type "text/plain";
-            alias        /var/lib/dehydrated/acme-challenges;
-        }
-        ```
-        
-        ### Configuration
-        
-        You can provide your own `server.conf` template which is used to generate the
-        NGINX configuration of a new domain. *webdomains* will look for a file with this
-        name in `/etc/webdomains/templates` at first. If it does not exist, the
-        [default template](webdomains/templates/server.conf) is used.
-        
-        ## Development
-        
-        To set up a development environment, all you need to have to install is a
-        Python 3 interpreter, Git and Make. Then, run the following:
-        
-        ```bash
-        git clone https://forge.cliss21.org/cliss21/webdomains.git
-        cd webdomains/
-        
-        # create and active a virtual environment
-        python3 -m venv venv/
-        source venv/bin/activate
-        
-        # install the package with test requirements
-        pip install -e .[test]
-        ```
-        
-        You can now run the following commands:
-        - `make lint`: check the code syntax
-        - `make tests`: run the tests
-        - `make coverage`: report the code coverage
-        
-        ## License
-        
-        *webdomains* is mainly developed by [Cliss XXI](https://www.cliss21.com) and
-        licensed under the [GPLv3+](LICENSE). Any contribution is welcome!
-        
-Platform: UNKNOWN
+Project-URL: Repository, https://framagit.org/cliss21/webdomains
+Project-URL: Issues, https://framagit.org/cliss21/webdomains/-/issues
+Author-email: Cliss XXI <contact@cliss21.com>
+License-Expression: GPL-3.0-or-later
+License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: <4,>=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Requires-Python: >=3.8
+Requires-Dist: click>=7.0
+Requires-Dist: jinja2>=2.10
+Provides-Extra: dev
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: ruff~=0.3.5; extra == 'dev'
 Description-Content-Type: text/markdown
-Provides-Extra: test
+
+# webdomains
+
+Manage your Web domains served by NGINX.
+
+## Installation
+### Requirements
+
+On a Debian-based host, you will need an already configured and running
+[NGINX server](https://nginx.net/). You may also install the following
+packages to satisfy the Python dependencies:
+- `python3-click`
+- `python3-jinja2`
+
+To generate the SSL/TLS certificates for the domains, you will also have to
+install and configure [dehydrated](https://dehydrated.io/). It is recommended
+to use a recent version - i.e. from `buster-backports`. To serve the ACME
+challenge, the default NGINX configuration of a domain is looking for
+`/etc/nginx/snippets/acme-challenge.conf` - which can just contain:
+
+```nginx
+location /.well-known/acme-challenge {
+    default_type "text/plain";
+    alias        /var/lib/dehydrated/acme-challenges;
+}
+```
+
+### Configuration
+
+You can provide your own `server.conf` template which is used to generate the
+NGINX configuration of a new domain. *webdomains* will look for a file with this
+name in `/etc/webdomains/templates` at first. If it does not exist, the
+[default template](webdomains/templates/server.conf) is used.
+
+## Development
+
+To set up a development environment, all you need to have to install is a
+Python 3 interpreter, Git and Make. Then, run the following:
+
+```bash
+git clone https://framagit.org/cliss21/webdomains.git
+cd webdomains/
+
+# create and active a virtual environment
+python3 -m venv venv/
+source venv/bin/activate
+
+# install the package with test requirements
+pip install --editable ".[dev]"
+```
+
+You can now run the following commands:
+- `make lint`: check the code syntax
+- `make test`: run the tests
+- `make coverage`: report the code coverage
+
+## License
+
+*webdomains* is mainly developed by [Cliss XXI](https://www.cliss21.com) and
+licensed under the [GPLv3+](LICENSE). Any contribution is welcome!
```

### Comparing `webdomains-1.0.0b2/README.md` & `webdomains-1.0.0b3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,27 +33,27 @@
 
 ## Development
 
 To set up a development environment, all you need to have to install is a
 Python 3 interpreter, Git and Make. Then, run the following:
 
 ```bash
-git clone https://forge.cliss21.org/cliss21/webdomains.git
+git clone https://framagit.org/cliss21/webdomains.git
 cd webdomains/
 
 # create and active a virtual environment
 python3 -m venv venv/
 source venv/bin/activate
 
 # install the package with test requirements
-pip install -e .[test]
+pip install --editable ".[dev]"
 ```
 
 You can now run the following commands:
 - `make lint`: check the code syntax
-- `make tests`: run the tests
+- `make test`: run the tests
 - `make coverage`: report the code coverage
 
 ## License
 
 *webdomains* is mainly developed by [Cliss XXI](https://www.cliss21.com) and
 licensed under the [GPLv3+](LICENSE). Any contribution is welcome!
```

### Comparing `webdomains-1.0.0b2/tests/test_core.py` & `webdomains-1.0.0b3/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     BaseDomain,
     ConfigurationError,
     get_nginx_directive_value,
 )
 
 
 class DummyDomain(BaseDomain):
-    conf_dir = Path('/etc/dummy/available')
-    enabled_conf_dir = Path('/etc/dummy/enabled')
+    conf_dir = Path("/etc/dummy/available")
+    enabled_conf_dir = Path("/etc/dummy/enabled")
 
     @property
     def conf_path(self):
         return self.conf_dir / self.name
 
     @property
     def enabled_conf_path(self):
@@ -27,59 +27,59 @@
         conf = """
 server {
   server_name domain.tld www.domain.tld;
 }
 """
 
         assert (
-            get_nginx_directive_value('server_name', conf)
-            == 'domain.tld www.domain.tld'
+            get_nginx_directive_value("server_name", conf)
+            == "domain.tld www.domain.tld"
         )
 
     def test_get_nginx_directive_value_error(self):
         with pytest.raises(ConfigurationError) as excinfo:
-            get_nginx_directive_value('test', "some configuration")
+            get_nginx_directive_value("test", "some configuration")
         assert str(excinfo.value) == "`test` directive is not defined."
 
 
 class TestBaseDomainConf:
     @pytest.fixture(autouse=True)
     def setup_domain(self):
-        self.domain = DummyDomain('test.example.org')
+        self.domain = DummyDomain("test.example.org")
 
     def test_get_property_from_conf(self):
         conf = """
 ## protocol=http
 ## empty=
 ## spaces = value
  ## indent=value
 """  # noqa: W291
 
-        assert self.domain.get_property_from_conf(conf, 'protocol') == 'http'
-        assert self.domain.get_property_from_conf(conf, 'empty') == ''
+        assert self.domain.get_property_from_conf(conf, "protocol") == "http"
+        assert self.domain.get_property_from_conf(conf, "empty") == ""
 
         with pytest.raises(ConfigurationError):
-            self.domain.get_property_from_conf(conf, 'spaces')
+            self.domain.get_property_from_conf(conf, "spaces")
         with pytest.raises(ConfigurationError):
-            self.domain.get_property_from_conf(conf, 'indent')
+            self.domain.get_property_from_conf(conf, "indent")
 
     def test_get_property_from_conf_pattern(self):
         conf = """
 ## protocol=http
 ## invalid=http1
 ## empty=
 """
 
         assert (
-            self.domain.get_property_from_conf(conf, 'protocol', r'[a-z]+')
-            == 'http'
+            self.domain.get_property_from_conf(conf, "protocol", r"[a-z]+")
+            == "http"
         )
 
         with pytest.raises(ConfigurationError):
-            self.domain.get_property_from_conf(conf, 'invalid', r'[a-z]+')
+            self.domain.get_property_from_conf(conf, "invalid", r"[a-z]+")
         with pytest.raises(ConfigurationError):
-            self.domain.get_property_from_conf(conf, 'empty', r'.+')
+            self.domain.get_property_from_conf(conf, "empty", r".+")
 
     def test_get_property_from_conf_not_defined(self):
         with pytest.raises(ConfigurationError) as excinfo:
-            self.domain.get_property_from_conf("some configuration", 'test')
+            self.domain.get_property_from_conf("some configuration", "test")
         assert excinfo.value.message == "`test` variable is not defined."
```

### Comparing `webdomains-1.0.0b2/webdomains/cli.py` & `webdomains-1.0.0b3/webdomains/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import re
 import subprocess
 from functools import update_wrapper
 from shutil import rmtree
 
 import click
 from click.exceptions import Exit
 
@@ -27,17 +28,17 @@
 
 
 def mkdir(path: str, **kwargs):
     """Create the directory `path` or change its mode if it exists."""
     if not os.path.isdir(path):
         logger.info("Creating directory '%s'…", path)
         os.mkdir(path, **kwargs)
-    elif 'mode' in kwargs:
+    elif "mode" in kwargs:
         logger.info("Changing mode of '%s'…", path)
-        os.chmod(path, kwargs['mode'])
+        os.chmod(path, kwargs["mode"])
 
 
 def reload_nginx_or_die(callback=None):
     """
     Try to reload the NGINX server and die if an error occurs - after calling
     the `callback` method.
     """
@@ -53,38 +54,38 @@
 # COMMANDS
 # -----------------------------------------------------------------------------
 
 
 def domain_argument(f):
     """Add a `domain` argument which will be passed as `WebDomain` object."""
 
-    @click.argument('domain', metavar='DOMAIN_NAME')
+    @click.argument("domain", metavar="DOMAIN_NAME")
     def new_func(domain, *args, **kwargs):
         if not isinstance(domain, WebDomain):
             domain = WebDomain(domain)
         return f(domain, *args, **kwargs)
 
     return update_wrapper(new_func, f)
 
 
 @click.group()
 @click.option(
-    '-q', '--quiet', is_flag=True, help="Suppress non-error messages."
+    "-q", "--quiet", is_flag=True, help="Suppress non-error messages."
 )
-@click.version_option(version=__version__, message='%(version)s')
+@click.version_option(version=__version__, message="%(version)s")
 def cli(quiet: bool = False):
     """Manage Web domains served by this host."""
     if quiet:
         logger.setLevel(logging.ERROR)
 
 
-@cli.command(name='list')
+@cli.command(name="list")
 @click.option(
-    '-e/-d',
-    '--enabled/--disabled',
+    "-e/-d",
+    "--enabled/--disabled",
     default=None,
     help="List enabled or disabled domains only.",
 )
 def list_webdomains(enabled: bool = None):
     """List existing domains."""
     if enabled is True:
 
@@ -105,20 +106,20 @@
                 click.echo(domain)
             else:
                 click.echo("{} (disabled)".format(domain))
 
     with os.scandir(WebDomain.nginx_sites_available_dir) as it:
         for entry in it:
             if entry.is_file() and not (
-                entry.name.startswith('.') or entry.name == 'default'
+                entry.name.startswith(".") or entry.name == "default"
             ):
                 _handle_domain(WebDomain(entry.name))
 
 
-@cli.command(name='info', short_help="Show domain informations.")
+@cli.command(name="info", short_help="Show domain informations.")
 @domain_argument
 def info_webdomain(domain: WebDomain):
     """Show informations about the domain DOMAIN_NAME."""
     if not domain.exists:
         die("Domain does not exist.")
 
     try:
@@ -132,62 +133,97 @@
     click.echo("protocol: {}".format(domain.protocol.value))
 
     if domain.has_https:
         click.echo("certs: {}".format("yes" if domain.has_certs else "no"))
 
     click.echo("template_name: {}".format(domain.template_name))
 
+    if domain.root_conf_path.is_file():
+        root_proxy_match = re.search(
+            "^location / { proxy_pass ([^;]+); }$",
+            domain.root_conf_path.read_text(),
+        )
+
+        if root_proxy_match is not None:
+            click.echo("proxy: {}".format(root_proxy_match.group(1)))
 
-@cli.command(name='add', short_help="Add a domain.")
+
+@cli.command(name="add", short_help="Add a domain.")
 @click.option(
-    '-n',
-    '--alternative-name',
+    "-n",
+    "--alternative-name",
     multiple=True,
     metavar="DOMAIN_NAME",
     help="Alternative server name (can be provided multiple times).",
 )
 @click.option(
-    '-h', '--http-only', is_flag=True, help="Do not serve over HTTPS."
+    "-h",
+    "--http-only",
+    is_flag=True,
+    help="Do not serve over HTTPS.",
+)
+@click.option(
+    "-s",
+    "--https-only",
+    is_flag=True,
+    help="Redirect HTTP to HTTPS.",
 )
 @click.option(
-    '-s', '--https-only', is_flag=True, help="Redirect HTTP to HTTPS."
+    "-e",
+    "--enable",
+    is_flag=True,
+    help="Enable the created domain.",
 )
 @click.option(
-    '-e', '--enable', is_flag=True, help="Enable the created domain."
+    "-f",
+    "--force",
+    is_flag=True,
+    help="Overwrite existing configuration.",
 )
 @click.option(
-    '-f', '--force', is_flag=True, help="Overwrite existing configuration."
+    "-t",
+    "--template-name",
+    metavar="NAME",
+    help="The template name to use.",
 )
 @click.option(
-    '-t', '--template-name', metavar="NAME", help="The template name to use."
+    "-p",
+    "--proxy",
+    metavar="URL",
+    help="Proxied server to which root location will be mapped.",
 )
 @domain_argument
 @click.pass_context
 def add_webdomain(
     ctx: click.Context,
     domain: WebDomain,
     alternative_name: tuple = None,
     http_only: bool = False,
     https_only: bool = False,
     enable: bool = False,
     force: bool = False,
     template_name: str = None,
+    proxy: str = None,
 ):
     """
     Create the NGINX configuration and directories for the domain DOMAIN_NAME.
 
     DOMAIN_NAME will be the principal server name used for all other commands.
     It is possible to provide alternative server names for the domain with
     `--alternative-name`.
 
     By default, the domain will be served over HTTP and HTTPS. It is possible
     to restrict the protocol with `--http-only` or `--https-only`. Note that if
     the SSL/TLS certificates of the domain does not exist yet, the domain will
     be served over HTTP only at first. They will be automatically generated
     using dehydrated when the domain is enabled.
+
+    It is possible to define the URL of a proxied server to which root location
+    will be mapped with `--proxy`. In that case, a `root.conf` file will be
+    automatically created with the relevant configuration.
     """
     if alternative_name:
         domain.alternative_names = tuple(alternative_name)
 
     if http_only and https_only:
         raise click.UsageError(
             "--http-only and --https-only are not compatible.", ctx
@@ -210,24 +246,30 @@
         domain.generate_conf(template_name)
     except OSError as e:
         die(str(e))
 
     mkdir(domain.local_conf_dir, mode=0o755)
     mkdir(domain.log_dir, mode=0o750)
 
+    if proxy:
+        logger.info("Generating configuration '%s'…", domain.root_conf_path)
+        domain.root_conf_path.write_text(
+            "location / { proxy_pass %s; }" % (proxy)
+        )
+
     if enable:
         ctx.invoke(enable_webdomain, domain=domain)
 
 
-@cli.command(name='remove', short_help="Remove a domain.")
+@cli.command(name="remove", short_help="Remove a domain.")
 @click.option(
-    '-c', '--clean', is_flag=True, help="Delete all associated directories."
+    "-c", "--clean", is_flag=True, help="Delete all associated directories."
 )
 @click.option(
-    '-f', '--force', is_flag=True, help="Remove even if the domain is enabled."
+    "-f", "--force", is_flag=True, help="Remove even if the domain is enabled."
 )
 @domain_argument
 @click.pass_context
 def remove_webdomain(
     ctx: click.Context,
     domain: WebDomain,
     clean: bool = False,
@@ -256,15 +298,15 @@
     if clean:
         for path in (domain.local_conf_dir, domain.log_dir):
             if os.path.isdir(path):
                 logger.info("Deleting directory « %s »…", path)
                 rmtree(path)
 
 
-@cli.command(name='enable', short_help="Enable a domain.")
+@cli.command(name="enable", short_help="Enable a domain.")
 @domain_argument
 def enable_webdomain(domain: WebDomain):
     """
     Enable the NGINX configuration of the domain DOMAIN_NAME and generate as
     needed its SSL/TLS certificates.
     """
     if not domain.exists:
@@ -303,15 +345,15 @@
 
         logger.info("Regenerating NGINX configuration…")
         domain.generate_conf()
 
         reload_nginx_or_die(domain.disable)
 
 
-@cli.command(name='disable', short_help="Disable a domain.")
+@cli.command(name="disable", short_help="Disable a domain.")
 @domain_argument
 def disable_webdomain(domain: WebDomain):
     """Disable the NGINX configuration of the domain DOMAIN_NAME."""
     if not domain.exists:
         die("Domain does not exist.")
 
     if not domain.is_enabled:
@@ -324,9 +366,9 @@
     try:
         logger.info("Reloading NGINX server…")
         reload_nginx()
     except subprocess.SubprocessError as e:
         logger.warning(str(e))
 
 
-if __name__ == '__main__':  # pragma: no cover
+if __name__ == "__main__":  # pragma: no cover
     cli()
```

### Comparing `webdomains-1.0.0b2/webdomains/core.py` & `webdomains-1.0.0b3/webdomains/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 
 # NGINX HELPERS
 # -----------------------------------------------------------------------------
 
 
 def get_nginx_directive_value(name: str, conf: str) -> str:
     """Retrieve a directive value from the given NGINX configuration."""
-    match = re.search(r'^[ \t]*%s[ \t]+([^;]+);' % name, conf, re.MULTILINE)
+    match = re.search(r"^[ \t]*%s[ \t]+([^;]+);" % name, conf, re.MULTILINE)
     if match is None:
         raise ConfigurationError("`%s` directive is not defined." % name)
     return match.group(1)
 
 
 def reload_nginx():
     """Reload NGINX server if the configuration is valid."""
     try:
         subprocess.run(
-            ['nginx', '-t', '-q'], stderr=subprocess.PIPE, check=True
+            ["nginx", "-t", "-q"], stderr=subprocess.PIPE, check=True
         )
     except subprocess.CalledProcessError as e:
         raise subprocess.SubprocessError(
             "The NGINX configuration is invalid:\n{}".format(
                 e.stderr.decode().strip()
             )
         )
     else:
-        proc = subprocess.run(['systemctl', '-q', 'reload', 'nginx.service'])
+        proc = subprocess.run(["systemctl", "-q", "reload", "nginx.service"])
         if proc.returncode:
             raise subprocess.SubprocessError(
                 "The unit 'nginx.service' fails to reload."
             )
 
 
 # BASE CLASS AND MIXINS
@@ -62,20 +62,20 @@
 
     Subclasses must define at least the `conf_path` and `enabled_conf_path`
     properties.
     """
 
     #: Ordered list of directories in which templates are looked for.
     templates_dir = [
-        '/etc/webdomains/templates',
-        os.path.join(os.path.dirname(__file__), 'templates'),
+        "/etc/webdomains/templates",
+        os.path.join(os.path.dirname(__file__), "templates"),
     ]
 
     #: The template name to use for the configuration.
-    template_name = 'server.conf'
+    template_name = "server.conf"
 
     def __init__(self, name: str):
         self.name = name
 
     def __str__(self):
         return self.name
 
@@ -139,42 +139,40 @@
         self.update_properties_from_conf(self.conf_path.read_text())
 
     # OVERRIDABLE METHODS
 
     def get_template_environment(self, **kwargs) -> Environment:
         """Return the Jinja environment to use for template rendering."""
         options = {
-            'loader': FileSystemLoader(self.templates_dir),
-            'trim_blocks': True,
-            'keep_trailing_newline': True,
+            "loader": FileSystemLoader(self.templates_dir),
+            "trim_blocks": True,
+            "keep_trailing_newline": True,
         }
         options.update(kwargs)
         return Environment(**options)
 
     def get_conf_context_data(self, **kwargs) -> dict:
         """Return the template context for the domain's configuration."""
-        kwargs.setdefault('domain', self)
+        kwargs.setdefault("domain", self)
         return kwargs
 
     def update_properties_from_conf(self, conf: str):
         """
         Retrieve and update the domain properties with values found in the
         given configuration.
         """
         self.template_name = self.get_property_from_conf(
-            conf, 'template_name', r'.+'
+            conf, "template_name", r".+"
         )
 
     def get_property_from_conf(
-        self, conf: str, name: str, pattern=r'.*'
+        self, conf: str, name: str, pattern=r".*"
     ) -> str:
         """Retrieve a property's value from the given configuration."""
-        match = re.search(
-            r'^## %s=(%s)$' % (name, pattern), conf, re.MULTILINE
-        )
+        match = re.search(r"^## %s=(%s)$" % (name, pattern), conf, re.MULTILINE)
         if match is None:
             raise ConfigurationError(
                 "`%s` variable is not defined." % name, self.conf_path
             )
         return match.group(1)
 
 
@@ -182,15 +180,15 @@
     """
     Provide a way to define alternative server names of a domain.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self._alternative_names = tuple()
+        self._alternative_names = ()
 
     # PROPERTIES
 
     @property
     def alternative_names(self) -> tuple:
         """Return the alternative server names of the domain."""
         return self._alternative_names
@@ -204,43 +202,43 @@
         self._alternative_names = value
 
     # DYNAMIC PROPERTIES
 
     @property
     def server_name(self) -> str:
         """The server name(s) of the domain."""
-        return ' '.join([self.name] + list(self.alternative_names))
+        return " ".join([self.name] + list(self.alternative_names))
 
 
 class DehydratedDomainMixin(AlternativeServerNamesMixin):
     """
     Provide a way to manage the domain's SSL/TLS certificates using dehydrated.
     """
 
-    dehydrated_certs_dir = Path('/var/lib/dehydrated/certs')
-    dehydrated_domains_path = Path('/etc/dehydrated/domains.txt')
+    dehydrated_certs_dir = Path("/var/lib/dehydrated/certs")
+    dehydrated_domains_path = Path("/etc/dehydrated/domains.txt")
 
     # DYNAMIC PROPERTIES
 
     @cached_property
     def certs_dir(self) -> Path:
         """The directory path to SSL/TLS certificates of the domain."""
         return self.dehydrated_certs_dir / self.name
 
     @property
     def has_certs(self) -> bool:
         """Whether SSL/TLS certificates of the domain exist."""
-        return (self.certs_dir / 'privkey.pem').exists()
+        return (self.certs_dir / "privkey.pem").exists()
 
     # PUBLIC METHODS
 
     def generate_certs(self, stdout=None, stderr=subprocess.PIPE):
         """Generate the domain's SSL/TLS certificates using dehydrated."""
         subprocess.run(
-            ['dehydrated', '--cron', '--domain', self.server_name],
+            ["dehydrated", "--cron", "--domain", self.server_name],
             check=True,
             stdout=stdout,
             stderr=stderr,
         )
 
         self._update_dehydrated_domains()
 
@@ -266,34 +264,34 @@
 
     # INTERNAL METHODS
 
     def _update_dehydrated_domains(self, remove=False):
         """Update the dehydrated domains' list for the domain."""
         if not self.dehydrated_domains_path.is_file():
             if not remove:
-                with open(self.dehydrated_domains_path, 'x') as f:
-                    f.write('%s\n' % self.server_name)
+                with open(self.dehydrated_domains_path, "x") as f:
+                    f.write("%s\n" % self.server_name)
             return
 
-        domain_name_re = re.compile(r'(?:^|.+ ){}(?:$| .+)'.format(self.name))
+        domain_name_re = re.compile(r"(?:^|.+ ){}(?:$| .+)".format(self.name))
 
-        with open(self.dehydrated_domains_path, 'r') as f:
+        with open(self.dehydrated_domains_path, "r") as f:
             lines = f.readlines()
-        with open(self.dehydrated_domains_path, 'w') as f:
+        with open(self.dehydrated_domains_path, "w") as f:
             is_domain_added = False
 
             for line in lines:
                 if not domain_name_re.match(line.strip()):
                     f.write(line)
                 elif not remove and not is_domain_added:
-                    f.write('%s\n' % self.server_name)
+                    f.write("%s\n" % self.server_name)
                     is_domain_added = True
 
             if not remove and not is_domain_added:
-                f.write('%s\n' % self.server_name)
+                f.write("%s\n" % self.server_name)
 
 
 # WEB DOMAIN CLASSES
 # -----------------------------------------------------------------------------
 
 
 class NGINXDomain(BaseDomain):
@@ -301,22 +299,22 @@
     A Web domain intended to be served by NGINX.
 
     It is defined by one or more server names, and the protocol on which it
     must be available.
     """
 
     class Protocol(Enum):
-        BOTH = 'both'
-        HTTP = 'http'
-        HTTPS = 'https'
-
-    nginx_etc_dir = Path('/etc/nginx')
-    nginx_log_dir = Path('/var/log/nginx')
-    nginx_sites_available_dir = nginx_etc_dir / 'sites-available'
-    nginx_sites_enabled_dir = nginx_etc_dir / 'sites-enabled'
+        BOTH = "both"
+        HTTP = "http"
+        HTTPS = "https"
+
+    nginx_etc_dir = Path("/etc/nginx")
+    nginx_log_dir = Path("/var/log/nginx")
+    nginx_sites_available_dir = nginx_etc_dir / "sites-available"
+    nginx_sites_enabled_dir = nginx_etc_dir / "sites-enabled"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._protocol = WebDomain.Protocol.BOTH
 
     # PROPERTIES
@@ -344,53 +342,58 @@
     @cached_property
     def enabled_conf_path(self) -> Path:
         """The path to the enabled NGINX configuration of the domain."""
         return self.nginx_sites_enabled_dir / self.name
 
     @cached_property
     def local_conf_dir(self) -> Path:
-        """The directory path to local NGINX configuration of the domain."""
-        return self.nginx_sites_available_dir / '{}.d'.format(self.name)
+        """The directory path to the local NGINX configuration of the domain."""
+        return self.nginx_sites_available_dir / "{}.d".format(self.name)
+
+    @cached_property
+    def root_conf_path(self) -> Path:
+        """The path to the NGINX configuration file for the domain's root."""
+        return self.local_conf_dir / "root.conf"
 
     @cached_property
     def log_dir(self) -> Path:
         """The directory path to NGINX logs of the domain."""
         return self.nginx_log_dir / self.name
 
     @property
     def has_https(self) -> bool:
         """Whether the domain is available in HTTPS."""
         return self.protocol != WebDomain.Protocol.HTTP
 
     # OVERRIDABLE METHODS
 
     def get_conf_context_data(self, **kwargs) -> dict:
-        if 'protocol' not in kwargs:
-            kwargs['protocol'] = (
+        if "protocol" not in kwargs:
+            kwargs["protocol"] = (
                 WebDomain.Protocol.HTTP.value
                 if not self.has_certs
                 else self.protocol.value
             )
         return super().get_conf_context_data(**kwargs)
 
     def update_properties_from_conf(self, conf: str):
         super().update_properties_from_conf(conf)
 
-        server_name = get_nginx_directive_value('server_name', conf).split(' ')
+        server_name = get_nginx_directive_value("server_name", conf).split(" ")
         if self.name not in server_name:
             raise ConfigurationError(
                 "'{}' is not in `server_name {}` directive.".format(
                     self.name, server_name
                 ),
                 self.conf_path,
             )
         server_name.remove(self.name)
         self.alternative_names = tuple(server_name)
 
-        protocol = self.get_property_from_conf(conf, 'protocol', r'[A-Z]+')
+        protocol = self.get_property_from_conf(conf, "protocol", r"[A-Z]+")
         try:
             self.protocol = WebDomain.Protocol[protocol]
         except KeyError:
             raise ConfigurationError(
                 "'{}' is not a valid protocol.".format(protocol),
                 self.conf_path,
             )
```

### Comparing `webdomains-1.0.0b2/webdomains/templates/server.conf` & `webdomains-1.0.0b3/webdomains/templates/server.conf`

 * *Files identical despite different names*

### Comparing `webdomains-1.0.0b2/webdomains/utils.py` & `webdomains-1.0.0b3/webdomains/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         raise TypeError(
             "Cannot use cached_property instance without calling "
             "__set_name__() on it."
         )
 
     def __init__(self, func):
         self.real_func = func
-        self.__doc__ = getattr(func, '__doc__')
+        self.__doc__ = getattr(func, "__doc__")
 
     def __set_name__(self, owner, name):
         if self.name is None:
             self.name = name
             self.func = self.real_func
         elif name != self.name:
             raise TypeError(
@@ -82,59 +82,57 @@
         return self.pwrite
 
     def close(self):
         """Close the write file descriptor of the pipe."""
         os.close(self.pwrite)
 
     def run(self):
-        for line in iter(self.preader.readline, ''):
-            self.logger.log(self.level, line.strip('\n'))
+        for line in iter(self.preader.readline, ""):
+            self.logger.log(self.level, line.strip("\n"))
         self.preader.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         self.close()
 
 
 class ClickHandler(logging.Handler):
     """Handler which sends logging output to `click.echo`."""
 
     def emit(self, record):
         try:
-            click.echo(
-                self.format(record), err=record.levelno >= logging.ERROR
-            )
-        except Exception:
+            click.echo(self.format(record), err=record.levelno >= logging.ERROR)
+        except Exception:  # noqa: BLE001
             self.handleError(record)
 
 
 class ColorFormatter(logging.Formatter):
     """Formatter which extends `LogRecord` attributes with 'levelprefix'.
 
     The 'levelprefix' attribute is almost a colored version of 'levelname', see
     `ColorFormatter.STYLES` for the styles attributes.
     """
 
     STYLES = {
-        'ERROR': dict(text='Error! ', fg='red'),
-        'EXCEPTION': dict(text='Error! ', fg='red'),
-        'CRITICAL': dict(text='Error! ', fg='red'),
-        'INFO': dict(text=' + ', fg='blue'),
-        'WARNING': dict(text='Warning: ', fg='yellow'),
+        "ERROR": {"text": "Error! ", "fg": "red"},
+        "EXCEPTION": {"text": "Error! ", "fg": "red"},
+        "CRITICAL": {"text": "Error! ", "fg": "red"},
+        "INFO": {"text": " + ", "fg": "blue"},
+        "WARNING": {"text": "Warning: ", "fg": "yellow"},
     }
 
     def formatMessage(self, record):
         style_kwargs = self.STYLES.get(record.levelname, {})
-        style_kwargs.setdefault('text', '')
+        style_kwargs.setdefault("text", "")
         record.levelprefix = click.style(**style_kwargs)
         return super().formatMessage(record)
 
 
 def setup_click_logger(logger, fmt=None):
     """Setup a logger to be used with `click`."""
-    formatter = ColorFormatter(fmt or '%(levelprefix)s%(message)s')
+    formatter = ColorFormatter(fmt or "%(levelprefix)s%(message)s")
     handler = ClickHandler()
     handler.setFormatter(formatter)
     logger.addHandler(handler)
     return logger
```

