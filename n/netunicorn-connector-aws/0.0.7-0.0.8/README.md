# Comparing `tmp/netunicorn-connector-aws-0.0.7.tar.gz` & `tmp/netunicorn-connector-aws-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-aws-0.0.7.tar", last modified: Sat Dec 23 04:12:38 2023, max compression
+gzip compressed data, was "netunicorn-connector-aws-0.0.8.tar", last modified: Wed Apr 10 22:15:15 2024, max compression
```

## Comparing `netunicorn-connector-aws-0.0.7.tar` & `netunicorn-connector-aws-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.256651 netunicorn-connector-aws-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-23 04:12:24.000000 netunicorn-connector-aws-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-23 04:12:38.256651 netunicorn-connector-aws-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-23 04:12:24.000000 netunicorn-connector-aws-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-23 04:12:24.000000 netunicorn-connector-aws-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 04:12:38.256651 netunicorn-connector-aws-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.252651 netunicorn-connector-aws-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.252651 netunicorn-connector-aws-0.0.7/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.252651 netunicorn-connector-aws-0.0.7/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.252651 netunicorn-connector-aws-0.0.7/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.252651 netunicorn-connector-aws-0.0.7/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:24.000000 netunicorn-connector-aws-0.0.7/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19102 2023-12-23 04:12:24.000000 netunicorn-connector-aws-0.0.7/src/netunicorn/director/infrastructure/connectors/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 04:12:38.256651 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-23 04:12:38.000000 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-23 04:12:38.000000 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 04:12:38.000000 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-23 04:12:38.000000 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-23 04:12:38.000000 netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-10 22:15:09.000000 netunicorn-connector-aws-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 22:15:09.000000 netunicorn-connector-aws-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 22:15:09.000000 netunicorn-connector-aws-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:09.000000 netunicorn-connector-aws-0.0.8/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19304 2024-04-10 22:15:09.000000 netunicorn-connector-aws-0.0.8/src/netunicorn/director/infrastructure/connectors/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:15:15.746496 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-10 22:15:15.000000 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-10 22:15:15.000000 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:15:15.000000 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-10 22:15:15.000000 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 22:15:15.000000 netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-aws-0.0.7/LICENSE` & `netunicorn-connector-aws-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aws-0.0.7/PKG-INFO` & `netunicorn-connector-aws-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aws
-Version: 0.0.7
+Version: 0.0.8
 Summary: AWS connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-aws-0.0.7/README.md` & `netunicorn-connector-aws-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-aws-0.0.7/pyproject.toml` & `netunicorn-connector-aws-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-aws"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "AWS connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-aws-0.0.7/src/netunicorn/director/infrastructure/connectors/aws.py` & `netunicorn-connector-aws-0.0.8/src/netunicorn/director/infrastructure/connectors/aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,17 +115,18 @@
         while True:
             try:
                 definitions = self.ecs_client.list_task_definitions(
                     status="INACTIVE",
                 )
 
                 if definitions["taskDefinitionArns"]:
-                    self.ecs_client.delete_task_definitions(
-                        taskDefinitions=definitions["taskDefinitionArns"]
-                    )
+                    for i in range(0, len(definitions["taskDefinitionArns"]), 5):
+                        self.ecs_client.deregister_task_definition(
+                            taskDefinition=definitions["taskDefinitionArns"][i:i+5]
+                        )
                     self.logger.debug(f"Cleaned {len(definitions['taskDefinitionArns'])} stopped containers")
             except Exception as e:
                 self.logger.error(f"Failed to clean task definitions: {e}")
             await asyncio.sleep(300)
 
     def _create_subnet(self) -> str:
         ec2_client = boto3.client(
@@ -486,17 +487,18 @@
                 familyPrefix=f"experiment-{experiment_id}",
             )
             for definition in definitions["taskDefinitionArns"]:
                 self.ecs_client.deregister_task_definition(
                     taskDefinition=definition,
                 )
             if definitions["taskDefinitionArns"]:
-                self.ecs_client.delete_task_definitions(
-                    taskDefinitions=definitions["taskDefinitionArns"]
-                )
+                for i in range(0, len(definitions["taskDefinitionArns"]), 5):
+                    self.ecs_client.deregister_task_definition(
+                        taskDefinition=definitions["taskDefinitionArns"][i:i+5]
+                    )
         except Exception as e:
             self.logger.exception(e)
 
 
 async def test():
     connector = AWSFargate(
         connector_name="test",
```

### Comparing `netunicorn-connector-aws-0.0.7/src/netunicorn_connector_aws.egg-info/PKG-INFO` & `netunicorn-connector-aws-0.0.8/src/netunicorn_connector_aws.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-aws
-Version: 0.0.7
+Version: 0.0.8
 Summary: AWS connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

