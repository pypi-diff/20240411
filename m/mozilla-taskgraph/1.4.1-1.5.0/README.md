# Comparing `tmp/mozilla-taskgraph-1.4.1.tar.gz` & `tmp/mozilla-taskgraph-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-taskgraph-1.4.1.tar", last modified: Tue Apr  9 17:51:12 2024, max compression
+gzip compressed data, was "mozilla-taskgraph-1.5.0.tar", last modified: Thu Apr 11 18:21:49 2024, max compression
```

## Comparing `mozilla-taskgraph-1.4.1.tar` & `mozilla-taskgraph-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.553421 mozilla-taskgraph-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/actions/release_promotion.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/worker_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-09 17:51:12.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-09 17:51:12.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:51:12.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-09 17:51:12.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 17:51:12.000000 mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:51:12.557421 mozilla-taskgraph-1.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/test/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-09 17:51:08.000000 mozilla-taskgraph-1.4.1/test/test_worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/release_promotion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/worker_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.658467 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 18:21:49.000000 mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:21:49.662467 mozilla-taskgraph-1.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-04-11 18:21:47.000000 mozilla-taskgraph-1.5.0/test/test_worker_types.py
```

### Comparing `mozilla-taskgraph-1.4.1/LICENSE` & `mozilla-taskgraph-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/PKG-INFO` & `mozilla-taskgraph-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.4.1
+Version: 1.5.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.4.1/README.md` & `mozilla-taskgraph-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/pyproject.toml` & `mozilla-taskgraph-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/setup.py` & `mozilla-taskgraph-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/__init__.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/actions/__init__.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/actions/release_promotion.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/actions/release_promotion.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/config.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/release_artifacts.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/transforms/scriptworker/shipit/mark_as_shipped.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph/worker_types.py` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph/worker_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,19 @@
                     description="Whether Bitrise should send a status report to "
                     "Github (default False).",
                 ): bool,
                 Optional(
                     "tag", description="The tag of the commit running the build."
                 ): str,
             },
+            Optional(
+                "artifact_prefix",
+                description="Directory prefix to store artifacts. Set this to 'public' "
+                "to create public artifacts.",
+            ): str,
         },
         Extra: object,
     },
 )
 def build_bitrise_payload(config, task, task_def):
     bitrise = task["worker"]["bitrise"]
     build_params = bitrise.get("build_params") or {}
@@ -125,15 +130,17 @@
             build_params.setdefault("branch_dest", base_ref)
 
         if config.params["base_repository"]:
             build_params.setdefault(
                 "branch_dest_repo_owner", config.params["base_repository"]
             )
 
-    task_def["payload"] = {"build_params": build_params}
+    payload = task_def["payload"] = {"build_params": build_params}
+    if bitrise.get("artifact_prefix"):
+        payload["artifact_prefix"] = bitrise["artifact_prefix"]
 
 
 @payload_builder(
     "scriptworker-shipit",
     schema={
         Required("release-name"): str,
     },
```

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/PKG-INFO` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-taskgraph
-Version: 1.4.1
+Version: 1.5.0
 Summary: Mozilla-specific transforms and utilities for Taskgraph
 Home-page: https://github.com/mozilla-releng/mozilla-taskgraph
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mozilla-taskgraph-1.4.1/src/mozilla_taskgraph.egg-info/SOURCES.txt` & `mozilla-taskgraph-1.5.0/src/mozilla_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/test/test_register.py` & `mozilla-taskgraph-1.5.0/test/test_register.py`

 * *Files identical despite different names*

### Comparing `mozilla-taskgraph-1.4.1/test/test_worker_types.py` & `mozilla-taskgraph-1.5.0/test/test_worker_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,40 @@
                     "foo:bitrise:app:some-app",
                     "foo:bitrise:workflow:bar",
                 ],
                 "tags": {"worker-implementation": "scriptworker"},
             },
             id="environments",
         ),
+        pytest.param(
+            {
+                "bitrise": {
+                    "artifact_prefix": "public",
+                    "app": "some-app",
+                    "workflows": ["bar"],
+                }
+            },
+            {},
+            {
+                "payload": {
+                    "artifact_prefix": "public",
+                    "build_params": {
+                        "branch": "default",
+                        "branch_repo_owner": "http://example.com/head/repo",
+                        "commit_hash": "abcdef",
+                    },
+                },
+                "scopes": [
+                    "foo:bitrise:app:some-app",
+                    "foo:bitrise:workflow:bar",
+                ],
+                "tags": {"worker-implementation": "scriptworker"},
+            },
+            id="artifact prefix",
+        ),
     ),
 )
 def test_build_bitrise_payload(
     make_graph_config, make_transform_config, parameters, worker, extra_params, expected
 ):
     schema = payload_builders["scriptworker-bitrise"].schema
```

