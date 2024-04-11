# Comparing `tmp/mypy-boto3-cloudwatch-1.34.75.tar.gz` & `tmp/mypy-boto3-cloudwatch-1.34.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudwatch-1.34.75.tar", last modified: Mon Apr  1 20:08:26 2024, max compression
+gzip compressed data, was "mypy-boto3-cloudwatch-1.34.83.tar", last modified: Thu Apr 11 19:18:06 2024, max compression
```

## Comparing `mypy-boto3-cloudwatch-1.34.75.tar` & `mypy-boto3-cloudwatch-1.34.83.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.245723 mypy-boto3-cloudwatch-1.34.75/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-01 20:08:26.245723 mypy-boto3-cloudwatch-1.34.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.241722 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32815 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32812 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23284 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    23275 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    47901 2024-04-01 20:07:57.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47901 2024-04-01 20:07:56.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.241722 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 20:08:26.000000 mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:08:26.245723 mypy-boto3-cloudwatch-1.34.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-01 20:07:55.000000 mypy-boto3-cloudwatch-1.34.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.363383 mypy-boto3-cloudwatch-1.34.83/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-11 19:18:06.363383 mypy-boto3-cloudwatch-1.34.83/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.363383 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32916 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32913 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23284 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23275 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    48303 2024-04-11 19:17:16.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48303 2024-04-11 19:17:16.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-11 19:17:15.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 19:18:06.363383 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16253 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 19:18:06.000000 mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 19:18:06.363383 mypy-boto3-cloudwatch-1.34.83/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 19:17:14.000000 mypy-boto3-cloudwatch-1.34.83/setup.py
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/LICENSE` & `mypy-boto3-cloudwatch-1.34.83/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/PKG-INFO` & `mypy-boto3-cloudwatch-1.34.83/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.34.75
-Summary: Type annotations for boto3.CloudWatch 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudWatch 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/README.md` & `mypy-boto3-cloudwatch-1.34.83/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__init__.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__init__.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/__main__.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatch 1.34.75\n"
-        "Version:         1.34.75\n"
+        "Type annotations for boto3.CloudWatch 1.34.83\n"
+        "Version:         1.34.83\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.75")
+    print("1.34.83")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/client.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
+    MetricCharacteristicsTypeDef,
     MetricDataQueryTypeDef,
     MetricDatumTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     MetricStreamFilterTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
@@ -472,14 +473,15 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         Configuration: AnomalyDetectorConfigurationTypeDef = ...,
+        MetricCharacteristics: MetricCharacteristicsTypeDef = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
         MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/client.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
+    MetricCharacteristicsTypeDef,
     MetricDataQueryTypeDef,
     MetricDatumTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     MetricStreamFilterTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
@@ -469,14 +470,15 @@
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
         Configuration: AnomalyDetectorConfigurationTypeDef = ...,
+        MetricCharacteristics: MetricCharacteristicsTypeDef = ...,
         SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
         MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/literals.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/literals.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/paginator.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/paginator.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/service_resource.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/service_resource.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/type_defs.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeTypeDef",
     "DimensionTypeDef",
+    "MetricCharacteristicsTypeDef",
     "CloudwatchEventStateTypeDef",
     "CloudwatchEventMetricStatsMetricTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
@@ -198,14 +199,20 @@
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
+MetricCharacteristicsTypeDef = TypedDict(
+    "MetricCharacteristicsTypeDef",
+    {
+        "PeriodicSpikes": NotRequired[bool],
+    },
+)
 CloudwatchEventStateTypeDef = TypedDict(
     "CloudwatchEventStateTypeDef",
     {
         "timestamp": str,
         "value": str,
         "reason": NotRequired[str],
         "reasonData": NotRequired[str],
@@ -1348,14 +1355,15 @@
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
         "StateValue": NotRequired[AnomalyDetectorStateValueType],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorPaginatorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorPaginatorTypeDef],
     },
 )
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
@@ -1386,14 +1394,15 @@
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
         "StateValue": NotRequired[AnomalyDetectorStateValueType],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorTypeDef],
     },
 )
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
@@ -1409,14 +1418,15 @@
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[Sequence[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorTypeDef],
     },
 )
 CloudwatchEventTypeDef = TypedDict(
     "CloudwatchEventTypeDef",
     {
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/type_defs.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AlarmHistoryItemTypeDef",
     "RangeTypeDef",
     "DimensionTypeDef",
+    "MetricCharacteristicsTypeDef",
     "CloudwatchEventStateTypeDef",
     "CloudwatchEventMetricStatsMetricTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
@@ -198,14 +199,20 @@
 DimensionTypeDef = TypedDict(
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
+MetricCharacteristicsTypeDef = TypedDict(
+    "MetricCharacteristicsTypeDef",
+    {
+        "PeriodicSpikes": NotRequired[bool],
+    },
+)
 CloudwatchEventStateTypeDef = TypedDict(
     "CloudwatchEventStateTypeDef",
     {
         "timestamp": str,
         "value": str,
         "reason": NotRequired[str],
         "reasonData": NotRequired[str],
@@ -1348,14 +1355,15 @@
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
         "StateValue": NotRequired[AnomalyDetectorStateValueType],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorPaginatorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorPaginatorTypeDef],
     },
 )
 DescribeAlarmsForMetricOutputTypeDef = TypedDict(
     "DescribeAlarmsForMetricOutputTypeDef",
     {
@@ -1386,14 +1394,15 @@
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[List[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
         "StateValue": NotRequired[AnomalyDetectorStateValueType],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorTypeDef],
     },
 )
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
@@ -1409,14 +1418,15 @@
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": NotRequired[str],
         "MetricName": NotRequired[str],
         "Dimensions": NotRequired[Sequence[DimensionTypeDef]],
         "Stat": NotRequired[str],
         "Configuration": NotRequired[AnomalyDetectorConfigurationTypeDef],
+        "MetricCharacteristics": NotRequired[MetricCharacteristicsTypeDef],
         "SingleMetricAnomalyDetector": NotRequired[SingleMetricAnomalyDetectorTypeDef],
         "MetricMathAnomalyDetector": NotRequired[MetricMathAnomalyDetectorTypeDef],
     },
 )
 CloudwatchEventTypeDef = TypedDict(
     "CloudwatchEventTypeDef",
     {
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/waiter.py` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch/waiter.pyi` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/PKG-INFO` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudwatch
-Version: 1.34.75
-Summary: Type annotations for boto3.CloudWatch 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.83
+Summary: Type annotations for boto3.CloudWatch 1.34.83 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudwatch.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudwatch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudwatch)](https://pepy.tech/project/mypy-boto3-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatch 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
+[boto3.CloudWatch 1.34.83](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudwatch-1.34.75/mypy_boto3_cloudwatch.egg-info/SOURCES.txt` & `mypy-boto3-cloudwatch-1.34.83/mypy_boto3_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudwatch-1.34.75/setup.py` & `mypy-boto3-cloudwatch-1.34.83/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudwatch",
-    version="1.34.75",
+    version="1.34.83",
     packages=["mypy_boto3_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudWatch 1.34.75 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CloudWatch 1.34.83 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

