# Comparing `tmp/circuitpython-mcp48xx-1.0.0rc1.tar.gz` & `tmp/circuitpython-mcp48xx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-mcp48xx-1.0.0rc1.tar", last modified: Thu Apr 11 07:22:40 2024, max compression
+gzip compressed data, was "circuitpython-mcp48xx-1.0.1.tar", last modified: Thu Apr 11 19:04:18 2024, max compression
```

## Comparing `circuitpython-mcp48xx-1.0.0rc1.tar` & `circuitpython-mcp48xx-1.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.754281 circuitpython-mcp48xx-1.0.0rc1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 07:22:40.000000 circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4801_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4802_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4811_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4812_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4821_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/examples/mcp4822_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/mcp48xx.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-11 07:22:38.000000 circuitpython-mcp48xx-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 07:22:28.000000 circuitpython-mcp48xx-1.0.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:22:40.758281 circuitpython-mcp48xx-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.236270 circuitpython-mcp48xx-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.236270 circuitpython-mcp48xx-1.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.236270 circuitpython-mcp48xx-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.236270 circuitpython-mcp48xx-1.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-11 19:04:18.000000 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 19:04:18.000000 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:04:18.000000 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 19:04:18.000000 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 19:04:18.000000 circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4801_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4802_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4811_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4812_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4821_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/examples/mcp4822_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15764 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/mcp48xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-11 19:04:15.000000 circuitpython-mcp48xx-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 19:04:09.000000 circuitpython-mcp48xx-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:04:18.240270 circuitpython-mcp48xx-1.0.1/setup.cfg
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython-mcp48xx-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/.github/adafruit_circuitpython_pr.md` & `circuitpython-mcp48xx-1.0.1/.github/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/.gitignore` & `circuitpython-mcp48xx-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/.pre-commit-config.yaml` & `circuitpython-mcp48xx-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/.pylintrc` & `circuitpython-mcp48xx-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/CODE_OF_CONDUCT.md` & `circuitpython-mcp48xx-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/LICENSE` & `circuitpython-mcp48xx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/LICENSES/CC-BY-4.0.txt` & `circuitpython-mcp48xx-1.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/LICENSES/MIT.txt` & `circuitpython-mcp48xx-1.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/LICENSES/Unlicense.txt` & `circuitpython-mcp48xx-1.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/PKG-INFO` & `circuitpython-mcp48xx-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mcp48xx
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters.
 Author-email: Steffen Kreutz <brushmate@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brushmate/CircuitPython_MCP48XX
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4801,mcp4811,mcp4821,mcp4802,mcp4812,mcp4822
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -53,16 +53,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/README.rst` & `circuitpython-mcp48xx-1.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/PKG-INFO` & `circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-mcp48xx
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters.
 Author-email: Steffen Kreutz <brushmate@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brushmate/CircuitPython_MCP48XX
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4801,mcp4811,mcp4821,mcp4802,mcp4812,mcp4822
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -53,16 +53,14 @@
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_
 or individual libraries can be installed using
 `circup <https://github.com/adafruit/circup>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/circuitpython-mcp48xx/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/circuitpython_mcp48xx.egg-info/SOURCES.txt` & `circuitpython-mcp48xx-1.0.1/circuitpython_mcp48xx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/docs/_static/favicon.ico` & `circuitpython-mcp48xx-1.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/docs/conf.py` & `circuitpython-mcp48xx-1.0.1/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,16 @@
     "sphinx.ext.autodoc",
     "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
-# TODO: Please Read!
-# Uncomment the below if you use native CircuitPython modules such as
-# digitalio, micropython and busio. List the modules you use. Without it, the
-# autodoc module docs will fail to generate with a warning.
-# autodoc_mock_imports = ["digitalio", "busio"]
-
+autodoc_default_options = {"inherited-members": True}
+autodoc_mock_imports = ["digitalio", "busio"]
 autodoc_preserve_defaults = True
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "BusDevice": ("https://docs.circuitpython.org/projects/busdevice/en/latest/", None),
     "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/docs/examples.rst` & `circuitpython-mcp48xx-1.0.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/docs/index.rst` & `circuitpython-mcp48xx-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4801_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4801_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4802_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4802_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4811_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4811_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4812_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4812_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4821_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4821_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/examples/mcp4822_simpletest.py` & `circuitpython-mcp48xx-1.0.1/examples/mcp4822_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-mcp48xx-1.0.0rc1/mcp48xx.py` & `circuitpython-mcp48xx-1.0.1/mcp48xx.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
-__version__ = "1.0.0-rc.1"
+__version__ = "1.0.1"
 __repo__ = "https://github.com/brushmate/CircuitPython_MCP48XX.git"
 
 # imports
 
 from struct import pack_into
 from adafruit_bus_device import spi_device
 
@@ -62,14 +62,38 @@
 
         :param bytearray output: the data that will be sent to the DAC.
         """
         with self._spi_device as spi:
             spi.write(output)
 
 
+class _OutputVoltageLatch:
+    """An internal helper class for writing data to the DAC.
+
+    .. note::
+        All instances are created automatically and should not be used by the user.
+    """
+
+    def __init__(self, latch_input: Optional[DigitalInOut] = None) -> None:
+        self._latch_input = latch_input
+        if self._latch_input:
+            self._latch_input.switch_to_output(True)
+
+    def update(self) -> None:
+        """Updates the output voltage(s) of the DAC. On dual channel devices output voltages for
+        both channels are updated at the same time.
+
+        .. note::
+            This operation has no effect if :attr:`latch_input` is not configured.
+        """
+        if self._latch_input:
+            self._latch_input.value = False
+            self._latch_input.value = True
+
+
 class Channel:
     """An instance of a single channel for a multi-channel DAC.
 
     :param dac_instance: Instance of the channel object
     :param index: Index of the channel
 
     .. note::
@@ -177,15 +201,37 @@
         buf[0] |= self._index << 7
         buf[0] |= self._gain << 5
         buf[0] |= self._shutdown_control << 4
 
         return buf
 
 
-class MCP4801(Channel):
+class _DualChannelDevice:
+    def __init__(
+        self,
+        spi_bus: SPI,
+        chip_select: DigitalInOut,
+        resolution: Literal[8, 10, 12],
+    ) -> None:
+        dac = _DAC(spi_bus, chip_select)
+        self._channel_a = Channel(0, resolution, dac)
+        self._channel_b = Channel(1, resolution, dac)
+
+    @property
+    def channel_a(self) -> Channel:
+        """Channel A of the DAC. This is a read-only property."""
+        return self._channel_a
+
+    @property
+    def channel_b(self) -> Channel:
+        """Channel B of the DAC. This is a read-only property."""
+        return self._channel_b
+
+
+class MCP4801(Channel, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4801 SPI 8-bit DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4801 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4801 chip select line is connected\
         to.
 
 
@@ -219,29 +265,18 @@
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
         Channel.__init__(self, 0, 8, _DAC(spi_bus, chip_select))
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
+        _OutputVoltageLatch.__init__(self, latch_input)
 
-    def update(self) -> None:
-        """Updates the output voltage of the DAC.
 
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
-
-
-class MCP4811(Channel):
+class MCP4811(Channel, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4811 SPI 10-bit DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4811 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4811 chip select line is connected
         to.
 
 
@@ -275,29 +310,18 @@
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
         Channel.__init__(self, 0, 10, _DAC(spi_bus, chip_select))
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
-
-    def update(self) -> None:
-        """Updates the output voltage of the DAC.
+        _OutputVoltageLatch.__init__(self, latch_input)
 
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
 
-
-class MCP4821(Channel):
+class MCP4821(Channel, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4821 SPI 12-bit DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4821 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4821 chip select line is connected
         to.
 
 
@@ -331,29 +355,18 @@
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
         Channel.__init__(self, 0, 12, _DAC(spi_bus, chip_select))
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
-
-    def update(self) -> None:
-        """Updates the output voltage of the DAC.
-
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
+        _OutputVoltageLatch.__init__(self, latch_input)
 
 
-class MCP4802:
+class MCP4802(_DualChannelDevice, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4802 SPI 8-bit Dual DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4802 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4802 chip select line is connected
         to.
 
 
@@ -387,42 +400,19 @@
 
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
-        dac = _DAC(spi_bus, chip_select)
-        self._channel_a = Channel(0, 8, dac)
-        self._channel_b = Channel(1, 8, dac)
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
+        _DualChannelDevice.__init__(self, spi_bus, chip_select, 8)
+        _OutputVoltageLatch.__init__(self, latch_input)
 
-    @property
-    def channel_a(self) -> Channel:
-        """Get channel A of the DAC."""
-        return self._channel_a
-
-    @property
-    def channel_b(self) -> Channel:
-        """Get channel B of the DAC."""
-        return self._channel_b
 
-    def update(self) -> None:
-        """Updates the output voltages of both channel A and channel B of the DAC at the same time.
-
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
-
-
-class MCP4812:
+class MCP4812(_DualChannelDevice, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4812 SPI 10-bit Dual DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4812 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4812 chip select line is connected
         to.
 
 
@@ -454,42 +444,19 @@
 
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
-        dac = _DAC(spi_bus, chip_select)
-        self._channel_a = Channel(0, 8, dac)
-        self._channel_b = Channel(1, 8, dac)
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
+        _DualChannelDevice.__init__(self, spi_bus, chip_select, 8)
+        _OutputVoltageLatch.__init__(self, latch_input)
 
-    @property
-    def channel_a(self) -> Channel:
-        """Get channel A of the DAC."""
-        return self._channel_a
 
-    @property
-    def channel_b(self) -> Channel:
-        """Get channel B of the DAC."""
-        return self._channel_b
-
-    def update(self) -> None:
-        """Updates the output voltages of both channel A and channel B of the DAC at the same time.
-
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
-
-
-class MCP4822:
+class MCP4822(_DualChannelDevice, _OutputVoltageLatch):
     """Helper class for the Microchip MCP4822 SPI 12-bit Dual DAC.
 
     :param ~busio.SPI spi_bus: The SPI bus the MCP4822 is connected to.
     :param digitalio.DigitalInOut chip_select: Board pin the MCP4822 chip select line is connected
         to.
 
 
@@ -523,32 +490,9 @@
 
     def __init__(
         self,
         spi_bus: SPI,
         chip_select: DigitalInOut,
         latch_input: Optional[DigitalInOut] = None,
     ) -> None:
-        dac = _DAC(spi_bus, chip_select)
-        self._channel_a = Channel(0, 8, dac)
-        self._channel_b = Channel(1, 8, dac)
-        self._latch_input = latch_input
-        if self._latch_input:
-            self._latch_input.switch_to_output(True)
-
-    @property
-    def channel_a(self) -> Channel:
-        """Get channel A of the DAC."""
-        return self._channel_a
-
-    @property
-    def channel_b(self) -> Channel:
-        """Get channel B of the DAC."""
-        return self._channel_b
-
-    def update(self) -> None:
-        """Updates the output voltages of both channel A and channel B of the DAC at the same time.
-
-        This operation has no effect if :attr:`latch_input` is not configured.
-        """
-        if self._latch_input:
-            self._latch_input.value = False
-            self._latch_input.value = True
+        _DualChannelDevice.__init__(self, spi_bus, chip_select, 8)
+        _OutputVoltageLatch.__init__(self, latch_input)
```

### Comparing `circuitpython-mcp48xx-1.0.0rc1/pyproject.toml` & `circuitpython-mcp48xx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-mcp48xx"
 description = "CircuitPython library for the MCP4801, MCP4811, MCP4821, MCP4802, MCP4812, and MCP4822 digital to analog converters."
-version = "1.0.0-rc.1"
+version = "1.0.1"
 readme = "README.rst"
 authors = [
     {name = "Steffen Kreutz", email = "brushmate@gmail.com"}
 ]
 urls = {Homepage = "https://github.com/brushmate/CircuitPython_MCP48XX"}
 keywords = [
     "adafruit",
```

