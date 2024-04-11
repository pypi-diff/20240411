# Comparing `tmp/zalando-cli-bundle-21.5.0.tar.gz` & `tmp/zalando_cli_bundle-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalando-cli-bundle-21.5.0.tar", max compression
+gzip compressed data, was "zalando_cli_bundle-24.5.0.tar", max compression
```

## Comparing `zalando-cli-bundle-21.5.0.tar` & `zalando_cli_bundle-24.5.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1120 2021-05-04 12:37:38.384271 zalando-cli-bundle-21.5.0/pyproject.toml
--rw-r--r--   0        0        0       30 2019-12-17 10:01:54.167242 zalando-cli-bundle-21.5.0/zalando_cli_bundle/__main__.py
--rw-r--r--   0        0        0      581 2020-01-21 16:02:17.988593 zalando-cli-bundle-21.5.0/zalando_cli_bundle/cli.py
--rw-r--r--   0        0        0     1014 2021-05-04 12:43:19.166683 zalando-cli-bundle-21.5.0/setup.py
--rw-r--r--   0        0        0     1165 2021-05-04 12:43:19.166993 zalando-cli-bundle-21.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1251 2024-04-10 11:54:28.000000 zalando_cli_bundle-24.5.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-04-10 08:25:25.000000 zalando_cli_bundle-24.5.0/zalando_cli_bundle/__main__.py
+-rw-r--r--   0        0        0      581 2024-04-10 08:25:25.000000 zalando_cli_bundle-24.5.0/zalando_cli_bundle/cli.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 zalando_cli_bundle-24.5.0/PKG-INFO
```

### Comparing `zalando-cli-bundle-21.5.0/pyproject.toml` & `zalando_cli_bundle-24.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [tool.poetry]
 name = "zalando-cli-bundle"
-version = "21.5.0"
+version = "24.5.0"
 description = "CLI bundle for Zalando developers"
 authors = ["Henning Jacobs <henning@zalando.de>"]
 classifiers = [
     "Framework :: Pytest",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
+repository = "https://github.bus.zalan.do/developer-productivity/zalando-cli-bundle"
 
 
 [tool.poetry.scripts]
 zalando-cli-bundle = 'zalando_cli_bundle:cli.main'
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 stups-cli-support = "^1.1.22"
-stups-piu = "^1.2.4"
-stups-senza = "^2.1.141"
 stups-zign = "^1.2"
-stups-pierone = "^1.1.47"
+stups-pierone = "^1.1.53"
 stups-kio = "^0.1.25"
 zalando-aws-cli = "^1.2.7"
-zalando-kubectl = "^1.19.6"
-click = "^7.0"
+zalando-kubectl = "^1"
+click = "^8"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.2.0"
 
-[tool.poetry.dev-dependencies]
-pre-commit = "^1.21.0"
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `zalando-cli-bundle-21.5.0/zalando_cli_bundle/cli.py` & `zalando_cli_bundle-24.5.0/zalando_cli_bundle/cli.py`

 * *Files identical despite different names*

### Comparing `zalando-cli-bundle-21.5.0/PKG-INFO` & `zalando_cli_bundle-24.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: zalando-cli-bundle
-Version: 21.5.0
+Version: 24.5.0
 Summary: CLI bundle for Zalando developers
+Home-page: https://github.bus.zalan.do/developer-productivity/zalando-cli-bundle
 Author: Henning Jacobs
 Author-email: henning@zalando.de
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: click (>=7.0,<8.0)
+Requires-Dist: click (>=8,<9)
 Requires-Dist: stups-cli-support (>=1.1.22,<2.0.0)
 Requires-Dist: stups-kio (>=0.1.25,<0.2.0)
-Requires-Dist: stups-pierone (>=1.1.47,<2.0.0)
-Requires-Dist: stups-piu (>=1.2.4,<2.0.0)
-Requires-Dist: stups-senza (>=2.1.141,<3.0.0)
+Requires-Dist: stups-pierone (>=1.1.53,<2.0.0)
 Requires-Dist: stups-zign (>=1.2,<2.0)
 Requires-Dist: zalando-aws-cli (>=1.2.7,<2.0.0)
-Requires-Dist: zalando-kubectl (>=1.19.6,<2.0.0)
+Requires-Dist: zalando-kubectl (>=1,<2)
+Project-URL: Repository, https://github.bus.zalan.do/developer-productivity/zalando-cli-bundle
```

