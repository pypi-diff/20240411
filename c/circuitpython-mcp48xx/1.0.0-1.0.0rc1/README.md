# Comparing `tmp/circuitpython-mcp48xx-1.0.0.tar.gz` & `tmp/circuitpython-mcp48xx-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mcp48xx-1.0.0.tar", last modified: Thu Apr 11 08:20:14 2024, max compression
+gzip compressed data, was "circuitpython-mcp48xx-1.0.0rc1.tar", last modified: Thu Apr 11 07:22:40 2024, max compression
```

## Comparing `circuitpython-mcp48xx-1.0.0.tar` & `circuitpython-mcp48xx-1.0.0rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.827028 circuitpython-mcp48xx-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.819028 circuitpython-mcp48xx-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.819028 circuitpython-mcp48xx-1.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.823028 circuitpython-mcp48xx-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.823028 circuitpython-mcp48xx-1.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-11 08:20:14.827028 circuitpython-mcp48xx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.827028 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-11 08:20:14.000000 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 08:20:14.000000 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:20:14.000000 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:20:14.000000 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 08:20:14.000000 circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.823028 circuitpython-mcp48xx-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.823028 circuitpython-mcp48xx-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:20:14.827028 circuitpython-mcp48xx-1.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4801_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4802_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4811_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4812_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4821_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/examples/mcp4822_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17369 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/mcp48xx.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 08:20:12.000000 circuitpython-mcp48xx-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 08:20:02.000000 circuitpython-mcp48xx-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 08:20:14.827028 circuitpython-mcp48xx-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4801_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4802_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4811_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4812_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4821_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4822_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/mcp48xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/setup.cfg
```

### Comparing `circuitpython-mcp48xx-1.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/.github/adafruit_circuitpython_pr.md` & `circuitpython-mcp48xx-1.0.0rc1/.github/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/.gitignore` & `circuitpython-mcp48xx-1.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/.pre-commit-config.yaml` & `circuitpython-mcp48xx-1.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/.pylintrc` & `circuitpython-mcp48xx-1.0.0rc1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/CODE_OF_CONDUCT.md` & `circuitpython-mcp48xx-1.0.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/LICENSE` & `circuitpython-mcp48xx-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/LICENSES/CC-BY-4.0.txt` & `circuitpython-mcp48xx-1.0.0rc1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/LICENSES/MIT.txt` & `circuitpython-mcp48xx-1.0.0rc1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/LICENSES/Unlicense.txt` & `circuitpython-mcp48xx-1.0.0rc1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/PKG-INFO` & `circuitpython-mcp48xx-1.0.0rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mcp48xx
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters.
 Author-email: Steffen Kreutz <brushmate@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brushmate/CircuitPython_MCP48XX
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4801,mcp4811,mcp4821,mcp4802,mcp4812,mcp4822
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -53,14 +53,16 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
+.. note:: This library is not available on PyPI yet. Install documentation is included
+   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0/README.rst` & `circuitpython-mcp48xx-1.0.0rc1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
+.. note:: This library is not available on PyPI yet. Install documentation is included
+   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/PKG-INFO` & `circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mcp48xx
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters.
 Author-email: Steffen Kreutz <brushmate@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brushmate/CircuitPython_MCP48XX
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4801,mcp4811,mcp4821,mcp4802,mcp4812,mcp4822
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -53,14 +53,16 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
+.. note:: This library is not available on PyPI yet. Install documentation is included
+   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0/circuitpython_mcp48xx.egg-info/SOURCES.txt` & `circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/docs/_static/favicon.ico` & `circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/docs/conf.py` & `circuitpython-mcp48xx-1.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/docs/examples.rst` & `circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/docs/index.rst` & `circuitpython-mcp48xx-1.0.0rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4801_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4801_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4802_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4802_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4811_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4811_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4812_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4812_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4821_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4821_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/examples/mcp4822_simpletest.py` & `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4822_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0/mcp48xx.py` & `circuitpython-mcp48xx-1.0.0rc1/mcp48xx.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.0-rc.1"
 __repo__ = "https://github.com/brushmate/CircuitPython_MCP48XX.git"
 
 # imports
 
 from struct import pack_into
 from adafruit_bus_device import spi_device
```

### Comparing `circuitpython-mcp48xx-1.0.0/pyproject.toml` & `circuitpython-mcp48xx-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mcp48xx"
 description = "CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters."
-version = "1.0.0"
+version = "1.0.0-rc.1"
 readme = "README.rst"
 authors = [
     {name = "Steffen Kreutz", email = "brushmate@gmail.com"}
 ]
 urls = {Homepage = "https://github.com/brushmate/CircuitPython_MCP48XX"}
 keywords = [
     "adafruit",
```

