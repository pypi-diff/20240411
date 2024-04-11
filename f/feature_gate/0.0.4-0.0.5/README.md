# Comparing `tmp/feature_gate-0.0.4.tar.gz` & `tmp/feature_gate-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_gate-0.0.4.tar", max compression
+gzip compressed data, was "feature_gate-0.0.5.tar", max compression
```

## Comparing `feature_gate-0.0.4.tar` & `feature_gate-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-03-15 15:15:32.681382 feature_gate-0.0.4/LICENSE
--rw-r--r--   0        0        0     2206 2024-03-15 15:15:32.681382 feature_gate-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/__init__.py
--rw-r--r--   0        0        0     2630 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/adapters/memory.py
--rw-r--r--   0        0        0     2812 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/adapters/posthog.py
--rw-r--r--   0        0        0     2329 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/client.py
--rw-r--r--   0        0        0     7538 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/clients/posthog_api_client.py
--rw-r--r--   0        0        0      310 2024-03-15 15:15:32.681382 feature_gate-0.0.4/feature_gate/feature.py
--rw-r--r--   0        0        0      679 2024-03-15 15:15:32.681382 feature_gate-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 feature_gate-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 13:20:34.143210 feature_gate-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2206 2024-04-11 13:20:34.143210 feature_gate-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/adapters/memory.py
+-rw-r--r--   0        0        0     2812 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/adapters/posthog.py
+-rw-r--r--   0        0        0     2329 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/client.py
+-rw-r--r--   0        0        0     7546 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/clients/posthog_api_client.py
+-rw-r--r--   0        0        0      310 2024-04-11 13:20:34.143210 feature_gate-0.0.5/feature_gate/feature.py
+-rw-r--r--   0        0        0      679 2024-04-11 13:20:34.143210 feature_gate-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 feature_gate-0.0.5/PKG-INFO
```

### Comparing `feature_gate-0.0.4/LICENSE` & `feature_gate-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_gate-0.0.4/README.md` & `feature_gate-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `feature_gate-0.0.4/feature_gate/adapters/memory.py` & `feature_gate-0.0.5/feature_gate/adapters/memory.py`

 * *Files identical despite different names*

### Comparing `feature_gate-0.0.4/feature_gate/adapters/posthog.py` & `feature_gate-0.0.5/feature_gate/adapters/posthog.py`

 * *Files identical despite different names*

### Comparing `feature_gate-0.0.4/feature_gate/client.py` & `feature_gate-0.0.5/feature_gate/client.py`

 * *Files identical despite different names*

### Comparing `feature_gate-0.0.4/feature_gate/clients/posthog_api_client.py` & `feature_gate-0.0.5/feature_gate/clients/posthog_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         'deleted': deleted,
         'active': active
       }
       response = self._post(path, payload)
       return self._map_single_response("POST", path, response)
 
   def fetch_feature(self, key):
-    features = self.list_features()["data"]
+    features = self.list_features().get("data", [])
     for entry in features:
         if "key" in entry and entry["key"] == key:
             return entry
     return None
 
   def delete_feature(self, key):
     feature = self.fetch_feature(key)
```

### Comparing `feature_gate-0.0.4/pyproject.toml` & `feature_gate-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "feature_gate"
-version = "0.0.4"
+version = "0.0.5"
 description = "An extensible feature flagging library for Python"
 authors = ["Patrick Wiseman <patrick@deft.services>"]
 maintainers = ["Patrick Wiseman <patrick@deft.services>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deftinc/feature_gate"
 repository = "https://github.com/deftinc/feature_gate"
```

### Comparing `feature_gate-0.0.4/PKG-INFO` & `feature_gate-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_gate
-Version: 0.0.4
+Version: 0.0.5
 Summary: An extensible feature flagging library for Python
 Home-page: https://github.com/deftinc/feature_gate
 License: MIT
 Keywords: feature flags,feature gate
 Author: Patrick Wiseman
 Author-email: patrick@deft.services
 Maintainer: Patrick Wiseman
```

