# Comparing `tmp/vjer-31.0.0.tar.gz` & `tmp/vjer-32.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-31.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-32.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-31.0.0.tar` & `vjer-32.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     6148 2024-03-22 00:46:11.656643 vjer-31.0.0/.DS_Store
--rw-r--r--   0        0        0     1948 2024-03-22 00:46:11.656643 vjer-31.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2018 2024-03-22 00:46:11.660644 vjer-31.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     4744 2024-03-22 00:46:11.660644 vjer-31.0.0/.gitignore
--rw-r--r--   0        0        0     4987 2024-03-22 00:46:11.660644 vjer-31.0.0/.p4ignore
--rw-r--r--   0        0        0      158 2024-03-22 00:46:11.660644 vjer-31.0.0/.pypirc
--rw-r--r--   0        0        0       42 2024-03-22 00:46:11.660644 vjer-31.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    39668 2024-03-22 00:46:11.660644 vjer-31.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-03-22 00:46:11.660644 vjer-31.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-03-22 00:46:11.660644 vjer-31.0.0/LICENSE
--rw-r--r--   0        0        0       90 2024-03-22 00:46:11.660644 vjer-31.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1499 2024-03-22 00:46:11.660644 vjer-31.0.0/README.md
--rwxr-xr-x   0        0        0     1741 2024-03-22 00:46:11.660644 vjer-31.0.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-03-22 00:46:11.660644 vjer-31.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2113 2024-03-22 00:46:40.708438 vjer-31.0.0/pyproject.toml
--rw-r--r--   0        0        0      211 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-03-22 00:46:40.708438 vjer-31.0.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/__main__.py
--rw-r--r--   0        0        0     5108 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/freeze.py
--rw-r--r--   0        0        0     1287 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/py.typed
--rw-r--r--   0        0        0     2874 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    25995 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2445 2024-03-22 00:46:11.660644 vjer-31.0.0/vjer/vjer.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 vjer-31.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-04-11 01:07:45.534438 vjer-32.0.0/.DS_Store
+-rw-r--r--   0        0        0     1788 2024-04-11 01:07:45.534438 vjer-32.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-11 01:07:45.534438 vjer-32.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     4755 2024-04-11 01:07:45.534438 vjer-32.0.0/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-11 01:07:45.534438 vjer-32.0.0/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-11 01:07:45.534438 vjer-32.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    39819 2024-04-11 01:07:45.534438 vjer-32.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-11 01:07:45.534438 vjer-32.0.0/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-11 01:07:45.534438 vjer-32.0.0/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-11 01:07:45.534438 vjer-32.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1499 2024-04-11 01:07:45.534438 vjer-32.0.0/README.md
+-rwxr-xr-x   0        0        0      878 2024-04-11 01:07:45.538438 vjer-32.0.0/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-11 01:07:45.538438 vjer-32.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     2180 2024-04-11 01:08:31.398089 vjer-32.0.0/pyproject.toml
+-rw-r--r--   0        0        0      476 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-11 01:08:31.398089 vjer-32.0.0/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/__main__.py
+-rw-r--r--   0        0        0     5208 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/freeze.py
+-rw-r--r--   0        0        0     1501 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/py.typed
+-rw-r--r--   0        0        0     3519 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    25133 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/utils.py
+-rwxr-xr-x   0        0        0     2445 2024-04-11 01:07:45.538438 vjer-32.0.0/vjer/vjer.py
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-32.0.0/setup.py
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-32.0.0/PKG-INFO
```

### Comparing `vjer-31.0.0/.DS_Store` & `vjer-32.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/.github/workflows/build.yml` & `vjer-32.0.0/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
   pull_request:
   workflow_dispatch:
 concurrency:
   group: ${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 env:
-  ARTIFACTS_DIR: dist
+  ARTIFACTS_DIR: artifacts
   PYTHON_BUILD_VER: "3.11"
   UNIT_TEST_DIR: unit_test_results
   VIRTUAL_ENV: venv
 
 jobs:
-  static-analysis:
+  test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
           - "3.11"
           - "3.12"
     steps:
@@ -31,15 +31,15 @@
         with:
           path: ${{ env.VIRTUAL_ENV }}
           key: pip-${{ runner.os }}-${{ matrix.python-version }}
       - run: cicd-support/cicd.sh "${{ github.job }}"
 
   build:
     needs:
-      - static-analysis
+      - test
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON_BUILD_VER }}
           cache: "pip"
@@ -58,19 +58,15 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ env.PYTHON_BUILD_VER }}
       - uses: actions/download-artifact@v4
-      - uses: actions/cache@v3
-        with:
-          path: ${{ env.VIRTUAL_ENV }}
-          key: pip-${{ runner.os }}-${{ env.PYTHON_BUILD_VER }}
-      - run: cicd-support/cicd.sh "${{ github.job }}"
+      - run: pip install ${{ env.ARTIFACTS_DIR }}/*.tar.gz
 
   show-run-id:
     runs-on: ubuntu-latest
     steps:
       - run: echo ${{ github.run_id }}
 
 # cSpell:ignore vjer venv
```

### Comparing `vjer-31.0.0/.github/workflows/publish.yml` & `vjer-32.0.0/.github/workflows/publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 name: Vjer Publish
+
 on:
   workflow_dispatch:
     inputs:
       run_id:
-        description: The run to publish
+        description: The run to release
         required: true
         type: number
 concurrency:
   group: ${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 env:
-  ARTIFACTS_DIR: dist
+  ARTIFACTS_DIR: artifacts
   GIT_AUTHOR_NAME: "${{ github.triggering_actor }}"
   GIT_AUTHOR_EMAIL: "${{ github.triggering_actor }}@users.noreply.github.com"
   PYTHON_BUILD_VER: "3.11"
   VIRTUAL_ENV: venv
 
 jobs:
-  publish-test:
+  pre_release:
     runs-on: ubuntu-latest
     environment: Staging
     permissions:
       contents: write
       id-token: write
     steps:
       - uses: actions/checkout@v4
@@ -36,18 +37,19 @@
       - uses: actions/download-artifact@v4
         with:
           run-id: ${{ github.event.inputs.run_id }}
           github-token: ${{ secrets.ARTIFACT_TOKEN }}
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository-url: https://test.pypi.org/legacy/
+          packages-dir: ${{ env.ARTIFACTS_DIR }}
       - run: cicd-support/cicd.sh "${{ github.job }}"
 
-  publish:
-    needs: publish-test
+  release:
+    needs: pre_release
     runs-on: ubuntu-latest
     environment: Production
     permissions:
       contents: write
       id-token: write
     env:
       GH_TOKEN: ${{ github.token }}
@@ -58,13 +60,15 @@
           python-version: ${{ env.PYTHON_BUILD_VER }}
       - uses: actions/cache@v3
         with:
           path: ${{ env.VIRTUAL_ENV }}
           key: pip-${{ runner.os }}-${{ matrix.python-version }}
       - run: cicd-support/cicd.sh "${{ github.job }}"
       - uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          packages-dir: ${{ env.ARTIFACTS_DIR }}
       - uses: actions/upload-artifact@v4
         with:
           name: ${{ env.ARTIFACTS_DIR }}
           path: ${{ env.ARTIFACTS_DIR }}
 
 # cSpell:ignore bumpver vjer noreply venv pypa pypi
```

### Comparing `vjer-31.0.0/.gitignore` & `vjer-32.0.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -234,10 +234,11 @@
 # Windows shortcuts
 *.lnk
 
 # End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
 
 # Custom rules (everything added below won't be overriden by 'Generate .gitignore File' if you use 'Update' option)
 
-.p4cfg
 .git/
+.p4cfg
+artifacts/
 unit_test_results/
```

### Comparing `vjer-31.0.0/.p4ignore` & `vjer-32.0.0/.p4ignore`

 * *Files 2% similar despite different names*

```diff
@@ -234,10 +234,11 @@
 # Windows shortcuts
 *.lnk
 
 # End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
 
 # Custom rules (everything added below won't be overriden by 'Generate .gitignore File' if you use 'Update' option)
 
-.p4cfg
 .git/
+.p4cfg
+artifacts/
 unit_test_results/
```

### Comparing `vjer-31.0.0/CHANGELOG.md` & `vjer-32.0.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
+### [32.0.0] - 2024-04-10
+
+- Added
+  - Added flit and bumpver support. (GitHub #2)
+
+- Removed
+  - Removed implicit release steps. (GitHub #6)
+
+## Release History
+
 ### [31.0.0] - 2024-03-21
 
 - Added
   - Added bumpver version service. (GitHub #3)
   - Added python test types: flake8, pylint, and mypy. (GitHub #3)
   - Added __main__.py to enable module execution. (GitHub #4)
 
@@ -18,16 +28,14 @@
   - Improved version code. (GitHub #4)
   - Report any OS. (GitHub #4)
   - Changed project.product to project.name. (GitHub #4)
 
 - Removed
   - Removed semver version service. (GitHub #4)
 
-## Release History
-
 ### [30.0.0] - 2024-03-20
 
 - Changed
   - Converted to installable module. (GitHub #1)
 
 - Removed
   - Removed support for all action types except Docker and Helm.
```

### Comparing `vjer-31.0.0/LICENSE` & `vjer-32.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/README.md` & `vjer-32.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 ## Publishing a Release
 
 This is the procedure for releasing Vjer
 
 1. Validate all issues are "Ready for Release"
 1. Update CHANGELOG.md
-1. Run the publish workflow against the Production environment
+1. Run the release workflow against the Production environment
 1. Validate GitHub release
 1. Validate PyPi
 1. Move issues to "Closed" and label res::complete
 1. Close Milestone
 1. Update source in Perforce
 
 <!--- cSpell:ignore virtualenv mkvirtualenv vjer stest mypy xmlrunner utest -->
```

### Comparing `vjer-31.0.0/docs/Makefile` & `vjer-32.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/docs/coding_standards.py` & `vjer-32.0.0/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/docs/conf.py` & `vjer-32.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/docs/make.bat` & `vjer-32.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/pyproject.toml` & `vjer-32.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Natural Language :: English",
 ]
 
 dependencies = [
-    "BatCave~=43.0",
+    "BatCave",
     "bumpver",
     "junitparser",
     "flake8",
     "flake8-annotations",
     "flake8-pyproject",
     "mypy",
     "pylint",
@@ -72,19 +72,23 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "dotmap.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
+module = "flit.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v31.0.0"
+current_version = "v32.0.0"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-31.0.0/vjer/__init__.py` & `vjer-32.0.0/vjer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
            '__author__', '__email__',
            '__license__', '__copyright__')
 
 __title__ = 'Vjer'
 __summary__ = 'CI/CD Toolkit'
 __uri__ = 'https://github.com/tardis4500/vjer/'
 
-__version__ = '31.0.0'
+__version__ = '32.0.0'
 __build_name__ = '{var:build_name}'
 __build_date__ = '{var:build_date}'
 
 __author__ = 'Jeffery G. Smith'
 __email__ = 'web@pobox.com'
 
 __license__ = 'MIT'
```

### Comparing `vjer-31.0.0/vjer/build.py` & `vjer-32.0.0/vjer/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,18 @@
                 self.log_message(line['stream'].strip())
         if error:
             raise error
         if push_image:
             self.log_message('Pushing image to registry', True)
             self.registry_client.get_image(self.image_tag).push()
 
+    def build_flit(self) -> None:
+        """Run a Python flit build."""
+        self.flit_build()
+
     def build_helm(self) -> None:
         """Build method for Helm charts."""
         helm('dependency', 'build', self.helm_chart_root)
         helm('package', self.helm_chart_root)
         self.copy_artifact(self.helm_package.name)
```

### Comparing `vjer-31.0.0/vjer/deploy.py` & `vjer-32.0.0/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/vjer/freeze.py` & `vjer-32.0.0/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/vjer/pre_release.py` & `vjer-32.0.0/vjer/pre_release.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,38 @@
-"""This module provides pre-release actions."""
+"""This module provides pre_release actions."""
 
 # Import standard modules
 from typing import cast
 
 # Import project modules
 from .release import ReleaseStep
 from .utils import VjerAction, VjerStep, helm
 
 
 class PreReleaseStep(ReleaseStep):
     """Provide pre_release support.
 
     Attributes:
-        is_pre_release: Specifies to the ReleaseStep parent class that this is a pre-release action.
+        is_pre_release: Specifies to the ReleaseStep parent class that this is a pre_release action.
     """
     is_pre_release = True
 
     def __init__(self):
-        """Sets the project version to a pre-release value."""
+        """Sets the project version to a pre_release value."""
         super().__init__()
         self.project.version = f'{self.project.version}-{self.pre_release_num}'
 
+    def release_bumpver(self) -> None:
+        """Perform a bumpver on release."""
+        if not self.step_info.args:
+            self.step_info.args = {'tag-num': True}
+        super().release_bumpver()
+
     def release_helm(self) -> None:
-        """Pre-release a Helm chart."""
+        """Pre_release a Helm chart."""
         if self.helm_repo.type == 'oci':
             self.update_version_files()
             try:
                 helm('package', self.helm_chart_root)
                 self.copy_artifact(self.helm_package.name)
             finally:
                 self.update_version_files(reset=True)
@@ -35,8 +41,8 @@
         super().release_helm()
 
 
 def pre_release() -> None:
     """This is the main entry point."""
     VjerAction('release', cast(VjerStep, PreReleaseStep)).execute()
 
-# cSpell:ignore batcave vjer
+# cSpell:ignore batcave vjer bumpver
```

### Comparing `vjer-31.0.0/vjer/release.py` & `vjer-32.0.0/vjer/release.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,40 @@
 """This module provides release actions."""
 
 # Import standard modules
 from typing import cast
 
 # Import third-party modules
 from batcave.cloudmgr import gcloud
+from batcave.sysutil import SysCmdRunner
 
 # Import project modules
 from .utils import helm, VjerAction, VjerStep
 
+bumpver_update = SysCmdRunner('bumpver', 'update', syscmd_args={'ignore_stderr': True}).run
+
 
 class ReleaseStep(VjerStep):
     """Provide release support.
 
     Attributes:
-        is_pre_release: Specifies that this is not a pre-release action.
+        is_pre_release: Specifies that this is not a pre_release action.
     """
     is_pre_release = False
 
+    def _execute(self) -> None:
+        if self.is_pre_release and self.step_info.release_only:
+            self.log_message('Skipping on pre_release')
+            return
+        super()._execute()
+
+    def release_bumpver(self) -> None:
+        """Perform a bumpver on release."""
+        bumpver_update(**(self.step_info.args if self.step_info.args else {'tag': 'final', 'tag-commit': True}))
+
     def release_docker(self) -> None:
         """Perform a release of a Docker image by tagging."""
         self._docker_init()
         if (registry := self.container_registry).type not in ('gcp', 'jfrog'):
             (image := self.registry_client.get_image(self.image_tag)).pull()
         default_tags = [self.version_tag.lower()]
         if not self.is_pre_release:
@@ -31,40 +44,42 @@
             match registry.type:
                 case 'gcp':
                     gcloud('container', 'images', 'add-tag', self.image_tag, tag, syscmd_args={'ignore_stderr': True})
                 case  _:
                     image.tag(tag)
                     image.push()
 
+    def release_flit_build(self) -> None:
+        """Run a Python flit build."""
+        self.flit_build()
+
+    def release_github(self) -> None:
+        """Create a GitHub release."""
+        SysCmdRunner('gh', 'release', 'create', self.version, title=f'Release {self.version}', latest=True, generate_notes=True).run()
+
     def release_helm(self) -> None:
         """Perform a release of a Helm chart."""
         helm('push', self.helm_package, self.helm_repo.name, **self.helm_repo.push_args)
 
     def release_increment_release(self) -> None:
         """Increment the project release version."""
-        if self.is_pre_release:
-            self.log_message('Skipping on pre-release')
-            return
         if hasattr(self.project, 'version_service'):
             self.log_message('Incrementing version service not supported...skipping')
             return
         version_tuple = self.project.version.split('.')
         version_tuple[len(version_tuple) - 1] = str(int(version_tuple[-1]) + 1)
         new_version = '.'.join(version_tuple)
         use_branch = self.step_info.increment_branch if self.step_info.increment_branch else self.git_client.CI_COMMIT_REF_NAME
         self.project.version = new_version
         self.log_message(f'Incrementing release to {new_version} on branch {use_branch}')
         self.commit_files('Automated pipeline version update check-in [skip ci]', use_branch, self.config.filename, file_updater=self.config.write)
 
     def release_tag_source(self) -> None:
         """Tag the source in Git with a release tag."""
-        if self.is_pre_release:
-            self.log_message('Skipping on pre-release')
-            return
         self.tag_source(self.release.release_tag, f'Release {self.release.release_tag}')
 
 
 def release() -> None:
     """This is the main entry point."""
     VjerAction('release', cast(VjerStep, ReleaseStep)).execute()
 
-# cSpell:ignore syscmd batcave cloudmgr vjer
+# cSpell:ignore syscmd batcave cloudmgr vjer bumpver
```

### Comparing `vjer-31.0.0/vjer/rollback.py` & `vjer-32.0.0/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/vjer/test.py` & `vjer-32.0.0/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/vjer/tool_reporter.py` & `vjer-32.0.0/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/vjer/utils.py` & `vjer-32.0.0/vjer/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 """Module to hold common values and utility functions for CI/CD support scripts.
 
 Attributes:
     PROJECT_CFG_FILE (str): The name of the project config file.
     TOOL_REPORT (Path): The path of the tool report.
 
-    RELEASE_PRE_STEPS (list): The list of release steps to perform before the ones specified for the project.
-    RELEASE_POST_STEPS (list): The list of release steps to perform before the ones specified for the project.
-
     There are several tool runners defined for simplified usage: git, helm.
 """
 # Import standard modules
 from copy import deepcopy as copy_object
 from datetime import datetime
 from os import getenv
 from pathlib import Path
@@ -27,14 +24,15 @@
 from batcave.cms import Client, ClientType
 from batcave.expander import Expander, file_expander
 from batcave.lang import BatCaveError, BatCaveException, PathName, DEFAULT_ENCODING, WIN32, yaml_to_dotmap
 from batcave.platarch import Platform
 from batcave.sysutil import CMDError, SysCmdRunner, syscmd
 from bumpver.config import init as bumpver_config
 from dotmap import DotMap
+from flit.build import main as flit_builder
 from yaml import safe_dump as yaml_dump, safe_load as yaml_load
 
 # Import project modules
 from . import __title__, __version__, __build_name__, __build_date__
 from .tool_reporter import tool_reporter
 
 _CONFIG_SECTIONS = ('project', 'test', 'build', 'deploy', 'rollback', 'release')
@@ -50,17 +48,14 @@
 
 PROJECT_CFG_FILE = getenv('VJER_CFG', 'vjer.yml')
 TOOL_REPORT = Path(__file__).parent.absolute() / 'tool_report.yml'
 
 HELM_CHART_FILE = 'Chart.yaml'
 DEFAULT_VERSION_FILES = {'helm': [HELM_CHART_FILE, 'values.yaml']}
 
-RELEASE_PRE_STEPS = ['tag_source']
-RELEASE_POST_STEPS = ['increment_release']
-
 VJER_ENV = getenv('VJER_ENV', 'local')
 REMOTE_REF = 'vjer_origin'
 
 apt = SysCmdRunner('apt-get', '-y').run
 apt_install = SysCmdRunner('apt-get', '-y', 'install', no_install_recommends=True).run
 git = SysCmdRunner('git').run
 helm = SysCmdRunner('helm', syscmd_args={'ignore_stderr': True}).run
@@ -210,15 +205,14 @@
 
     def __init__(self):
         """
         Attributes:
             _config_file: The config file for the project configuration.
             _sections: A list of the sections in the project configuration.
             schema: The schema version of the project configuration.
-            use_steps: A dictionary of steps by section.
         """
         project_root = Path.cwd()
         self._sections = {'project': ConfigSection(**(DotMap(project_root=project_root) | _PROJECT_DEFAULTS)),
                           'test': ConfigSection(),
                           'deploy': ConfigSection(clean=True),
                           'rollback': ConfigSection(clean=True),
                           'release': ConfigSection()}
@@ -231,20 +225,14 @@
         self._load_config()
         self._set_defaults()
         self._set_version()
 
         for section in _CONFIG_SECTIONS:
             self._sections[section].update_expander(property_holders=list(self._sections.values()))
 
-        release_steps = [self._get_phase_step('release', s) for s in RELEASE_PRE_STEPS]
-        if hasattr(self.release, 'steps'):
-            release_steps += [copy_object(s) for s in self.release.steps if s.get('type') not in RELEASE_PRE_STEPS + RELEASE_POST_STEPS]
-        release_steps += [self._get_phase_step('release', s) for s in RELEASE_POST_STEPS]
-        self.use_steps = {'release': release_steps}
-
     def __getattr__(self, attr: str):
         if attr not in self._sections:
             raise AttributeError(f'Configuration section not found: {attr}')
         return self._sections[attr]
 
     def _get_phase_step(self, phase: str, step_type: str) -> DotMap:
         """Get the specified step type for the specified phase.
@@ -330,15 +318,15 @@
         Attributes:
             build: The project build configuration.
             config: The project configuration.
             docker_client: The Docker client.
             git_client: The Git repository for the project.
             image_name: The Docker image name.
             image_tag: The Docker image tag.
-            pre_release_num: The pre-release suffix for the project.
+            pre_release_num: The pre_release suffix for the project.
             project: The project name.
             registry_client: The Docker image registry.
             release: The release configuration.
             step_info: The step information.
             version_tag: The Docker image version.
         """
         super().__init__()
@@ -452,14 +440,19 @@
             except CMDError as err:
                 if err.vars['returncode'] != 1:
                     raise
             return
 
         copytree(str(src), str(use_dest), dirs_exist_ok=True)
 
+    def flit_build(self) -> None:
+        """Run a Python flit build."""
+        flit_builder(Path('pyproject.toml'))
+        self.copy_artifact('dist')
+
     def tag_source(self, tag: str, label: Optional[str] = None) -> None:
         """Tag the source in Git.
 
         Args:
             tag: The label which which to tag the source.
             label (optional, default=None): The annotation to apply to the tag.
 
@@ -548,27 +541,19 @@
     def execute(self) -> None:
         """Run the action."""
         VjerStep().log_message(f'Starting {__title__} version {__version__} ({__build_name__}) [{__build_date__}]', True)
         for (category, info) in (yaml_to_dotmap(TOOL_REPORT) if TOOL_REPORT.exists() else tool_reporter()).items():
             VjerStep().log_message(category.replace('_', ' ').title(), True)
             for (name, data) in info.items():
                 VjerStep().log_message(f'  {name}: {data}')
-        steps = []
-        if self.action_type in self.config.use_steps:
-            steps = self.config.use_steps[self.action_type]
-        elif hasattr(action_def := getattr(self.config, self.action_type), 'steps'):
-            steps = action_def.steps
-        if not steps:
+        if not hasattr(action_def := getattr(self.config, self.action_type), 'steps'):
             return
 
         is_first_step = True
-        for step in [DotMap(s) for s in steps]:
+        for step in [DotMap(s) for s in action_def.steps]:
             step.is_first_step = is_first_step
-            verb = 'Skipping' if step.ignore else 'Executing'
-            VjerStep().log_message(f'{verb} {self.action_type} step: {step.type if (not step.name) else step.name}', True)
-            if step.ignore:
-                continue
+            VjerStep().log_message(f'Executing {self.action_type} step: {step.type if (not step.name) else step.name}', True)
             (executor := cast(Callable, self.action_step_class)()).step_info = step
             executor.execute()
             is_first_step = False
 
 # cSpell:ignore batcave bumpver cloudmgr dotmap platarch syscmd vjer checkin
```

### Comparing `vjer-31.0.0/vjer/vjer.py` & `vjer-32.0.0/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-31.0.0/PKG-INFO` & `vjer-32.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 31.0.0
+Version: 32.0.0
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Natural Language :: English
-Requires-Dist: BatCave~=43.0
+Requires-Dist: BatCave
 Requires-Dist: bumpver
 Requires-Dist: junitparser
 Requires-Dist: flake8
 Requires-Dist: flake8-annotations
 Requires-Dist: flake8-pyproject
 Requires-Dist: mypy
 Requires-Dist: pylint
```

