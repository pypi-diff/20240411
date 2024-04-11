# Comparing `tmp/batcave-43.1.1.tar.gz` & `tmp/batcave-43.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batcave-43.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "batcave-43.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `batcave-43.1.1.tar` & `batcave-43.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     3265 2024-03-19 00:29:12.499843 batcave-43.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     2171 2024-03-19 00:29:12.499843 batcave-43.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     4797 2024-03-19 00:29:12.499843 batcave-43.1.1/.gitignore
--rw-r--r--   0        0        0       23 2024-03-19 00:29:12.499843 batcave-43.1.1/.p4cfg
--rw-r--r--   0        0        0     5049 2024-03-19 00:29:12.499843 batcave-43.1.1/.p4ignore
--rw-r--r--   0        0        0      158 2024-03-19 00:29:12.499843 batcave-43.1.1/.pypirc
--rw-r--r--   0        0        0       39 2024-03-19 00:29:12.499843 batcave-43.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     4034 2024-03-19 00:29:12.499843 batcave-43.1.1/.vscode/.ropeproject/config.py
--rw-r--r--   0        0        0      592 2024-03-19 00:29:12.499843 batcave-43.1.1/.vscode/.ropeproject/objectdb
--rw-r--r--   0        0        0     5757 2024-03-19 00:29:12.499843 batcave-43.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      468 2024-03-19 00:29:12.499843 batcave-43.1.1/.vscode/tasks.json
--rw-r--r--   0        0        0    39603 2024-03-19 00:29:12.499843 batcave-43.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       86 2024-03-19 00:29:12.499843 batcave-43.1.1/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-03-19 00:29:12.499843 batcave-43.1.1/LICENSE
--rw-r--r--   0        0        0       93 2024-03-19 00:29:12.499843 batcave-43.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1517 2024-03-19 00:29:12.499843 batcave-43.1.1/README.md
--rw-r--r--   0        0        0     1834 2024-03-19 00:29:25.339791 batcave-43.1.1/batcave/__init__.py
--rw-r--r--   0        0        0     5485 2024-03-19 00:29:12.499843 batcave-43.1.1/batcave/automation.py
--rw-r--r--   0        0        0    14410 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/cloudmgr.py
--rw-r--r--   0        0        0    74576 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/cms.py
--rw-r--r--   0        0        0     8590 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/commander.py
--rw-r--r--   0        0        0     9592 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/configmgr.py
--rw-r--r--   0        0        0    27694 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/data.py
--rw-r--r--   0        0        0    31760 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/expander.py
--rw-r--r--   0        0        0    10672 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/fileutil.py
--rw-r--r--   0        0        0    10747 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/gui.py
--rw-r--r--   0        0        0    28944 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/iispy.py
--rw-r--r--   0        0        0    21680 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/k8s.py
--rw-r--r--   0        0        0    10608 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/lang.py
--rw-r--r--   0        0        0     3035 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/menu.py
--rw-r--r--   0        0        0     2378 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/netutil.py
--rw-r--r--   0        0        0     3842 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/platarch.py
--rw-r--r--   0        0        0        0 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/py.typed
--rw-r--r--   0        0        0    13106 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/qbpy.py
--rw-r--r--   0        0        0    28331 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/reporter.py
--rw-r--r--   0        0        0    52861 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/servermgr.py
--rw-r--r--   0        0        0    11200 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/serverpath.py
--rw-r--r--   0        0        0     7801 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/statemachine.py
--rw-r--r--   0        0        0    23562 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/sysutil.py
--rw-r--r--   0        0        0     5429 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/tcpy.py
--rw-r--r--   0        0        0     3342 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/time.py
--rw-r--r--   0        0        0     3340 2024-03-19 00:29:12.503843 batcave-43.1.1/batcave/version.py
--rwxr-xr-x   0        0        0     1560 2024-03-19 00:29:12.503843 batcave-43.1.1/cicd-support/cicd.sh
--rwxr-xr-x   0        0        0      441 2024-03-19 00:29:12.503843 batcave-43.1.1/cicd-support/unit-tests.ps1
--rw-r--r--   0        0        0      634 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/Makefile
--rw-r--r--   0        0        0     3747 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/batcave.rst
--rw-r--r--   0        0        0     9167 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/coding_standards.py
--rw-r--r--   0        0        0     2109 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/conf.py
--rw-r--r--   0        0        0      469 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/index.rst
--rw-r--r--   0        0        0      795 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/make.bat
--rw-r--r--   0        0        0       65 2024-03-19 00:29:12.503843 batcave-43.1.1/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-03-19 00:29:12.507843 batcave-43.1.1/docs/requirements.txt
--rw-r--r--   0        0        0     2838 2024-03-19 00:29:25.339791 batcave-43.1.1/pyproject.toml
--rw-r--r--   0        0        0       44 2024-03-19 00:29:12.507843 batcave-43.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2808 2024-03-19 00:29:12.507843 batcave-43.1.1/tests/test_fileutil.py
--rw-r--r--   0        0        0     1288 2024-03-19 00:29:12.507843 batcave-43.1.1/tests/test_lang.py
--rw-r--r--   0        0        0     2806 2024-03-19 00:29:12.507843 batcave-43.1.1/tests/test_statemachine.py
--rw-r--r--   0        0        0     3132 2024-03-19 00:29:12.507843 batcave-43.1.1/tests/test_sysutil.py
--rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 batcave-43.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3265 2024-04-11 17:43:10.080204 batcave-43.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2092 2024-04-11 17:43:10.080204 batcave-43.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     4797 2024-04-11 17:43:10.080204 batcave-43.2.0/.gitignore
+-rw-r--r--   0        0        0       23 2024-04-11 17:43:10.080204 batcave-43.2.0/.p4cfg
+-rw-r--r--   0        0        0     5049 2024-04-11 17:43:10.080204 batcave-43.2.0/.p4ignore
+-rw-r--r--   0        0        0      158 2024-04-11 17:43:10.080204 batcave-43.2.0/.pypirc
+-rw-r--r--   0        0        0       39 2024-04-11 17:43:10.080204 batcave-43.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0     4034 2024-04-11 17:43:10.080204 batcave-43.2.0/.vscode/.ropeproject/config.py
+-rw-r--r--   0        0        0      592 2024-04-11 17:43:10.080204 batcave-43.2.0/.vscode/.ropeproject/objectdb
+-rw-r--r--   0        0        0     5757 2024-04-11 17:43:10.080204 batcave-43.2.0/.vscode/launch.json
+-rw-r--r--   0        0        0      468 2024-04-11 17:43:10.080204 batcave-43.2.0/.vscode/tasks.json
+-rw-r--r--   0        0        0    39782 2024-04-11 17:43:10.080204 batcave-43.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       86 2024-04-11 17:43:10.080204 batcave-43.2.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-11 17:43:10.080204 batcave-43.2.0/LICENSE
+-rw-r--r--   0        0        0       93 2024-04-11 17:43:10.080204 batcave-43.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     1632 2024-04-11 17:43:10.080204 batcave-43.2.0/README.md
+-rw-r--r--   0        0        0     1834 2024-04-11 17:43:23.948198 batcave-43.2.0/batcave/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/automation.py
+-rw-r--r--   0        0        0    14410 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/cloudmgr.py
+-rw-r--r--   0        0        0    74565 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/cms.py
+-rw-r--r--   0        0        0     8590 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/commander.py
+-rw-r--r--   0        0        0     9592 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/configmgr.py
+-rw-r--r--   0        0        0    27694 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/data.py
+-rw-r--r--   0        0        0    31760 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/expander.py
+-rw-r--r--   0        0        0    10672 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/fileutil.py
+-rw-r--r--   0        0        0    10747 2024-04-11 17:43:10.080204 batcave-43.2.0/batcave/gui.py
+-rw-r--r--   0        0        0    28944 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/iispy.py
+-rw-r--r--   0        0        0    22563 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/k8s.py
+-rw-r--r--   0        0        0    10608 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/lang.py
+-rw-r--r--   0        0        0     3035 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/menu.py
+-rw-r--r--   0        0        0     2378 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/netutil.py
+-rw-r--r--   0        0        0     3842 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/platarch.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/py.typed
+-rw-r--r--   0        0        0    13106 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/qbpy.py
+-rw-r--r--   0        0        0    28331 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/reporter.py
+-rw-r--r--   0        0        0    52861 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/servermgr.py
+-rw-r--r--   0        0        0    11200 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/serverpath.py
+-rw-r--r--   0        0        0     7801 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/statemachine.py
+-rw-r--r--   0        0        0    23562 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/sysutil.py
+-rw-r--r--   0        0        0     5429 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/tcpy.py
+-rw-r--r--   0        0        0     3342 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/time.py
+-rw-r--r--   0        0        0     3340 2024-04-11 17:43:10.084204 batcave-43.2.0/batcave/version.py
+-rwxr-xr-x   0        0        0     1560 2024-04-11 17:43:10.084204 batcave-43.2.0/cicd-support/cicd.sh
+-rwxr-xr-x   0        0        0      441 2024-04-11 17:43:10.084204 batcave-43.2.0/cicd-support/unit-tests.ps1
+-rw-r--r--   0        0        0      634 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/Makefile
+-rw-r--r--   0        0        0     3747 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/batcave.rst
+-rw-r--r--   0        0        0     9167 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2109 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/conf.py
+-rw-r--r--   0        0        0      469 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/make.bat
+-rw-r--r--   0        0        0       65 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-11 17:43:10.084204 batcave-43.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2838 2024-04-11 17:43:23.948198 batcave-43.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2024-04-11 17:43:10.084204 batcave-43.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     2808 2024-04-11 17:43:10.084204 batcave-43.2.0/tests/test_fileutil.py
+-rw-r--r--   0        0        0     1288 2024-04-11 17:43:10.084204 batcave-43.2.0/tests/test_lang.py
+-rw-r--r--   0        0        0     2806 2024-04-11 17:43:10.084204 batcave-43.2.0/tests/test_statemachine.py
+-rw-r--r--   0        0        0     3132 2024-04-11 17:43:10.084204 batcave-43.2.0/tests/test_sysutil.py
+-rw-r--r--   0        0        0     2205 1970-01-01 00:00:00.000000 batcave-43.2.0/PKG-INFO
```

### Comparing `batcave-43.1.1/.github/workflows/build.yml` & `batcave-43.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/.github/workflows/publish.yml` & `batcave-43.2.0/.github/workflows/publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,53 +22,52 @@
 
 jobs:
   publish-test:
     runs-on: ubuntu-latest
     environment: Staging
     permissions:
       contents: write
+      id-token: write
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON_BUILD_VER }}
       - uses: actions/cache@v3
         with:
           path: ${{ env.VIRTUAL_ENV }}
           key: pip-${{ runner.os }}-${{ matrix.python-version }}
       - uses: actions/download-artifact@v4
         with:
           run-id: ${{ github.event.inputs.run_id }}
-          github-token: ${{ secrets.ARTIFACT_TOKEN_NEW }}
+          github-token: ${{ secrets.ARTIFACT_TOKEN }}
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository-url: https://test.pypi.org/legacy/
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
       - run: cicd-support/cicd.sh "${{ github.job }}"
 
   publish:
     needs: publish-test
     runs-on: ubuntu-latest
     environment: Production
     permissions:
       contents: write
+      id-token: write
     env:
       GH_TOKEN: ${{ github.token }}
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON_BUILD_VER }}
       - uses: actions/cache@v3
         with:
           path: ${{ env.VIRTUAL_ENV }}
           key: pip-${{ runner.os }}-${{ matrix.python-version }}
       - run: cicd-support/cicd.sh "${{ github.job }}"
       - uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
       - uses: actions/upload-artifact@v4
         with:
           name: ${{ env.ARTIFACTS_DIR }}
           path: ${{ env.ARTIFACTS_DIR }}
 
 # cSpell:ignore bumpver noreply venv pypa pypi
```

### Comparing `batcave-43.1.1/.gitignore` & `batcave-43.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/.p4ignore` & `batcave-43.2.0/.p4ignore`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/.vscode/.ropeproject/config.py` & `batcave-43.2.0/.vscode/.ropeproject/config.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/.vscode/.ropeproject/objectdb` & `batcave-43.2.0/.vscode/.ropeproject/objectdb`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/.vscode/launch.json` & `batcave-43.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/CHANGELOG.md` & `batcave-43.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
+### [43.2.0] - 2024-04-11
+
+- Added:
+  - Added patch support to objects in the k8s module. (GitHub #113)
+
+- Changed:
+  - Switch to OICD for publishing. (GitHub #111)
+
+## Release History
+
 ### [43.1.1] - 2024-03-18
 
 - Changed:
   - Fixed project URLs. (GitHub #110)
   - Fixed release number. (GitHub #110)
 
-## Release History
-
 ### [43.1.0] - 2024-03-18
 
 - Added:
   - Added argument switch to fileutil.prune. (GitHub #106)
 
 - Changed:
   - Allow fileutil.prune exts arg to be any iterable. (GitHub #107)
@@ -1471,8 +1479,8 @@
 ### [0.1] - 2017-01-12
 
 - Initial release.
 
 <!--- cSpell:ignore docstrings platarch cmds psutil servermgr pywin sqlscript verfiles cloudmgr qbpy pkgtype unittest recopytree pathlib pypiwin
       cSpell:ignore pythonval fileutil cmsclient civars chmodtree sysutl cmdspec webapp virtualwrapper configmgr buildname vsver hasapp useshell
       cSpell:ignore GNUC envcfg pipenv statemachine psexec getattr contextlib logname xmltodict ignorestderr USERPROFILE netutil assemblyinfo
-      cSpell:ignore setattr iispy virtualenv prdb syscmd splitlines dataclasses pylance removeprefix dotmap bumpver -->
+      cSpell:ignore setattr iispy virtualenv prdb syscmd splitlines dataclasses pylance removeprefix dotmap bumpver oicd -->
```

### Comparing `batcave-43.1.1/LICENSE` & `batcave-43.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/README.md` & `batcave-43.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Windows: flit install --deps all
     Linux: flit install -s --deps all
 
 To update the current development environment
 
     python -m pip install --upgrade pip
     pip install --upgrade --upgrade-strategy eager setuptools wheel
-    Windows: pip freeze | %{$_.split('==')[0]} | %{pip install --upgrade $_}
-    Linux: pip freeze | grep -v '^\-e' | cut -d = -f 1 | xargs -n1 pip install --upgrade
+    Windows: pip freeze | %{$_.split('==')[0]} | %{pip install --upgrade $_} && flit install --deps all
+    Linux: pip freeze | grep -v '^\-e' | cut -d = -f 1 | xargs -n1 pip install --upgrade && flit install -s --deps all
 
 ## Testing
 
 ### Static Analysis
 
 The static analysis test can be run with
 
@@ -42,17 +42,18 @@
 
     flit build
 
 ## Publishing a Release
 
 This is the procedure for releasing BatCave
 
-1. Validate all issues are "Ready for Release"
-1. Update CHANGELOG.md
-1. Run the publish workflow against the Production environment
-1. Validate GitHub release
-1. Validate PyPi
-1. Move issues to "Closed"
-1. Close Milestone
-1. Update source in Perforce
+1. Validate all issues are "Ready for Release".
+1. Update CHANGELOG.md.
+1. Run the publish workflow against the Production environment.
+1. Validate GitHub release.
+1. Validate PyPi.
+1. Move issues to "Closed".
+1. Close Milestone.
+1. Update source in Perforce.
+1. If this was a release branch, merge to master.
 
 <!--- cSpell:ignore virtualenv mkvirtualenv batcave stest mypy xmlrunner utest -->
```

### Comparing `batcave-43.1.1/batcave/__init__.py` & `batcave-43.2.0/batcave/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'BatCave'
 __summary__ = 'Python Programming Toolkit'
 __uri__ = 'https://github.com/tardis4500/batcave/'
 
-__version__ = '43.1.1'
+__version__ = '43.2.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `batcave-43.1.1/batcave/automation.py` & `batcave-43.2.0/batcave/automation.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/cloudmgr.py` & `batcave-43.2.0/batcave/cloudmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/cms.py` & `batcave-43.2.0/batcave/cms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1679,15 +1679,15 @@
     Raises
         CMSError.INVALID_TYPE: If the CMS type is not valid.
     """
     if ctype not in ClientType:
         raise CMSError(CMSError.INVALID_TYPE, ctype=ctype)
 
 
-def walk_git_tree(tree: GitTree, /, *, parent: Optional[GitTree] = None) -> Generator[Tuple, Tuple, None]:
+def walk_git_tree(tree: GitTree, /, *, parent: Optional[str] = '') -> Generator[Tuple, Tuple, None]:
     """Walk the git tree similar to os.walk().
 
     Attributes:
         tree: The git tree to walk.
         parent (optional, default=None): Use a different parent than the root of the tree.
 
     Yields:
@@ -1698,14 +1698,14 @@
     for entry in tree:
         if isinstance(entry, GitTree):
             tree_names.append(entry.name)
             trees.append(entry)
         else:
             blobs.append(entry.name)
 
-    new_parent: str = f'{parent}/{tree.name}' if parent else tree.name
+    new_parent = f'{parent}/{tree.name}' if parent else tree.name
     for subtree in trees:
         yield from walk_git_tree(subtree, parent=new_parent)
 
     yield new_parent, tree_names, blobs
 
 # cSpell:ignore checkin unedit fileutil labelsync hostless revertunchanged changelists winerror
```

### Comparing `batcave-43.1.1/batcave/commander.py` & `batcave-43.2.0/batcave/commander.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/configmgr.py` & `batcave-43.2.0/batcave/configmgr.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/data.py` & `batcave-43.2.0/batcave/data.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/expander.py` & `batcave-43.2.0/batcave/expander.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/fileutil.py` & `batcave-43.2.0/batcave/fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/gui.py` & `batcave-43.2.0/batcave/gui.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/iispy.py` & `batcave-43.2.0/batcave/iispy.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/k8s.py` & `batcave-43.2.0/batcave/k8s.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,32 @@
         config_args = {}
         if self.config:
             config_args['kubeconfig'] = self.config
         if self._context:
             config_args['context'] = self._context
         return kubectl(*args, **config_args, **kwargs)
 
+    def patch_item(self, item_class: Type[K8sObject], name: str, item_spec: K8sObject, /, namespace: str = 'default') -> K8sObject:
+        """Patch the named item.
+
+        Args:
+            item_class: The class of the item to patch.
+            name: The name of the item to patch.
+            item_spec: The new specification for the patched item.
+            namespace (optional, default='default'): The Kubernetes namespace from which to return the item.
+
+        Returns:
+            The patched item.
+        """
+        args: list[Any] = [name]
+        if item_class.NAMESPACED:
+            args.append(namespace)
+        args.append(item_spec.spec)
+        return item_class(self, self.find_method(item_class, 'patch')(*args))
+
 
 class ClusterObject:  # pylint: disable=too-few-public-methods
     """Class to create a universal abstract interface for a Kubernetes cluster object.
 
     Attributes:
         NAMESPACED: If True, the object is a cluster namespaced object.
     """
@@ -310,14 +328,16 @@
         self._object_ref = object_ref
 
     def __getattr__(self, attr: str) -> 'ClusterObject':
         if hasattr(self._object_ref, attr):
             return getattr(self._object_ref, attr)
         return getattr(self._object_ref.metadata, attr)
 
+    spec = property(lambda s: s._cluster_obj, doc='A read-only property which returns Kubernetes API spec for the object.')
+
 
 class Binding(ClusterObject):  # pylint: disable=too-few-public-methods
     """Class to create a universal abstract interface for a Kubernetes cron job."""
 
 
 class Configmap(ClusterObject):  # pylint: disable=too-few-public-methods
     """Class to create a universal abstract interface for a Kubernetes cron job."""
```

### Comparing `batcave-43.1.1/batcave/lang.py` & `batcave-43.2.0/batcave/lang.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/menu.py` & `batcave-43.2.0/batcave/menu.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/netutil.py` & `batcave-43.2.0/batcave/netutil.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/platarch.py` & `batcave-43.2.0/batcave/platarch.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/qbpy.py` & `batcave-43.2.0/batcave/qbpy.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/reporter.py` & `batcave-43.2.0/batcave/reporter.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/servermgr.py` & `batcave-43.2.0/batcave/servermgr.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/serverpath.py` & `batcave-43.2.0/batcave/serverpath.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/statemachine.py` & `batcave-43.2.0/batcave/statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/sysutil.py` & `batcave-43.2.0/batcave/sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/tcpy.py` & `batcave-43.2.0/batcave/tcpy.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/time.py` & `batcave-43.2.0/batcave/time.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/batcave/version.py` & `batcave-43.2.0/batcave/version.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/cicd-support/cicd.sh` & `batcave-43.2.0/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/docs/Makefile` & `batcave-43.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/docs/batcave.rst` & `batcave-43.2.0/docs/batcave.rst`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/docs/coding_standards.py` & `batcave-43.2.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/docs/conf.py` & `batcave-43.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/docs/make.bat` & `batcave-43.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/pyproject.toml` & `batcave-43.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "wmi.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v43.1.1"
+current_version = "v43.2.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip-ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `batcave-43.1.1/tests/test_fileutil.py` & `batcave-43.2.0/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/tests/test_lang.py` & `batcave-43.2.0/tests/test_lang.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/tests/test_statemachine.py` & `batcave-43.2.0/tests/test_statemachine.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/tests/test_sysutil.py` & `batcave-43.2.0/tests/test_sysutil.py`

 * *Files identical despite different names*

### Comparing `batcave-43.1.1/PKG-INFO` & `batcave-43.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batcave
-Version: 43.1.1
+Version: 43.2.0
 Summary: BatCave Utilities module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

