# Comparing `tmp/mypy-boto3-1.34.82.tar.gz` & `tmp/mypy-boto3-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-1.34.82.tar", last modified: Wed Apr 10 19:19:32 2024, max compression
+gzip compressed data, was "mypy-boto3-1.34.9.tar", last modified: Wed Dec 27 20:32:14 2023, max compression
```

## Comparing `mypy-boto3-1.34.82.tar` & `mypy-boto3-1.34.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:32.449248 mypy-boto3-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 19:19:32.449248 mypy-boto3-1.34.82/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:32.449248 mypy-boto3-1.34.82/mypy_boto3/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/boto3_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/boto3_init_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/boto3_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/boto3_session_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 19:18:53.000000 mypy-boto3-1.34.82/mypy_boto3/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   116049 2024-04-10 19:18:53.000000 mypy-boto3-1.34.82/mypy_boto3/submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/mypy_boto3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:19:32.449248 mypy-boto3-1.34.82/mypy_boto3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-10 19:19:32.000000 mypy-boto3-1.34.82/mypy_boto3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:19:32.449248 mypy-boto3-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-10 19:18:51.000000 mypy-boto3-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.351771 mypy-boto3-1.34.9/mypy_boto3/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_init_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/mypy_boto3/boto3_session_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   114250 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-27 20:31:55.000000 mypy-boto3-1.34.9/mypy_boto3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/mypy_boto3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-27 20:32:14.000000 mypy-boto3-1.34.9/mypy_boto3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 20:32:14.355771 mypy-boto3-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-27 20:31:54.000000 mypy-boto3-1.34.9/setup.py
```

### Comparing `mypy-boto3-1.34.82/LICENSE` & `mypy-boto3-1.34.9/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-1.34.82/PKG-INFO` & `mypy-boto3-1.34.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.82
-Summary: Type annotations for boto3 1.34.82 master module generated with mypy-boto3-builder 7.23.2
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,35 +25,33 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3
-Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3"></a>
 
 # mypy-boto3
 
 [![PyPI - mypy-boto3](https://img.shields.io/pypi/v/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/1.34.82/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.34.82/README.md` & `mypy-boto3-1.34.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/1.34.82/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.34.82/mypy_boto3/boto3_init_stub.py` & `mypy-boto3-1.34.9/mypy_boto3/boto3_init_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.82/mypy_boto3/boto3_session_stub.py` & `mypy-boto3-1.34.9/mypy_boto3/boto3_session_stub.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-1.34.82/mypy_boto3/literals.py` & `mypy-boto3-1.34.9/mypy_boto3/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -50,15 +49,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -76,15 +74,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -97,26 +94,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -177,14 +172,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -358,21 +354,19 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
-    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-1.34.82/mypy_boto3/main.py` & `mypy-boto3-1.34.9/mypy_boto3/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,20 +114,18 @@
             "mypy-boto3",
         ]
         for submodule in SUBMODULES:
             if submodule.is_installed:
                 package_names.append(submodule.pypi_name)
 
         logger.info(
-            (
-                "You can now uninstall boto3-stubs with:\n\n"
-                "    python -m pip uninstall %s\n\n"
-                "If you want to use auto-typing for boto3.client/resource functions, run:\n\n"
-                "    mypy_boto3\n"
-            ),
+            "You can now uninstall boto3-stubs with:\n\n"
+            "    python -m pip uninstall %s\n\n"
+            "If you want to use auto-typing for boto3.client/resource functions, run:\n\n"
+            "    mypy_boto3\n",
             " ".join(package_names),
         )
         return
     build_package_methods(logger)
     for submodule in SUBMODULES:
         if not submodule.is_installed:
             submodule_path = ROOT_PATH / submodule.import_name
```

### Comparing `mypy-boto3-1.34.82/mypy_boto3/submodules.py` & `mypy-boto3-1.34.9/mypy_boto3/submodules.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,24 +283,14 @@
         class_name="ARCZonalShift",
         pypi_name="mypy-boto3-arc-zonal-shift",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
-        module_name="mypy_boto3_artifact",
-        import_name="artifact",
-        boto3_name="artifact",
-        class_name="Artifact",
-        pypi_name="mypy-boto3-artifact",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=True,
-    ),
-    Submodule(
         module_name="mypy_boto3_athena",
         import_name="athena",
         boto3_name="athena",
         class_name="Athena",
         pypi_name="mypy-boto3-athena",
         has_resource=False,
         has_waiter=False,
@@ -473,24 +463,14 @@
         class_name="CostExplorer",
         pypi_name="mypy-boto3-ce",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
-        module_name="mypy_boto3_chatbot",
-        import_name="chatbot",
-        boto3_name="chatbot",
-        class_name="Chatbot",
-        pypi_name="mypy-boto3-chatbot",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=False,
-    ),
-    Submodule(
         module_name="mypy_boto3_chime",
         import_name="chime",
         boto3_name="chime",
         class_name="Chime",
         pypi_name="mypy-boto3-chime",
         has_resource=False,
         has_waiter=False,
@@ -733,24 +713,14 @@
         class_name="CodeCommit",
         pypi_name="mypy-boto3-codecommit",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
-        module_name="mypy_boto3_codeconnections",
-        import_name="codeconnections",
-        boto3_name="codeconnections",
-        class_name="CodeConnections",
-        pypi_name="mypy-boto3-codeconnections",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=False,
-    ),
-    Submodule(
         module_name="mypy_boto3_codedeploy",
         import_name="codedeploy",
         boto3_name="codedeploy",
         class_name="CodeDeploy",
         pypi_name="mypy-boto3-codedeploy",
         has_resource=False,
         has_waiter=True,
@@ -943,24 +913,14 @@
         class_name="ConnectParticipant",
         pypi_name="mypy-boto3-connectparticipant",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
-        module_name="mypy_boto3_controlcatalog",
-        import_name="controlcatalog",
-        boto3_name="controlcatalog",
-        class_name="ControlCatalog",
-        pypi_name="mypy-boto3-controlcatalog",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=True,
-    ),
-    Submodule(
         module_name="mypy_boto3_controltower",
         import_name="controltower",
         boto3_name="controltower",
         class_name="ControlTower",
         pypi_name="mypy-boto3-controltower",
         has_resource=False,
         has_waiter=False,
@@ -1053,24 +1013,14 @@
         class_name="DAX",
         pypi_name="mypy-boto3-dax",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
-        module_name="mypy_boto3_deadline",
-        import_name="deadline",
-        boto3_name="deadline",
-        class_name="DeadlineCloud",
-        pypi_name="mypy-boto3-deadline",
-        has_resource=False,
-        has_waiter=True,
-        has_paginator=True,
-    ),
-    Submodule(
         module_name="mypy_boto3_detective",
         import_name="detective",
         boto3_name="detective",
         class_name="Detective",
         pypi_name="mypy-boto3-detective",
         has_resource=False,
         has_waiter=False,
@@ -1743,14 +1693,24 @@
         class_name="IoTJobsDataPlane",
         pypi_name="mypy-boto3-iot-jobs-data",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
+        module_name="mypy_boto3_iot_roborunner",
+        import_name="iot_roborunner",
+        boto3_name="iot-roborunner",
+        class_name="IoTRoboRunner",
+        pypi_name="mypy-boto3-iot-roborunner",
+        has_resource=False,
+        has_waiter=False,
+        has_paginator=True,
+    ),
+    Submodule(
         module_name="mypy_boto3_iot1click_devices",
         import_name="iot1click_devices",
         boto3_name="iot1click-devices",
         class_name="IoT1ClickDevicesService",
         pypi_name="mypy-boto3-iot1click-devices",
         has_resource=False,
         has_waiter=False,
@@ -3553,24 +3513,14 @@
         class_name="STS",
         pypi_name="mypy-boto3-sts",
         has_resource=False,
         has_waiter=False,
         has_paginator=False,
     ),
     Submodule(
-        module_name="mypy_boto3_supplychain",
-        import_name="supplychain",
-        boto3_name="supplychain",
-        class_name="SupplyChain",
-        pypi_name="mypy-boto3-supplychain",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=False,
-    ),
-    Submodule(
         module_name="mypy_boto3_support",
         import_name="support",
         boto3_name="support",
         class_name="Support",
         pypi_name="mypy-boto3-support",
         has_resource=False,
         has_waiter=False,
@@ -3613,24 +3563,14 @@
         class_name="Textract",
         pypi_name="mypy-boto3-textract",
         has_resource=False,
         has_waiter=False,
         has_paginator=True,
     ),
     Submodule(
-        module_name="mypy_boto3_timestream_influxdb",
-        import_name="timestream_influxdb",
-        boto3_name="timestream-influxdb",
-        class_name="TimestreamInfluxDB",
-        pypi_name="mypy-boto3-timestream-influxdb",
-        has_resource=False,
-        has_waiter=False,
-        has_paginator=True,
-    ),
-    Submodule(
         module_name="mypy_boto3_timestream_query",
         import_name="timestream_query",
         boto3_name="timestream-query",
         class_name="TimestreamQuery",
         pypi_name="mypy-boto3-timestream-query",
         has_resource=False,
         has_waiter=False,
```

### Comparing `mypy-boto3-1.34.82/mypy_boto3.egg-info/PKG-INFO` & `mypy-boto3-1.34.9/mypy_boto3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3
-Version: 1.34.82
-Summary: Type annotations for boto3 1.34.82 master module generated with mypy-boto3-builder 7.23.2
+Version: 1.34.9
+Summary: Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -25,35 +25,33 @@
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3
-Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3"></a>
 
 # mypy-boto3
 
 [![PyPI - mypy-boto3](https://img.shields.io/pypi/v/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3.svg?color=blue)](https://pypi.org/project/mypy-boto3)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3)](https://pepy.tech/project/mypy-boto3)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Dynamic
-[boto3 1.34.82](https://boto3.amazonaws.com/v1/documentation/api/1.34.82/index.html)
+[boto3 1.34.9](https://boto3.amazonaws.com/v1/documentation/api/1.34.9/index.html)
 type annotations builder for
 [boto3-stubs](https://pypi.org/project/boto3-stubs/).
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page.
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `mypy-boto3-1.34.82/setup.py` & `mypy-boto3-1.34.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3",
-    version="1.34.82",
+    version="1.34.9",
     packages=[
         "mypy_boto3",
     ],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.34.82 master module generated with mypy-boto3-builder 7.23.2",
+    description=(
+        "Type annotations for boto3 1.34.9 master module generated with mypy-boto3-builder 7.23.0"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -34,15 +36,17 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Stubs Only",
     ],
-    keywords="boto3 type-annotations boto3-stubs mypy mypy-stubs typeshed autocomplete auto-generated",
+    keywords=(
+        "boto3 type-annotations boto3-stubs mypy mypy-stubs typeshed autocomplete auto-generated"
+    ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
```

