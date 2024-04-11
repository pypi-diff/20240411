# Comparing `tmp/swf-typed-1.1.1rc1.tar.gz` & `tmp/swf-typed-1.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swf-typed-1.1.1rc1.tar", last modified: Wed Oct 12 13:30:59 2022, max compression
+gzip compressed data, was "swf-typed-1.1.2rc0.tar", last modified: Thu Apr 11 02:40:05 2024, max compression
```

## Comparing `swf-typed-1.1.1rc1.tar` & `swf-typed-1.1.2rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.706625 swf-typed-1.1.1rc1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.698624 swf-typed-1.1.1rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.702624 swf-typed-1.1.1rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.702624 swf-typed-1.1.1rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.github/workflows/publish-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3359 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-12 13:30:59.706625 swf-typed-1.1.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.702624 swf-typed-1.1.1rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.702624 swf-typed-1.1.1rc1/docs/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/docs/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/docs/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-12 13:30:59.706625 swf-typed-1.1.1rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.698624 swf-typed-1.1.1rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.706625 swf-typed-1.1.1rc1/src/swf_typed/
--rw-r--r--   0 runner    (1001) docker     (121)     8497 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6172 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_activities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    16751 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_decisions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_domains.py
--rw-r--r--   0 runner    (1001) docker     (121)     7264 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21730 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_executions.py
--rw-r--r--   0 runner    (1001) docker     (121)    59975 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_history.py
--rw-r--r--   0 runner    (1001) docker     (121)    21047 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     8723 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6350 2022-10-12 13:30:47.000000 swf-typed-1.1.1rc1/src/swf_typed/_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-12 13:30:59.706625 swf-typed-1.1.1rc1/src/swf_typed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-12 13:30:59.000000 swf-typed-1.1.1rc1/src/swf_typed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-10-12 13:30:59.000000 swf-typed-1.1.1rc1/src/swf_typed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-12 13:30:59.000000 swf-typed-1.1.1rc1/src/swf_typed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-12 13:30:59.000000 swf-typed-1.1.1rc1/src/swf_typed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-12 13:30:59.000000 swf-typed-1.1.1rc1/src/swf_typed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.255994 swf-typed-1.1.2rc0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.github/workflows/publish-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-11 02:40:05.255994 swf-typed-1.1.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/docs/src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/docs/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 02:40:05.255994 swf-typed-1.1.2rc0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.251994 swf-typed-1.1.2rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.255994 swf-typed-1.1.2rc0/src/swf_typed/
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16751 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_decisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59975 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21047 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-11 02:40:00.000000 swf-typed-1.1.2rc0/src/swf_typed/_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:40:05.255994 swf-typed-1.1.2rc0/src/swf_typed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-11 02:40:05.000000 swf-typed-1.1.2rc0/src/swf_typed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-11 02:40:05.000000 swf-typed-1.1.2rc0/src/swf_typed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:40:05.000000 swf-typed-1.1.2rc0/src/swf_typed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 02:40:05.000000 swf-typed-1.1.2rc0/src/swf_typed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 02:40:05.000000 swf-typed-1.1.2rc0/src/swf_typed.egg-info/top_level.txt
```

### Comparing `swf-typed-1.1.1rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `swf-typed-1.1.2rc0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/.github/workflows/test-python-package.yml` & `swf-typed-1.1.2rc0/.github/workflows/test-python-package.yml`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/CODE_OF_CONDUCT.md` & `swf-typed-1.1.2rc0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/LICENSE` & `swf-typed-1.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/PKG-INFO` & `swf-typed-1.1.2rc0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: swf-typed
-Version: 1.1.1rc1
+Version: 1.1.2rc0
 Summary: Typed Python interface to AWS Simple Workflow service
-Home-page: https://github.com/EpicWink/swf-typed
+Home-page: https://github.com/EpicWink/python-swf-typed
 Author: Laurie
 Author-email: laurie_opperman@hotmail.com
 License: "MIT"
 Project-URL: Documentation, https://python-swf-typed.readthedocs.io/
-Project-URL: Source, https://github.com/EpicWink/swf-typed
-Project-URL: Tracker, https://github.com/EpicWink/swf-typed/issues
+Project-URL: Source, https://github.com/EpicWink/python-swf-typed
+Project-URL: Tracker, https://github.com/EpicWink/python-swf-typed/issues
+Project-URL: Changelog, https://github.com/EpicWink/python-swf-typed/releases
 Keywords: swf,typed
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3~=1.18
 
 # Python interface to SWF
 Typed Python interface to AWS Simple Workflow service
 
 * Type annotations
 * Explicit exceptions
 * Execution state construction
 * Consistent method/attribute/parameter names (see below)
 * Consistent model struture
 * Automatic flattening of paged-list responses
   * next-page calls are run concurrently and on-demand
 * Better execution filtering
 
+The most interesting part is state construction: given an execution history, this
+library can build a full state of the execution and all of its tasks with all details;
+see [`swf_typed.build_state`](
+  https://python-swf-typed.readthedocs.io/en/latest/swf_typed._state.html#swf_typed.build_state
+). The rest of the API simply mirror's SWF's.
+
 ### See also
 * [py-swf](https://pypi.org/project/py-swf/) - typed and object-oriented interface layer
 * [mypy-boto3-swf](https://pypi.org/project/mypy-boto3-swf/) - type-annotated layer
 * [python-simple-workflow](https://pypi.org/project/simple-workflow/) - higher-level
   interface layer
 
 ## Installation
```

### Comparing `swf-typed-1.1.1rc1/README.md` & `swf-typed-1.1.2rc0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 * Execution state construction
 * Consistent method/attribute/parameter names (see below)
 * Consistent model struture
 * Automatic flattening of paged-list responses
   * next-page calls are run concurrently and on-demand
 * Better execution filtering
 
+The most interesting part is state construction: given an execution history, this
+library can build a full state of the execution and all of its tasks with all details;
+see [`swf_typed.build_state`](
+  https://python-swf-typed.readthedocs.io/en/latest/swf_typed._state.html#swf_typed.build_state
+). The rest of the API simply mirror's SWF's.
+
 ### See also
 * [py-swf](https://pypi.org/project/py-swf/) - typed and object-oriented interface layer
 * [mypy-boto3-swf](https://pypi.org/project/mypy-boto3-swf/) - type-annotated layer
 * [python-simple-workflow](https://pypi.org/project/simple-workflow/) - higher-level
   interface layer
 
 ## Installation
```

### Comparing `swf-typed-1.1.1rc1/docs/src/conf.py` & `swf-typed-1.1.2rc0/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/docs/src/index.rst` & `swf-typed-1.1.2rc0/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/setup.cfg` & `swf-typed-1.1.2rc0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [metadata]
 name = swf-typed
-url = https://github.com/EpicWink/swf-typed
+url = https://github.com/EpicWink/python-swf-typed
 author = Laurie
 author_email = laurie_opperman@hotmail.com
 license = "MIT"
 description = Typed Python interface to AWS Simple Workflow service
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = swf, typed
 project_urls = 
 	Documentation = https://python-swf-typed.readthedocs.io/
-	Source = https://github.com/EpicWink/swf-typed
-	Tracker = https://github.com/EpicWink/swf-typed/issues
+	Source = https://github.com/EpicWink/python-swf-typed
+	Tracker = https://github.com/EpicWink/python-swf-typed/issues
+	Changelog = https://github.com/EpicWink/python-swf-typed/releases
 
 [options]
 install_requires = 
 	boto3 ~= 1.18
 packages = find:
 package_dir = =src
 python_requires = ~= 3.7
```

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/__init__.py` & `swf-typed-1.1.2rc0/src/swf_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_activities.py` & `swf-typed-1.1.2rc0/src/swf_typed/_activities.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_common.py` & `swf-typed-1.1.2rc0/src/swf_typed/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 T = t.TypeVar("T")
 
 is_deprecated_by_registration_status = {"REGISTERED": False, "DEPRECATED": True}
 registration_status_by_is_deprecated = {
     v: k for k, v in is_deprecated_by_registration_status.items()
 }
 
-executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
-
 
 class _Sentinel:
     """Not-provided value sentinel."""
 
     def __repr__(self):
         return f"{self.__class__.__name__}()"
 
@@ -119,14 +117,15 @@
 
         while response.get("nextPageToken"):
             future = executor.submit(call, nextPageToken=response["nextPageToken"])
             yield from (model(d) for d in response.get(data_key) or [])
             response = future.result()
         yield from (model(d) for d in response.get(data_key) or [])
 
+    executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
     response = call()
     return iter_()
 
 
 @contextlib.contextmanager
 def polling_socket_timeout(
     timeout: datetime.timedelta = datetime.timedelta(seconds=70),
```

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_decisions.py` & `swf-typed-1.1.2rc0/src/swf_typed/_decisions.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_domains.py` & `swf-typed-1.1.2rc0/src/swf_typed/_domains.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_exceptions.py` & `swf-typed-1.1.2rc0/src/swf_typed/_exceptions.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_executions.py` & `swf-typed-1.1.2rc0/src/swf_typed/_executions.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_history.py` & `swf-typed-1.1.2rc0/src/swf_typed/_history.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_state.py` & `swf-typed-1.1.2rc0/src/swf_typed/_state.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_tasks.py` & `swf-typed-1.1.2rc0/src/swf_typed/_tasks.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed/_workflows.py` & `swf-typed-1.1.2rc0/src/swf_typed/_workflows.py`

 * *Files identical despite different names*

### Comparing `swf-typed-1.1.1rc1/src/swf_typed.egg-info/PKG-INFO` & `swf-typed-1.1.2rc0/src/swf_typed.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 Metadata-Version: 2.1
 Name: swf-typed
-Version: 1.1.1rc1
+Version: 1.1.2rc0
 Summary: Typed Python interface to AWS Simple Workflow service
-Home-page: https://github.com/EpicWink/swf-typed
+Home-page: https://github.com/EpicWink/python-swf-typed
 Author: Laurie
 Author-email: laurie_opperman@hotmail.com
 License: "MIT"
 Project-URL: Documentation, https://python-swf-typed.readthedocs.io/
-Project-URL: Source, https://github.com/EpicWink/swf-typed
-Project-URL: Tracker, https://github.com/EpicWink/swf-typed/issues
+Project-URL: Source, https://github.com/EpicWink/python-swf-typed
+Project-URL: Tracker, https://github.com/EpicWink/python-swf-typed/issues
+Project-URL: Changelog, https://github.com/EpicWink/python-swf-typed/releases
 Keywords: swf,typed
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3~=1.18
 
 # Python interface to SWF
 Typed Python interface to AWS Simple Workflow service
 
 * Type annotations
 * Explicit exceptions
 * Execution state construction
 * Consistent method/attribute/parameter names (see below)
 * Consistent model struture
 * Automatic flattening of paged-list responses
   * next-page calls are run concurrently and on-demand
 * Better execution filtering
 
+The most interesting part is state construction: given an execution history, this
+library can build a full state of the execution and all of its tasks with all details;
+see [`swf_typed.build_state`](
+  https://python-swf-typed.readthedocs.io/en/latest/swf_typed._state.html#swf_typed.build_state
+). The rest of the API simply mirror's SWF's.
+
 ### See also
 * [py-swf](https://pypi.org/project/py-swf/) - typed and object-oriented interface layer
 * [mypy-boto3-swf](https://pypi.org/project/mypy-boto3-swf/) - type-annotated layer
 * [python-simple-workflow](https://pypi.org/project/simple-workflow/) - higher-level
   interface layer
 
 ## Installation
```

### Comparing `swf-typed-1.1.1rc1/src/swf_typed.egg-info/SOURCES.txt` & `swf-typed-1.1.2rc0/src/swf_typed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

