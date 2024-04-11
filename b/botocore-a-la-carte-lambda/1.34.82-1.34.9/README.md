# Comparing `tmp/botocore-a-la-carte-lambda-1.34.82.tar.gz` & `tmp/botocore-a-la-carte-lambda-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-lambda-1.34.82.tar", last modified: Thu Apr 11 01:00:59 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-lambda-1.34.9.tar", last modified: Thu Dec 28 01:06:51 2023, max compression
```

## Comparing `botocore-a-la-carte-lambda-1.34.82.tar` & `botocore-a-la-carte-lambda-1.34.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 01:00:58.000000 botocore-a-la-carte-lambda-1.34.82/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.212837 botocore-a-la-carte-lambda-1.34.82/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.212837 botocore-a-la-carte-lambda-1.34.82/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.212837 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2014-11-11/
--rw-r--r--   0 runner    (1001) docker     (127)    17624 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2014-11-11/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    38698 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2014-11-11/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    52811 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   314105 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-11 01:00:33.000000 botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-11 01:00:59.000000 botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-11 01:00:59.000000 botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:59.000000 botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 01:00:59.000000 botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:00:59.216837 botocore-a-la-carte-lambda-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-11 01:00:58.000000 botocore-a-la-carte-lambda-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.870358 botocore-a-la-carte-lambda-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-28 01:06:51.870358 botocore-a-la-carte-lambda-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2014-11-11/
+-rw-r--r--   0 runner    (1001) docker     (127)    17624 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2014-11-11/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38698 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2014-11-11/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    13726 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    52811 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   311019 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2023-12-28 01:06:26.000000 botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:51.866358 botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:51.870358 botocore-a-la-carte-lambda-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-12-28 01:06:51.000000 botocore-a-la-carte-lambda-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-lambda-1.34.82/LICENSE.txt` & `botocore-a-la-carte-lambda-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/PKG-INFO` & `botocore-a-la-carte-lambda-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lambda
-Version: 1.34.82
+Version: 1.34.9
 Summary: lambda data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2014-11-11/endpoint-rule-set-1.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2014-11-11/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2014-11-11/service-2.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2014-11-11/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/examples-1.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/paginators-1.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/service-2.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998916898851355%*

 * *Differences: {"'operations'": "{'InvokeAsync': {'documentation': '<important> <p>For asynchronous function "*

 * *                 'invocation, use <a>Invoke</a>.</p> </important> <p>Invokes a function '*

 * *                 "asynchronously.</p>'}}",*

 * * "'shapes'": "{'AddPermissionRequest': {'members': {'FunctionName': {'documentation': '<p>The name "*

 * *             'of the Lambda function, version, or alias.</p> <p class="title"> <b>Name formats</b> '*

 * *             '</p> <ul> <li> <p> <b>Function name</b> – <code>my-function</code>  […]*

```diff
@@ -1095,15 +1095,15 @@
             "name": "Invoke",
             "output": {
                 "shape": "InvocationResponse"
             }
         },
         "InvokeAsync": {
             "deprecated": true,
-            "documentation": "<important> <p>For asynchronous function invocation, use <a>Invoke</a>.</p> </important> <p>Invokes a function asynchronously.</p> <note> <p>If you do use the InvokeAsync action, note that it doesn't support the use of X-Ray active tracing. Trace ID is not propagated to the function, even if X-Ray active tracing is turned on.</p> </note>",
+            "documentation": "<important> <p>For asynchronous function invocation, use <a>Invoke</a>.</p> </important> <p>Invokes a function asynchronously.</p>",
             "errors": [
                 {
                     "shape": "ServiceException"
                 },
                 {
                     "shape": "ResourceNotFoundException"
                 },
@@ -2280,15 +2280,15 @@
                     "shape": "Action"
                 },
                 "EventSourceToken": {
                     "documentation": "<p>For Alexa Smart Home functions, a token that the invoker must supply.</p>",
                     "shape": "EventSourceToken"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "FunctionUrlAuthType": {
                     "documentation": "<p>The type of authentication that your function URL uses. Set to <code>AWS_IAM</code> if you want to restrict access to authenticated users only. Set to <code>NONE</code> if you want to bypass IAM authentication to create a public endpoint. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/urls-auth.html\">Security and auth model for Lambda function URLs</a>.</p>",
                     "shape": "FunctionUrlAuthType"
@@ -2677,15 +2677,15 @@
         "CreateAliasRequest": {
             "members": {
                 "Description": {
                     "documentation": "<p>A description of the alias.</p>",
                     "shape": "Description"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "FunctionVersion": {
                     "documentation": "<p>The function version that the alias invokes.</p>",
                     "shape": "Version"
@@ -2749,35 +2749,35 @@
                     "shape": "BatchSize"
                 },
                 "BisectBatchOnFunctionError": {
                     "documentation": "<p>(Kinesis and DynamoDB Streams only) If the function returns an error, split the batch in two and retry.</p>",
                     "shape": "BisectBatchOnFunctionError"
                 },
                 "DestinationConfig": {
-                    "documentation": "<p>(Kinesis, DynamoDB Streams, Amazon MSK, and self-managed Kafka only) A configuration object that specifies the destination of an event after Lambda processes it.</p>",
+                    "documentation": "<p>(Kinesis and DynamoDB Streams only) A standard Amazon SQS queue or standard Amazon SNS topic destination for discarded records.</p>",
                     "shape": "DestinationConfig"
                 },
                 "DocumentDBEventSourceConfig": {
                     "documentation": "<p>Specific configuration settings for a DocumentDB event source.</p>",
                     "shape": "DocumentDBEventSourceConfig"
                 },
                 "Enabled": {
                     "documentation": "<p>When true, the event source mapping is active. When false, Lambda pauses polling and invocation.</p> <p>Default: True</p>",
                     "shape": "Enabled"
                 },
                 "EventSourceArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the event source.</p> <ul> <li> <p> <b>Amazon Kinesis</b> \u2013 The ARN of the data stream or a stream consumer.</p> </li> <li> <p> <b>Amazon DynamoDB Streams</b> \u2013 The ARN of the stream.</p> </li> <li> <p> <b>Amazon Simple Queue Service</b> \u2013 The ARN of the queue.</p> </li> <li> <p> <b>Amazon Managed Streaming for Apache Kafka</b> \u2013 The ARN of the cluster or the ARN of the VPC connection (for <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/with-msk.html#msk-multi-vpc\">cross-account event source mappings</a>).</p> </li> <li> <p> <b>Amazon MQ</b> \u2013 The ARN of the broker.</p> </li> <li> <p> <b>Amazon DocumentDB</b> \u2013 The ARN of the DocumentDB change stream.</p> </li> </ul>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the event source.</p> <ul> <li> <p> <b>Amazon Kinesis</b> \u2013 The ARN of the data stream or a stream consumer.</p> </li> <li> <p> <b>Amazon DynamoDB Streams</b> \u2013 The ARN of the stream.</p> </li> <li> <p> <b>Amazon Simple Queue Service</b> \u2013 The ARN of the queue.</p> </li> <li> <p> <b>Amazon Managed Streaming for Apache Kafka</b> \u2013 The ARN of the cluster.</p> </li> <li> <p> <b>Amazon MQ</b> \u2013 The ARN of the broker.</p> </li> <li> <p> <b>Amazon DocumentDB</b> \u2013 The ARN of the DocumentDB change stream.</p> </li> </ul>",
                     "shape": "Arn"
                 },
                 "FilterCriteria": {
                     "documentation": "<p>An object that defines the filter criteria that determine whether Lambda should process an event. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html\">Lambda event filtering</a>.</p>",
                     "shape": "FilterCriteria"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
                     "shape": "FunctionName"
                 },
                 "FunctionResponseTypes": {
                     "documentation": "<p>(Kinesis, DynamoDB Streams, and Amazon SQS) A list of current response type enums applied to the event source mapping.</p>",
                     "shape": "FunctionResponseTypeList"
                 },
                 "MaximumBatchingWindowInSeconds": {
@@ -2861,31 +2861,31 @@
                     "shape": "Description"
                 },
                 "Environment": {
                     "documentation": "<p>Environment variables that are accessible from function code during execution.</p>",
                     "shape": "Environment"
                 },
                 "EphemeralStorage": {
-                    "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-function-common.html#configuration-ephemeral-storage\">Configuring ephemeral storage (console)</a>.</p>",
+                    "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB.</p>",
                     "shape": "EphemeralStorage"
                 },
                 "FileSystemConfigs": {
                     "documentation": "<p>Connection settings for an Amazon EFS file system.</p>",
                     "shape": "FileSystemConfigList"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "shape": "FunctionName"
                 },
                 "Handler": {
                     "documentation": "<p>The name of the method within your code that Lambda calls to run your function. Handler is required if the deployment package is a .zip file archive. The format includes the file name. It can also include namespaces and other qualifiers, depending on the runtime. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/foundation-progmodel.html\">Lambda programming model</a>.</p>",
                     "shape": "Handler"
                 },
                 "ImageConfig": {
-                    "documentation": "<p>Container image <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/images-create.html#images-parms\">configuration values</a> that override the values in the container image Dockerfile.</p>",
+                    "documentation": "<p>Container image <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-images.html#configuration-images-settings\">configuration values</a> that override the values in the container image Dockerfile.</p>",
                     "shape": "ImageConfig"
                 },
                 "KMSKeyArn": {
                     "documentation": "<p>The ARN of the Key Management Service (KMS) customer managed key that's used to encrypt your function's <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html#configuration-envvars-encryption\">environment variables</a>. When <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/snapstart-security.html\">Lambda SnapStart</a> is activated, Lambda also uses this key is to encrypt your function's snapshot. If you deploy your function using a container image, Lambda also uses this key to encrypt your function when it's deployed. Note that this is not the same key that's used to protect your container image in the Amazon Elastic Container Registry (Amazon ECR). If you don't provide a customer managed key, Lambda uses a default service key.</p>",
                     "shape": "KMSKeyArn"
                 },
                 "Layers": {
@@ -2951,15 +2951,15 @@
                     "shape": "FunctionUrlAuthType"
                 },
                 "Cors": {
                     "documentation": "<p>The <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS\">cross-origin resource sharing (CORS)</a> settings for your function URL.</p>",
                     "shape": "Cors"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "InvokeMode": {
                     "documentation": "<p>Use one of the following options:</p> <ul> <li> <p> <code>BUFFERED</code> \u2013 This is the default option. Lambda invokes your function using the <code>Invoke</code> API operation. Invocation results are available when the payload is complete. The maximum payload size is 6 MB.</p> </li> <li> <p> <code>RESPONSE_STREAM</code> \u2013 Your function streams payload results as they become available. Lambda invokes your function using the <code>InvokeWithResponseStream</code> API operation. The maximum response payload size is 20 MB, however, you can <a href=\"https://docs.aws.amazon.com/servicequotas/latest/userguide/request-quota-increase.html\">request a quota increase</a>.</p> </li> </ul>",
                     "shape": "InvokeMode"
@@ -3030,15 +3030,15 @@
                 }
             },
             "type": "structure"
         },
         "DeleteAliasRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Name": {
                     "documentation": "<p>The name of the alias.</p>",
                     "location": "uri",
@@ -3083,43 +3083,43 @@
                 "UUID"
             ],
             "type": "structure"
         },
         "DeleteFunctionCodeSigningConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "FunctionName"
             ],
             "type": "structure"
         },
         "DeleteFunctionConcurrencyRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "FunctionName"
             ],
             "type": "structure"
         },
         "DeleteFunctionEventInvokeConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>A version number or alias name.</p>",
                     "location": "querystring",
@@ -3131,15 +3131,15 @@
                 "FunctionName"
             ],
             "type": "structure"
         },
         "DeleteFunctionRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function or version.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:1</code> (with version).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function or version.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:1</code> (with version).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version to delete. You can't delete a version that an alias references.</p>",
                     "location": "querystring",
@@ -3151,15 +3151,15 @@
                 "FunctionName"
             ],
             "type": "structure"
         },
         "DeleteFunctionUrlConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>The alias name.</p>",
                     "location": "querystring",
@@ -3192,15 +3192,15 @@
                 "VersionNumber"
             ],
             "type": "structure"
         },
         "DeleteProvisionedConcurrencyConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>The version number or alias name.</p>",
                     "location": "querystring",
@@ -3476,15 +3476,15 @@
             "sensitive": true,
             "type": "map",
             "value": {
                 "shape": "EnvironmentVariableValue"
             }
         },
         "EphemeralStorage": {
-            "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-function-common.html#configuration-ephemeral-storage\">Configuring ephemeral storage (console)</a>.</p>",
+            "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but it can be any whole number between 512 and 10,240 MB.</p>",
             "members": {
                 "Size": {
                     "documentation": "<p>The size of the function's <code>/tmp</code> directory.</p>",
                     "shape": "EphemeralStorageSize"
                 }
             },
             "required": [
@@ -3509,15 +3509,15 @@
                     "shape": "BatchSize"
                 },
                 "BisectBatchOnFunctionError": {
                     "documentation": "<p>(Kinesis and DynamoDB Streams only) If the function returns an error, split the batch in two and retry. The default value is false.</p>",
                     "shape": "BisectBatchOnFunctionError"
                 },
                 "DestinationConfig": {
-                    "documentation": "<p>(Kinesis, DynamoDB Streams, Amazon MSK, and self-managed Apache Kafka event sources only) A configuration object that specifies the destination of an event after Lambda processes it.</p>",
+                    "documentation": "<p>(Kinesis and DynamoDB Streams only) An Amazon SQS queue or Amazon SNS topic destination for discarded records.</p>",
                     "shape": "DestinationConfig"
                 },
                 "DocumentDBEventSourceConfig": {
                     "documentation": "<p>Specific configuration settings for a DocumentDB event source.</p>",
                     "shape": "DocumentDBEventSourceConfig"
                 },
                 "EventSourceArn": {
@@ -3776,15 +3776,15 @@
                     "shape": "Description"
                 },
                 "Environment": {
                     "documentation": "<p>The function's <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html\">environment variables</a>. Omitted from CloudTrail logs.</p>",
                     "shape": "EnvironmentResponse"
                 },
                 "EphemeralStorage": {
-                    "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-function-common.html#configuration-ephemeral-storage\">Configuring ephemeral storage (console)</a>.</p>",
+                    "documentation": "<p>The size of the function\u2019s <code>/tmp</code> directory in MB. The default value is 512, but it can be any whole number between 512 and 10,240 MB.</p>",
                     "shape": "EphemeralStorage"
                 },
                 "FileSystemConfigs": {
                     "documentation": "<p>Connection settings for an <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-filesystem.html\">Amazon EFS file system</a>.</p>",
                     "shape": "FileSystemConfigList"
                 },
                 "FunctionArn": {
@@ -4046,15 +4046,15 @@
                 }
             },
             "type": "structure"
         },
         "GetAliasRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Name": {
                     "documentation": "<p>The name of the alias.</p>",
                     "location": "uri",
@@ -4107,15 +4107,15 @@
                 "UUID"
             ],
             "type": "structure"
         },
         "GetFunctionCodeSigningConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "FunctionName"
@@ -4125,28 +4125,28 @@
         "GetFunctionCodeSigningConfigResponse": {
             "members": {
                 "CodeSigningConfigArn": {
                     "documentation": "<p>The The Amazon Resource Name (ARN) of the code signing configuration.</p>",
                     "shape": "CodeSigningConfigArn"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "CodeSigningConfigArn",
                 "FunctionName"
             ],
             "type": "structure"
         },
         "GetFunctionConcurrencyRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "FunctionName"
@@ -4161,15 +4161,15 @@
                 }
             },
             "type": "structure"
         },
         "GetFunctionConfigurationRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version or alias to get details about a published version of the function.</p>",
                     "location": "querystring",
@@ -4181,15 +4181,15 @@
                 "FunctionName"
             ],
             "type": "structure"
         },
         "GetFunctionEventInvokeConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>A version number or alias name.</p>",
                     "location": "querystring",
@@ -4201,15 +4201,15 @@
                 "FunctionName"
             ],
             "type": "structure"
         },
         "GetFunctionRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version or alias to get details about a published version of the function.</p>",
                     "location": "querystring",
@@ -4242,15 +4242,15 @@
                 }
             },
             "type": "structure"
         },
         "GetFunctionUrlConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>The alias name.</p>",
                     "location": "querystring",
@@ -4412,15 +4412,15 @@
                 }
             },
             "type": "structure"
         },
         "GetPolicyRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version or alias to get the policy for that resource.</p>",
                     "location": "querystring",
@@ -4445,15 +4445,15 @@
                 }
             },
             "type": "structure"
         },
         "GetProvisionedConcurrencyConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>The version number or alias name.</p>",
                     "location": "querystring",
@@ -4495,15 +4495,15 @@
                 }
             },
             "type": "structure"
         },
         "GetRuntimeManagementConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version of the function. This can be <code>$LATEST</code> or a published version number. If no value is specified, the configuration for the <code>$LATEST</code> version is returned.</p>",
                     "location": "querystring",
@@ -4717,21 +4717,21 @@
                 }
             },
             "type": "structure"
         },
         "InvocationRequest": {
             "members": {
                 "ClientContext": {
-                    "documentation": "<p>Up to 3,583 bytes of base64-encoded data about the invoking client to pass to the function in the context object. Lambda passes the <code>ClientContext</code> object to your function for synchronous invocations only.</p>",
+                    "documentation": "<p>Up to 3,583 bytes of base64-encoded data about the invoking client to pass to the function in the context object.</p>",
                     "location": "header",
                     "locationName": "X-Amz-Client-Context",
                     "shape": "String"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "InvocationType": {
                     "documentation": "<p>Choose from the following options.</p> <ul> <li> <p> <code>RequestResponse</code> (default) \u2013 Invoke the function synchronously. Keep the connection open until the function returns a response or times out. The API response includes the function response and additional data.</p> </li> <li> <p> <code>Event</code> \u2013 Invoke the function asynchronously. Send events that fail multiple times to the function's dead-letter queue (if one is configured). The API response only includes a status code.</p> </li> <li> <p> <code>DryRun</code> \u2013 Validate parameter values and verify that the user or role has permission to invoke the function.</p> </li> </ul>",
                     "location": "header",
@@ -4802,15 +4802,15 @@
             ],
             "type": "string"
         },
         "InvokeAsyncRequest": {
             "deprecated": true,
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "InvokeArgs": {
                     "documentation": "<p>The JSON that you want to provide to your Lambda function as input.</p>",
                     "shape": "BlobStream"
@@ -4878,15 +4878,15 @@
                 "ClientContext": {
                     "documentation": "<p>Up to 3,583 bytes of base64-encoded data about the invoking client to pass to the function in the context object.</p>",
                     "location": "header",
                     "locationName": "X-Amz-Client-Context",
                     "shape": "String"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "InvocationType": {
                     "documentation": "<p>Use one of the following options:</p> <ul> <li> <p> <code>RequestResponse</code> (default) \u2013 Invoke the function synchronously. Keep the connection open until the function returns a response or times out. The API operation response includes the function response and additional data.</p> </li> <li> <p> <code>DryRun</code> \u2013 Validate parameter values and verify that the IAM user or role has permission to invoke the function.</p> </li> </ul>",
                     "location": "header",
@@ -5242,15 +5242,15 @@
         "LicenseInfo": {
             "max": 512,
             "type": "string"
         },
         "ListAliasesRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "FunctionVersion": {
                     "documentation": "<p>Specify a function version to only list aliases that invoke that version.</p>",
                     "location": "querystring",
@@ -5317,21 +5317,21 @@
                 }
             },
             "type": "structure"
         },
         "ListEventSourceMappingsRequest": {
             "members": {
                 "EventSourceArn": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the event source.</p> <ul> <li> <p> <b>Amazon Kinesis</b> \u2013 The ARN of the data stream or a stream consumer.</p> </li> <li> <p> <b>Amazon DynamoDB Streams</b> \u2013 The ARN of the stream.</p> </li> <li> <p> <b>Amazon Simple Queue Service</b> \u2013 The ARN of the queue.</p> </li> <li> <p> <b>Amazon Managed Streaming for Apache Kafka</b> \u2013 The ARN of the cluster or the ARN of the VPC connection (for <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/with-msk.html#msk-multi-vpc\">cross-account event source mappings</a>).</p> </li> <li> <p> <b>Amazon MQ</b> \u2013 The ARN of the broker.</p> </li> <li> <p> <b>Amazon DocumentDB</b> \u2013 The ARN of the DocumentDB change stream.</p> </li> </ul>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the event source.</p> <ul> <li> <p> <b>Amazon Kinesis</b> \u2013 The ARN of the data stream or a stream consumer.</p> </li> <li> <p> <b>Amazon DynamoDB Streams</b> \u2013 The ARN of the stream.</p> </li> <li> <p> <b>Amazon Simple Queue Service</b> \u2013 The ARN of the queue.</p> </li> <li> <p> <b>Amazon Managed Streaming for Apache Kafka</b> \u2013 The ARN of the cluster.</p> </li> <li> <p> <b>Amazon MQ</b> \u2013 The ARN of the broker.</p> </li> <li> <p> <b>Amazon DocumentDB</b> \u2013 The ARN of the DocumentDB change stream.</p> </li> </ul>",
                     "location": "querystring",
                     "locationName": "EventSourceArn",
                     "shape": "Arn"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
                     "location": "querystring",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Marker": {
                     "documentation": "<p>A pagination token returned by a previous call.</p>",
                     "location": "querystring",
@@ -5359,15 +5359,15 @@
                 }
             },
             "type": "structure"
         },
         "ListFunctionEventInvokeConfigsRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Marker": {
                     "documentation": "<p>Specify the pagination token that's returned by a previous request to retrieve the next page of results.</p>",
                     "location": "querystring",
@@ -5398,15 +5398,15 @@
                 }
             },
             "type": "structure"
         },
         "ListFunctionUrlConfigsRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Marker": {
                     "documentation": "<p>Specify the pagination token that's returned by a previous request to retrieve the next page of results.</p>",
                     "location": "querystring",
@@ -5528,15 +5528,15 @@
                 "CompatibleArchitecture": {
                     "documentation": "<p>The compatible <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/foundation-arch.html\">instruction set architecture</a>.</p>",
                     "location": "querystring",
                     "locationName": "CompatibleArchitecture",
                     "shape": "Architecture"
                 },
                 "CompatibleRuntime": {
-                    "documentation": "<p>A runtime identifier. For example, <code>java21</code>.</p> <p>The following list includes deprecated runtimes. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy\">Runtime deprecation policy</a>.</p>",
+                    "documentation": "<p>A runtime identifier. For example, <code>go1.x</code>.</p> <p>The following list includes deprecated runtimes. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy\">Runtime deprecation policy</a>.</p>",
                     "location": "querystring",
                     "locationName": "CompatibleRuntime",
                     "shape": "Runtime"
                 },
                 "LayerName": {
                     "documentation": "<p>The name or Amazon Resource Name (ARN) of the layer.</p>",
                     "location": "uri",
@@ -5579,15 +5579,15 @@
                 "CompatibleArchitecture": {
                     "documentation": "<p>The compatible <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/foundation-arch.html\">instruction set architecture</a>.</p>",
                     "location": "querystring",
                     "locationName": "CompatibleArchitecture",
                     "shape": "Architecture"
                 },
                 "CompatibleRuntime": {
-                    "documentation": "<p>A runtime identifier. For example, <code>java21</code>.</p> <p>The following list includes deprecated runtimes. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy\">Runtime deprecation policy</a>.</p>",
+                    "documentation": "<p>A runtime identifier. For example, <code>go1.x</code>.</p> <p>The following list includes deprecated runtimes. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html#runtime-support-policy\">Runtime deprecation policy</a>.</p>",
                     "location": "querystring",
                     "locationName": "CompatibleRuntime",
                     "shape": "Runtime"
                 },
                 "Marker": {
                     "documentation": "<p>A pagination token returned by a previous call.</p>",
                     "location": "querystring",
@@ -5615,15 +5615,15 @@
                 }
             },
             "type": "structure"
         },
         "ListProvisionedConcurrencyConfigsRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Marker": {
                     "documentation": "<p>Specify the pagination token that's returned by a previous request to retrieve the next page of results.</p>",
                     "location": "querystring",
@@ -5677,15 +5677,15 @@
                 }
             },
             "type": "structure"
         },
         "ListVersionsByFunctionRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "NamespacedFunctionName"
                 },
                 "Marker": {
                     "documentation": "<p>Specify the pagination token that's returned by a previous request to retrieve the next page of results.</p>",
                     "location": "querystring",
@@ -5742,27 +5742,27 @@
             ],
             "type": "string"
         },
         "LoggingConfig": {
             "documentation": "<p>The function's Amazon CloudWatch Logs configuration settings.</p>",
             "members": {
                 "ApplicationLogLevel": {
-                    "documentation": "<p>Set this property to filter the application logs for your function that Lambda sends to CloudWatch. Lambda only sends application logs at the selected level of detail and lower, where <code>TRACE</code> is the highest level and <code>FATAL</code> is the lowest.</p>",
+                    "documentation": "<p>Set this property to filter the application logs for your function that Lambda sends to CloudWatch. Lambda only sends application logs at the selected level and lower.</p>",
                     "shape": "ApplicationLogLevel"
                 },
                 "LogFormat": {
                     "documentation": "<p>The format in which Lambda sends your function's application and system logs to CloudWatch. Select between plain text and structured JSON.</p>",
                     "shape": "LogFormat"
                 },
                 "LogGroup": {
                     "documentation": "<p>The name of the Amazon CloudWatch log group the function sends logs to. By default, Lambda functions send logs to a default log group named <code>/aws/lambda/&lt;function name&gt;</code>. To use a different log group, enter an existing log group or enter a new log group name.</p>",
                     "shape": "LogGroup"
                 },
                 "SystemLogLevel": {
-                    "documentation": "<p>Set this property to filter the system logs for your function that Lambda sends to CloudWatch. Lambda only sends system logs at the selected level of detail and lower, where <code>DEBUG</code> is the highest level and <code>WARN</code> is the lowest.</p>",
+                    "documentation": "<p>Set this property to filter the system logs for your function that Lambda sends to CloudWatch. Lambda only sends system logs at the selected level and lower.</p>",
                     "shape": "SystemLogLevel"
                 }
             },
             "type": "structure"
         },
         "Long": {
             "type": "long"
@@ -5864,15 +5864,15 @@
         "NullableBoolean": {
             "type": "boolean"
         },
         "OnFailure": {
             "documentation": "<p>A destination for events that failed processing.</p>",
             "members": {
                 "Destination": {
-                    "documentation": "<p>The Amazon Resource Name (ARN) of the destination resource.</p> <p>To retain records of <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html#invocation-async-destinations\">asynchronous invocations</a>, you can configure an Amazon SNS topic, Amazon SQS queue, Lambda function, or Amazon EventBridge event bus as the destination.</p> <p>To retain records of failed invocations from <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventsourcemapping.html#event-source-mapping-destinations\">Kinesis and DynamoDB event sources</a>, you can configure an Amazon SNS topic or Amazon SQS queue as the destination.</p> <p>To retain records of failed invocations from <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/with-kafka.html#services-smaa-onfailure-destination\">self-managed Kafka</a> or <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/with-msk.html#services-msk-onfailure-destination\">Amazon MSK</a>, you can configure an Amazon SNS topic, Amazon SQS queue, or Amazon S3 bucket as the destination.</p>",
+                    "documentation": "<p>The Amazon Resource Name (ARN) of the destination resource.</p>",
                     "shape": "DestinationArn"
                 }
             },
             "type": "structure"
         },
         "OnSuccess": {
             "documentation": "<p>A destination for events that were processed successfully.</p>",
@@ -6108,15 +6108,15 @@
                     "shape": "String"
                 },
                 "Description": {
                     "documentation": "<p>A description for the version to override the description in the function configuration.</p>",
                     "shape": "Description"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "RevisionId": {
                     "documentation": "<p>Only update the function if the revision ID matches the ID that's specified. Use this option to avoid publishing a version if the function configuration has changed since you last updated it.</p>",
                     "shape": "String"
@@ -6130,15 +6130,15 @@
         "PutFunctionCodeSigningConfigRequest": {
             "members": {
                 "CodeSigningConfigArn": {
                     "documentation": "<p>The The Amazon Resource Name (ARN) of the code signing configuration.</p>",
                     "shape": "CodeSigningConfigArn"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "CodeSigningConfigArn",
@@ -6149,28 +6149,28 @@
         "PutFunctionCodeSigningConfigResponse": {
             "members": {
                 "CodeSigningConfigArn": {
                     "documentation": "<p>The The Amazon Resource Name (ARN) of the code signing configuration.</p>",
                     "shape": "CodeSigningConfigArn"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "shape": "FunctionName"
                 }
             },
             "required": [
                 "CodeSigningConfigArn",
                 "FunctionName"
             ],
             "type": "structure"
         },
         "PutFunctionConcurrencyRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "ReservedConcurrentExecutions": {
                     "documentation": "<p>The number of simultaneous executions to reserve for the function.</p>",
                     "shape": "ReservedConcurrentExecutions"
@@ -6185,15 +6185,15 @@
         "PutFunctionEventInvokeConfigRequest": {
             "members": {
                 "DestinationConfig": {
                     "documentation": "<p>A destination for events after they have been sent to a function for processing.</p> <p class=\"title\"> <b>Destinations</b> </p> <ul> <li> <p> <b>Function</b> - The Amazon Resource Name (ARN) of a Lambda function.</p> </li> <li> <p> <b>Queue</b> - The ARN of a standard SQS queue.</p> </li> <li> <p> <b>Topic</b> - The ARN of a standard SNS topic.</p> </li> <li> <p> <b>Event Bus</b> - The ARN of an Amazon EventBridge event bus.</p> </li> </ul>",
                     "shape": "DestinationConfig"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "MaximumEventAgeInSeconds": {
                     "documentation": "<p>The maximum age of a request that Lambda sends to a function for processing.</p>",
                     "shape": "MaximumEventAgeInSeconds"
@@ -6213,15 +6213,15 @@
                 "FunctionName"
             ],
             "type": "structure"
         },
         "PutProvisionedConcurrencyConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "ProvisionedConcurrentExecutions": {
                     "documentation": "<p>The amount of provisioned concurrency to allocate for the version or alias.</p>",
                     "shape": "PositiveInteger"
@@ -6268,15 +6268,15 @@
                 }
             },
             "type": "structure"
         },
         "PutRuntimeManagementConfigRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version of the function. This can be <code>$LATEST</code> or a published version number. If no value is specified, the configuration for the <code>$LATEST</code> version is returned.</p>",
                     "location": "querystring",
@@ -6390,15 +6390,15 @@
                 "StatementId"
             ],
             "type": "structure"
         },
         "RemovePermissionRequest": {
             "members": {
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Qualifier": {
                     "documentation": "<p>Specify a version or alias to remove permissions from a published version of the function.</p>",
                     "location": "querystring",
@@ -6546,26 +6546,24 @@
                 "python3.8",
                 "python3.9",
                 "dotnetcore1.0",
                 "dotnetcore2.0",
                 "dotnetcore2.1",
                 "dotnetcore3.1",
                 "dotnet6",
-                "dotnet8",
                 "nodejs4.3-edge",
                 "go1.x",
                 "ruby2.5",
                 "ruby2.7",
                 "provided",
                 "provided.al2",
                 "nodejs18.x",
                 "python3.10",
                 "java17",
                 "ruby3.2",
-                "ruby3.3",
                 "python3.11",
                 "nodejs20.x",
                 "provided.al2023",
                 "python3.12",
                 "java21"
             ],
             "type": "string"
@@ -7084,15 +7082,15 @@
         "UpdateAliasRequest": {
             "members": {
                 "Description": {
                     "documentation": "<p>A description of the alias.</p>",
                     "shape": "Description"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "FunctionVersion": {
                     "documentation": "<p>The function version that the alias invokes.</p>",
                     "shape": "Version"
@@ -7163,15 +7161,15 @@
                     "shape": "BatchSize"
                 },
                 "BisectBatchOnFunctionError": {
                     "documentation": "<p>(Kinesis and DynamoDB Streams only) If the function returns an error, split the batch in two and retry.</p>",
                     "shape": "BisectBatchOnFunctionError"
                 },
                 "DestinationConfig": {
-                    "documentation": "<p>(Kinesis, DynamoDB Streams, Amazon MSK, and self-managed Kafka only) A configuration object that specifies the destination of an event after Lambda processes it.</p>",
+                    "documentation": "<p>(Kinesis and DynamoDB Streams only) A standard Amazon SQS queue or standard Amazon SNS topic destination for discarded records.</p>",
                     "shape": "DestinationConfig"
                 },
                 "DocumentDBEventSourceConfig": {
                     "documentation": "<p>Specific configuration settings for a DocumentDB event source.</p>",
                     "shape": "DocumentDBEventSourceConfig"
                 },
                 "Enabled": {
@@ -7179,15 +7177,15 @@
                     "shape": "Enabled"
                 },
                 "FilterCriteria": {
                     "documentation": "<p>An object that defines the filter criteria that determine whether Lambda should process an event. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html\">Lambda event filtering</a>.</p>",
                     "shape": "FilterCriteria"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>MyFunction</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction</code>.</p> </li> <li> <p> <b>Version or Alias ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:MyFunction:PROD</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:MyFunction</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it's limited to 64 characters in length.</p>",
                     "shape": "FunctionName"
                 },
                 "FunctionResponseTypes": {
                     "documentation": "<p>(Kinesis, DynamoDB Streams, and Amazon SQS) A list of current response type enums applied to the event source mapping.</p>",
                     "shape": "FunctionResponseTypeList"
                 },
                 "MaximumBatchingWindowInSeconds": {
@@ -7237,15 +7235,15 @@
                     "shape": "ArchitecturesList"
                 },
                 "DryRun": {
                     "documentation": "<p>Set to true to validate the request parameters and access permissions without modifying the function code.</p>",
                     "shape": "Boolean"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "ImageUri": {
                     "documentation": "<p>URI of a container image in the Amazon ECR registry. Do not use for a function defined with a .zip file archive.</p>",
                     "shape": "String"
@@ -7291,33 +7289,33 @@
                     "shape": "Description"
                 },
                 "Environment": {
                     "documentation": "<p>Environment variables that are accessible from function code during execution.</p>",
                     "shape": "Environment"
                 },
                 "EphemeralStorage": {
-                    "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-function-common.html#configuration-ephemeral-storage\">Configuring ephemeral storage (console)</a>.</p>",
+                    "documentation": "<p>The size of the function's <code>/tmp</code> directory in MB. The default value is 512, but can be any whole number between 512 and 10,240 MB.</p>",
                     "shape": "EphemeralStorage"
                 },
                 "FileSystemConfigs": {
                     "documentation": "<p>Connection settings for an Amazon EFS file system.</p>",
                     "shape": "FileSystemConfigList"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "Handler": {
                     "documentation": "<p>The name of the method within your code that Lambda calls to run your function. Handler is required if the deployment package is a .zip file archive. The format includes the file name. It can also include namespaces and other qualifiers, depending on the runtime. For more information, see <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/foundation-progmodel.html\">Lambda programming model</a>.</p>",
                     "shape": "Handler"
                 },
                 "ImageConfig": {
-                    "documentation": "<p> <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/images-create.html#images-parms\">Container image configuration values</a> that override the values in the container image Docker file.</p>",
+                    "documentation": "<p> <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/images-parms.html\">Container image configuration values</a> that override the values in the container image Docker file.</p>",
                     "shape": "ImageConfig"
                 },
                 "KMSKeyArn": {
                     "documentation": "<p>The ARN of the Key Management Service (KMS) customer managed key that's used to encrypt your function's <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html#configuration-envvars-encryption\">environment variables</a>. When <a href=\"https://docs.aws.amazon.com/lambda/latest/dg/snapstart-security.html\">Lambda SnapStart</a> is activated, Lambda also uses this key is to encrypt your function's snapshot. If you deploy your function using a container image, Lambda also uses this key to encrypt your function when it's deployed. Note that this is not the same key that's used to protect your container image in the Amazon Elastic Container Registry (Amazon ECR). If you don't provide a customer managed key, Lambda uses a default service key.</p>",
                     "shape": "KMSKeyArn"
                 },
                 "Layers": {
@@ -7369,15 +7367,15 @@
         "UpdateFunctionEventInvokeConfigRequest": {
             "members": {
                 "DestinationConfig": {
                     "documentation": "<p>A destination for events after they have been sent to a function for processing.</p> <p class=\"title\"> <b>Destinations</b> </p> <ul> <li> <p> <b>Function</b> - The Amazon Resource Name (ARN) of a Lambda function.</p> </li> <li> <p> <b>Queue</b> - The ARN of a standard SQS queue.</p> </li> <li> <p> <b>Topic</b> - The ARN of a standard SNS topic.</p> </li> <li> <p> <b>Event Bus</b> - The ARN of an Amazon EventBridge event bus.</p> </li> </ul>",
                     "shape": "DestinationConfig"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function, version, or alias.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> - <code>my-function</code> (name-only), <code>my-function:v1</code> (with alias).</p> </li> <li> <p> <b>Function ARN</b> - <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> - <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>You can append a version number or alias to any of the formats. The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "MaximumEventAgeInSeconds": {
                     "documentation": "<p>The maximum age of a request that Lambda sends to a function for processing.</p>",
                     "shape": "MaximumEventAgeInSeconds"
@@ -7405,15 +7403,15 @@
                     "shape": "FunctionUrlAuthType"
                 },
                 "Cors": {
                     "documentation": "<p>The <a href=\"https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS\">cross-origin resource sharing (CORS)</a> settings for your function URL.</p>",
                     "shape": "Cors"
                 },
                 "FunctionName": {
-                    "documentation": "<p>The name or ARN of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
+                    "documentation": "<p>The name of the Lambda function.</p> <p class=\"title\"> <b>Name formats</b> </p> <ul> <li> <p> <b>Function name</b> \u2013 <code>my-function</code>.</p> </li> <li> <p> <b>Function ARN</b> \u2013 <code>arn:aws:lambda:us-west-2:123456789012:function:my-function</code>.</p> </li> <li> <p> <b>Partial ARN</b> \u2013 <code>123456789012:function:my-function</code>.</p> </li> </ul> <p>The length constraint applies only to the full ARN. If you specify only the function name, it is limited to 64 characters in length.</p>",
                     "location": "uri",
                     "locationName": "FunctionName",
                     "shape": "FunctionName"
                 },
                 "InvokeMode": {
                     "documentation": "<p>Use one of the following options:</p> <ul> <li> <p> <code>BUFFERED</code> \u2013 This is the default option. Lambda invokes your function using the <code>Invoke</code> API operation. Invocation results are available when the payload is complete. The maximum payload size is 6 MB.</p> </li> <li> <p> <code>RESPONSE_STREAM</code> \u2013 Your function streams payload results as they become available. Lambda invokes your function using the <code>InvokeWithResponseStream</code> API operation. The maximum response payload size is 20 MB, however, you can <a href=\"https://docs.aws.amazon.com/servicequotas/latest/userguide/request-quota-increase.html\">request a quota increase</a>.</p> </li> </ul>",
                     "shape": "InvokeMode"
```

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore/data/lambda/2015-03-31/waiters-2.json` & `botocore-a-la-carte-lambda-1.34.9/botocore/data/lambda/2015-03-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/PKG-INFO` & `botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lambda
-Version: 1.34.82
+Version: 1.34.9
 Summary: lambda data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lambda-1.34.82/botocore_a_la_carte_lambda.egg-info/SOURCES.txt` & `botocore-a-la-carte-lambda-1.34.9/botocore_a_la_carte_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lambda-1.34.82/setup.py` & `botocore-a-la-carte-lambda-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-lambda',
-    version="1.34.82",
+    version="1.34.9",
     description='lambda data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/lambda/*/*.json'],
```

