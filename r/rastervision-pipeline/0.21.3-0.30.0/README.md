# Comparing `tmp/rastervision_pipeline-0.21.3.tar.gz` & `tmp/rastervision_pipeline-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_pipeline-0.21.3.tar", last modified: Tue Oct 17 19:14:41 2023, max compression
+gzip compressed data, was "rastervision_pipeline-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
```

## Comparing `rastervision_pipeline-0.21.3.tar` & `rastervision_pipeline-0.30.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      577 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.255295 rastervision_pipeline-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.255295 rastervision_pipeline-0.21.3/rastervision/pipeline/
--rw-rw-r--   0 root         (0) root         (0)     1657 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8435 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/cli.py
--rw-rw-r--   0 root         (0) root         (0)    11120 2023-09-26 14:00:58.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/
--rw-rw-r--   0 root         (0) root         (0)      360 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4908 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/file_system.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/http_file_system.py
--rw-rw-r--   0 root         (0) root         (0)     4777 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/local_file_system.py
--rw-rw-r--   0 root         (0) root         (0)    11240 2023-10-12 15:13:45.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/utils.py
--rw-rw-r--   0 root         (0) root         (0)     1850 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     1794 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/pipeline_config.py
--rw-rw-r--   0 root         (0) root         (0)     9242 2023-09-26 14:00:58.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/rastervision/pipeline/runner/
--rw-rw-r--   0 root         (0) root         (0)      274 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/runner/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      755 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/runner/inprocess_runner.py
--rw-rw-r--   0 root         (0) root         (0)     2944 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/runner/local_runner.py
--rw-rw-r--   0 root         (0) root         (0)     1432 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/runner/runner.py
--rw-rw-r--   0 root         (0) root         (0)    10109 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/rv_config.py
--rw-rw-r--   0 root         (0) root         (0)     1254 2023-09-26 14:00:58.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/utils.py
--rw-rw-r--   0 root         (0) root         (0)      351 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/verbosity.py
--rw-rw-r--   0 root         (0) root         (0)       45 2023-10-17 13:37:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/
--rw-rw-r--   0 root         (0) root         (0)      951 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      833 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/config1.py
--rw-rw-r--   0 root         (0) root         (0)      440 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/config2.py
--rw-rw-r--   0 root         (0) root         (0)     2764 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/sample_pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     2252 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/sample_pipeline2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/
--rw-rw-r--   0 root         (0) root         (0)      894 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      523 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/config3.py
--rw-rw-r--   0 root         (0) root         (0)      779 2023-08-22 15:58:07.000000 rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/deluxe_message_maker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/
--rw-r--r--   0 root         (0) root         (0)      577 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1536 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:41.000000 rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      115 2023-08-24 18:41:21.000000 rastervision_pipeline-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:41.259295 rastervision_pipeline-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1267 2023-10-17 13:37:07.000000 rastervision_pipeline-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1657 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8465 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/cli.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13496 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      360 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4721 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4452 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/http_file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4777 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/local_file_system.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11469 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1850 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1794 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9604 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/registry.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      274 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      927 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/inprocess_runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4145 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/local_runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1580 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/runner/runner.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11204 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/rv_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1643 2024-04-06 20:13:30.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/utils.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      351 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/verbosity.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       45 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/rastervision/pipeline/version.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      951 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      833 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config1.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      440 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config2.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2764 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2252 2024-04-07 00:38:15.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline2.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      894 2023-08-24 18:41:21.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      523 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/config3.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      779 2023-08-22 15:58:07.000000 rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/deluxe_message_maker.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      577 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1536 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       65 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       56 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      108 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.335694 rastervision_pipeline-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1878 2024-04-10 21:55:10.000000 rastervision_pipeline-0.30.0/setup.py
```

### Comparing `rastervision_pipeline-0.21.3/PKG-INFO` & `rastervision_pipeline-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision_pipeline
-Version: 0.21.3
+Version: 0.30.0
 Summary: The main rastervision package for configuring, defining, and running pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/__init__.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/cli.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,26 +65,24 @@
         cfg_module = importlib.import_module(cfg_module_path)
 
     _get_config = getattr(cfg_module, 'get_config', None)
     _get_configs = _get_config
     if _get_config is None:
         _get_configs = getattr(cfg_module, 'get_configs', None)
     if _get_configs is None:
-        raise Exception(
-            'There must be a get_config or get_configs function in {}.'.format(
-                cfg_module_path))
+        raise Exception('There must be a get_config or get_configs function '
+                        f'in {cfg_module_path}.')
     cfgs = _get_configs(runner, **args)
     if not isinstance(cfgs, list):
         cfgs = [cfgs]
 
     for cfg in cfgs:
         if not issubclass(type(cfg), PipelineConfig):
-            raise Exception(
-                ('All objects returned by get_configs in {} must be '
-                 'PipelineConfigs.').format(cfg_module_path))
+            raise Exception('All objects returned by get_configs in '
+                            f'{cfg_module_path} must be PipelineConfigs.')
     return cfgs
 
 
 @click.group()
 @click.pass_context
 @click.option(
     '--profile', '-p', help='Sets the configuration profile name to use.')
@@ -118,14 +116,16 @@
     build_config(cfg.dict())
     cfg_json_uri = cfg.get_config_uri()
     save_pipeline_config(cfg, cfg_json_uri)
     pipeline = cfg.build(tmp_dir)
     if not commands:
         commands = pipeline.commands
 
+    click.secho(f'Stages to run: {commands}', fg='white', bold=True)
+
     runner.run(
         cfg_json_uri,
         pipeline,
         commands,
         num_splits=splits,
         pipeline_run_name=pipeline_run_name)
 
@@ -204,20 +204,19 @@
     if num_splits is not None and split_ind is None and runner is not None:
         runner = registry.get_runner(runner)()
         split_ind = runner.get_split_ind()
 
     command_fn = getattr(pipeline, command)
 
     if num_splits is not None and num_splits > 1:
-        msg = 'Running {} command split {}/{}...'.format(
-            command, split_ind + 1, num_splits)
+        msg = f'Running {command} command split {split_ind + 1}/{num_splits}...'
         click.secho(msg, fg='green', bold=True)
         command_fn(split_ind=split_ind, num_splits=num_splits)
     else:
-        msg = 'Running {} command...'.format(command)
+        msg = f'Running {command} command...'
         click.secho(msg, fg='green', bold=True)
         command_fn()
 
 
 @main.command(
     'run_command', short_help='Run an individual command within a pipeline.')
 @click.argument('cfg_json_uri')
@@ -237,15 +236,15 @@
         cfg_json_uri,
         command,
         split_ind=split_ind,
         num_splits=num_splits,
         runner=runner)
 
 
-def _main():
+def _main():  # pragma: no cover
     for pc in registry.get_plugin_commands():
         main.add_command(pc)
     main()
 
 
 if __name__ == '__main__':
     _main()
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/config.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import List, Type, Union, Optional, Callable, Dict, TYPE_CHECKING
+from typing import (TYPE_CHECKING, Callable, Dict, List, Literal, Optional,
+                    Type, Union)
 import inspect
 import logging
+import json
 
 from pydantic import (  # noqa
     BaseModel, create_model, Field, root_validator, validate_model,
     ValidationError, validator)
 
-from typing_extensions import Literal
-
 from rastervision.pipeline import (registry_ as registry, rv_config_ as
                                    rv_config)
-from rastervision.pipeline.file_system import str_to_file
+from rastervision.pipeline.file_system import (str_to_file, json_to_file,
+                                               file_to_json)
 
 if TYPE_CHECKING:
+    from typing import Self
     from rastervision.pipeline.pipeline_config import PipelineConfig
 
 log = logging.getLogger(__name__)
 
 
 class ConfigError(ValueError):
     """Exception raised for invalid configuration."""
-    pass
 
 
 class Config(BaseModel):
     """Base class that can be extended to provide custom configurations.
 
     This adds some extra methods to Pydantic BaseModel.
     See https://pydantic-docs.helpmanual.io/
@@ -46,31 +47,28 @@
     def update(self, *args, **kwargs):
         """Update any fields before validation.
 
         Subclasses should override this to provide complex default behavior, for
         example, setting default values as a function of the values of other
         fields. The arguments to this method will vary depending on the type of Config.
         """
-        pass
 
     def build(self):
         """Build an instance of the corresponding type of object using this config.
 
         For example, BackendConfig will build a Backend object. The arguments to this
         method will vary depending on the type of Config.
         """
-        pass
 
     def validate_config(self):
         """Validate fields that should be checked after update is called.
 
         This is to complement the builtin validation that Pydantic performs at the time
         of object construction.
         """
-        pass
 
     def revalidate(self):
         """Re-validate an instantiated Config.
 
         Runs all Pydantic validators plus self.validate_config().
 
         Adapted from:
@@ -113,14 +111,70 @@
             for v in val:
                 if v not in valid_options:
                     raise ConfigError(f'{v} is not a valid option for {field}')
         else:
             if val not in valid_options:
                 raise ConfigError(f'{val} is not a valid option for {field}')
 
+    def to_file(self, uri: str, with_rv_metadata: bool = True) -> None:
+        """Save a Config to a JSON file, optionally with RV metadata.
+
+        Args:
+            uri: URI to save to.
+            with_rv_metadata: If True, inject Raster Vision metadata such as
+                ``plugin_versions``, so that the config can be upgraded when
+                loaded.
+        """
+        cfg_json = self.json()
+        if with_rv_metadata:
+            # self.dict() --> json_to_file() would be simpler but runs into
+            # JSON serialization problems
+            cfg_dict = json.loads(cfg_json)
+            cfg_dict['plugin_versions'] = registry.plugin_versions
+            cfg_json = json.dumps(cfg_dict)
+        json_to_file(cfg_dict, uri)
+
+    @classmethod
+    def deserialize(cls, inp: 'str | dict | Config') -> 'Self':
+        """Deserialize Config from a JSON file or dict, upgrading if possible.
+
+        If ``inp`` is already a :class:`.Config`, it is returned as is.
+
+        Args:
+            inp: a URI to a JSON file or a dict.
+        """
+        if isinstance(inp, Config):
+            return inp
+        if isinstance(inp, dict):
+            return cls.from_dict(inp)
+        if isinstance(inp, str):
+            return cls.from_file(inp)
+        raise TypeError(f'Cannot deserialize Config from type: {type(inp)}.')
+
+    @classmethod
+    def from_file(cls, uri: str) -> 'Self':
+        """Deserialize Config from a JSON file, upgrading if possible.
+
+        Args:
+            uri: URI to load from.
+        """
+        cfg_dict = load_config_dict(uri)
+        cfg = cls.from_dict(cfg_dict)
+        return cfg
+
+    @classmethod
+    def from_dict(cls, cfg_dict: dict) -> 'Self':
+        """Deserialize Config from a dict.
+
+        Args:
+            cfg_dict: Dict to deserialize.
+        """
+        cfg = build_config(cfg_dict)
+        return cfg
+
     def __repr_args__(self):
         """Override to delete 'type_hint' field."""
         args = dict(super().__repr_args__())
         try:
             del args['type_hint']
         except KeyError:
             pass
@@ -134,14 +188,23 @@
     """
     cfg.rv_config = rv_config.get_config_dict(registry.rv_config_schema)
     cfg.plugin_versions = registry.plugin_versions
     cfg_json = cfg.json()
     str_to_file(cfg_json, output_uri)
 
 
+def load_config_dict(uri: str) -> dict:
+    """Load a serialized Config from a JSON file as a dict and upgrade it."""
+    cfg_dict = file_to_json(uri)
+    if 'plugin_versions' in cfg_dict:
+        cfg_dict = upgrade_config(cfg_dict)
+        cfg_dict.pop('plugin_versions', None)
+    return cfg_dict
+
+
 def build_config(x: Union[dict, List[Union[dict, Config]], Config]
                  ) -> Union[Config, List[Config]]:
     """Build a Config from various types of input.
 
     This is useful for deserializing from JSON. It implements polymorphic
     deserialization by using the `type_hint` in each dict to get the
     corresponding Config class from the registry.
@@ -183,24 +246,28 @@
         current version.
     """
     if isinstance(x, dict):
         new_x = {}
         for k, v in x.items():
             new_x[k] = _upgrade_config(v, plugin_versions)
         type_hint = new_x.get('type_hint')
-        if type_hint is not None:
-            type_hint_lineage = registry.get_type_hint_lineage(type_hint)
-            for th in type_hint_lineage:
-                plugin = registry.get_plugin(th)
-                old_version = plugin_versions[plugin]
-                curr_version = registry.get_plugin_version(plugin)
-                upgrader = registry.get_upgrader(th)
-                if upgrader:
-                    for version in range(old_version, curr_version):
-                        new_x = upgrader(new_x, version)
+        if type_hint is None:
+            return new_x
+        if type_hint in registry.renamed_type_hints:
+            type_hint = registry.renamed_type_hints[type_hint]
+            new_x['type_hint'] = type_hint
+        type_hint_lineage = registry.get_type_hint_lineage(type_hint)
+        for th in type_hint_lineage:
+            plugin = registry.get_plugin(th)
+            old_version = plugin_versions[plugin]
+            curr_version = registry.get_plugin_version(plugin)
+            upgrader = registry.get_upgrader(th)
+            if upgrader:
+                for version in range(old_version, curr_version):
+                    new_x = upgrader(new_x, version)
         return new_x
     elif isinstance(x, list):
         return [_upgrade_config(v, plugin_versions) for v in x]
     else:
         return x
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/file_system.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/file_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from typing import Optional, List
 
 from rastervision.pipeline import registry_ as registry
 
 
 class NotReadableError(Exception):
     """Exception raised when files are not readable."""
-    pass
 
 
 class NotWritableError(Exception):
     """Exception raised when files are not writable."""
-    pass
 
 
 class FileSystem(ABC):
     """Abstraction for a local or remote file system.
 
     This can be subclassed to handle different cloud storage providers, etc.
     """
@@ -36,139 +34,126 @@
     def matches_uri(uri: str, mode: str) -> bool:
         """Returns True if this FS can be used for the given URI/mode pair.
 
         Args:
             uri: URI of file
             mode: mode to open file in, 'r' or 'w'
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def file_exists(uri: str, include_dir: bool = True) -> bool:
         """Check if a file exists.
 
         Args:
           uri: The URI to check
           include_dir: Include directories in check, if this file_system
             supports directory reads. Otherwise only return true if a single
             file exists at the URI.
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def read_str(uri: str) -> str:
         """Read contents of URI to a string."""
-        pass
 
     @staticmethod
     @abstractmethod
     def read_bytes(uri: str) -> bytes:
         """Read contents of URI to bytes."""
-        pass
 
     @staticmethod
     @abstractmethod
     def write_str(uri: str, data: str):
         """Write string in data to URI."""
-        pass
 
     @staticmethod
     @abstractmethod
     def write_bytes(uri: str, data: bytes):
         """Write bytes in data to URI."""
-        pass
 
     @staticmethod
     @abstractmethod
     def sync_to_dir(src_dir: str, dst_dir_uri: str, delete: bool = False):
         """Syncs a local source directory to a destination directory.
 
         If the FileSystem is remote, this involves uploading.
 
         Args:
             src_dir: local source directory to sync from
             dst_dir_uri: A destination directory that can be synced to by this
                 FileSystem
             delete: True if the destination should be deleted first.
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def sync_from_dir(src_dir_uri: str, dst_dir: str, delete: bool = False):
         """Syncs a source directory to a local destination directory.
 
         If the FileSystem is remote, this involves downloading.
 
         Args:
             src_dir_uri: source directory that can be synced from by this FileSystem
             dst_dir: A local destination directory
             delete: True if the destination should be deleted first.
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def copy_to(src_path: str, dst_uri: str):
         """Copy a local source file to a destination.
 
         If the FileSystem is remote, this involves uploading.
 
         Args:
             src_path: local path to source file
             dst_uri: uri of destination that can be copied to by this FileSystem
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def copy_from(src_uri: str, dst_path: str):
         """Copy a source file to a local destination.
 
         If the FileSystem is remote, this involves downloading.
 
         Args:
             src_uri: uri of source that can be copied from by this FileSystem
             dst_path: local path to destination file
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def local_path(uri: str, download_dir: str) -> str:
         """Return the path where a local copy should be stored.
 
         Args:
             uri: the URI of the file to be copied
             download_dir: path of the local directory in which files should
                 be copied
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def last_modified(uri: str) -> Optional[datetime]:
         """Get the last modified date of a file.
 
         Args:
             uri: the URI of the file
 
         Returns:
             the last modified date in UTC of a file or None if this FileSystem
             does not support this operation.
         """
-        pass
 
     @staticmethod
     @abstractmethod
     def list_paths(uri: str, ext: Optional[str] = None) -> List[str]:
         """List paths rooted at URI.
 
         Optionally only includes paths with a certain file extension.
 
         Args:
             uri: the URI of a directory
             ext: the optional file extension to filter by
         """
-        pass
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/http_file_system.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/http_file_system.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 
 from tqdm.auto import tqdm
 
 from rastervision.pipeline.file_system import (FileSystem, NotReadableError,
                                                NotWritableError)
 
 
-def get_file_obj(uri: str, with_progress: bool = True) -> ContextManager:
+def get_file_obj(uri: str, with_progress: bool = True,
+                 **kwargs) -> ContextManager:
     """Returns a context manager for a file-like object that supports buffered
     reads. If with_progress is True, wraps the read() method of the object in
     a function that updates a tqdm progress bar.
 
     Usage:
 
     .. code-block:: python
 
         with get_file_obj(uri) as f:
             ...
 
     Adapted from https://stackoverflow.com/a/63831344/5908685.
     """
-    r = requests.get(uri, stream=True, allow_redirects=True)
+    r = requests.get(uri, stream=True, allow_redirects=True, **kwargs)
     if r.status_code != 200:
         r.raise_for_status()  # Will only raise for 4xx codes, so...
         raise RuntimeError(
             f'Request to {uri} returned status code {r.status_code}')
     file_obj = r.raw
     # Decompress if needed
     file_obj.read = partial(file_obj.read, decode_content=True)
@@ -100,18 +101,18 @@
             'Cannot read directory from HTTP {}'.format(src_dir_uri))
 
     @staticmethod
     def copy_to(src_path: str, dst_uri: str) -> None:
         raise NotWritableError('Could not write {}'.format(dst_uri))
 
     @staticmethod
-    def copy_from(src_uri: str, dst_path: str) -> None:
-        with get_file_obj(src_uri) as in_file, open(dst_path,
-                                                    'wb') as out_file:
-            shutil.copyfileobj(in_file, out_file)
+    def copy_from(src_uri: str, dst_path: str, **kwargs) -> None:
+        with get_file_obj(src_uri, **kwargs) as in_file:
+            with open(dst_path, 'wb') as out_file:
+                shutil.copyfileobj(in_file, out_file)
 
     @staticmethod
     def local_path(uri: str, download_dir: str) -> None:
         parsed_uri = urlparse(uri)
         path = os.path.join(download_dir, 'http', parsed_uri.netloc,
                             parsed_uri.path[1:])
         # This function is expected to return something that is file path-like
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/local_file_system.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/local_file_system.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/file_system/utils.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/file_system/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from threading import Timer
 import time
 import logging
 import json
 import zipfile
 from typing import TYPE_CHECKING, Optional, List
 
+from tqdm.auto import tqdm
+
 from rastervision.pipeline import rv_config_ as rv_config
 from rastervision.pipeline.file_system import FileSystem
 from rastervision.pipeline.file_system.local_file_system import (
     LocalFileSystem, make_dir)
 
 if TYPE_CHECKING:
     from tempfile import TemporaryDirectory
@@ -319,17 +321,22 @@
 
     Args:
         dir: directory to zip
         zip_path: path to zip file to create
     """
     make_dir(zip_path, use_dirname=True)
     with zipfile.ZipFile(zip_path, 'w', zipfile.ZIP_DEFLATED) as ziph:
-        for dirpath, dirnames, filenames in os.walk(dir):
-            for fn in filenames:
-                ziph.write(join(dirpath, fn), join(dirpath[len(dir):], fn))
+        with tqdm(desc='Zipping', delay=5) as bar:
+            for dirpath, dirnames, filenames in os.walk(dir):
+                for fn in filenames:
+                    bar.set_postfix_str(fn)
+                    src = join(dirpath, fn)
+                    dst = join(dirpath[len(dir):], fn)
+                    ziph.write(src, dst)
+                    bar.update(1)
 
 
 def unzip(zip_path: str, target_dir: str):
     """Unzip contents of zip file at zip_path into target_dir.
 
     Creates target_dir if needed.
     """
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/pipeline.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/pipeline_config.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/registry.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     from rastervision.pipeline.runner import Runner  # noqa
     from rastervision.pipeline.file_system import FileSystem  # noqa
     from rastervision.pipeline.config import Upgrader, Config  # noqa
 
 
 class RegistryError(Exception):
     """Exception raised for invalid use of registry."""
-    pass
 
 
 class Registry():
     """A registry for resources that are built-in or contributed by plugins."""
 
     def __init__(self):
         self.runners = {}
@@ -24,14 +23,15 @@
 
         self.plugin_versions = {}
         self.alias_to_plugin = {}
         self.plugin_commands = []
         self.type_hint_to_lineage = {}
         self.type_hint_to_plugin = {}
         self.type_hint_to_upgrader = {}
+        self.renamed_type_hints = {}
 
     def add_plugin_command(self, cmd: Command):
         """Add a click command contributed by a plugin."""
         self.plugin_commands.append(cmd)
 
     def get_plugin_commands(self) -> List[Command]:
         """Get the click commands contributed by plugins."""
@@ -53,14 +53,24 @@
         Args:
             plugin: module path of plugin (eg. rastervision.core)
             version: a non-negative integer version number that should be incremented
                 each time a config schema changes
         """
         self.plugin_versions[plugin] = version
 
+    def register_renamed_type_hints(self, type_hint_old: str,
+                                    type_hint_new: str):
+        """Register renamed type_hints.
+
+        Args:
+            type_hint_old: Old type hint.
+            type_hint_new: New type hint.
+        """
+        self.renamed_type_hints[type_hint_old] = type_hint_new
+
     def get_type_hint_lineage(self, type_hint: str) -> List[str]:
         """Get the lineage for a type hint.
 
         Returns:
             List of type hints of all Config classes in the subclass is-a
             "lineage" from Config to the class with type hint type_hint.
         """
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/runner/inprocess_runner.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/inprocess_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 from rastervision.pipeline.cli import _run_command
 from rastervision.pipeline.runner.runner import Runner
 
 INPROCESS = 'inprocess'
 
 
 class InProcessRunner(Runner):
@@ -19,7 +20,11 @@
 
         for command in commands:
             if command in pipeline.split_commands and num_splits > 1:
                 for split_ind in range(num_splits):
                     _run_command(cfg_json_uri, command, split_ind, num_splits)
             else:
                 _run_command(cfg_json_uri, command, 0, 1)
+
+    def run_command(self, cmd: List[str]):
+        raise NotImplementedError(
+            'Use LocalRunner.run_command to run a command locally.')
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/runner/local_runner.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/local_runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,109 @@
+from typing import TYPE_CHECKING, List, Optional
 import sys
 from os.path import dirname, join
 from subprocess import Popen
 
 from rastervision.pipeline.file_system import str_to_file, download_if_needed
 from rastervision.pipeline.runner.runner import Runner
 from rastervision.pipeline.utils import terminate_at_exit
 
+if TYPE_CHECKING:
+    from rastervision.pipeline.pipeline import Pipeline
+
 LOCAL = 'local'
 
 
+def make_run_cmd_invocation(cfg_json_uri: str,
+                            command: str,
+                            opts: Optional[dict] = None) -> str:
+    opts_str = ''
+    if opts is not None:
+        opts_str = ' ' + ' '.join(f'{k} {v}' for k, v in opts.items())
+    return ('python -m rastervision.pipeline.cli run_command '
+            f'{cfg_json_uri} {command}{opts_str}')
+
+
+def make_makefile_entry_for_cmd(curr_command_ind: int,
+                                prev_command_inds: List[int],
+                                cfg_json_uri: str,
+                                command: str,
+                                opts: Optional[dict] = None) -> str:
+    out = f'{curr_command_ind}: '
+    out += ' '.join([str(ci) for ci in prev_command_inds])
+    out += '\n'
+    invocation = make_run_cmd_invocation(cfg_json_uri, command, opts=opts)
+    out += f'\t{invocation}\n\n'
+    return out
+
+
 class LocalRunner(Runner):
-    """Runs each command locally using different processes for each command/split.
+    """
+    Runs each command locally using different processes for each command/split.
 
-    This is implemented by generating a Makefile and then running it using make.
+    This is implemented by generating a Makefile and then running it using
+    make.
     """
 
     def run(self,
-            cfg_json_uri,
-            pipeline,
-            commands,
-            num_splits=1,
+            cfg_json_uri: str,
+            pipeline: 'Pipeline',
+            commands: List[str],
+            num_splits: int = 1,
             pipeline_run_name: str = 'raster-vision'):
+        makefile = self.build_makefile_string(cfg_json_uri, pipeline, commands,
+                                              num_splits)
+        makefile_path = join(dirname(cfg_json_uri), 'Makefile')
+        str_to_file(makefile, makefile_path)
+        makefile_path_local = download_if_needed(makefile_path)
+        return self.run_command(['make', '-j', '-f', makefile_path_local])
+
+    def run_command(self, cmd: List[str]):
+        process = Popen(cmd)
+        terminate_at_exit(process)
+        exitcode = process.wait()
+        if exitcode != 0:
+            sys.exit(exitcode)
+        else:
+            return 0
+
+    def build_makefile_string(self,
+                              cfg_json_uri: str,
+                              pipeline: 'Pipeline',
+                              commands: List[str],
+                              num_splits: int = 1) -> str:
         num_commands = 0
         for command in commands:
             if command in pipeline.split_commands and num_splits > 1:
                 num_commands += num_splits
             else:
                 num_commands += 1
 
-        makefile = '.PHONY: '
-        makefile += ' '.join([str(ci) for ci in range(num_commands)])
-        makefile += '\n\n'
-
-        makefile += 'all: '
-        makefile += ' '.join([str(ci) for ci in range(num_commands)])
-        makefile += '\n\n'
+        all_command_inds_str = ' '.join([str(i) for i in range(num_commands)])
+        makefile = f'.PHONY: {all_command_inds_str}\n\n'
+        makefile += f'all: {all_command_inds_str}\n\n'
 
         prev_command_inds = []
         curr_command_ind = 0
         for command in commands:
-
             curr_command_inds = []
             if command in pipeline.split_commands and num_splits > 1:
+                opts = {'--num-splits': num_splits}
                 for split_ind in range(num_splits):
-                    makefile += '{}: '.format(curr_command_ind)
-                    makefile += ' '.join([str(ci) for ci in prev_command_inds])
-                    makefile += '\n'
-                    invocation = (
-                        'python -m rastervision.pipeline.cli run_command '
-                        '{} {} --split-ind {} --num-splits {}').format(
-                            cfg_json_uri, command, split_ind, num_splits)
-                    makefile += '\t{}\n\n'.format(invocation)
+                    opts['--split-ind'] = split_ind
+                    makefile_entry = make_makefile_entry_for_cmd(
+                        curr_command_ind,
+                        prev_command_inds,
+                        cfg_json_uri,
+                        command,
+                        opts=opts)
+                    makefile += makefile_entry
                     curr_command_inds.append(curr_command_ind)
                     curr_command_ind += 1
             else:
-                makefile += '{}: '.format(curr_command_ind)
-                makefile += ' '.join([str(ci) for ci in prev_command_inds])
-                makefile += '\n'
-                invocation = (
-                    'python -m rastervision.pipeline.cli run_command '
-                    '{} {}'.format(cfg_json_uri, command))
-                makefile += '\t{}\n\n'.format(invocation)
+                makefile_entry = make_makefile_entry_for_cmd(
+                    curr_command_ind, prev_command_inds, cfg_json_uri, command)
+                makefile += makefile_entry
                 curr_command_inds.append(curr_command_ind)
                 curr_command_ind += 1
-
             prev_command_inds = curr_command_inds
-
-        makefile_path = join(dirname(cfg_json_uri), 'Makefile')
-        str_to_file(makefile, makefile_path)
-        makefile_path_local = download_if_needed(makefile_path)
-        process = Popen(['make', '-j', '-f', makefile_path_local])
-        terminate_at_exit(process)
-        exitcode = process.wait()
-        if exitcode != 0:
-            sys.exit(exitcode)
-        else:
-            return 0
+        return makefile
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/runner/runner.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/runner/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,22 @@
 
         Args:
             cfg_json_uri: URI of a JSON file with a serialized PipelineConfig
             pipeline: the Pipeline to run
             commands: names of commands to run
             num_splits: number of splits to use for splittable commands
         """
-        pass
+
+    @abstractmethod
+    def run_command(self, cmd: List[str]):
+        """Run a single command.
+
+        Args:
+            cmd: The command to run.
+        """
 
     def get_split_ind(self) -> Optional[int]:
         """Get the split_ind for the process.
 
         For split commands, the split_ind determines which split of work to perform
         within the current OS process. The CLI has a --split-ind option, but some runners
         may have their own means of communicating the split_ind, and this method should
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/rv_config.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/rv_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from typing import Any, Dict, List, Optional
 import os
 from tempfile import TemporaryDirectory
 from pathlib import Path
 import logging
 import json
-from typing import Optional, List, Dict
 
 from everett.manager import (ConfigManager, ConfigDictEnv, ConfigOSEnv,
                              ConfigurationMissingError)
 from everett.ext.inifile import ConfigIniEnv
 
 from rastervision.pipeline.verbosity import Verbosity
 
@@ -63,31 +63,42 @@
         else:
             root_log.setLevel(logging.WARN)
 
     def get_verbosity(self) -> Verbosity:
         """Returns verbosity level for logging."""
         return self.verbosity
 
+    def get_verbosity_cli_opt(self) -> str:
+        """Returns verbosity in a form that can be passed to RV CLI cmds.
+
+        Returns:
+            str: string like "-vvv...".
+        """
+        num_vs = max(0, self.get_verbosity() - 1)
+        if num_vs == 0:
+            return ''
+        return f'-{"v" * num_vs}'
+
     def get_tmp_dir(self) -> TemporaryDirectory:
         """Return a new TemporaryDirectory object."""
         return TemporaryDirectory(dir=self.tmp_dir_root)
 
     def get_tmp_dir_root(self) -> str:
         """Return the root of all temp dirs."""
         return self.tmp_dir_root
 
     def set_tmp_dir_root(self, tmp_dir_root: Optional[str] = None):
         """Set root of all temporary directories.
 
         To set the value, the following rules are used in decreasing priority:
 
-        1) the tmp_dir_root argument if it is not None
-        2) an environment variable (TMPDIR, TEMP, or TMP)
-        3) a default temporary directory which is
-        4) a directory returned by tempfile.TemporaryDirectory()
+        1) the ``tmp_dir_root`` argument if it is not ``None``
+        2) an environment variable (``TMPDIR``, ``TEMP``, or ``TMP``)
+        3) a default temporary directory which is a directory returned by
+           :class:`tempfile.TemporaryDirectory`
         """
         # Check the various possibilities in order of priority.
         env_arr = [
             os.environ.get(k) for k in ['TMPDIR', 'TEMP', 'TMP']
             if k in os.environ
         ]
 
@@ -195,18 +206,35 @@
                 config_ini_env,
             ],
             doc=(
                 'Check https://docs.rastervision.io/ for docs. '
                 'Switch to the version being run and search for Raster Vision '
                 'Configuration.'))
 
-    def get_namespace_config(self, namespace: str) -> Dict[str, str]:
+    def get_namespace_config(self, namespace: str) -> ConfigManager:
         """Get the key-val pairs associated with a namespace."""
         return self.config.with_namespace(namespace)
 
+    def get_namespace_option(self,
+                             namespace: str,
+                             key: str,
+                             default: Optional[Any] = None,
+                             as_bool: bool = False) -> Optional[Any]:
+        """Get the value of an option from a namespace."""
+        namespace_options = self.config.with_namespace(namespace)
+        try:
+            val: str = namespace_options(key)
+            if as_bool:
+                val = val.lower() in ('1', 'true', 'y', 'yes')
+            return val
+        except ConfigurationMissingError:
+            if as_bool:
+                return bool(default)
+            return default
+
     def get_config_dict(
             self, rv_config_schema: Dict[str, List[str]]) -> Dict[str, str]:
         """Get all Everett configuration.
 
         This method is used to serialize an Everett configuration so it can be used on
         a remote instance.
 
@@ -217,16 +245,17 @@
         Returns:
             Each key is of form namespace_i_key_ij with corresponding value val_ij.
         """
         config_dict = {}
         for namespace, keys in rv_config_schema.items():
             for key in keys:
                 try:
-                    config_dict[namespace + '_' + key] = \
-                        self.get_namespace_config(namespace)(key)
+                    namespace_options = self.get_namespace_config(namespace)
+                    full_key = f'{namespace}_{key}'
+                    config_dict[full_key] = namespace_options(key)
                 except ConfigurationMissingError:
                     pass
 
         return config_dict
 
     def _discover_config_file_locations(self, profile) -> List[str]:
         """Discover the location of RV config files.
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline/utils.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any
+from typing import Any, Callable, Optional
+import os
 import atexit
 import logging
 from math import ceil
 
 log = logging.getLogger(__name__)
 
 
@@ -41,7 +42,17 @@
 
 def repr_with_args(obj: Any, **kwargs) -> str:
     """Builds a string of the form: <obj's class name>(k1=v1, k2=v2, ...)."""
     cls = type(obj).__name__
     arg_strs = [f'{k}={v!r}' for k, v in kwargs.items()]
     arg_str = ', '.join(arg_strs)
     return f'{cls}({arg_str})'
+
+
+def get_env_var(key: str,
+                default: Optional[Any] = None,
+                out_type: Optional[type | Callable] = None) -> Optional[Any]:
+    val = os.environ.get(key, default)
+    if val is not None and out_type is not None:
+        if out_type == bool:
+            return val.lower() in ('1', 'true', 'y', 'yes')
+        return out_type(val)
```

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/__init__.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/config1.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/config1.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/sample_pipeline.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin1/sample_pipeline2.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin1/sample_pipeline2.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/__init__.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/config3.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/config3.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision/pipeline_example_plugin2/deluxe_message_maker.py` & `rastervision_pipeline-0.30.0/rastervision/pipeline_example_plugin2/deluxe_message_maker.py`

 * *Files identical despite different names*

### Comparing `rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/PKG-INFO` & `rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastervision-pipeline
-Version: 0.21.3
+Version: 0.30.0
 Summary: The main rastervision package for configuring, defining, and running pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_pipeline-0.21.3/rastervision_pipeline.egg-info/SOURCES.txt` & `rastervision_pipeline-0.30.0/rastervision_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

