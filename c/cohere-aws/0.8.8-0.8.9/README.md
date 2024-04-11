# Comparing `tmp/cohere-aws-0.8.8.tar.gz` & `tmp/cohere-aws-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-aws-0.8.8.tar", last modified: Mon Nov 13 18:23:06 2023, max compression
+gzip compressed data, was "cohere-aws-0.8.9.tar", last modified: Mon Nov 13 21:37:30 2023, max compression
```

## Comparing `cohere-aws-0.8.8.tar` & `cohere-aws-0.8.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 leila      (502) staff       (20)        0 2023-11-13 18:23:06.581367 cohere-aws-0.8.8/
--rw-r--r--   0 leila      (502) staff       (20)     1066 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/LICENSE
--rw-r--r--   0 leila      (502) staff       (20)     1520 2023-11-13 18:23:06.581245 cohere-aws-0.8.8/PKG-INFO
--rw-r--r--   0 leila      (502) staff       (20)     1058 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/README.md
-drwxr-xr-x   0 leila      (502) staff       (20)        0 2023-11-13 18:23:06.580336 cohere-aws-0.8.8/cohere_aws/
--rw-r--r--   0 leila      (502) staff       (20)       81 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/cohere_aws/__init__.py
--rw-r--r--   0 leila      (502) staff       (20)     2471 2023-09-28 19:13:26.000000 cohere-aws-0.8.8/cohere_aws/classification.py
--rw-r--r--   0 leila      (502) staff       (20)    24757 2023-11-13 18:22:00.000000 cohere-aws-0.8.8/cohere_aws/client.py
--rw-r--r--   0 leila      (502) staff       (20)      617 2023-09-28 19:13:26.000000 cohere-aws-0.8.8/cohere_aws/embeddings.py
--rw-r--r--   0 leila      (502) staff       (20)      591 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/cohere_aws/error.py
--rw-r--r--   0 leila      (502) staff       (20)     3631 2023-09-28 23:59:27.000000 cohere-aws-0.8.8/cohere_aws/generation.py
--rw-r--r--   0 leila      (502) staff       (20)       76 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/cohere_aws/mode.py
--rw-r--r--   0 leila      (502) staff       (20)     2063 2023-09-28 19:13:26.000000 cohere-aws-0.8.8/cohere_aws/rerank.py
--rw-r--r--   0 leila      (502) staff       (20)      337 2023-09-27 17:07:59.000000 cohere-aws-0.8.8/cohere_aws/response.py
--rw-r--r--   0 leila      (502) staff       (20)      479 2023-09-28 19:13:26.000000 cohere-aws-0.8.8/cohere_aws/summary.py
-drwxr-xr-x   0 leila      (502) staff       (20)        0 2023-11-13 18:23:06.581077 cohere-aws-0.8.8/cohere_aws.egg-info/
--rw-r--r--   0 leila      (502) staff       (20)     1520 2023-11-13 18:23:06.000000 cohere-aws-0.8.8/cohere_aws.egg-info/PKG-INFO
--rw-r--r--   0 leila      (502) staff       (20)      423 2023-11-13 18:23:06.000000 cohere-aws-0.8.8/cohere_aws.egg-info/SOURCES.txt
--rw-r--r--   0 leila      (502) staff       (20)        1 2023-11-13 18:23:06.000000 cohere-aws-0.8.8/cohere_aws.egg-info/dependency_links.txt
--rw-r--r--   0 leila      (502) staff       (20)       25 2023-11-13 18:23:06.000000 cohere-aws-0.8.8/cohere_aws.egg-info/requires.txt
--rw-r--r--   0 leila      (502) staff       (20)       11 2023-11-13 18:23:06.000000 cohere-aws-0.8.8/cohere_aws.egg-info/top_level.txt
--rw-r--r--   0 leila      (502) staff       (20)       38 2023-11-13 18:23:06.581407 cohere-aws-0.8.8/setup.cfg
--rw-r--r--   0 leila      (502) staff       (20)     1532 2023-11-13 18:22:00.000000 cohere-aws-0.8.8/setup.py
+drwxr-xr-x   0 lfayoux    (502) staff       (20)        0 2023-11-13 21:37:30.003064 cohere-aws-0.8.9/
+-rw-r--r--   0 lfayoux    (502) staff       (20)     1066 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/LICENSE
+-rw-r--r--   0 lfayoux    (502) staff       (20)     1520 2023-11-13 21:37:30.002942 cohere-aws-0.8.9/PKG-INFO
+-rw-r--r--   0 lfayoux    (502) staff       (20)     1058 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/README.md
+drwxr-xr-x   0 lfayoux    (502) staff       (20)        0 2023-11-13 21:37:30.001529 cohere-aws-0.8.9/cohere_aws/
+-rw-r--r--   0 lfayoux    (502) staff       (20)       81 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/__init__.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)     2471 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/classification.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)    24764 2023-11-13 21:28:03.000000 cohere-aws-0.8.9/cohere_aws/client.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)      617 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/embeddings.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)      591 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/error.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)     3631 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/generation.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)       76 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/mode.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)     2063 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/rerank.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)      337 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/response.py
+-rw-r--r--   0 lfayoux    (502) staff       (20)      479 2023-10-31 20:48:13.000000 cohere-aws-0.8.9/cohere_aws/summary.py
+drwxr-xr-x   0 lfayoux    (502) staff       (20)        0 2023-11-13 21:37:30.002770 cohere-aws-0.8.9/cohere_aws.egg-info/
+-rw-r--r--   0 lfayoux    (502) staff       (20)     1520 2023-11-13 21:37:29.000000 cohere-aws-0.8.9/cohere_aws.egg-info/PKG-INFO
+-rw-r--r--   0 lfayoux    (502) staff       (20)      423 2023-11-13 21:37:29.000000 cohere-aws-0.8.9/cohere_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 lfayoux    (502) staff       (20)        1 2023-11-13 21:37:29.000000 cohere-aws-0.8.9/cohere_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 lfayoux    (502) staff       (20)       25 2023-11-13 21:37:29.000000 cohere-aws-0.8.9/cohere_aws.egg-info/requires.txt
+-rw-r--r--   0 lfayoux    (502) staff       (20)       11 2023-11-13 21:37:29.000000 cohere-aws-0.8.9/cohere_aws.egg-info/top_level.txt
+-rw-r--r--   0 lfayoux    (502) staff       (20)       38 2023-11-13 21:37:30.003099 cohere-aws-0.8.9/setup.cfg
+-rw-r--r--   0 lfayoux    (502) staff       (20)     1532 2023-11-13 21:28:11.000000 cohere-aws-0.8.9/setup.py
```

### Comparing `cohere-aws-0.8.8/LICENSE` & `cohere-aws-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/PKG-INFO` & `cohere-aws-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-aws
-Version: 0.8.8
+Version: 0.8.9
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker & Bedrock
 Home-page: https://github.com/cohere-ai/cohere-aws
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-aws-0.8.8/README.md` & `cohere-aws-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws/classification.py` & `cohere-aws-0.8.9/cohere_aws/classification.py`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws/client.py` & `cohere-aws-0.8.9/cohere_aws/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,19 +312,14 @@
         self,
         texts: List[str],
         truncate: Optional[str] = None,
         variant: Optional[str] = None,
         input_type: Optional[str] = None,
         model_id: Optional[str] = None,
     ) -> Embeddings:
-
-        if self._endpoint_name is None:
-            raise CohereError("No endpoint connected. "
-                              "Run connect_to_endpoint() first.")
-
         json_params = {
             'texts': texts,
             'truncate': truncate,
             "input_type": input_type
         }
         for key, value in list(json_params.items()):
             if value is None:
@@ -334,14 +329,18 @@
             return self._sagemaker_embed(json_params, variant)
         elif self.mode == Mode.BEDROCK:
             return self._bedrock_embed(json_params, model_id)
         else:
             raise CohereError("Unsupported mode")
 
     def _sagemaker_embed(self, json_params: Dict[str, Any], variant: str):
+        if self._endpoint_name is None:
+            raise CohereError("No endpoint connected. "
+                              "Run connect_to_endpoint() first.")
+        
         json_body = json.dumps(json_params)
         params = {
             'EndpointName': self._endpoint_name,
             'ContentType': 'application/json',
             'Body': json_body,
         }
         if variant:
```

### Comparing `cohere-aws-0.8.8/cohere_aws/embeddings.py` & `cohere-aws-0.8.9/cohere_aws/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws/error.py` & `cohere-aws-0.8.9/cohere_aws/error.py`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws/generation.py` & `cohere-aws-0.8.9/cohere_aws/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws/rerank.py` & `cohere-aws-0.8.9/cohere_aws/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-aws-0.8.8/cohere_aws.egg-info/PKG-INFO` & `cohere-aws-0.8.9/cohere_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere-aws
-Version: 0.8.8
+Version: 0.8.9
 Summary: A Python library for the Cohere endpoints in AWS Sagemaker & Bedrock
 Home-page: https://github.com/cohere-ai/cohere-aws
 Author: Cohere
 Author-email: support@cohere.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cohere-aws-0.8.8/setup.py` & `cohere-aws-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 
 setuptools.setup(name='cohere-aws',
-                 version='0.8.8',
+                 version='0.8.9',
                  author='Cohere',
                  author_email='support@cohere.ai',
                  description='A Python library for the Cohere endpoints in AWS Sagemaker & Bedrock',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://github.com/cohere-ai/cohere-aws',
                  packages=setuptools.find_packages(),
```

