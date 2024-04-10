# Comparing `tmp/mslarkin-utils-1.8.tar.gz` & `tmp/mslarkin-utils-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mslarkin-utils-1.8.tar", last modified: Thu Oct 12 23:33:10 2023, max compression
+gzip compressed data, was "mslarkin-utils-1.9.tar", last modified: Thu Oct 12 23:46:31 2023, max compression
```

## Comparing `mslarkin-utils-1.8.tar` & `mslarkin-utils-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:33:10.927997 mslarkin-utils-1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-10-12 23:33:10.927997 mslarkin-utils-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-10-12 23:32:57.000000 mslarkin-utils-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 23:33:10.927997 mslarkin-utils-1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:33:10.915996 mslarkin-utils-1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:33:10.919996 mslarkin-utils-1.8/src/mslarkin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/gunicorn_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/load_gen_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-10-12 23:32:51.000000 mslarkin-utils-1.8/src/mslarkin/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:33:10.927997 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-10-12 23:33:10.000000 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-10-12 23:33:10.000000 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 23:33:10.000000 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-12 23:33:10.000000 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 23:33:10.000000 mslarkin-utils-1.8/src/mslarkin_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:46:31.855183 mslarkin-utils-1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-10-12 23:46:31.855183 mslarkin-utils-1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-10-12 23:46:20.000000 mslarkin-utils-1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 23:46:31.855183 mslarkin-utils-1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:46:31.851183 mslarkin-utils-1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:46:31.851183 mslarkin-utils-1.9/src/mslarkin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/gunicorn_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/load_gen_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-10-12 23:46:16.000000 mslarkin-utils-1.9/src/mslarkin/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 23:46:31.855183 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-10-12 23:46:31.000000 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-10-12 23:46:31.000000 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 23:46:31.000000 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-12 23:46:31.000000 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 23:46:31.000000 mslarkin-utils-1.9/src/mslarkin_utils.egg-info/top_level.txt
```

### Comparing `mslarkin-utils-1.8/PKG-INFO` & `mslarkin-utils-1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mslarkin-utils
-Version: 1.8
+Version: 1.9
 Summary: Frequently used utilities for Python
 Keywords: mslarkin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: google-cloud-pubsub
 Requires-Dist: google-cloud-monitoring
```

### Comparing `mslarkin-utils-1.8/README.md` & `mslarkin-utils-1.9/README.md`

 * *Files identical despite different names*

### Comparing `mslarkin-utils-1.8/pyproject.toml` & `mslarkin-utils-1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mslarkin-utils"
-version = "1.8"
+version = "1.9"
 description = "Frequently used utilities for Python"
 readme = "README.md"
 keywords = ["mslarkin"]
 requires-python = ">=3.8"
 dependencies = [
     "requests",
     "google-cloud-pubsub",
@@ -16,15 +16,15 @@
 ]
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "1.8"
+current_version = "1.9"
 version_pattern = "MAJOR.MINOR"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
```

### Comparing `mslarkin-utils-1.8/src/mslarkin/gcp_utils.py` & `mslarkin-utils-1.9/src/mslarkin/gcp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     service_id = os.environ.get('K_SERVICE', os.environ.get('GAE_SERVICE'))
     return service_id
 
 def get_revision_id():
     revision_id = os.environ.get('K_REVISION', os.environ.get('GAE_VERSION'))
     return revision_id
 
-def call_api(url, name):
+def call_api(name, url=None):
     if url==None:
         project_id = get_project_id()
         region = get_gcp_region()
         path_base = f"projects/{project_id}/locations/{region}"
         url=f'https://run.googleapis.com/v2/{path_base}'
     
     access_token = get_access_token()
```

### Comparing `mslarkin-utils-1.8/src/mslarkin/gunicorn_app.py` & `mslarkin-utils-1.9/src/mslarkin/gunicorn_app.py`

 * *Files identical despite different names*

### Comparing `mslarkin-utils-1.8/src/mslarkin/load_gen_tools.py` & `mslarkin-utils-1.9/src/mslarkin/load_gen_tools.py`

 * *Files identical despite different names*

### Comparing `mslarkin-utils-1.8/src/mslarkin/run_utils.py` & `mslarkin-utils-1.9/src/mslarkin/run_utils.py`

 * *Files identical despite different names*

### Comparing `mslarkin-utils-1.8/src/mslarkin/tools.py` & `mslarkin-utils-1.9/src/mslarkin/tools.py`

 * *Files identical despite different names*

### Comparing `mslarkin-utils-1.8/src/mslarkin_utils.egg-info/PKG-INFO` & `mslarkin-utils-1.9/src/mslarkin_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mslarkin-utils
-Version: 1.8
+Version: 1.9
 Summary: Frequently used utilities for Python
 Keywords: mslarkin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: google-cloud-pubsub
 Requires-Dist: google-cloud-monitoring
```

