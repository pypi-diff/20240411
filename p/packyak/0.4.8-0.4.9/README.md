# Comparing `tmp/packyak-0.4.8.tar.gz` & `tmp/packyak-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packyak-0.4.8.tar", max compression
+gzip compressed data, was "packyak-0.4.9.tar", max compression
```

## Comparing `packyak-0.4.8.tar` & `packyak-0.4.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     5433 2024-02-23 08:15:58.848693 packyak-0.4.8/README.md
--rw-r--r--   0        0        0      993 2024-02-26 09:31:52.166939 packyak-0.4.8/packyak/__init__.py
--rw-r--r--   0        0        0      433 2024-02-12 19:51:41.337451 packyak-0.4.8/packyak/asset/asset.py
--rw-r--r--   0        0        0       72 2024-02-26 09:31:52.167028 packyak-0.4.8/packyak/asset/manifest.py
--rw-r--r--   0        0        0     1555 2024-02-26 09:31:52.167119 packyak-0.4.8/packyak/asset/namespace.py
--rw-r--r--   0        0        0      415 2024-02-10 02:53:25.975611 packyak-0.4.8/packyak/asset/partition_key.py
--rw-r--r--   0        0        0     1013 2024-02-26 09:31:52.167202 packyak-0.4.8/packyak/asset/source.py
--rw-r--r--   0        0        0      276 2024-02-26 09:31:52.167305 packyak-0.4.8/packyak/cli/__init__.py
--rw-r--r--   0        0        0      283 2024-02-26 09:31:52.167394 packyak-0.4.8/packyak/cli/__main__.py
--rw-r--r--   0        0        0       50 2024-02-22 04:42:16.104618 packyak-0.4.8/packyak/cli/cli.py
--rw-r--r--   0        0        0      775 2024-02-26 09:31:52.167456 packyak-0.4.8/packyak/cli/materialize.py
--rw-r--r--   0        0        0      189 2024-02-26 09:31:52.167551 packyak-0.4.8/packyak/cli/new.py
--rw-r--r--   0        0        0      700 2024-02-26 09:31:52.167609 packyak-0.4.8/packyak/cli/run.py
--rw-r--r--   0        0        0     7457 2024-02-27 21:28:34.082311 packyak-0.4.8/packyak/cli/ssh.py
--rw-r--r--   0        0        0     1873 2024-02-26 09:31:52.167807 packyak-0.4.8/packyak/cli/synth.py
--rw-r--r--   0        0        0      451 2024-02-26 09:31:52.167860 packyak-0.4.8/packyak/duration.py
--rw-r--r--   0        0        0      426 2024-02-26 09:31:52.167947 packyak-0.4.8/packyak/resource.py
--rw-r--r--   0        0        0      922 2024-02-26 09:31:52.168012 packyak-0.4.8/packyak/runtime/binding.py
--rw-r--r--   0        0        0     1334 2024-02-26 09:31:52.168077 packyak-0.4.8/packyak/runtime/cluster.py
--rw-r--r--   0        0        0     2365 2024-02-26 09:31:52.168131 packyak-0.4.8/packyak/runtime/function.py
--rw-r--r--   0        0        0      769 2024-02-26 09:31:52.168192 packyak-0.4.8/packyak/runtime/integration.py
--rw-r--r--   0        0        0     1062 2024-02-26 09:31:52.168249 packyak-0.4.8/packyak/runtime/job.py
--rw-r--r--   0        0        0      245 2024-02-26 09:31:52.168300 packyak-0.4.8/packyak/runtime/pool.py
--rw-r--r--   0        0        0     1069 2024-02-26 09:31:52.168357 packyak-0.4.8/packyak/runtime/runnable.py
--rw-r--r--   0        0        0      312 2024-02-26 09:31:52.168424 packyak-0.4.8/packyak/scheduling/cron.py
--rw-r--r--   0        0        0      332 2024-02-26 09:31:52.168477 packyak-0.4.8/packyak/scheduling/every.py
--rw-r--r--   0        0        0     1916 2024-02-26 09:31:52.168604 packyak-0.4.8/packyak/spec.py
--rw-r--r--   0        0        0     8482 2024-02-26 09:31:52.168717 packyak-0.4.8/packyak/storage/bucket.py
--rw-r--r--   0        0        0     2509 2024-02-26 09:31:52.168783 packyak-0.4.8/packyak/storage/folder.py
--rw-r--r--   0        0        0     5991 2024-02-26 09:31:52.168887 packyak-0.4.8/packyak/streaming/queue.py
--rw-r--r--   0        0        0       59 2024-02-26 09:31:52.168944 packyak-0.4.8/packyak/synth/__init__.py
--rw-r--r--   0        0        0     1438 2024-02-02 03:06:06.481825 packyak-0.4.8/packyak/synth/__main__.py
--rw-r--r--   0        0        0     6017 2024-02-26 09:31:52.169098 packyak-0.4.8/packyak/synth/analyze.py
--rw-r--r--   0        0        0      335 2024-02-26 09:31:52.169192 packyak-0.4.8/packyak/synth/call.py
--rw-r--r--   0        0        0      364 2024-02-02 03:06:06.481977 packyak-0.4.8/packyak/synth/file_utils.py
--rw-r--r--   0        0        0      353 2024-02-02 03:06:06.482027 packyak-0.4.8/packyak/synth/loaded_module.py
--rw-r--r--   0        0        0     5710 2024-02-26 09:31:52.169334 packyak-0.4.8/packyak/synth/synth.py
--rw-r--r--   0        0        0      218 2024-02-26 09:31:52.169393 packyak-0.4.8/packyak/util/fqn.py
--rw-r--r--   0        0        0      181 2024-02-26 09:31:52.169454 packyak-0.4.8/packyak/util/git.py
--rw-r--r--   0        0        0      262 2024-02-02 03:06:06.482168 packyak-0.4.8/packyak/util/memoize.py
--rw-r--r--   0        0        0      950 2024-02-07 23:45:47.362506 packyak-0.4.8/packyak/util/typed_resource.py
--rw-r--r--   0        0        0       89 2024-02-26 09:31:52.169543 packyak-0.4.8/packyak/web/streamlit-site.py
--rw-r--r--   0        0        0        0 2024-02-12 19:29:28.647856 packyak-0.4.8/py.typed
--rw-r--r--   0        0        0     1100 2024-02-27 21:32:37.840345 packyak-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6443 1970-01-01 00:00:00.000000 packyak-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     5433 2024-02-23 08:15:58.848693 packyak-0.4.9/README.md
+-rw-r--r--   0        0        0      993 2024-02-26 09:31:52.166939 packyak-0.4.9/packyak/__init__.py
+-rw-r--r--   0        0        0      433 2024-02-12 19:51:41.337451 packyak-0.4.9/packyak/asset/asset.py
+-rw-r--r--   0        0        0       72 2024-02-26 09:31:52.167028 packyak-0.4.9/packyak/asset/manifest.py
+-rw-r--r--   0        0        0     1555 2024-02-26 09:31:52.167119 packyak-0.4.9/packyak/asset/namespace.py
+-rw-r--r--   0        0        0      415 2024-02-10 02:53:25.975611 packyak-0.4.9/packyak/asset/partition_key.py
+-rw-r--r--   0        0        0     1013 2024-02-26 09:31:52.167202 packyak-0.4.9/packyak/asset/source.py
+-rw-r--r--   0        0        0      276 2024-02-26 09:31:52.167305 packyak-0.4.9/packyak/cli/__init__.py
+-rw-r--r--   0        0        0      283 2024-02-26 09:31:52.167394 packyak-0.4.9/packyak/cli/__main__.py
+-rw-r--r--   0        0        0       50 2024-02-22 04:42:16.104618 packyak-0.4.9/packyak/cli/cli.py
+-rw-r--r--   0        0        0      775 2024-02-26 09:31:52.167456 packyak-0.4.9/packyak/cli/materialize.py
+-rw-r--r--   0        0        0      189 2024-02-26 09:31:52.167551 packyak-0.4.9/packyak/cli/new.py
+-rw-r--r--   0        0        0      700 2024-02-26 09:31:52.167609 packyak-0.4.9/packyak/cli/run.py
+-rw-r--r--   0        0        0     8268 2024-02-28 03:33:00.732400 packyak-0.4.9/packyak/cli/ssh.py
+-rw-r--r--   0        0        0     1873 2024-02-26 09:31:52.167807 packyak-0.4.9/packyak/cli/synth.py
+-rw-r--r--   0        0        0      451 2024-02-26 09:31:52.167860 packyak-0.4.9/packyak/duration.py
+-rw-r--r--   0        0        0      426 2024-02-26 09:31:52.167947 packyak-0.4.9/packyak/resource.py
+-rw-r--r--   0        0        0      922 2024-02-26 09:31:52.168012 packyak-0.4.9/packyak/runtime/binding.py
+-rw-r--r--   0        0        0     1334 2024-02-26 09:31:52.168077 packyak-0.4.9/packyak/runtime/cluster.py
+-rw-r--r--   0        0        0     2365 2024-02-26 09:31:52.168131 packyak-0.4.9/packyak/runtime/function.py
+-rw-r--r--   0        0        0      769 2024-02-26 09:31:52.168192 packyak-0.4.9/packyak/runtime/integration.py
+-rw-r--r--   0        0        0     1062 2024-02-26 09:31:52.168249 packyak-0.4.9/packyak/runtime/job.py
+-rw-r--r--   0        0        0      245 2024-02-26 09:31:52.168300 packyak-0.4.9/packyak/runtime/pool.py
+-rw-r--r--   0        0        0     1069 2024-02-26 09:31:52.168357 packyak-0.4.9/packyak/runtime/runnable.py
+-rw-r--r--   0        0        0      312 2024-02-26 09:31:52.168424 packyak-0.4.9/packyak/scheduling/cron.py
+-rw-r--r--   0        0        0      332 2024-02-26 09:31:52.168477 packyak-0.4.9/packyak/scheduling/every.py
+-rw-r--r--   0        0        0     1916 2024-02-26 09:31:52.168604 packyak-0.4.9/packyak/spec.py
+-rw-r--r--   0        0        0     8482 2024-02-26 09:31:52.168717 packyak-0.4.9/packyak/storage/bucket.py
+-rw-r--r--   0        0        0     2509 2024-02-26 09:31:52.168783 packyak-0.4.9/packyak/storage/folder.py
+-rw-r--r--   0        0        0     5991 2024-02-26 09:31:52.168887 packyak-0.4.9/packyak/streaming/queue.py
+-rw-r--r--   0        0        0       59 2024-02-26 09:31:52.168944 packyak-0.4.9/packyak/synth/__init__.py
+-rw-r--r--   0        0        0     1438 2024-02-02 03:06:06.481825 packyak-0.4.9/packyak/synth/__main__.py
+-rw-r--r--   0        0        0     6017 2024-02-26 09:31:52.169098 packyak-0.4.9/packyak/synth/analyze.py
+-rw-r--r--   0        0        0      335 2024-02-26 09:31:52.169192 packyak-0.4.9/packyak/synth/call.py
+-rw-r--r--   0        0        0      364 2024-02-02 03:06:06.481977 packyak-0.4.9/packyak/synth/file_utils.py
+-rw-r--r--   0        0        0      353 2024-02-02 03:06:06.482027 packyak-0.4.9/packyak/synth/loaded_module.py
+-rw-r--r--   0        0        0     5710 2024-02-26 09:31:52.169334 packyak-0.4.9/packyak/synth/synth.py
+-rw-r--r--   0        0        0      218 2024-02-26 09:31:52.169393 packyak-0.4.9/packyak/util/fqn.py
+-rw-r--r--   0        0        0      181 2024-02-26 09:31:52.169454 packyak-0.4.9/packyak/util/git.py
+-rw-r--r--   0        0        0      262 2024-02-02 03:06:06.482168 packyak-0.4.9/packyak/util/memoize.py
+-rw-r--r--   0        0        0      950 2024-02-07 23:45:47.362506 packyak-0.4.9/packyak/util/typed_resource.py
+-rw-r--r--   0        0        0       89 2024-02-26 09:31:52.169543 packyak-0.4.9/packyak/web/streamlit-site.py
+-rw-r--r--   0        0        0        0 2024-02-12 19:29:28.647856 packyak-0.4.9/py.typed
+-rw-r--r--   0        0        0     1126 2024-02-28 03:34:59.819268 packyak-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6447 1970-01-01 00:00:00.000000 packyak-0.4.9/PKG-INFO
```

### Comparing `packyak-0.4.8/README.md` & `packyak-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/__init__.py` & `packyak-0.4.9/packyak/__init__.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/asset/namespace.py` & `packyak-0.4.9/packyak/asset/namespace.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/asset/source.py` & `packyak-0.4.9/packyak/asset/source.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/cli/materialize.py` & `packyak-0.4.9/packyak/cli/materialize.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/cli/run.py` & `packyak-0.4.9/packyak/cli/run.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/cli/ssh.py` & `packyak-0.4.9/packyak/cli/ssh.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from packyak.cli.cli import cli
 
 
 @cli.command()
 @click.argument(
     "instance-id",
     type=str,
-    # prompt="What is the EC2 Instance ID of the instance you wish to tunnel to?",
+    # prompt="What is the ID of the EC2 Instance or EMR Cluster you wish to tunnel to?",
     # help="The EC2 Instance ID of the instance you wish to tunnel to",
 )
 @click.option(
     "--ssh-key",
     default="~/.ssh/id_rsa",
     help="Path to the the SSH public key to copy to the remote host. Default: ~/.ssh/id_rsa.pub",
 )
@@ -52,24 +52,44 @@
 
     -L: Ports to forward. Default: 9001:localhost:22
     """
 
     if profile is not None:
         os.environ["AWS_PROFILE"] = profile
 
+    def log(message: str):
+        if verbose:
+            print(message)
+
+    def resolve_primary_node() -> str:
+        emr = boto3.client("emr")
+
+        for group in emr.list_instance_groups(ClusterId=instance_id)["InstanceGroups"]:
+            if group["InstanceGroupType"] == "MASTER":
+                instances = emr.list_instances(
+                    ClusterId=instance_id, InstanceGroupId=group["Id"]
+                )["Instances"]
+                if len(instances) == 1:
+                    return instances[0]["Ec2InstanceId"]
+
+        raise Exception(f"No primary instance found for EMR cluster {instance_id}")
+
+    if instance_id.startswith("j"):
+        log(
+            f"Instance ID {instance_id} looks like an EMR cluster ID. Resolving the Primary node."
+        )
+        instance_id = resolve_primary_node()
+        log(f"Resolved primary node: {instance_id}")
+
     if user is None:
         sts_client = boto3.client("sts")
         caller_identity = sts_client.get_caller_identity()
         user_id = caller_identity.get("UserId", "")
         user = user_id.split(":")[1] if ":" in user_id else "root"
-    print(f"Logging in as {user}")
-
-    def log(message: str):
-        if verbose:
-            print(message)
+    log(f"Logging in as {user}")
 
     log(f"{time.ctime()} sm-connect-ssh-proxy: Connecting to: {instance_id}")
     # print(f"{time.ctime()} sm-connect-ssh-proxy: Extra args: {extra_ssh_args}")
 
     ssm_client = boto3.client("ssm")
     instance_info = ssm_client.describe_instance_information(
         Filters=[{"Key": "InstanceIds", "Values": [instance_id]}]
```

### Comparing `packyak-0.4.8/packyak/cli/synth.py` & `packyak-0.4.9/packyak/cli/synth.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/binding.py` & `packyak-0.4.9/packyak/runtime/binding.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/cluster.py` & `packyak-0.4.9/packyak/runtime/cluster.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/function.py` & `packyak-0.4.9/packyak/runtime/function.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/integration.py` & `packyak-0.4.9/packyak/runtime/integration.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/job.py` & `packyak-0.4.9/packyak/runtime/job.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/runtime/runnable.py` & `packyak-0.4.9/packyak/runtime/runnable.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/spec.py` & `packyak-0.4.9/packyak/spec.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/storage/bucket.py` & `packyak-0.4.9/packyak/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/storage/folder.py` & `packyak-0.4.9/packyak/storage/folder.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/streaming/queue.py` & `packyak-0.4.9/packyak/streaming/queue.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/synth/__main__.py` & `packyak-0.4.9/packyak/synth/__main__.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/synth/analyze.py` & `packyak-0.4.9/packyak/synth/analyze.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/synth/synth.py` & `packyak-0.4.9/packyak/synth/synth.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/packyak/util/typed_resource.py` & `packyak-0.4.9/packyak/util/typed_resource.py`

 * *Files identical despite different names*

### Comparing `packyak-0.4.8/pyproject.toml` & `packyak-0.4.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "packyak"
-version = "0.4.8"
+version = "0.4.9"
 description = "Infrastructure for AI applications and machine learning pipelines"
 authors = ["sam <sam@eventual.ai>"]
 readme = "README.md"
 include = ["py.typed"]
 
 [tool.poetry.scripts]
 yak = "packyak.cli:cli"
@@ -12,15 +12,20 @@
 
 [tool.poetry.dependencies]
 types-aiobotocore = { extras = ["essential"], version = "^2.9.0" }
 types-boto3 = "^1.0.2"
 aioboto3 = "^12.1.0"
 aiobotocore = { version = "2.8.0", extras = ["boto3"] }
 aws-lambda-typing = "^2.18.0"
-boto3-stubs = { extras = ["essential", "sts", "ssm"], version = "^1.34.15" }
+boto3-stubs = { extras = [
+    "essential",
+    "sts",
+    "ssm",
+    "emr",
+], version = "^1.34.15" }
 pandas = ">2"
 pandera = "*"
 pydantic = "^2.5.3"
 python = "^3.10"
 pandas-stubs = ">2"
 aiofiles = "^23.2.1"
 pyspark = { extras = ["pandas-on-spark"], version = "^3.5.0" }
```

### Comparing `packyak-0.4.8/PKG-INFO` & `packyak-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: packyak
-Version: 0.4.8
+Version: 0.4.9
 Summary: Infrastructure for AI applications and machine learning pipelines
 Author: sam
 Author-email: sam@eventual.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aioboto3 (>=12.1.0,<13.0.0)
 Requires-Dist: aiobotocore[boto3] (==2.8.0)
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aws-lambda-typing (>=2.18.0,<3.0.0)
-Requires-Dist: boto3-stubs[essential,ssm,sts] (>=1.34.15,<2.0.0)
+Requires-Dist: boto3-stubs[emr,essential,ssm,sts] (>=1.34.15,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: pandas (>2)
 Requires-Dist: pandas-stubs (>2)
 Requires-Dist: pandera
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pyspark[pandas-on-spark] (>=3.5.0,<4.0.0)
 Requires-Dist: types-aiobotocore[essential] (>=2.9.0,<3.0.0)
```

