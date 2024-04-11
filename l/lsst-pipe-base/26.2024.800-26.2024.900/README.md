# Comparing `tmp/lsst-pipe-base-26.2024.800.tar.gz` & `tmp/lsst-pipe-base-26.2024.900.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-pipe-base-26.2024.800.tar", last modified: Thu Feb 22 10:44:14 2024, max compression
+gzip compressed data, was "lsst-pipe-base-26.2024.900.tar", last modified: Thu Feb 29 10:21:38 2024, max compression
```

## Comparing `lsst-pipe-base-26.2024.800.tar` & `lsst-pipe-base-26.2024.900.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.860341 lsst-pipe-base-26.2024.800/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-22 10:44:14.860341 lsst-pipe-base-26.2024.800/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.836341 lsst-pipe-base-26.2024.800/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.840341 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-pipelinetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/task-framework-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/task-retargeting-howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/testing-a-pipeline-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.836341 lsst-pipe-base-26.2024.800/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.840341 lsst-pipe-base-26.2024.800/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.840341 lsst-pipe-base-26.2024.800/python/lsst/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_datasetQueryConstraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_observation_dimension_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17418 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_quantumContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    20334 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27499 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/automatic_connection_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/connectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/executionButlerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/execution_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/formatters/pexConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.848341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_implDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_loadHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27947 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_versionDeserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53094 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/quantumNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    62364 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipelineTask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.852341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    72184 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    36635 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.852341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
--rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/prerequisite_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53756 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/quantum_graph_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.852341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/register_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/transfer_from_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/testUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.856341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.856341 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_data_id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    28357 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/no_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/pipelineStepTester.py
--rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/simpleQGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst/pipe/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.860341 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 10:44:14.000000 lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-22 10:44:14.860341 lsst-pipe-base-26.2024.800/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 10:44:14.860341 lsst-pipe-base-26.2024.800/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_cliCmdRegisterInstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_config_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_dataid_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_dynamic_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_executionButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_execution_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26675 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipelineLoadSubset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipelineTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    66381 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    25662 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_quantumGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_taskmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-02-22 10:44:01.000000 lsst-pipe-base-26.2024.800/tests/test_testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.628640 lsst-pipe-base-26.2024.900/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipelinetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-framework-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-retargeting-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-a-pipeline-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.628640 lsst-pipe-base-26.2024.900/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/python/lsst/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.636640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_datasetQueryConstraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_observation_dimension_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17418 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_quantumContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24073 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27499 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/automatic_connection_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/executionButlerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/execution_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/pexConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_implDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_loadHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27947 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_versionDeserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53094 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/quantumNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62364 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72184 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36635 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/prerequisite_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53756 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/register_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/transfer_from_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_data_id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28357 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/no_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/pipelineStepTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/simpleQGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_cliCmdRegisterInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_config_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dataid_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dynamic_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_executionButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_execution_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26675 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineLoadSubset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25662 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_quantumGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_taskmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_testUtils.py
```

### Comparing `lsst-pipe-base-26.2024.800/PKG-INFO` & `lsst-pipe-base-26.2024.900/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pipe-base-26.2024.800/README.md` & `lsst-pipe-base-26.2024.900/README.md`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/bsd_license.txt` & `lsst-pipe-base-26.2024.900/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/CHANGES.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-pipeline.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipeline.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-pipelinetask.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipelinetask.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/creating-a-task.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-task.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/index.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/index.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/task-framework-overview.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-framework-overview.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/task-retargeting-howto.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-retargeting-howto.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/testing-a-pipeline-task.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-a-pipeline-task.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/doc/lsst.pipe.base/working-with-pipeline-graphs.rst` & `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/gpl-v3.0.txt` & `lsst-pipe-base-26.2024.900/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/pyproject.toml` & `lsst-pipe-base-26.2024.900/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_datasetQueryConstraints.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_datasetQueryConstraints.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_dataset_handle.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_instrument.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_observation_dimension_packer.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_observation_dimension_packer.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_quantumContext.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_quantumContext.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_status.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,26 @@
 
 __all__ = (
     "NoWorkFound",
     "RepeatableQuantumError",
     "InvalidQuantumError",
 )
 
+from typing import Protocol
+
+from ._task_metadata import GetSetDictMetadata
+
+
+class GetSetDictMetadataHolder(Protocol):
+    """Protocol for objects that have a ``metadata`` attribute that satisfies
+    `GetSetDictMetadata`.
+    """
+
+    metadata: GetSetDictMetadata | None
+
 
 class NoWorkFound(BaseException):
     """An exception raised when a Quantum should not exist because there is no
     work for it to do.
 
     This usually occurs because a non-optional input dataset is not present, or
     a spatiotemporal overlap that was conservatively predicted does not
```

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/_task_metadata.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_task_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,28 +21,38 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__all__ = ["TaskMetadata"]
+__all__ = [
+    "TaskMetadata",
+    "SetDictMetadata",
+    "GetDictMetadata",
+    "GetSetDictMetadata",
+    "NestedMetadataDict",
+]
 
 import itertools
 import numbers
 import sys
 from collections.abc import Collection, Iterator, Mapping, Sequence
-from typing import Any, Protocol
+from typing import Any, Protocol, TypeAlias, Union
 
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 
 # The types allowed in a Task metadata field are restricted
 # to allow predictable serialization.
 _ALLOWED_PRIMITIVE_TYPES = (str, float, int, bool)
 
+# Note that '|' syntax for unions doesn't work when we have to use a string
+# literal (and we do since it's recursive and not an annotation).
+NestedMetadataDict: TypeAlias = Mapping[str, Union[str, float, int, bool, "NestedMetadataDict"]]
+
 
 class PropertySetLike(Protocol):
     """Protocol that looks like a ``lsst.daf.base.PropertySet``.
 
     Enough of the API is specified to support conversion of a
     ``PropertySet`` to a `TaskMetadata`.
     """
@@ -52,14 +62,58 @@
     def getArray(self, name: str) -> Any: ...
 
 
 def _isListLike(v: Any) -> bool:
     return isinstance(v, Sequence) and not isinstance(v, str)
 
 
+class SetDictMetadata(Protocol):
+    """Protocol for objects that can be assigned a possibly-nested `dict` of
+    primitives.
+
+    This protocol is satisfied by `TaskMetadata`, `lsst.daf.base.PropertySet`,
+    and `lsst.daf.base.PropertyList`, providing a consistent way to insert a
+    dictionary into these objects that avoids their historical idiosyncrasies.
+
+    The form in which these entries appear in the object's native keys and
+    values is implementation-defined.  *Empty nested dictionaries may be
+    dropped, and if the top-level dictionary is empty this method may do
+    nothing.*
+
+    Neither the top-level key nor nested keys may contain ``.`` (period)
+    characters.
+    """
+
+    def set_dict(self, key: str, nested: NestedMetadataDict) -> None: ...
+
+
+class GetDictMetadata(Protocol):
+    """Protocol for objects that can extract a possibly-nested mapping of
+    primitives.
+
+    This protocol is satisfied by `TaskMetadata`, `lsst.daf.base.PropertySet`,
+    and `lsst.daf.base.PropertyList`, providing a consistent way to extract a
+    dictionary from these objects that avoids their historical idiosyncrasies.
+
+    This is guaranteed to work for mappings inserted by
+    `~SetMapping.set_dict`.  It should not be expected to work for values
+    inserted in other ways.  If a value was never inserted with the given key
+    at all, *an empty `dict` will be returned* (this is a concession to
+    implementation constraints in `~lsst.daf.base.PropertyList`.
+    """
+
+    def get_dict(self, key: str) -> NestedMetadataDict: ...
+
+
+class GetSetDictMetadata(SetDictMetadata, GetDictMetadata, Protocol):
+    """Protocol for objects that can assign and extract a possibly-nested
+    mapping of primitives.
+    """
+
+
 class TaskMetadata(BaseModel):
     """Dict-like object for storing task metadata.
 
     Metadata can be stored at two levels: single task or task plus subtasks.
     The later is called full metadata of a task and has a form
 
         topLevelTaskName:subtaskName:subsubtaskName.itemName
@@ -473,14 +527,57 @@
 
         try:
             del self.metadata[key0][".".join(keys)]
         except KeyError:
             # Report the correct key.
             raise KeyError(f"'{key}' not found'") from None
 
+    def get_dict(self, key: str) -> NestedMetadataDict:
+        """Return a possibly-hierarchical nested `dict`.
+
+        This implements the `GetDictMetadata` protocol for consistency with
+        `lsst.daf.base.PropertySet` and `lsst.daf.base.PropertyList`.  The
+        returned `dict` is guaranteed to be a deep copy, not a view.
+
+        Parameters
+        ----------
+        key : `str`
+            String key associated with the mapping.  May not have a ``.``
+            character.
+
+        Returns
+        -------
+        value : `~collections.abc.Mapping`
+            Possibly-nested mapping, with `str` keys and values that are `int`,
+            `float`, `str`, `bool`, or another `dict` with the same key and
+            value types.  Will be empty if ``key`` does not exist.
+        """
+        if value := self.get(key):
+            return value.to_dict()
+        else:
+            return {}
+
+    def set_dict(self, key: str, value: NestedMetadataDict) -> None:
+        """Assign a possibly-hierarchical nested `dict`.
+
+        This implements the `SetDictMetadata` protocol for consistency with
+        `lsst.daf.base.PropertySet` and `lsst.daf.base.PropertyList`.
+
+        Parameters
+        ----------
+        key : `str`
+            String key associated with the mapping.  May not have a ``.``
+            character.
+        value : `~collections.abc.Mapping`
+            Possibly-nested mapping, with `str` keys and values that are `int`,
+            `float`, `str`, `bool`, or another `dict` with the same key and
+            value types.  Nested keys may not have a ``.`` character.
+        """
+        self[key] = value
+
     def _validate_value(self, value: Any) -> tuple[str, Any]:
         """Validate the given value.
 
         Parameters
         ----------
         value : Any
             Value to check.
```

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/automatic_connection_constants.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/automatic_connection_constants.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/cmd/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/cmd/commands.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/arguments.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/cli/opt/options.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/config.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/config.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/configOverrides.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/connectionTypes.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connectionTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/connections.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connections.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/executionButlerBuilder.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/executionButlerBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/execution_reports.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/execution_reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,20 +355,32 @@
         pipeline_dataset_types = PipelineDatasetTypes.fromPipeline(task_defs, registry=butler.registry)
         for dataset_type in itertools.chain(
             pipeline_dataset_types.initIntermediates,
             pipeline_dataset_types.initOutputs,
             pipeline_dataset_types.intermediates,
             pipeline_dataset_types.outputs,
         ):
-            refs[dataset_type.name] = {
-                ref.id: ref
-                for ref in butler.registry.queryDatasets(
-                    dataset_type.name, collections=collection, findFirst=False
-                )
-            }
+            if (component := dataset_type.component()) is not None:
+                # Work around the fact that component support has been phased
+                # out of daf_butler queries but not pipe_base's QGs.  This
+                # should go away on DM-40441.
+                parent_dataset_type = dataset_type.makeCompositeDatasetType()
+                refs[dataset_type.name] = {
+                    ref.id: ref.makeComponentRef(component)
+                    for ref in butler.registry.queryDatasets(
+                        parent_dataset_type.name, collections=collection, findFirst=False
+                    )
+                }
+            else:
+                refs[dataset_type.name] = {
+                    ref.id: ref
+                    for ref in butler.registry.queryDatasets(
+                        dataset_type.name, collections=collection, findFirst=False
+                    )
+                }
         for task_def in qg.iterTaskGraph():
             for node in qg.getNodesForTask(task_def):
                 status_graph.add_node(node.nodeId)
                 for ref in itertools.chain.from_iterable(node.quantum.outputs.values()):
                     status_graph.add_edge(node.nodeId, ref.id)
                 for ref in itertools.chain.from_iterable(node.quantum.inputs.values()):
                     status_graph.add_edge(ref.id, node.nodeId)
```

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/formatters/pexConfig.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/pexConfig.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_implDetails.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_implDetails.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_loadHelpers.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_loadHelpers.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/_versionDeserializers.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_versionDeserializers.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/graph.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/graph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graph/quantumNode.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/quantumNode.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/graphBuilder.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeTools.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeTools.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipelineIR.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipelineTask.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/__main__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_dataset_types.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_edges.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_edges.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_exceptions.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_mapping_views.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_nodes.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_nodes.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_task_subsets.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/_tasks.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_tasks.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/io.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/io.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_options.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/pipeline_graph/visualization/_show.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/prerequisite_helpers.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/prerequisite_helpers.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/quantum_graph_builder.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_builder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/quantum_graph_skeleton.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_skeleton.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/register_instrument.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/register_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/script/transfer_from_graph.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/transfer_from_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/struct.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/struct.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/task.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/task.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/taskFactory.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/taskFactory.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/testUtils.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/__init__.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_data_id_match.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_data_id_match.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_pipeline_task.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/mocks/_storage_class.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/no_dimensions.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/no_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/pipelineStepTester.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/pipelineStepTester.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/simpleQGraph.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/simpleQGraph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst/pipe/base/tests/util.py` & `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/util.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/PKG-INFO` & `lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 26.2024.800
+Version: 26.2024.900
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pipe-base-26.2024.800/python/lsst_pipe_base.egg-info/SOURCES.txt` & `lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_cliCmdRegisterInstrument.py` & `lsst-pipe-base-26.2024.900/tests/test_cliCmdRegisterInstrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_configOverrides.py` & `lsst-pipe-base-26.2024.900/tests/test_configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_config_formatter.py` & `lsst-pipe-base-26.2024.900/tests/test_config_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_connections.py` & `lsst-pipe-base-26.2024.900/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_dataid_match.py` & `lsst-pipe-base-26.2024.900/tests/test_dataid_match.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_dataset_handle.py` & `lsst-pipe-base-26.2024.900/tests/test_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_dynamic_connections.py` & `lsst-pipe-base-26.2024.900/tests/test_dynamic_connections.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_executionButler.py` & `lsst-pipe-base-26.2024.900/tests/test_executionButler.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_execution_reports.py` & `lsst-pipe-base-26.2024.900/tests/test_execution_reports.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_graphBuilder.py` & `lsst-pipe-base-26.2024.900/tests/test_graphBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_instrument.py` & `lsst-pipe-base-26.2024.900/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipeTools.py` & `lsst-pipe-base-26.2024.900/tests/test_pipeTools.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipeline.py` & `lsst-pipe-base-26.2024.900/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipelineIR.py` & `lsst-pipe-base-26.2024.900/tests/test_pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipelineLoadSubset.py` & `lsst-pipe-base-26.2024.900/tests/test_pipelineLoadSubset.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipelineTask.py` & `lsst-pipe-base-26.2024.900/tests/test_pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_pipeline_graph.py` & `lsst-pipe-base-26.2024.900/tests/test_pipeline_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_quantumGraph.py` & `lsst-pipe-base-26.2024.900/tests/test_quantumGraph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_struct.py` & `lsst-pipe-base-26.2024.900/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_task.py` & `lsst-pipe-base-26.2024.900/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.800/tests/test_taskmetadata.py` & `lsst-pipe-base-26.2024.900/tests/test_taskmetadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -237,10 +237,30 @@
 
         with self.assertRaises(ValueError):
             meta.add("mixed", [1.5, numpy.float64(4.5)])
 
         with self.assertRaises(ValueError):
             meta["numpy"] = numpy.zeros(5)
 
+    def test_get_set_dict(self):
+        """Test the get_dict and set_dict methods."""
+        obj = TaskMetadata()
+        d1 = {"one": 1, "two": 2.0, "three": True, "four": {"a": 4, "b": "B"}, "five": {}}
+        obj.set_dict("d", d1)
+        obj.set_dict("e", {})
+        d2 = obj.get_dict("d")
+        # Keys with empty-dict values may or may not be round-tripped.
+        self.assertGreaterEqual(d2.keys(), {"one", "two", "three", "four"})
+        self.assertLessEqual(d2.keys(), {"one", "two", "three", "four", "five"})
+        self.assertEqual(d2["one"], d1["one"])
+        self.assertEqual(d2["two"], d1["two"])
+        self.assertEqual(d2["three"], d1["three"])
+        self.assertEqual(d2["four"], d1["four"])
+        self.assertEqual(d2.get("five", {}), d1["five"])
+        # Empty dict may or may not have been added, and retrieving it or
+        # a key that was never added yields an empty dict.
+        self.assertEqual(obj.get_dict("e"), {})
+        self.assertEqual(obj.get_dict("f"), {})
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-pipe-base-26.2024.800/tests/test_testUtils.py` & `lsst-pipe-base-26.2024.900/tests/test_testUtils.py`

 * *Files identical despite different names*

