# Comparing `tmp/s3path-0.5.2.tar.gz` & `tmp/s3path-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3path-0.5.2.tar", last modified: Tue Jan 30 16:43:44 2024, max compression
+gzip compressed data, was "s3path-0.5.3.tar", last modified: Thu Apr 11 08:55:40 2024, max compression
```

## Comparing `s3path-0.5.2.tar` & `s3path-0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:43:44.579953 s3path-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-30 16:43:34.000000 s3path-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-30 16:43:34.000000 s3path-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-01-30 16:43:44.579953 s3path-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-01-30 16:43:34.000000 s3path-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:43:44.575953 s3path-0.5.2/s3path/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-30 16:43:34.000000 s3path-0.5.2/s3path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19411 2024-01-30 16:43:34.000000 s3path-0.5.2/s3path/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29168 2024-01-30 16:43:34.000000 s3path-0.5.2/s3path/current_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-01-30 16:43:34.000000 s3path-0.5.2/s3path/old_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:43:44.579953 s3path-0.5.2/s3path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-01-30 16:43:44.000000 s3path-0.5.2/s3path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-30 16:43:44.000000 s3path-0.5.2/s3path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 16:43:44.000000 s3path-0.5.2/s3path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-30 16:43:44.000000 s3path-0.5.2/s3path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-30 16:43:44.000000 s3path-0.5.2/s3path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-30 16:43:44.579953 s3path-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-01-30 16:43:34.000000 s3path-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 16:43:44.579953 s3path-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-30 16:43:34.000000 s3path-0.5.2/tests/test_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (127)    31127 2024-01-30 16:43:34.000000 s3path-0.5.2/tests/test_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-01-30 16:43:34.000000 s3path-0.5.2/tests/test_pure_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-01-30 16:43:34.000000 s3path-0.5.2/tests/test_s3path_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-11 08:55:32.000000 s3path-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 08:55:32.000000 s3path-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-11 08:55:40.421542 s3path-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 08:55:32.000000 s3path-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/s3path/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28111 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/current_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50156 2024-04-11 08:55:32.000000 s3path-0.5.3/s3path/old_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/s3path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 08:55:40.000000 s3path-0.5.3/s3path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 08:55:40.421542 s3path-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-11 08:55:32.000000 s3path-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:55:40.421542 s3path-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_pure_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-11 08:55:32.000000 s3path-0.5.3/tests/test_s3path_configuration.py
```

### Comparing `s3path-0.5.2/LICENSE` & `s3path-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s3path-0.5.2/PKG-INFO` & `s3path-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.2
+Version: 0.5.3
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.2 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.3 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s3path-0.5.2/README.rst` & `s3path-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `s3path-0.5.2/s3path/__init__.py` & `s3path-0.5.3/s3path/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 s3path provides a Pythonic API to S3 by wrapping boto3 with pathlib interface
 """
 import sys
 
 from . import accessor
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 __all__ = (
     'register_configuration_parameter',
     'StatResult',
     'PureS3Path',
     'S3Path',
     'VersionedS3Path',
     'PureVersionedS3Path',
```

### Comparing `s3path-0.5.2/s3path/accessor.py` & `s3path-0.5.3/s3path/accessor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+import sys
+import importlib.util
 from os import stat_result
 from threading import Lock
 from itertools import chain
 from functools import lru_cache
+from contextlib import suppress
 from collections import namedtuple
 from io import UnsupportedOperation
 
-import boto3
-from boto3.s3.transfer import TransferManager
-from botocore.exceptions import ClientError
-from botocore.docs.docstring import LazyLoadedDocstring
-import smart_open
+
+def _lazy_import_resources(name):
+    spec = importlib.util.find_spec(name)
+    loader = importlib.util.LazyLoader(spec.loader)
+    spec.loader = loader
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[name] = module
+    loader.exec_module(module)
+    return module
+
+
+boto3 = _lazy_import_resources('boto3')
+smart_open = _lazy_import_resources('smart_open')
+# For Development on Cli, or in general application that require fast startup
+# This will lazy load boto3 resources
+# boto3 increase startup time by X10!
 
 
 class StatResult(namedtuple('BaseStatResult', 'size, last_modified, version_id', defaults=(None,))):
     """
     Base of os.stat_result but with boto3 s3 features
     """
 
@@ -79,39 +93,39 @@
 def rename(path, target):
     source_bucket_name = path.bucket
     source_key_name = path.key
     target_bucket_name = target.bucket
     target_key_name = target.key
 
     resource, config = configuration_map.get_configuration(path)
+    allowed_copy_args = boto3.s3.transfer.TransferManager.ALLOWED_COPY_ARGS
 
     if not is_dir(path):
         target_bucket = resource.Bucket(target_bucket_name)
         object_summary = resource.ObjectSummary(source_bucket_name, source_key_name)
         old_source = {'Bucket': object_summary.bucket_name, 'Key': object_summary.key}
         _boto3_method_with_extraargs(
             target_bucket.copy,
             config=config,
             args=(old_source, target_key_name),
-            allowed_extra_args=TransferManager.ALLOWED_COPY_ARGS,
-        )
+            allowed_extra_args=allowed_copy_args)
         _boto3_method_with_parameters(object_summary.delete)
         return
+
     bucket = resource.Bucket(source_bucket_name)
     target_bucket = resource.Bucket(target_bucket_name)
     for object_summary in bucket.objects.filter(Prefix=source_key_name):
         old_source = {'Bucket': object_summary.bucket_name, 'Key': object_summary.key}
         new_key = object_summary.key.replace(source_key_name, target_key_name)
         _, config = configuration_map.get_configuration(type(path)(target_bucket_name, new_key))
         _boto3_method_with_extraargs(
             target_bucket.copy,
             config=config,
             args=(old_source, new_key),
-            allowed_extra_args=TransferManager.ALLOWED_COPY_ARGS,
-        )
+            allowed_extra_args=allowed_copy_args)
         _boto3_method_with_parameters(object_summary.delete)
 
 
 replace = rename
 
 
 def rmdir(path):
@@ -155,20 +169,21 @@
         # See https://stackoverflow.com/questions/26871884
         try:
             _boto3_method_with_parameters(
                 resource.meta.client.head_bucket,
                 kwargs={'Bucket': bucket_name},
                 config=config)
             return True
-        except ClientError as e:
-            error_code = e.response['Error']['Code']
-            if error_code == '404':
-                # Not found
-                return False
-            raise e
+        except Exception as client_error:
+            with suppress(AttributeError, KeyError):
+                error_code = client_error.response['Error']['Code']
+                if error_code == '404':
+                    # Not found
+                    return False
+            raise client_error
 
     bucket = resource.Bucket(bucket_name)
     key_name = str(path.key)
 
     def query_method():
         return _boto3_method_with_parameters(
             bucket.object_versions.filter,
@@ -249,46 +264,42 @@
     with scandir(path) as scandir_iter:
         return [entry.name for entry in scandir_iter]
 
 
 def open(path, *, mode='r', buffering=-1, encoding=None, errors=None, newline=None):
     resource, config = configuration_map.get_configuration(path)
 
-    if smart_open.__version__ < '4.0.0' and mode.startswith('b'):
-        mode = ''.join(reversed(mode))
-    smart_open_kwargs = {
-        'uri': "s3:/" + str(path),
-        'mode': mode,
-        'buffering': buffering,
-        'encoding': encoding,
-        'errors': errors,
-        'newline': newline,
-    }
+    dummy_object = resource.Object('bucket', 'key')
+    get_object_kwargs = _update_kwargs_with_config(
+        dummy_object.meta.client.get_object, config=config)
+    create_multipart_upload_kwargs = _update_kwargs_with_config(
+        dummy_object.meta.client.create_multipart_upload, config=config)
+
+
     transport_params = {'defer_seek': True}
     if _is_versioned_path(path):
         transport_params['version_id'] = path.version_id
-    dummy_object = resource.Object('bucket', 'key')
 
-    if smart_open.__version__ >= '5.1.0':
-        _smart_open_new_version_kwargs(
-            dummy_object,
-            resource,
-            config,
-            transport_params,
-            smart_open_kwargs)
-    else:
-        _smart_open_old_version_kwargs(
-            dummy_object,
-            resource,
-            config,
-            transport_params,
-            smart_open_kwargs)
+    transport_params.update(
+        client=resource.meta.client,
+        client_kwargs={
+            'S3.Client.get_object': get_object_kwargs,
+            'S3.Client.create_multipart_upload': create_multipart_upload_kwargs,
+        },
+    )
 
-    file_object = smart_open.open(**smart_open_kwargs)
-    return file_object
+    return smart_open.open(
+        uri="s3:/" + str(path),
+        mode=mode,
+        buffering=buffering,
+        encoding=encoding,
+        errors=errors,
+        newline=newline,
+        compression='disable',
+        transport_params=transport_params)
 
 
 def get_presigned_url(path, expire_in: int) -> str:
     resource, config = configuration_map.get_configuration(path)
     return _boto3_method_with_parameters(
         resource.meta.client.generate_presigned_url,
         config=config,
@@ -325,88 +336,14 @@
         raise OSError(f'/{bucket_name}/{key_name}')
 
 
 def _is_versioned_path(path):
     return hasattr(path, 'version_id') and bool(path.version_id)
 
 
-def _smart_open_new_version_kwargs(
-        dummy_object,
-        resource,
-        config,
-        transport_params,
-        smart_open_kwargs):
-    """
-    New Smart-Open api
-    Doc: https://github.com/RaRe-Technologies/smart_open/blob/develop/MIGRATING_FROM_OLDER_VERSIONS.rst
-    """
-    get_object_kwargs = _update_kwargs_with_config(
-        dummy_object.meta.client.get_object, config=config)
-    create_multipart_upload_kwargs = _update_kwargs_with_config(
-        dummy_object.meta.client.create_multipart_upload, config=config)
-    transport_params.update(
-        client=resource.meta.client,
-        client_kwargs={
-            'S3.Client.create_multipart_upload': create_multipart_upload_kwargs,
-            'S3.Client.get_object': get_object_kwargs
-        },
-    )
-    smart_open_kwargs.update(
-        compression='disable',
-        transport_params=transport_params,
-    )
-
-
-def _smart_open_old_version_kwargs(
-        dummy_object,
-        resource,
-        config,
-        transport_params,
-        smart_open_kwargs):
-    """
-    Old Smart-Open api
-    <5.0.0
-    """
-    def get_resource_kwargs():
-        # This is a good example of the complicity of boto3 and botocore
-        # resource arguments from the resource object :-/
-        # very annoying...
-
-        try:
-            access_key = resource.meta.client._request_signer._credentials.access_key
-            secret_key = resource.meta.client._request_signer._credentials.secret_key
-            token = resource.meta.client._request_signer._credentials.token
-        except AttributeError:
-            access_key = secret_key = token = None
-        return {
-            'endpoint_url': resource.meta.client.meta._endpoint_url,
-            'config': resource.meta.client._client_config,
-            'region_name': resource.meta.client._client_config.region_name,
-            'use_ssl': resource.meta.client._endpoint.host.startswith('https'),
-            'verify': resource.meta.client._endpoint.http_session._verify,
-            'aws_access_key_id': access_key,
-            'aws_secret_access_key': secret_key,
-            'aws_session_token': token,
-        }
-
-    initiate_multipart_upload_kwargs = _update_kwargs_with_config(
-        dummy_object.initiate_multipart_upload, config=config)
-    object_kwargs = _update_kwargs_with_config(dummy_object.get, config=config)
-    transport_params.update(
-        multipart_upload_kwargs=initiate_multipart_upload_kwargs,
-        object_kwargs=object_kwargs,
-        resource_kwargs=get_resource_kwargs(),
-        session=boto3.DEFAULT_SESSION,
-    )
-    smart_open_kwargs.update(
-        ignore_ext=True,
-        transport_params=transport_params,
-    )
-
-
 def _update_kwargs_with_config(boto3_method, config, kwargs=None):
     kwargs = kwargs or {}
     if config is not None:
         kwargs.update({
             key: value
             for key, value in config.items()
             if key in _get_action_arguments(boto3_method)
@@ -436,18 +373,17 @@
         })
     kwargs["ExtraArgs"] = extra_args
     return boto3_method(*args, **kwargs)
 
 
 @lru_cache()
 def _get_action_arguments(action):
-    if isinstance(action.__doc__, LazyLoadedDocstring):
+    docs = action.__doc__
+    with suppress(AttributeError):
         docs = action.__doc__._generate()
-    else:
-        docs = action.__doc__
     return set(
         line.replace(':param ', '').strip().strip(':')
         for line in docs.splitlines()
         if line.startswith(':param ')
     )
```

### Comparing `s3path-0.5.2/s3path/current_version.py` & `s3path-0.5.3/s3path/current_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 import re
 import sys
+import typing
 import fnmatch
 import posixpath
-from collections import deque
 from datetime import timedelta
 from contextlib import suppress
 from urllib.parse import unquote
 from pathlib import PurePath, Path
 from typing import Union, Literal, Optional
 from io import DEFAULT_BUFFER_SIZE, TextIOWrapper
 
-import smart_open
 from botocore.exceptions import ClientError
-from boto3.resources.factory import ServiceResource
+
+if typing.TYPE_CHECKING:
+    import smart_open
+    from boto3.resources.factory import ServiceResource
+    KeyFileObjectType = Union[TextIOWrapper, smart_open.s3.Reader, smart_open.s3.MultipartWriter]
 
 from . import accessor
 
 
 def register_configuration_parameter(
         path: PureS3Path,
         *,
@@ -428,26 +431,23 @@
         """
         self._absolute_path_validation()
         for name in accessor.listdir(self):
             yield self._make_child_relpath(name)
 
     def open(
             self,
-            mode: Literal["r", "w", "rb", "wb"] = 'r',
+            mode: Literal['r', 'w', 'rb', 'wb'] = 'r',
             buffering: int = DEFAULT_BUFFER_SIZE,
             encoding: Optional[str] = None,
             errors: Optional[str] = None,
-            newline: Optional[str] = None
-    ) -> Union[TextIOWrapper, smart_open.s3.Reader,   smart_open.s3.MultipartWriter]:
+            newline: Optional[str] = None) -> KeyFileObjectType:
         """
         Opens the Bucket key pointed to by the path, returns a Key file object that you can read/write with
         """
         self._absolute_path_validation()
-        if smart_open.__version__ < '4.0.0' and mode.startswith('b'):
-            mode = ''.join(reversed(mode))
         return accessor.open(
             self,
             mode=mode,
             buffering=buffering,
             encoding=encoding,
             errors=errors,
             newline=newline)
@@ -683,15 +683,15 @@
         self._prefix, pattern = self._prefix_splitter(pattern)
         self._full_keys = self._calculate_full_or_just_folder(pattern)
         self._target_level = self._calculate_pattern_level(pattern)
         self.match = self._compile_pattern_parts(self._prefix, pattern, path.bucket)
 
     def select(self):
         for target in self._deep_cached_dir_scan():
-            target = self._path._flavour.sep.join(('', self._path.bucket, target))
+            target = f'{self._path._flavour.sep}{self._path.bucket}{target}'
             if self.match(target):
                 yield type(self._path)(target)
 
     def _prefix_splitter(self, pattern):
         if not _is_wildcard_pattern(pattern):
             if self._path.key:
                 return f'{self._path.key}{self._path._flavour.sep}{pattern}', ''
@@ -726,25 +726,27 @@
         *_, pattern_parts = self._path._parse_path(pattern)
         for part in pattern_parts[:-1]:
             if '*' in part:
                 return True
         return False
 
     def _deep_cached_dir_scan(self):
-        cache = _DeepDirCache()
+        cache = set()
         prefix_sep_count = self._prefix.count(self._path._flavour.sep)
         for key in accessor.iter_keys(self._path, prefix=self._prefix, full_keys=self._full_keys):
             key_sep_count = key.count(self._path._flavour.sep) + 1
             key_parts = key.rsplit(self._path._flavour.sep, maxsplit=key_sep_count - prefix_sep_count)
             target_path_parts = key_parts[:self._target_level]
-            target_path = (self._path._flavour.sep).join(target_path_parts)
-            if cache.in_cache(target_path):
-                continue
-            yield target_path
-            cache.add(target_path_parts)
+            target_path = ''
+            for part in target_path_parts:
+                target_path += f'{self._path._flavour.sep}{part}'
+                if target_path in cache:
+                    continue
+                yield target_path
+                cache.add(target_path)
 
     def _compile_pattern_parts(self, prefix, pattern, bucket):
         pattern = self._path._flavour.sep.join((
             '',
             bucket,
             prefix,
             pattern,
@@ -756,46 +758,8 @@
             if part == self._path._flavour.sep:
                 continue
             if '**' in part:
                 new_regex_pattern += f'{self._path._flavour.sep}*(?s:{part.replace("**", ".*")})'
                 continue
             new_regex_pattern += f'{self._path._flavour.sep}{fnmatch.translate(part)[:-2]}'
         new_regex_pattern += r'/*\Z'
-
         return re.compile(new_regex_pattern).fullmatch
-
-
-class _DeepDirCache:
-    def __init__(self):
-        self._queue = deque()
-        self._tree = {}
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._tree, self._queue})'
-
-    def in_cache(self, target_path: str) -> bool:
-        return target_path in self._queue
-
-    def add(self, directory_parts):
-        tree = self._tree
-        for part in directory_parts:
-            if part in tree:
-                tree = tree[part]
-                continue
-            if tree:
-                deep_count = self._deep_count(tree)
-                tree.clear()
-                for _ in range(deep_count):
-                    with suppress(IndexError):
-                        self._queue.pop()
-            tree[part] = {}
-        directory = '/'.join(directory_parts)
-        self._queue.append(directory)
-
-    def _deep_count(self, tree):
-        count = 0
-        while True:
-            try:
-                tree = next(iter(tree.values()))
-            except StopIteration:
-                return count
-            count += 1
```

### Comparing `s3path-0.5.2/s3path/old_versions.py` & `s3path-0.5.3/s3path/old_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from boto3.resources.factory import ServiceResource
 from botocore.exceptions import ClientError
 from botocore.docs.docstring import LazyLoadedDocstring
 import smart_open
 import smart_open.s3
 
 
-__version__ = '0.5.0'
 __all__ = (
     'register_configuration_parameter',
     'S3Path',
     'VersionedS3Path',
     'PureS3Path',
     'PureVersionedS3Path',
     'StatResult',
@@ -708,15 +707,15 @@
         self._prefix, pattern = self._prefix_splitter(pattern)
         self._full_keys = self._calculate_full_or_just_folder(pattern)
         self._target_level = self._calculate_pattern_level(pattern)
         self.match = self._path._flavour.compile_pattern_parts(self._prefix, pattern, path.bucket)
 
     def select(self):
         for target in self._deep_cached_dir_scan():
-            target = self._path._flavour.sep.join(('', self._path.bucket, target))
+            target = f'{self._path._flavour.sep}{self._path.bucket}{target}'
             if self.match(target):
                 yield type(self._path)(target)
 
     def _prefix_splitter(self, pattern):
         if not _is_wildcard_pattern(pattern):
             if self._path.key:
                 return f'{self._path.key}{self._path._flavour.sep}{pattern}', ''
@@ -751,62 +750,27 @@
         *_, pattern_parts = self._path._flavour.parse_parts((pattern,))
         for part in pattern_parts[:-1]:
             if '*' in part:
                 return True
         return False
 
     def _deep_cached_dir_scan(self):
-        cache = _DeepDirCache()
+        cache = set()
         prefix_sep_count = self._prefix.count(self._path._flavour.sep)
         for key in self._path._accessor.iter_keys(self._path, prefix=self._prefix, full_keys=self._full_keys):
             key_sep_count = key.count(self._path._flavour.sep) + 1
             key_parts = key.rsplit(self._path._flavour.sep, maxsplit=key_sep_count - prefix_sep_count)
             target_path_parts = key_parts[:self._target_level]
-            target_path = (self._path._flavour.sep).join(target_path_parts)
-            if cache.in_cache(target_path):
-                continue
-            yield target_path
-            cache.add(target_path_parts)
-
-
-class _DeepDirCache:
-    def __init__(self):
-        self._queue = deque()
-        self._tree = {}
-
-    def __repr__(self):
-        return f'{type(self).__name__}({self._tree, self._queue})'
-
-    def in_cache(self, target_path: str) -> bool:
-        return target_path in self._queue
-
-    def add(self, directory_parts):
-        tree = self._tree
-        for part in directory_parts:
-            if part in tree:
-                tree = tree[part]
-                continue
-            if tree:
-                deep_count = self._deep_count(tree)
-                tree.clear()
-                for _ in range(deep_count):
-                    with suppress(IndexError):
-                        self._queue.pop()
-            tree[part] = {}
-        directory = '/'.join(directory_parts)
-        self._queue.append(directory)
-
-    def _deep_count(self, tree):
-        count = 0
-        while True:
-            try:
-                tree = next(iter(tree.values()))
-            except StopIteration:
-                return count
-            count += 1
+            target_path = ''
+            for part in target_path_parts:
+                target_path += f'{self._path._flavour.sep}{part}'
+                if target_path in cache:
+                    continue
+                yield target_path
+                cache.add(target_path)
 
 
 _s3_flavour = _S3Flavour()
 _s3_accessor = _S3Accessor()
 _versioned_s3_accessor = _VersionedS3Accessor()
```

### Comparing `s3path-0.5.2/s3path.egg-info/PKG-INFO` & `s3path-0.5.3/s3path.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.2
+Version: 0.5.3
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.2 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.3 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s3path-0.5.2/setup.py` & `s3path-0.5.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 setup(
     name='s3path',
-    version='0.5.2',
+    version='0.5.3',
     url='https://github.com/liormizr/s3path',
     author='Lior Mizrahi',
     author_email='li.mizr@gmail.com',
-    # py_modules=['s3path'],
     packages=['s3path'],
     install_requires=[
         'boto3>=1.16.35',
         'smart-open',
     ],
     license='Apache 2.0',
     long_description=long_description,
```

### Comparing `s3path-0.5.2/tests/test_not_supported.py` & `s3path-0.5.3/tests/test_not_supported.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.2/tests/test_path_operations.py` & `s3path-0.5.3/tests/test_path_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,49 @@
     test_glob(s3_mock)
 
 
 def test_glog_nested_folders_issue_no_115_old_algo(s3_mock, enable_old_glob):
     test_glog_nested_folders_issue_no_115(s3_mock)
 
 
+def test_glob_issue_160(s3_mock):
+    s3 = boto3.resource('s3')
+    s3.create_bucket(Bucket='my-bucket')
+    example_paths = [
+        's3path/output',
+        's3path/1/output',
+        's3path/2/output',
+        's3path/3/output',
+    ]
+    for example_path in example_paths:
+        object_summary = s3.ObjectSummary('my-bucket', f'{example_path}/test.txt')
+        object_summary.put(Body=b'test data')
+
+    path = S3Path.from_uri("s3://my-bucket/s3path")
+    assert set(path.glob('**/output/')) == {
+        S3Path('/my-bucket/s3path/output'),
+        S3Path('/my-bucket/s3path/1/output'),
+        S3Path('/my-bucket/s3path/2/output'),
+        S3Path('/my-bucket/s3path/3/output'),
+    }
+    assert sum(1 for _ in path.glob('**/output/')) == 4
+
+    assert set(path.rglob('output/')) == {
+        S3Path('/my-bucket/s3path/output'),
+        S3Path('/my-bucket/s3path/1/output'),
+        S3Path('/my-bucket/s3path/2/output'),
+        S3Path('/my-bucket/s3path/3/output'),
+    }
+    assert sum(1 for _ in path.rglob('output/')) == 4
+
+
+def test_glob_issue_160_old_algo(s3_mock, enable_old_glob):
+    test_glob_issue_160(s3_mock)
+
+
 def test_rglob(s3_mock):
     s3 = boto3.resource('s3')
     s3.create_bucket(Bucket='test-bucket')
     object_summary = s3.ObjectSummary('test-bucket', 'directory/Test.test')
     object_summary.put(Body=b'test data')
 
     assert list(S3Path('/test-bucket/').rglob('*.test')) == [S3Path('/test-bucket/directory/Test.test')]
```

### Comparing `s3path-0.5.2/tests/test_pure_path_operations.py` & `s3path-0.5.3/tests/test_pure_path_operations.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.2/tests/test_s3path_configuration.py` & `s3path-0.5.3/tests/test_s3path_configuration.py`

 * *Files identical despite different names*

