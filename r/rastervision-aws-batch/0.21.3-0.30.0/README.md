# Comparing `tmp/rastervision_aws_batch-0.21.3.tar.gz` & `tmp/rastervision_aws_batch-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_aws_batch-0.21.3.tar", last modified: Tue Oct 17 19:14:41 2023, max compression
+gzip compressed data, was "rastervision_aws_batch-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
```

## Comparing `rastervision_aws_batch-0.21.3.tar` & `rastervision_aws_batch-0.30.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_aws_batch-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      560 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/rastervision/aws_batch/
--rw-rw-r--   0 root         (0) root         (0)      617 2023-08-24 18:41:21.000000 rastervision_aws_batch-0.21.3/rastervision/aws_batch/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5259 2023-09-11 19:40:54.000000 rastervision_aws_batch-0.21.3/rastervision/aws_batch/aws_batch_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)      560 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       59 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:41.000000 rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       59 2023-10-17 13:37:07.000000 rastervision_aws_batch-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:41.523303 rastervision_aws_batch-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1139 2023-10-17 13:37:07.000000 rastervision_aws_batch-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_aws_batch-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.559693 rastervision_aws_batch-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/rastervision/aws_batch/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      592 2024-04-06 20:13:30.000000 rastervision_aws_batch-0.30.0/rastervision/aws_batch/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6121 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/rastervision/aws_batch/aws_batch_runner.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      560 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      389 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       35 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       61 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.563693 rastervision_aws_batch-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1727 2024-04-10 21:55:10.000000 rastervision_aws_batch-0.30.0/setup.py
```

### Comparing `rastervision_aws_batch-0.21.3/PKG-INFO` & `rastervision_aws_batch-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_aws_batch
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds an AWS Batch pipeline runner
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_batch-0.21.3/rastervision/aws_batch/__init__.py` & `rastervision_aws_batch-0.30.0/rastervision/aws_batch/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 
 import rastervision.pipeline
 from rastervision.aws_batch.aws_batch_runner import *
 
 __all__ = [
     'AWS_BATCH',
     AWSBatchRunner.__name__,
-    submit_job.__name__,
 ]
```

### Comparing `rastervision_aws_batch-0.21.3/rastervision/aws_batch/aws_batch_runner.py` & `rastervision_aws_batch-0.30.0/rastervision/aws_batch/aws_batch_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,176 @@
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 import logging
 import os
 import uuid
-from typing import List, Optional
+from pprint import pformat
 
 from rastervision.pipeline import rv_config_ as rv_config
 from rastervision.pipeline.runner import Runner
 
-log = logging.getLogger(__name__)
-AWS_BATCH = 'batch'
-
+if TYPE_CHECKING:
+    from rastervision.pipeline.pipeline import Pipeline
 
-def submit_job(cmd: List[str],
-               job_name: str,
-               debug: bool = False,
-               profile: str = False,
-               attempts: int = 5,
-               parent_job_ids: List[str] = None,
-               num_array_jobs: Optional[int] = None,
-               use_gpu: bool = False,
-               job_queue: Optional[str] = None,
-               job_def: Optional[str] = None) -> str:
-    """Submit a job to run on AWS Batch.
-
-    Args:
-        cmd: a command to run in the Docker container for the remote job
-        debug: if True, run the command using a ptvsd wrapper which sets up a remote
-            VS Code Python debugger server
-        profile: if True, run the command using kernprof, a line profiler
-        attempts: the number of times to try running the command which is useful
-            in case of failure.
-        parent_job_ids: optional list of parent Batch job ids. The job created by this
-            will only run after the parent jobs complete successfully.
-        num_array_jobs: if set, make this a Batch array job with size equal to
-            num_array_jobs
-        use_gpu: if True, run the job in a GPU-enabled queue
-        job_queue: if set, use this job queue
-        job_def: if set, use this job definition
-    """
-    batch_config = rv_config.get_namespace_config(AWS_BATCH)
-
-    if job_queue is None:
-        if use_gpu:
-            job_queue = batch_config('gpu_job_queue')
-        else:
-            job_queue = batch_config('cpu_job_queue')
-
-    if job_def is None:
-        if use_gpu:
-            job_def = batch_config('gpu_job_def')
-        else:
-            job_def = batch_config('cpu_job_def')
-
-    import boto3
-    client = boto3.client('batch')
-
-    cmd_list = cmd.split(' ')
-    if debug:
-        cmd_list = [
-            'python', '-m', 'ptvsd', '--host', '0.0.0.0', '--port', '6006',
-            '--wait', '-m'
-        ] + cmd_list
-
-    if profile:
-        cmd_list = ['kernprof', '-v', '-l'] + cmd_list
-
-    kwargs = {
-        'jobName': job_name,
-        'jobQueue': job_queue,
-        'jobDefinition': job_def,
-        'containerOverrides': {
-            'command': cmd_list
-        },
-        'retryStrategy': {
-            'attempts': attempts
-        },
-    }
-    if parent_job_ids:
-        kwargs['dependsOn'] = [{'jobId': id} for id in parent_job_ids]
-    if num_array_jobs:
-        kwargs['arrayProperties'] = {'size': num_array_jobs}
-
-    job_id = client.submit_job(**kwargs)['jobId']
-    msg = 'submitted job with jobName={} and jobId={} w/ parent(s)={}'.format(
-        job_name, job_id, parent_job_ids)
-    log.info(msg)
-    log.info(cmd_list)
+log = logging.getLogger(__name__)
 
-    return job_id
+AWS_BATCH = 'batch'
 
 
 class AWSBatchRunner(Runner):
     """Runs pipelines remotely using AWS Batch.
 
     Requires Everett configuration of form:
 
-    ```
-    [AWS_BATCH]
-    cpu_job_queue=
-    cpu_job_def=
-    gpu_job_queue=
-    gpu_job_def=
-    attempts=
-    ```
+    .. code-block:: ini
+
+        [AWS_BATCH]
+        cpu_job_queue=
+        cpu_job_def=
+        gpu_job_queue=
+        gpu_job_def=
+        attempts=
     """
 
     def run(self,
-            cfg_json_uri,
-            pipeline,
-            commands,
-            num_splits=1,
-            pipeline_run_name: str = 'raster-vision'):
+            cfg_json_uri: str,
+            pipeline: 'Pipeline',
+            commands: List[str],
+            num_splits: int = 1,
+            pipeline_run_name: str = 'raster-vision'):  # pragma: no cover
         parent_job_ids = []
-
-        # pipeline-specific job queue
-        if hasattr(pipeline, 'job_queue'):
-            pipeline_job_queue = pipeline.job_queue
-        else:
-            pipeline_job_queue = None
-
-        # pipeline-specific job definition
-        if hasattr(pipeline, 'job_def'):
-            pipeline_job_def = pipeline.job_def
-        else:
-            pipeline_job_def = None
-
         for command in commands:
+            cmd, args = self.build_cmd(
+                command,
+                cfg_json_uri,
+                pipeline,
+                num_splits,
+                pipeline_run_name=pipeline_run_name)
+            job_id = self.run_command(
+                cmd, parent_job_ids=parent_job_ids, **args)
+
+            job_info = dict(
+                name=args['job_name'],
+                id=job_id,
+                parents=parent_job_ids,
+                cmd=cmd,
+            )
+            job_info_str = pformat(job_info, sort_dicts=False)
+            msg = (f'Job submitted:\n{job_info_str}')
+            log.info(msg)
 
-            # command-specific job queue, job definition
-            job_def = pipeline_job_def
-            job_queue = pipeline_job_queue
-            if hasattr(pipeline, command):
-                fn = getattr(pipeline, command)
-                if hasattr(fn, 'job_def'):
-                    job_def = fn.job_def
-                if hasattr(fn, 'job_queue'):
-                    job_queue = fn.job_queue
-
-            num_array_jobs = None
-            use_gpu = command in pipeline.gpu_commands
-
-            job_name = f'{pipeline_run_name}-{command}-{uuid.uuid4()}'
-
-            cmd = ['python', '-m', 'rastervision.pipeline.cli']
-            if rv_config.get_verbosity() > 1:
-                cmd.append('-' + 'v' * (rv_config.get_verbosity() - 1))
-            cmd.extend(
-                ['run_command', cfg_json_uri, command, '--runner', AWS_BATCH])
-
-            if command in pipeline.split_commands and num_splits > 1:
-                num_array_jobs = num_splits
-                cmd += ['--num-splits', str(num_splits)]
-            job_id = submit_job(
-                cmd=' '.join(cmd),
-                job_name=job_name,
-                parent_job_ids=parent_job_ids,
-                num_array_jobs=num_array_jobs,
-                use_gpu=use_gpu,
-                job_queue=job_queue,
-                job_def=job_def)
             parent_job_ids = [job_id]
 
-            job_queue = None
-            job_def = None
+    def build_cmd(self,
+                  command: str,
+                  cfg_json_uri: str,
+                  pipeline: 'Pipeline',
+                  num_splits: int = 1,
+                  pipeline_run_name: str = 'raster-vision'
+                  ) -> Tuple[List[str], Dict[str, Any]]:
+
+        verbosity = rv_config.get_verbosity_cli_opt()
+
+        # pipeline-specific job queue and job definition
+        pipeline_job_queue = getattr(pipeline, 'job_queue', None)
+        pipeline_job_def = getattr(pipeline, 'job_def', None)
+
+        # command-specific job queue, job definition
+        cmd_obj = getattr(pipeline, command, None)
+        job_def = getattr(cmd_obj, 'job_def', pipeline_job_def)
+        job_queue = getattr(cmd_obj, 'job_queue', pipeline_job_queue)
+
+        num_array_jobs = None
+        use_gpu = command in pipeline.gpu_commands
+
+        job_name = f'{pipeline_run_name}-{command}-{uuid.uuid4()}'
+
+        cmd = ['python', '-m', 'rastervision.pipeline.cli']
+        if verbosity:
+            cmd += [verbosity]
+        cmd += ['run_command', cfg_json_uri, command, '--runner', AWS_BATCH]
+
+        if command in pipeline.split_commands and num_splits > 1:
+            num_array_jobs = num_splits
+            cmd += ['--num-splits', str(num_splits)]
+
+        args = dict(
+            job_name=job_name,
+            num_array_jobs=num_array_jobs,
+            use_gpu=use_gpu,
+            job_queue=job_queue,
+            job_def=job_def,
+        )
+        return cmd, args
 
-    def get_split_ind(self):
+    def get_split_ind(self) -> int:
         return int(os.environ.get('AWS_BATCH_JOB_ARRAY_INDEX', 0))
+
+    def run_command(self,
+                    cmd: List[str],
+                    job_name: Optional[str] = None,
+                    debug: bool = False,
+                    attempts: int = 1,
+                    parent_job_ids: Optional[List[str]] = None,
+                    num_array_jobs: Optional[int] = None,
+                    use_gpu: bool = False,
+                    job_queue: Optional[str] = None,
+                    job_def: Optional[str] = None,
+                    **kwargs) -> str:  # pragma: no cover
+        """Submit a command as a job to AWS Batch.
+
+        Args:
+            cmd: Command to run in the Docker container for the remote job as
+                list of strings.
+            job_name: Optional job name. If None, is set to
+                "raster-vision-<uuid>".
+            debug: If True, run the command using a ptvsd wrapper which sets up
+                a remote VS Code Python debugger server. Defaults to False.
+            attempts: The number of times to try running the command which is
+                useful in case of failure. Defaults to 5.
+            parent_job_ids: Optional list of parent Batch job IDs. The job
+                created by this will only run after the parent jobs complete
+                successfully. Defaults to None.
+            num_array_jobs: If set, make this a Batch array job with size equal
+                to num_array_jobs. Defaults to None.
+            use_gpu: If True, run the job in a GPU-enabled queue. Defaults to
+                False.
+            job_queue: If set, use this job queue. Default to None.
+            job_def: If set, use this job definition. Default to None.
+            **kwargs: Any other kwargs to pass to Batch when submitting job.
+        """
+        import boto3
+
+        batch_config = rv_config.get_namespace_config(AWS_BATCH)
+        device = 'gpu' if use_gpu else 'cpu'
+
+        if job_name is None:
+            job_name = f'raster-vision-{uuid.uuid4()}'
+        if job_queue is None:
+            job_queue = batch_config(f'{device}_job_queue')
+        if job_def is None:
+            job_def = batch_config(f'{device}_job_def')
+
+        if debug:
+            cmd = [
+                'python', '-m', 'ptvsd', '--host', '0.0.0.0', '--port', '6006',
+                '--wait', '-m'
+            ] + cmd
+
+        args = {
+            'jobName': job_name,
+            'jobQueue': job_queue,
+            'jobDefinition': job_def,
+            'containerOverrides': {
+                'command': cmd
+            },
+            'retryStrategy': {
+                'attempts': attempts
+            },
+        }
+        if parent_job_ids:
+            args['dependsOn'] = [{'jobId': id} for id in parent_job_ids]
+        if num_array_jobs:
+            args['arrayProperties'] = {'size': num_array_jobs}
+
+        client = boto3.client('batch')
+        job_id = client.submit_job(**args, **kwargs)['jobId']
+        return job_id
```

### Comparing `rastervision_aws_batch-0.21.3/rastervision_aws_batch.egg-info/PKG-INFO` & `rastervision_aws_batch-0.30.0/rastervision_aws_batch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-aws-batch
-Version: 0.21.3
+Version: 0.30.0
 Summary: A rastervision plugin that adds an AWS Batch pipeline runner
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_aws_batch-0.21.3/setup.py` & `rastervision_aws_batch-0.30.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 # flake8: noqa
 
-from os import path as op
-import io
-from setuptools import (setup, find_namespace_packages)
-
-here = op.abspath(op.dirname(__file__))
-with io.open(op.join(here, 'requirements.txt'), encoding='utf-8') as f:
-    all_reqs = f.read().split('\n')
-install_requires = [x.strip() for x in all_reqs if 'git+' not in x]
+from os.path import abspath, dirname, join
+from setuptools import setup, find_namespace_packages
+import re
 
 name = 'rastervision_aws_batch'
-version = '0.21.3'
+version = '0.30.0'
 description = 'A rastervision plugin that adds an AWS Batch pipeline runner'
+requirement_constraints = {}
+
+here = abspath(dirname(__file__))
+
+
+def parse_requirements(requirements_path: str) -> list[str]:
+    requirements = []
+    with open(requirements_path, 'r', encoding='utf-8') as f:
+        for line in f:
+            if 'git+' in line:
+                continue
+            # match package name, ignoring version constraints
+            match = re.match(r'^\s*([^\s<=>]+)', line)
+            if not match:
+                continue
+            package_name = match.group(1)
+            if package_name in requirement_constraints:
+                constraint = requirement_constraints[package_name]
+                package_name = f'{package_name}{constraint}'
+            requirements.append(package_name)
+    return requirements
+
 
 setup(
     name=name,
     version=version,
     description=description,
     url='https://github.com/azavea/raster-vision',
     author='Azavea',
@@ -26,9 +43,9 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
     ],
     keywords=
     'raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing',
     packages=find_namespace_packages(exclude=['integration_tests*', 'tests*']),
-    install_requires=install_requires,
+    install_requires=parse_requirements(join(here, 'requirements.txt')),
     zip_safe=False)
```

