# Comparing `tmp/aws-parallelcluster-node-3.9.0.tar.gz` & `tmp/aws-parallelcluster-node-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-node-3.9.0.tar", last modified: Tue Mar 12 01:16:08 2024, max compression
+gzip compressed data, was "aws-parallelcluster-node-3.9.1.tar", last modified: Thu Apr 11 10:38:24 2024, max compression
```

## Comparing `aws-parallelcluster-node-3.9.0.tar` & `aws-parallelcluster-node-3.9.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.724695 aws-parallelcluster-node-3.9.0/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11358 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/LICENSE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      102 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/NOTICE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2024-03-12 01:16:08.724695 aws-parallelcluster-node-3.9.0/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      748 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/README.md
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2024-03-12 01:16:08.724695 aws-parallelcluster-node-3.9.0/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2346 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.716695 aws-parallelcluster-node-3.9.0/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.720695 aws-parallelcluster-node-3.9.0/src/aws/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/aws/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6042 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/aws/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3435 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/aws/ec2.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.720695 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1486 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      257 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       30 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       24 2024-03-12 01:16:08.000000 aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.720695 aws-parallelcluster-node-3.9.0/src/common/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1675 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/ec2_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.720695 aws-parallelcluster-node-3.9.0/src/common/schedulers/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/schedulers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18850 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/schedulers/slurm_commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11268 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/schedulers/slurm_reservation_commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      831 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/time_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15164 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/common/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.724695 aws-parallelcluster-node-3.9.0/src/slurm_plugin/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19666 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/capacity_block_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    31761 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/cluster_event_publisher.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    68278 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/clustermgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5841 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9891 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/computemgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4232 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/console_logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20271 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/fleet_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6753 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51778 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/instance_manager.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:16:08.724695 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1117 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      343 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      382 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      724 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      369 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12965 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/resume.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    33965 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/slurm_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3707 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/suspend.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3302 2024-03-11 21:02:56.000000 aws-parallelcluster-node-3.9.0/src/slurm_plugin/task_executor.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.739313 aws-parallelcluster-node-3.9.1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11358 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/LICENSE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      102 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/NOTICE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2024-04-11 10:38:24.739313 aws-parallelcluster-node-3.9.1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      748 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/README.md
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2024-04-11 10:38:24.739313 aws-parallelcluster-node-3.9.1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2346 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.731313 aws-parallelcluster-node-3.9.1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.731313 aws-parallelcluster-node-3.9.1/src/aws/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/aws/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6042 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/aws/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3435 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/aws/ec2.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.731313 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      732 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1486 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      257 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       30 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       24 2024-04-11 10:38:24.000000 aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.731313 aws-parallelcluster-node-3.9.1/src/common/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1675 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/ec2_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.735313 aws-parallelcluster-node-3.9.1/src/common/schedulers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/schedulers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18850 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/schedulers/slurm_commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11268 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/schedulers/slurm_reservation_commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      831 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/time_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15164 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/common/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.735313 aws-parallelcluster-node-3.9.1/src/slurm_plugin/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19666 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/capacity_block_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    31761 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/cluster_event_publisher.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    68278 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/clustermgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5841 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9891 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/computemgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4232 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/console_logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20271 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/fleet_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6753 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51778 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/instance_manager.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:24.735313 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1117 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      343 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      382 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      724 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      369 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12965 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/resume.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    33965 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/slurm_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3707 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/suspend.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3302 2024-04-11 06:43:49.000000 aws-parallelcluster-node-3.9.1/src/slurm_plugin/task_executor.py
```

### Comparing `aws-parallelcluster-node-3.9.0/LICENSE.txt` & `aws-parallelcluster-node-3.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/PKG-INFO` & `aws-parallelcluster-node-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.9.0
+Version: 3.9.1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.9.0/README.md` & `aws-parallelcluster-node-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/setup.py` & `aws-parallelcluster-node-3.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 console_scripts = [
     "slurm_resume = slurm_plugin.resume:main",
     "slurm_suspend = slurm_plugin.suspend:main",
     "slurm_fleet_status_manager = slurm_plugin.fleet_status_manager:main",
     "clustermgtd = slurm_plugin.clustermgtd:main",
     "computemgtd = slurm_plugin.computemgtd:main",
 ]
-version = "3.9.0"
+version = "3.9.1"
 requires = ["boto3>=1.7.55", "retrying>=1.3.3"]
 
 setup(
     name="aws-parallelcluster-node",
     version=version,
     author="Amazon Web Services",
     description="aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.",
```

### Comparing `aws-parallelcluster-node-3.9.0/src/aws/__init__.py` & `aws-parallelcluster-node-3.9.1/src/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/aws/common.py` & `aws-parallelcluster-node-3.9.1/src/aws/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/aws/ec2.py` & `aws-parallelcluster-node-3.9.1/src/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/PKG-INFO` & `aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.9.0
+Version: 3.9.1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.9.0/src/aws_parallelcluster_node.egg-info/SOURCES.txt` & `aws-parallelcluster-node-3.9.1/src/aws_parallelcluster_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/__init__.py` & `aws-parallelcluster-node-3.9.1/src/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/ec2_utils.py` & `aws-parallelcluster-node-3.9.1/src/common/ec2_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/schedulers/__init__.py` & `aws-parallelcluster-node-3.9.1/src/common/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/schedulers/slurm_commands.py` & `aws-parallelcluster-node-3.9.1/src/common/schedulers/slurm_commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/schedulers/slurm_reservation_commands.py` & `aws-parallelcluster-node-3.9.1/src/common/schedulers/slurm_reservation_commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/time_utils.py` & `aws-parallelcluster-node-3.9.1/src/common/time_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/common/utils.py` & `aws-parallelcluster-node-3.9.1/src/common/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/__init__.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/capacity_block_manager.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/capacity_block_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/cluster_event_publisher.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/cluster_event_publisher.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/clustermgtd.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/clustermgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/common.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/computemgtd.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/computemgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/console_logger.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/console_logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/fleet_manager.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/fleet_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/fleet_status_manager.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/fleet_status_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/instance_manager.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/instance_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/logging/parallelcluster_resume_logging.conf` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/resume.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/resume.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/slurm_resources.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/slurm_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/suspend.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/suspend.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.9.0/src/slurm_plugin/task_executor.py` & `aws-parallelcluster-node-3.9.1/src/slurm_plugin/task_executor.py`

 * *Files identical despite different names*

