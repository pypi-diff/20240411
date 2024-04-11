# Comparing `tmp/takeoff_launcher-0.0.8.tar.gz` & `tmp/takeoff_launcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "takeoff_launcher-0.0.8.tar", last modified: Wed Mar 27 12:09:14 2024, max compression
+gzip compressed data, was "takeoff_launcher-0.0.9.tar", last modified: Thu Apr 11 13:27:41 2024, max compression
```

## Comparing `takeoff_launcher-0.0.8.tar` & `takeoff_launcher-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1206 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/CHANGELOG.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1763 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/PKG-INFO
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1264 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/README.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     6560 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/Taskfile.yml
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.989743 takeoff_launcher-0.0.8/docs/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2233 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/docs/CHANGELOG_OLD.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     8058 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/docs/takeoff_env_setting.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2508 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/docs/takeoff_sdk_internal.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2084 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/docs/usage.md
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     7843 2024-03-27 12:09:12.000000 takeoff_launcher-0.0.8/pyproject.toml
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.989743 takeoff_launcher-0.0.8/scripts/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2725 2024-03-21 12:10:00.000000 takeoff_launcher-0.0.8/scripts/bump_version.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1319 2024-03-22 11:11:33.000000 takeoff_launcher-0.0.8/scripts/extract_version.py
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.989743 takeoff_launcher-0.0.8/setup/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     3088 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/setup/Taskfile.yml
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1004 2024-03-19 19:44:53.000000 takeoff_launcher-0.0.8/setup/requirements.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     3014 2024-03-21 08:57:28.000000 takeoff_launcher-0.0.8/setup/requirements_develop.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)       38 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/setup.cfg
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.981743 takeoff_launcher-0.0.8/src/
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/src/takeoff_launcher/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)      106 2024-03-21 09:10:19.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/__init__.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5286 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/conf_mgr.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)    20838 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/main.py
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)      123 2024-03-21 09:10:19.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/__init__.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5187 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/schema.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5589 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/takeoff.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     6483 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/utils.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5209 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/utils.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)        5 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/src/takeoff_launcher/version.txt
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1763 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/PKG-INFO
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)      913 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)        1 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)       55 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/entry_points.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)      148 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/requires.txt
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)       17 2024-03-27 12:09:14.000000 takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/top_level.txt
-drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-03-27 12:09:14.993743 takeoff_launcher-0.0.8/tests/
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)      693 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/tests/test_manifest.yaml
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2149 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/tests/test_schema.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2742 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.8/tests/test_takeoff.py
--rw-r--r--   0 titan-1   (1000) titan-1   (1000)        5 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.8/version.txt
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1320 2024-04-11 13:27:37.000000 takeoff_launcher-0.0.9/CHANGELOG.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1763 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/PKG-INFO
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1264 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/README.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     6560 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/Taskfile.yml
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.121574 takeoff_launcher-0.0.9/docs/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2233 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/docs/CHANGELOG_OLD.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     8058 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/docs/takeoff_env_setting.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2508 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/docs/takeoff_sdk_internal.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2084 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.9/docs/usage.md
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     7846 2024-04-11 13:27:38.000000 takeoff_launcher-0.0.9/pyproject.toml
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.121574 takeoff_launcher-0.0.9/scripts/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2725 2024-03-21 12:10:00.000000 takeoff_launcher-0.0.9/scripts/bump_version.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1319 2024-03-22 11:11:33.000000 takeoff_launcher-0.0.9/scripts/extract_version.py
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.121574 takeoff_launcher-0.0.9/setup/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     3088 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/setup/Taskfile.yml
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1004 2024-03-19 19:44:53.000000 takeoff_launcher-0.0.9/setup/requirements.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     3014 2024-03-21 08:57:28.000000 takeoff_launcher-0.0.9/setup/requirements_develop.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)       38 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/setup.cfg
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.117574 takeoff_launcher-0.0.9/src/
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/src/takeoff_launcher/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)      106 2024-03-21 09:10:19.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/__init__.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5286 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/conf_mgr.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)    20838 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/main.py
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)      123 2024-03-21 09:10:19.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/__init__.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5187 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/schema.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5589 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/takeoff.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     6486 2024-04-11 12:37:15.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/utils.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     5209 2024-03-27 12:09:11.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/utils.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)        5 2024-04-11 13:27:37.000000 takeoff_launcher-0.0.9/src/takeoff_launcher/version.txt
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     1763 2024-04-11 13:27:40.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)      913 2024-04-11 13:27:41.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)        1 2024-04-11 13:27:40.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)       55 2024-04-11 13:27:40.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/entry_points.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)      148 2024-04-11 13:27:40.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/requires.txt
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)       17 2024-04-11 13:27:40.000000 takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/top_level.txt
+drwxr-xr-x   0 titan-1   (1000) titan-1   (1000)        0 2024-04-11 13:27:41.125574 takeoff_launcher-0.0.9/tests/
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)      693 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/tests/test_manifest.yaml
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2149 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/tests/test_schema.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)     2742 2024-03-19 14:14:38.000000 takeoff_launcher-0.0.9/tests/test_takeoff.py
+-rw-r--r--   0 titan-1   (1000) titan-1   (1000)        5 2024-04-11 13:27:37.000000 takeoff_launcher-0.0.9/version.txt
```

### Comparing `takeoff_launcher-0.0.8/CHANGELOG.md` & `takeoff_launcher-0.0.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 The format is based on [Keep a Changelog],
 and this project adheres to [Semantic Versioning].
 
 ## [Unreleased]
 
 - /
 
+## [0.0.9] - 2024-04-11
+
+### Changed
+
+- Removed any reference to `iris_cache` and replaced with `takeoff_cache`.
+
 
 ## [0.0.8] - 2024-03-26
 
 ### Added
 
 - add the ability to switch version in `takeoff version` command. store the version information in takeoff_cache
```

### Comparing `takeoff_launcher-0.0.8/PKG-INFO` & `takeoff_launcher-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takeoff_launcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Takeoff Launcher package is a python cli tool that provides a simple interface to launch Takeoff container
 Author-email: TitanML <hello@titanml.co>
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==2.5.1
 Requires-Dist: pydantic-settings==2.1.0
 Requires-Dist: loguru==0.6.0
 Requires-Dist: docker==7.0.0
```

### Comparing `takeoff_launcher-0.0.8/README.md` & `takeoff_launcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/Taskfile.yml` & `takeoff_launcher-0.0.9/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/docs/CHANGELOG_OLD.md` & `takeoff_launcher-0.0.9/docs/CHANGELOG_OLD.md`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/docs/takeoff_env_setting.md` & `takeoff_launcher-0.0.9/docs/takeoff_env_setting.md`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/docs/takeoff_sdk_internal.md` & `takeoff_launcher-0.0.9/docs/takeoff_sdk_internal.md`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/docs/usage.md` & `takeoff_launcher-0.0.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/pyproject.toml` & `takeoff_launcher-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 #                                                Project Configuration                                                 #
 # ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────── #
 
 [project]
 name = "takeoff_launcher"
-version = "0.0.8"
+version = "0.0.9"
 description = "Takeoff Launcher package is a python cli tool that provides a simple interface to launch Takeoff container"
 authors = [{name = "TitanML", email="hello@titanml.co"}]
 readme = "README.md"
 dependencies = [
     "pydantic==2.5.1",
     "pydantic-settings==2.1.0",
     "loguru==0.6.0",
@@ -177,15 +177,15 @@
     "--cov-report=xml:docs/coverage/coverage.xml",
     "--verbose",
     "--cache-clear",
     "-m", "not slow",
 ]
 
 [tool.pytest_env]
-CACHE_DIR_OVERRIDE = "~/.iris_cache"
+CACHE_DIR_OVERRIDE = "~/.takeoff_cache"
 TAKEOFF_READER_ID = "test"
 TAKEOFF_CONSUMER_GROUP = "primary"
 TAKEOFF_LOG_LEVEL="TRACE"
 
 
 
 [tool.coverage.run]
```

### Comparing `takeoff_launcher-0.0.8/scripts/bump_version.py` & `takeoff_launcher-0.0.9/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/scripts/extract_version.py` & `takeoff_launcher-0.0.9/scripts/extract_version.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/setup/Taskfile.yml` & `takeoff_launcher-0.0.9/setup/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/setup/requirements.txt` & `takeoff_launcher-0.0.9/setup/requirements.txt`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/setup/requirements_develop.txt` & `takeoff_launcher-0.0.9/setup/requirements_develop.txt`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/conf_mgr.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/conf_mgr.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/main.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/main.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/schema.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/schema.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/takeoff.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/takeoff.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/sdk/utils.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/sdk/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     Returns:
         tuple: (takeoff_port, management_port, openai_port, container)
     """
     image = os.environ.get("TAKEOFF_IMAGE", "tytn/takeoff-pro:0.12.0-gpu")
 
     random_name = "takeoff_" + str(uuid.uuid4())[:8]
-    volumes = [f"{Path.home()}/.iris_cache:/code/models", f"{manifest_path}:/code/config.yaml"]
+    volumes = [f"{Path.home()}/.takeoff_cache:/code/models", f"{manifest_path}:/code/config.yaml"]
     device_requests = [docker.types.DeviceRequest(count=-1, capabilities=[["gpu"]])] if device == "cuda" else None
 
     container = start_container(
         image_name=image,
         container_name=random_name,
         ports={"3000/tcp": None, "3001/tcp": None, "3003/tcp": None, "9090/tcp": None},
         volumes=volumes,
```

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher/utils.py` & `takeoff_launcher-0.0.9/src/takeoff_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/PKG-INFO` & `takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: takeoff_launcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: Takeoff Launcher package is a python cli tool that provides a simple interface to launch Takeoff container
 Author-email: TitanML <hello@titanml.co>
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==2.5.1
 Requires-Dist: pydantic-settings==2.1.0
 Requires-Dist: loguru==0.6.0
 Requires-Dist: docker==7.0.0
```

### Comparing `takeoff_launcher-0.0.8/src/takeoff_launcher.egg-info/SOURCES.txt` & `takeoff_launcher-0.0.9/src/takeoff_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/tests/test_manifest.yaml` & `takeoff_launcher-0.0.9/tests/test_manifest.yaml`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/tests/test_schema.py` & `takeoff_launcher-0.0.9/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `takeoff_launcher-0.0.8/tests/test_takeoff.py` & `takeoff_launcher-0.0.9/tests/test_takeoff.py`

 * *Files identical despite different names*

