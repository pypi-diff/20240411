# Comparing `tmp/surfkit-0.1.8.tar.gz` & `tmp/surfkit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.8.tar", max compression
+gzip compressed data, was "surfkit-0.1.9.tar", max compression
```

## Comparing `surfkit-0.1.8.tar` & `surfkit-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.8/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.8/README.md
--rw-r--r--   0        0        0      442 2024-04-04 17:28:55.859187 surfkit-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      610 2024-04-03 16:41:37.648579 surfkit-0.1.8/surfkit/agent.py
--rw-r--r--   0        0        0        0 2024-04-03 16:41:36.393225 surfkit-0.1.8/surfkit/cli.py
--rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.8/surfkit/db/conn.py
--rw-r--r--   0        0        0     1473 2024-04-03 16:41:49.842770 surfkit-0.1.8/surfkit/db/models.py
--rw-r--r--   0        0        0      195 2024-04-03 16:41:34.576256 surfkit-0.1.8/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.8/surfkit/hub.py
--rw-r--r--   0        0        0     5562 2024-04-03 22:24:56.115885 surfkit-0.1.8/surfkit/llm.py
--rw-r--r--   0        0        0     1721 2024-04-03 20:39:21.080498 surfkit-0.1.8/surfkit/models.py
--rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.8/surfkit/types.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.9/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.9/README.md
+-rw-r--r--   0        0        0      442 2024-04-04 18:10:08.442909 surfkit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-03 16:41:37.648579 surfkit-0.1.9/surfkit/agent.py
+-rw-r--r--   0        0        0        0 2024-04-03 16:41:36.393225 surfkit-0.1.9/surfkit/cli.py
+-rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.9/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1473 2024-04-03 16:41:49.842770 surfkit-0.1.9/surfkit/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-03 16:41:34.576256 surfkit-0.1.9/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.9/surfkit/hub.py
+-rw-r--r--   0        0        0     5562 2024-04-03 22:24:56.115885 surfkit-0.1.9/surfkit/llm.py
+-rw-r--r--   0        0        0     1721 2024-04-03 20:39:21.080498 surfkit-0.1.9/surfkit/models.py
+-rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.9/surfkit/types.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.9/PKG-INFO
```

### Comparing `surfkit-0.1.8/LICENSE` & `surfkit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/agent.py` & `surfkit-0.1.9/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/db/conn.py` & `surfkit-0.1.9/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/db/models.py` & `surfkit-0.1.9/surfkit/db/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/hub.py` & `surfkit-0.1.9/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/llm.py` & `surfkit-0.1.9/surfkit/llm.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/models.py` & `surfkit-0.1.9/surfkit/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/surfkit/types.py` & `surfkit-0.1.9/surfkit/types.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.8/PKG-INFO` & `surfkit-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolkit to build GUI surfing AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: agentdesk (>=0.2.43,<0.3.0)
 Requires-Dist: litellm (>=1.34.21,<2.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: taskara (>=0.1.7,<0.2.0)
+Requires-Dist: taskara (>=0.1.8,<0.2.0)
 Requires-Dist: threadmem (>=0.2.11,<0.3.0)
 Description-Content-Type: text/markdown
 
 # SurfKit
 
 A toolkit to build GUI surfer AI agents
```

