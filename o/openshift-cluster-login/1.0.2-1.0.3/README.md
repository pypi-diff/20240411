# Comparing `tmp/openshift_cluster_login-1.0.2.tar.gz` & `tmp/openshift_cluster_login-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_cluster_login-1.0.2.tar", max compression
+gzip compressed data, was "openshift_cluster_login-1.0.3.tar", max compression
```

## Comparing `openshift_cluster_login-1.0.2.tar` & `openshift_cluster_login-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-01-15 10:18:26.598281 openshift_cluster_login-1.0.2/LICENSE
--rw-r--r--   0        0        0     5190 2024-01-15 10:18:26.598281 openshift_cluster_login-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/__init__.py
--rw-r--r--   0        0        0    13360 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/__main__.py
--rw-r--r--   0        0        0        0 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/__init__.py
--rw-r--r--   0        0        0       97 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/clusters.gql
--rw-r--r--   0        0        0     1728 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/clusters.py
--rw-r--r--   0        0        0        0 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/fragments/__init__.py
--rw-r--r--   0        0        0      152 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/fragments/cluster.gql
--rw-r--r--   0        0        0     1095 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/fragments/cluster.py
--rw-r--r--   0        0        0      145 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/namespaces.gql
--rw-r--r--   0        0        0     1982 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/ocl/gql_definitions/namespaces.py
--rw-r--r--   0        0        0     1745 2024-01-15 10:18:26.606281 openshift_cluster_login-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 09:34:54.611325 openshift_cluster_login-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5190 2024-04-11 09:34:54.611325 openshift_cluster_login-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/__init__.py
+-rw-r--r--   0        0        0    13422 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.gql
+-rw-r--r--   0        0        0     1728 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.py
+-rw-r--r--   0        0        0        0 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.gql
+-rw-r--r--   0        0        0     1095 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.py
+-rw-r--r--   0        0        0      145 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.gql
+-rw-r--r--   0        0        0     1982 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.py
+-rw-r--r--   0        0        0     1745 2024-04-11 09:34:54.623324 openshift_cluster_login-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6273 1970-01-01 00:00:00.000000 openshift_cluster_login-1.0.3/PKG-INFO
```

### Comparing `openshift_cluster_login-1.0.2/LICENSE` & `openshift_cluster_login-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.2/README.md` & `openshift_cluster_login-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.2/ocl/__main__.py` & `openshift_cluster_login-1.0.3/ocl/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,17 @@
     md5_hash.update(input_string.encode("utf-8"))
     return md5_hash.hexdigest()
 
 
 def gql_query(query: str) -> dict[Any, Any]:
     checksum = generate_md5_sum(query)
     if checksum not in cache:
-        headers = {"Authorization": get_var("APP_INT_TOKEN", hidden=True)}
+        headers = {}
+        if token := get_var("APP_INT_TOKEN", hidden=True, default=""):
+            headers["Authorization"] = token
         res = requests.post(
             url=get_var("APP_INTERFACE_URL"),
             json={"query": query},
             headers=headers,
         )
         res.raise_for_status()
         cache.set(checksum, res.json()["data"], expire=ONE_WEEK)
```

### Comparing `openshift_cluster_login-1.0.2/ocl/gql_definitions/clusters.py` & `openshift_cluster_login-1.0.3/ocl/gql_definitions/clusters.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.2/ocl/gql_definitions/fragments/cluster.py` & `openshift_cluster_login-1.0.3/ocl/gql_definitions/fragments/cluster.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.2/ocl/gql_definitions/namespaces.py` & `openshift_cluster_login-1.0.3/ocl/gql_definitions/namespaces.py`

 * *Files identical despite different names*

### Comparing `openshift_cluster_login-1.0.2/pyproject.toml` & `openshift_cluster_login-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openshift-cluster-login"
-version = "1.0.2"
+version = "1.0.3"
 description = "Openshift cluster login on command line"
 authors = ["Christian Assing <cassing@redhat.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/chassing/ocl"
 packages = [{ include = "ocl" }]
```

### Comparing `openshift_cluster_login-1.0.2/PKG-INFO` & `openshift_cluster_login-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-login
-Version: 1.0.2
+Version: 1.0.3
 Summary: Openshift cluster login on command line
 Home-page: http://github.com/chassing/ocl
 License: MIT
 Author: Christian Assing
 Author-email: cassing@redhat.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

