# Comparing `tmp/pulumi_awsx-2.5.0.tar.gz` & `tmp/pulumi_awsx-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_awsx-2.5.0.tar", last modified: Tue Jan 30 19:05:16 2024, max compression
+gzip compressed data, was "pulumi_awsx-2.6.0.tar", last modified: Tue Mar 12 20:41:17 2024, max compression
```

## Comparing `pulumi_awsx-2.5.0.tar` & `pulumi_awsx-2.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.838634 pulumi_awsx-2.5.0/pulumi_awsx/
--rw-------   0 runner    (1001) docker     (127)     2193 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8056 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.842634 pulumi_awsx-2.5.0/pulumi_awsx/awsx/
--rw-------   0 runner    (1001) docker     (127)      223 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)    57488 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/awsx/_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.842634 pulumi_awsx-2.5.0/pulumi_awsx/cloudtrail/
--rw-------   0 runner    (1001) docker     (127)      265 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/cloudtrail/__init__.py
--rw-------   0 runner    (1001) docker     (127)    23412 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/cloudtrail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.842634 pulumi_awsx-2.5.0/pulumi_awsx/ec2/
--rw-------   0 runner    (1001) docker     (127)      388 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1983 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/_enums.py
--rw-------   0 runner    (1001) docker     (127)    34412 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     3839 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     3454 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/get_default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     4520 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/outputs.py
--rw-------   0 runner    (1001) docker     (127)    41223 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ec2/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.842634 pulumi_awsx-2.5.0/pulumi_awsx/ecr/
--rw-------   0 runner    (1001) docker     (127)      336 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecr/__init__.py
--rw-------   0 runner    (1001) docker     (127)      834 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecr/_enums.py
--rw-------   0 runner    (1001) docker     (127)     7578 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecr/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    12285 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecr/image.py
--rw-------   0 runner    (1001) docker     (127)    14431 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecr/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/pulumi_awsx/ecs/
--rw-------   0 runner    (1001) docker     (127)      421 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/__init__.py
--rw-------   0 runner    (1001) docker     (127)      354 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/_enums.py
--rw-------   0 runner    (1001) docker     (127)    86174 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    46322 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/ec2_service.py
--rw-------   0 runner    (1001) docker     (127)    31286 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/ec2_task_definition.py
--rw-------   0 runner    (1001) docker     (127)    45038 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/fargate_service.py
--rw-------   0 runner    (1001) docker     (127)    30189 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/ecs/fargate_task_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/pulumi_awsx/lb/
--rw-------   0 runner    (1001) docker     (127)      384 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/lb/__init__.py
--rw-------   0 runner    (1001) docker     (127)    97738 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/lb/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    43234 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/lb/application_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    40347 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/lb/network_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    11113 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/lb/target_group_attachment.py
--rw-------   0 runner    (1001) docker     (127)     2719 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/provider.py
--rw-------   0 runner    (1001) docker     (127)       41 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pulumi_awsx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-01-30 19:05:16.000000 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-30 19:05:16.000000 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 19:05:16.000000 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-30 19:05:16.000000 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 19:05:16.000000 pulumi_awsx-2.5.0/pulumi_awsx.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      747 2024-01-30 19:05:07.000000 pulumi_awsx-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 19:05:16.846634 pulumi_awsx-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.339311 pulumi_awsx-2.6.0/pulumi_awsx/
+-rw-------   0 runner    (1001) docker     (127)     2193 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     8056 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.339311 pulumi_awsx-2.6.0/pulumi_awsx/awsx/
+-rw-------   0 runner    (1001) docker     (127)      223 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    57488 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/awsx/_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.343311 pulumi_awsx-2.6.0/pulumi_awsx/cloudtrail/
+-rw-------   0 runner    (1001) docker     (127)      265 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/cloudtrail/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    23412 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/cloudtrail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.343311 pulumi_awsx-2.6.0/pulumi_awsx/ec2/
+-rw-------   0 runner    (1001) docker     (127)      388 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1983 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    34412 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     3839 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     3454 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/get_default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     4520 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    41221 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ec2/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.343311 pulumi_awsx-2.6.0/pulumi_awsx/ecr/
+-rw-------   0 runner    (1001) docker     (127)      336 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecr/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      834 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecr/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     7578 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecr/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    13292 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecr/image.py
+-rw-------   0 runner    (1001) docker     (127)    14431 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecr/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/pulumi_awsx/ecs/
+-rw-------   0 runner    (1001) docker     (127)      421 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      354 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    86174 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    46322 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/ec2_service.py
+-rw-------   0 runner    (1001) docker     (127)    31286 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/ec2_task_definition.py
+-rw-------   0 runner    (1001) docker     (127)    45038 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/fargate_service.py
+-rw-------   0 runner    (1001) docker     (127)    30189 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/ecs/fargate_task_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/pulumi_awsx/lb/
+-rw-------   0 runner    (1001) docker     (127)      384 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/lb/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    97738 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/lb/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    43234 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/lb/application_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    40347 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/lb/network_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    11113 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/lb/target_group_attachment.py
+-rw-------   0 runner    (1001) docker     (127)     2719 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/provider.py
+-rw-------   0 runner    (1001) docker     (127)       41 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pulumi_awsx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-03-12 20:41:17.000000 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-03-12 20:41:17.000000 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:41:17.000000 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-12 20:41:17.000000 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 20:41:17.000000 pulumi_awsx-2.6.0/pulumi_awsx.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      747 2024-03-12 20:41:10.000000 pulumi_awsx-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 20:41:17.347311 pulumi_awsx-2.6.0/setup.cfg
```

### Comparing `pulumi_awsx-2.5.0/PKG-INFO` & `pulumi_awsx-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.5.0
+Version: 2.6.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-aws<7.0.0,>=6.0.4
-Requires-Dist: pulumi-docker<5.0.0,>=4.5.0
+Requires-Dist: pulumi-docker<5.0.0,>=4.5.1
 Requires-Dist: semver>=2.8.1
 
 [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
 [![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
 [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
```

### Comparing `pulumi_awsx-2.5.0/README.md` & `pulumi_awsx-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/__init__.py` & `pulumi_awsx-2.6.0/pulumi_awsx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/_utilities.py` & `pulumi_awsx-2.6.0/pulumi_awsx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/awsx/_inputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/awsx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/cloudtrail/trail.py` & `pulumi_awsx-2.6.0/pulumi_awsx/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/_enums.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/_inputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/default_vpc.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/get_default_vpc.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/get_default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/outputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ec2/vpc.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ec2/vpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -404,15 +404,15 @@
 
         ### Explicit CIDR Blocks
 
         If you prefer to do your CIDR block calculations yourself, you can specify a list of CIDR blocks for each subnet spec which it will be allocated for in each availability zone. If using explicit layouts, all subnet specs must be declared with explicit CIDR blocks. Each list of CIDR blocks must have the same length as the number of availability zones for the VPC.
 
         ### Legacy
 
-        The "Legacy" works similarly to the "Auto" strategy except that within each availability zone it allocates the private subnet first, followed by the private subnets, and lastly the isolated subnets. The order of subnet specifications of the same type can be changed, but the ordering of private, public, isolated is not overridable. For more flexibility we recommend moving to the "Auto" strategy. The output property `subnetLayout` shows the configuration required if specifying the "Auto" strategy to maintain the current layout.
+        The "Legacy" works similarly to the "Auto" strategy except that within each availability zone it allocates the private subnet first, followed by the public subnets, and lastly the isolated subnets. The order of subnet specifications of the same type can be changed, but the ordering of private, public, isolated is not overridable. For more flexibility we recommend moving to the "Auto" strategy. The output property `subnetLayout` shows the configuration required if specifying the "Auto" strategy to maintain the current layout.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] assign_generated_ipv6_cidr_block: Requests an Amazon-provided IPv6 CIDR block with a /56 prefix length for the VPC. You cannot specify the range of IP addresses, or the size of the CIDR block. Default is `false`. Conflicts with `ipv6_ipam_pool_id`
         :param int availability_zone_cidr_mask: The netmask for each available zone to be aligned to. This is optional, the default value is inferred based on an even distribution of available space from the VPC's CIDR block after being divided evenly by the number of availability zones.
         :param Sequence[str] availability_zone_names: A list of availability zone names to which the subnets defined in subnetSpecs will be deployed. Optional, defaults to the first 3 AZs in the current region.
         :param str cidr_block: The CIDR block for the VPC. Optional. Defaults to 10.0.0.0/16.
@@ -474,15 +474,15 @@
 
         ### Explicit CIDR Blocks
 
         If you prefer to do your CIDR block calculations yourself, you can specify a list of CIDR blocks for each subnet spec which it will be allocated for in each availability zone. If using explicit layouts, all subnet specs must be declared with explicit CIDR blocks. Each list of CIDR blocks must have the same length as the number of availability zones for the VPC.
 
         ### Legacy
 
-        The "Legacy" works similarly to the "Auto" strategy except that within each availability zone it allocates the private subnet first, followed by the private subnets, and lastly the isolated subnets. The order of subnet specifications of the same type can be changed, but the ordering of private, public, isolated is not overridable. For more flexibility we recommend moving to the "Auto" strategy. The output property `subnetLayout` shows the configuration required if specifying the "Auto" strategy to maintain the current layout.
+        The "Legacy" works similarly to the "Auto" strategy except that within each availability zone it allocates the private subnet first, followed by the public subnets, and lastly the isolated subnets. The order of subnet specifications of the same type can be changed, but the ordering of private, public, isolated is not overridable. For more flexibility we recommend moving to the "Auto" strategy. The output property `subnetLayout` shows the configuration required if specifying the "Auto" strategy to maintain the current layout.
 
         :param str resource_name: The name of the resource.
         :param VpcArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecr/_enums.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecr/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecr/_inputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecr/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecr/image.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecr/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,38 +17,42 @@
     def __init__(__self__, *,
                  repository_url: pulumi.Input[str],
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Image resource.
         :param pulumi.Input[str] repository_url: Url of the repository
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] args: An optional map of named build-time argument variables to set during the Docker build.  This flag allows you to pass built-time variables that can be accessed like environment variables inside the `RUN` instruction.
         :param 'BuilderVersion' builder_version: The version of the Docker builder.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cache_from: Images to consider as cache sources
         :param pulumi.Input[str] context: Path to a directory to use for the Docker build context, usually the directory in which the Dockerfile resides (although dockerfile may be used to choose a custom location independent of this choice). If not specified, the context defaults to the current working directory; if a relative path is used, it is relative to the current working directory that Pulumi is evaluating.
         :param pulumi.Input[str] dockerfile: dockerfile may be used to override the default Dockerfile name and/or location.  By default, it is assumed to be a file named Dockerfile in the root of the build context.
+        :param pulumi.Input[str] image_tag: Custom image tag for the resulting docker image. If omitted a random string will be used
         :param pulumi.Input[str] platform: The architecture of the platform you want to build this image for, e.g. `linux/arm64`.
         :param pulumi.Input[str] target: The target of the dockerfile to build
         """
         pulumi.set(__self__, "repository_url", repository_url)
         if args is not None:
             pulumi.set(__self__, "args", args)
         if builder_version is not None:
             pulumi.set(__self__, "builder_version", builder_version)
         if cache_from is not None:
             pulumi.set(__self__, "cache_from", cache_from)
         if context is not None:
             pulumi.set(__self__, "context", context)
         if dockerfile is not None:
             pulumi.set(__self__, "dockerfile", dockerfile)
+        if image_tag is not None:
+            pulumi.set(__self__, "image_tag", image_tag)
         if platform is not None:
             pulumi.set(__self__, "platform", platform)
         if target is not None:
             pulumi.set(__self__, "target", target)
 
     @property
     @pulumi.getter(name="repositoryUrl")
@@ -119,14 +123,26 @@
         return pulumi.get(self, "dockerfile")
 
     @dockerfile.setter
     def dockerfile(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dockerfile", value)
 
     @property
+    @pulumi.getter(name="imageTag")
+    def image_tag(self) -> Optional[pulumi.Input[str]]:
+        """
+        Custom image tag for the resulting docker image. If omitted a random string will be used
+        """
+        return pulumi.get(self, "image_tag")
+
+    @image_tag.setter
+    def image_tag(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "image_tag", value)
+
+    @property
     @pulumi.getter
     def platform(self) -> Optional[pulumi.Input[str]]:
         """
         The architecture of the platform you want to build this image for, e.g. `linux/arm64`.
         """
         return pulumi.get(self, "platform")
 
@@ -153,28 +169,30 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  repository_url: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Builds a docker image and pushes to the ECR repository
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] args: An optional map of named build-time argument variables to set during the Docker build.  This flag allows you to pass built-time variables that can be accessed like environment variables inside the `RUN` instruction.
         :param 'BuilderVersion' builder_version: The version of the Docker builder.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cache_from: Images to consider as cache sources
         :param pulumi.Input[str] context: Path to a directory to use for the Docker build context, usually the directory in which the Dockerfile resides (although dockerfile may be used to choose a custom location independent of this choice). If not specified, the context defaults to the current working directory; if a relative path is used, it is relative to the current working directory that Pulumi is evaluating.
         :param pulumi.Input[str] dockerfile: dockerfile may be used to override the default Dockerfile name and/or location.  By default, it is assumed to be a file named Dockerfile in the root of the build context.
+        :param pulumi.Input[str] image_tag: Custom image tag for the resulting docker image. If omitted a random string will be used
         :param pulumi.Input[str] platform: The architecture of the platform you want to build this image for, e.g. `linux/arm64`.
         :param pulumi.Input[str] repository_url: Url of the repository
         :param pulumi.Input[str] target: The target of the dockerfile to build
         """
         ...
     @overload
     def __init__(__self__,
@@ -200,14 +218,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  repository_url: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -219,14 +238,15 @@
             __props__ = ImageArgs.__new__(ImageArgs)
 
             __props__.__dict__["args"] = args
             __props__.__dict__["builder_version"] = builder_version
             __props__.__dict__["cache_from"] = cache_from
             __props__.__dict__["context"] = context
             __props__.__dict__["dockerfile"] = dockerfile
+            __props__.__dict__["image_tag"] = image_tag
             __props__.__dict__["platform"] = platform
             if repository_url is None and not opts.urn:
                 raise TypeError("Missing required property 'repository_url'")
             __props__.__dict__["repository_url"] = repository_url
             __props__.__dict__["target"] = target
             __props__.__dict__["image_uri"] = None
         super(Image, __self__).__init__(
```

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecr/repository.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecs/_inputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecs/ec2_service.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecs/ec2_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecs/ec2_task_definition.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecs/ec2_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecs/fargate_service.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecs/fargate_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/ecs/fargate_task_definition.py` & `pulumi_awsx-2.6.0/pulumi_awsx/ecs/fargate_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/lb/_inputs.py` & `pulumi_awsx-2.6.0/pulumi_awsx/lb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/lb/application_load_balancer.py` & `pulumi_awsx-2.6.0/pulumi_awsx/lb/application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/lb/network_load_balancer.py` & `pulumi_awsx-2.6.0/pulumi_awsx/lb/network_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/lb/target_group_attachment.py` & `pulumi_awsx-2.6.0/pulumi_awsx/lb/target_group_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx/provider.py` & `pulumi_awsx-2.6.0/pulumi_awsx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx.egg-info/PKG-INFO` & `pulumi_awsx-2.6.0/pulumi_awsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.5.0
+Version: 2.6.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-aws<7.0.0,>=6.0.4
-Requires-Dist: pulumi-docker<5.0.0,>=4.5.0
+Requires-Dist: pulumi-docker<5.0.0,>=4.5.1
 Requires-Dist: semver>=2.8.1
 
 [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
 [![Python version](https://badge.fury.io/py/pulumi-awsx.svg)](https://pypi.org/project/pulumi-awsx)
 [![NuGet version](https://badge.fury.io/nu/pulumi.awsx.svg)](https://badge.fury.io/nu/pulumi.awsx)
```

### Comparing `pulumi_awsx-2.5.0/pulumi_awsx.egg-info/SOURCES.txt` & `pulumi_awsx-2.6.0/pulumi_awsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.5.0/pyproject.toml` & `pulumi_awsx-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_awsx"
   description = "Pulumi Amazon Web Services (AWS) AWSX Components."
-  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-aws>=6.0.4,<7.0.0", "pulumi-docker>=4.5.0,<5.0.0", "semver>=2.8.1"]
+  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-aws>=6.0.4,<7.0.0", "pulumi-docker>=4.5.1,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "awsx", "kind/component", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.7"
-  version = "2.5.0"
+  version = "2.6.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-awsx"
 
 [build-system]
```

