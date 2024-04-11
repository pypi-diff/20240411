# Comparing `tmp/dagster-1.7.0.tar.gz` & `tmp/dagster-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.0.tar", last modified: Thu Apr  4 19:44:34 2024, max compression
+gzip compressed data, was "dagster-1.7.1.tar", last modified: Thu Apr 11 18:04:47 2024, max compression
```

## Comparing `dagster-1.7.0.tar` & `dagster-1.7.1.tar`

### file list

```diff
@@ -1,691 +1,692 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.235781 dagster-1.7.0/
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-04 19:44:07.000000 dagster-1.7.0/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:07.000000 dagster-1.7.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-04-04 19:44:07.000000 dagster-1.7.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8934 2024-04-04 19:44:34.235781 dagster-1.7.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7220 2024-04-04 19:44:07.000000 dagster-1.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.143781 dagster-1.7.0/dagster/
--rw-r--r--   0 root         (0) root         (0)    29822 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.143781 dagster-1.7.0/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.143781 dagster-1.7.0/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.147781 dagster-1.7.0/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.147781 dagster-1.7.0/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.147781 dagster-1.7.0/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.147781 dagster-1.7.0/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18042 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11496 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4022 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)    41251 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.151781 dagster-1.7.0/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.151781 dagster-1.7.0/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.151781 dagster-1.7.0/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.171781 dagster-1.7.0/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7409 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5426 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6073 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.171781 dagster-1.7.0/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21345 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16484 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26160 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10572 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10251 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7570 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16483 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    29917 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)     9802 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79547 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13884 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    54395 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21660 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34626 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    29993 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.175781 dagster-1.7.0/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    68510 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42247 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9750 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.175781 dagster-1.7.0/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5166 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7677 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4029 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    15650 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2722 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5610 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.175781 dagster-1.7.0/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42305 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10371 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    22439 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27569 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.175781 dagster-1.7.0/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6225 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    21859 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102142 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17805 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.175781 dagster-1.7.0/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7635 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.183781 dagster-1.7.0/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.187781 dagster-1.7.0/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78765 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    39887 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    55076 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18533 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    16535 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40549 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11036 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   131811 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     5736 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.191781 dagster-1.7.0/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    82857 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10931 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.195781 dagster-1.7.0/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.199781 dagster-1.7.0/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.199781 dagster-1.7.0/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.211781 dagster-1.7.0/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.211781 dagster-1.7.0/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25656 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.215781 dagster-1.7.0/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18330 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   122582 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.215781 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.215781 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.215781 dagster-1.7.0/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17131 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37454 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19355 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.219781 dagster-1.7.0/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    28842 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    41787 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12112 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-04-04 19:44:07.000000 dagster-1.7.0/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18369 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39110 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.139781 dagster-1.7.0/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.223781 dagster-1.7.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)      919 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.227781 dagster-1.7.0/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41378 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.231781 dagster-1.7.0/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8916 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    42415 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.231781 dagster-1.7.0/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.231781 dagster-1.7.0/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.235781 dagster-1.7.0/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    24377 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5404 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42589 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33171 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.235781 dagster-1.7.0/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7622 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    35720 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.235781 dagster-1.7.0/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:08.000000 dagster-1.7.0/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:44:34.143781 dagster-1.7.0/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8934 2024-04-04 19:44:33.000000 dagster-1.7.0/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    27927 2024-04-04 19:44:34.000000 dagster-1.7.0/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:44:33.000000 dagster-1.7.0/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-04 19:44:33.000000 dagster-1.7.0/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-04 19:44:33.000000 dagster-1.7.0/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:33.000000 dagster-1.7.0/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-04-04 19:44:34.235781 dagster-1.7.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6827 2024-04-04 19:44:08.000000 dagster-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.426220 dagster-1.7.1/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-11 18:04:20.000000 dagster-1.7.1/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-1.7.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-11 18:04:20.000000 dagster-1.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-04-11 18:04:47.426220 dagster-1.7.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7214 2024-04-11 18:04:20.000000 dagster-1.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.310219 dagster-1.7.1/dagster/
+-rw-r--r--   0 root         (0) root         (0)    29822 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.314219 dagster-1.7.1/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.318220 dagster-1.7.1/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.322219 dagster-1.7.1/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18042 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11496 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4022 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)    41251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21047 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.326219 dagster-1.7.1/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.338220 dagster-1.7.1/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7827 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6073 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.338220 dagster-1.7.1/dagster/_core/definitions/asset_condition/
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21008 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16484 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+-rw-r--r--   0 root         (0) root         (0)    26160 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7621 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16483 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    29917 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6764 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)     9802 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79547 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13880 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    54395 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21660 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34626 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    69203 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12664 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_based_auto_materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7677 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     7938 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/shared_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4669 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)    10573 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_checks/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    42305 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10371 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22439 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27737 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    44126 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19244 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    21859 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102142 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11017 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    18062 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.342220 dagster-1.7.1/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7635 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.350220 dagster-1.7.1/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    64654 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.354220 dagster-1.7.1/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    56002 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    16535 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40549 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11036 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    14043 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.358220 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   131945 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.362220 dagster-1.7.1/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83392 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28809 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10931 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.366220 dagster-1.7.1/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.370220 dagster-1.7.1/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.374220 dagster-1.7.1/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.374220 dagster-1.7.1/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.390220 dagster-1.7.1/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.390220 dagster-1.7.1/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25656 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18330 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   122582 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32629 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    17131 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37454 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.394220 dagster-1.7.1/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7236 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25146 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19355 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.398220 dagster-1.7.1/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.402220 dagster-1.7.1/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    28842 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    41787 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.406220 dagster-1.7.1/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18369 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39110 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.306219 dagster-1.7.1/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.410220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.414220 dagster-1.7.1/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)      919 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41378 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8916 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    42415 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.418220 dagster-1.7.1/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.422220 dagster-1.7.1/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    24377 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    42589 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33171 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.422220 dagster-1.7.1/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7622 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    35720 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.426220 dagster-1.7.1/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-11 18:04:20.000000 dagster-1.7.1/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:04:47.310219 dagster-1.7.1/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    27988 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:47.000000 dagster-1.7.1/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-04-11 18:04:47.426220 dagster-1.7.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6827 2024-04-11 18:04:20.000000 dagster-1.7.1/setup.py
```

### Comparing `dagster-1.7.0/COPYING` & `dagster-1.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/LICENSE` & `dagster-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/MANIFEST.in` & `dagster-1.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/PKG-INFO` & `dagster-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.0
+Version: 1.7.1
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -117,15 +117,15 @@
 ```
 
 This installs two packages:
 
 - `dagster`: The core programming model.
 - `dagster-webserver`: The server that hosts Dagster's web UI for developing and operating Dagster jobs and assets.
 
-Running on Using a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
+Running on a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
 
 ## Documentation
 
 You can find the full Dagster documentation [here](https://docs.dagster.io), including the ['getting started' guide](https://docs.dagster.io/getting-started).
 
 <hr/>
```

### Comparing `dagster-1.7.0/README.md` & `dagster-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 ```
 
 This installs two packages:
 
 - `dagster`: The core programming model.
 - `dagster-webserver`: The server that hosts Dagster's web UI for developing and operating Dagster jobs and assets.
 
-Running on Using a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
+Running on a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
 
 ## Documentation
 
 You can find the full Dagster documentation [here](https://docs.dagster.io), including the ['getting started' guide](https://docs.dagster.io/getting-started).
 
 <hr/>
```

### Comparing `dagster-1.7.0/dagster/__init__.py` & `dagster-1.7.1/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_annotations.py` & `dagster-1.7.1/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/get_server_id.py` & `dagster-1.7.1/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/list_repositories.py` & `dagster-1.7.1/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/notebook_data.py` & `dagster-1.7.1/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.1/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_job.py` & `dagster-1.7.1/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_partition.py` & `dagster-1.7.1/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_repository.py` & `dagster-1.7.1/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_schedule.py` & `dagster-1.7.1/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_api/snapshot_sensor.py` & `dagster-1.7.1/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_check/README.md` & `dagster-1.7.1/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_check/__init__.py` & `dagster-1.7.1/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/__init__.py` & `dagster-1.7.1/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/api.py` & `dagster-1.7.1/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/asset.py` & `dagster-1.7.1/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/code_server.py` & `dagster-1.7.1/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/config_scaffolder.py` & `dagster-1.7.1/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/debug.py` & `dagster-1.7.1/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/dev.py` & `dagster-1.7.1/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/instance.py` & `dagster-1.7.1/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/job.py` & `dagster-1.7.1/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/load_handle.py` & `dagster-1.7.1/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/project.py` & `dagster-1.7.1/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/run.py` & `dagster-1.7.1/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/schedule.py` & `dagster-1.7.1/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/sensor.py` & `dagster-1.7.1/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/utils.py` & `dagster-1.7.1/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.1/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/__init__.py` & `dagster-1.7.1/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/config_schema.py` & `dagster-1.7.1/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/config_type.py` & `dagster-1.7.1/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/errors.py` & `dagster-1.7.1/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/evaluate_value_result.py` & `dagster-1.7.1/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/field.py` & `dagster-1.7.1/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/field_utils.py` & `dagster-1.7.1/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/post_process.py` & `dagster-1.7.1/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/primitive_mapping.py` & `dagster-1.7.1/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.1/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.1/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/config.py` & `dagster-1.7.1/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.1/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.1/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/pydantic_compat_layer.py` & `dagster-1.7.1/dagster/_config/pythonic_config/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.1/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.1/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.1/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/snap.py` & `dagster-1.7.1/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/source.py` & `dagster-1.7.1/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/stack.py` & `dagster-1.7.1/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/traversal_context.py` & `dagster-1.7.1/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/type_printer.py` & `dagster-1.7.1/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_config/validate.py` & `dagster-1.7.1/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.1/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/assets.py` & `dagster-1.7.1/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/code_pointer.py` & `dagster-1.7.1/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/container_context/config.py` & `dagster-1.7.1/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/debug.py` & `dagster-1.7.1/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/decorator_utils.py` & `dagster-1.7.1/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/__init__.py` & `dagster-1.7.1/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.1/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.1/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.1/dagster/_core/definitions/asset_check_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 class AssetCheckSpec(
     NamedTuple(
         "_AssetCheckSpec",
         [
             ("name", PublicAttr[str]),
             ("asset_key", PublicAttr[AssetKey]),
             ("description", PublicAttr[Optional[str]]),
-            ("additional_deps", PublicAttr[Optional[Iterable["AssetDep"]]]),
+            ("additional_deps", PublicAttr[Iterable["AssetDep"]]),
             (
                 "blocking",  # intentionally not public, see https://github.com/dagster-io/dagster/issues/20659
                 bool,
             ),
             ("metadata", PublicAttr[Optional[Mapping[str, Any]]]),
         ],
     )
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.1/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import functools
 import hashlib
 from abc import ABC, abstractmethod, abstractproperty
+from dataclasses import dataclass
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Dict,
     FrozenSet,
     List,
     Mapping,
@@ -15,15 +16,14 @@
     Type,
     TypeVar,
     Union,
 )
 
 import pendulum
 
-import dagster._check as check
 from dagster._annotations import experimental
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
 from dagster._core.definitions.partition import AllPartitionsSubset
 from dagster._serdes.serdes import PackableValue, whitelist_for_serdes
 
 from ..asset_subset import AssetSubset, ValidAssetSubset
@@ -303,17 +303,16 @@
         return self.evaluation.asset_key
 
     @property
     def num_requested(self) -> int:
         return self.evaluation.true_subset.size
 
 
-# Adding the NamedTuple inheritance to avoid bugs with the experimental decorator and subclasses.
 @experimental
-class AssetCondition(NamedTuple("_AssetCondition", []), ABC):
+class AssetCondition(ABC):
     """An AssetCondition represents some state of the world that can influence if an asset
     partition should be materialized or not. AssetConditions can be combined to create
     new conditions using the `&` (and), `|` (or), and `~` (not) operators.
 
     Examples:
         .. code-block:: python
 
@@ -340,25 +339,25 @@
     @abstractproperty
     def description(self) -> str:
         raise NotImplementedError()
 
     def __and__(self, other: "AssetCondition") -> "AssetCondition":
         # group AndAssetConditions together
         if isinstance(self, AndAssetCondition):
-            return AndAssetCondition(children=[*self.children, other])
-        return AndAssetCondition(children=[self, other])
+            return AndAssetCondition(operands=[*self.operands, other])
+        return AndAssetCondition(operands=[self, other])
 
     def __or__(self, other: "AssetCondition") -> "AssetCondition":
         # group OrAssetConditions together
         if isinstance(self, OrAssetCondition):
-            return OrAssetCondition(children=[*self.children, other])
-        return OrAssetCondition(children=[self, other])
+            return OrAssetCondition(operands=[*self.operands, other])
+        return OrAssetCondition(operands=[self, other])
 
     def __invert__(self) -> "AssetCondition":
-        return NotAssetCondition(children=[self])
+        return NotAssetCondition(operand=self)
 
     @property
     def is_legacy(self) -> bool:
         """Returns if this condition is in the legacy format. This is used to determine if we can
         do certain types of backwards-compatible operations on it.
         """
         return (
@@ -441,20 +440,21 @@
 
         return ~RuleCondition(
             AutoMaterializeRule.skip_on_not_all_parents_updated_since_cron(cron_schedule, timezone)
         )
 
 
 @experimental
-class RuleCondition(  # type: ignore # related to AssetCondition being experimental
-    NamedTuple("_RuleCondition", [("rule", "AutoMaterializeRule")]),
-    AssetCondition,
-):
+@whitelist_for_serdes
+@dataclass(frozen=True)
+class RuleCondition(AssetCondition):
     """This class represents the condition that a particular AutoMaterializeRule is satisfied."""
 
+    rule: "AutoMaterializeRule"
+
     @property
     def unique_id(self) -> str:
         parts = [self.rule.__class__.__name__, self.description]
         return hashlib.md5("".join(parts).encode()).hexdigest()
 
     @property
     def description(self) -> str:
@@ -469,20 +469,25 @@
             f"Rule returned {evaluation_result.true_subset.size} partitions "
             f"({evaluation_result.end_timestamp - evaluation_result.start_timestamp:.2f} seconds)"
         )
         return evaluation_result
 
 
 @experimental
-class AndAssetCondition(  # type: ignore # related to AssetCondition being experimental
-    NamedTuple("_AndAssetCondition", [("children", Sequence[AssetCondition])]),
-    AssetCondition,
-):
+@whitelist_for_serdes
+@dataclass(frozen=True)
+class AndAssetCondition(AssetCondition):
     """This class represents the condition that all of its children evaluate to true."""
 
+    operands: Sequence[AssetCondition]
+
+    @property
+    def children(self) -> Sequence[AssetCondition]:
+        return self.operands
+
     @property
     def description(self) -> str:
         return "All of"
 
     def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
         child_results: List[AssetConditionResult] = []
         true_subset = context.candidate_subset
@@ -491,20 +496,25 @@
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_subset &= child_result.true_subset
         return AssetConditionResult.create_from_children(context, true_subset, child_results)
 
 
 @experimental
-class OrAssetCondition(  # type: ignore # related to AssetCondition being experimental
-    NamedTuple("_OrAssetCondition", [("children", Sequence[AssetCondition])]),
-    AssetCondition,
-):
+@whitelist_for_serdes
+@dataclass(frozen=True)
+class OrAssetCondition(AssetCondition):
     """This class represents the condition that any of its children evaluate to true."""
 
+    operands: Sequence[AssetCondition]
+
+    @property
+    def children(self) -> Sequence[AssetCondition]:
+        return self.operands
+
     @property
     def description(self) -> str:
         return "Any of"
 
     def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
         child_results: List[AssetConditionResult] = []
         true_subset = context.empty_subset()
@@ -515,33 +525,30 @@
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_subset |= child_result.true_subset
         return AssetConditionResult.create_from_children(context, true_subset, child_results)
 
 
 @experimental
-class NotAssetCondition(  # type: ignore # related to AssetCondition being experimental
-    NamedTuple("_NotAssetCondition", [("children", Sequence[AssetCondition])]),
-    AssetCondition,
-):
+@whitelist_for_serdes
+@dataclass(frozen=True)
+class NotAssetCondition(AssetCondition):
     """This class represents the condition that none of its children evaluate to true."""
 
-    def __new__(cls, children: Sequence[AssetCondition]):
-        check.invariant(len(children) == 1)
-        return super().__new__(cls, children)
+    operand: AssetCondition
 
     @property
     def description(self) -> str:
         return "Not"
 
     @property
-    def child(self) -> AssetCondition:
-        return self.children[0]
+    def children(self) -> Sequence[AssetCondition]:
+        return [self.operand]
 
     def evaluate(self, context: "AssetConditionEvaluationContext") -> AssetConditionResult:
         child_context = context.for_child(
-            condition=self.child, candidate_subset=context.candidate_subset
+            condition=self.operand, candidate_subset=context.candidate_subset
         )
-        child_result = self.child.evaluate(child_context)
+        child_result = self.operand.evaluate(child_context)
         true_subset = context.candidate_subset - child_result.true_subset
 
         return AssetConditionResult.create_from_children(context, true_subset, [child_result])
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.1/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.1/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.1/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.1/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.1/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.1/dagster/_core/definitions/asset_graph_differ.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         AssetKey,
     )
 
 
 class ChangeReason(Enum):
     NEW = "NEW"
     CODE_VERSION = "CODE_VERSION"
-    INPUTS = "INPUTS"
+    DEPENDENCIES = "DEPENDENCIES"
     PARTITIONS_DEFINITION = "PARTITIONS_DEFINITION"
 
 
 def _get_external_repo_from_context(
     context: BaseWorkspaceRequestContext, code_location_name: str, repository_name: str
 ) -> Optional[ExternalRepository]:
     """Returns the ExternalRepository specified by the code location name and repository name
@@ -126,23 +126,23 @@
         ):
             changes.append(ChangeReason.CODE_VERSION)
 
         if (
             self.branch_asset_graph.get(asset_key).parent_keys
             != self.base_asset_graph.get(asset_key).parent_keys
         ):
-            changes.append(ChangeReason.INPUTS)
+            changes.append(ChangeReason.DEPENDENCIES)
         else:
-            # if the set of inputs is different, then we don't need to check if the partition mappings
-            # for inputs have changed since ChangeReason.INPUTS is already in the list of changes
+            # if the set of upstream dependencies is different, then we don't need to check if the partition mappings
+            # for dependencies have changed since ChangeReason.DEPENDENCIES is already in the list of changes
             for upstream_asset in self.branch_asset_graph.get(asset_key).parent_keys:
                 if self.branch_asset_graph.get_partition_mapping(
                     asset_key, upstream_asset
                 ) != self.base_asset_graph.get_partition_mapping(asset_key, upstream_asset):
-                    changes.append(ChangeReason.INPUTS)
+                    changes.append(ChangeReason.DEPENDENCIES)
                     break
 
         if (
             self.branch_asset_graph.get(asset_key).partitions_def
             != self.base_asset_graph.get(asset_key).partitions_def
         ):
             changes.append(ChangeReason.PARTITIONS_DEFINITION)
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.1/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_in.py` & `dagster-1.7.1/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_job.py` & `dagster-1.7.1/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_key.py` & `dagster-1.7.1/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.1/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_out.py` & `dagster-1.7.1/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.1/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.1/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.1/dagster/_core/definitions/asset_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/assets.py` & `dagster-1.7.1/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.1/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,30 +294,30 @@
         )
         from .auto_materialize_rule import DiscardOnMaxMaterializationsExceededRule
 
         if self.asset_condition is not None:
             return self.asset_condition
 
         materialize_condition = OrAssetCondition(
-            children=[
+            operands=[
                 rule.to_asset_condition()
                 for rule in sorted(self.materialize_rules, key=lambda rule: rule.description)
             ]
         )
         skip_condition = OrAssetCondition(
-            children=[
+            operands=[
                 rule.to_asset_condition()
                 for rule in sorted(self.skip_rules, key=lambda rule: rule.description)
             ]
         )
         children = [
             materialize_condition,
-            NotAssetCondition([skip_condition]),
+            NotAssetCondition(skip_condition),
         ]
         if self.max_materializations_per_minute:
             discard_condition = DiscardOnMaxMaterializationsExceededRule(
                 self.max_materializations_per_minute
             ).to_asset_condition()
-            children.append(NotAssetCondition([discard_condition]))
+            children.append(NotAssetCondition(discard_condition))
 
         # results in an expression of the form (m1 | m2 | ... | mn) & ~(s1 | s2 | ... | sn) & ~d
         return AndAssetCondition(children)
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.1/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.1/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.1/dagster/_core/definitions/base_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.1/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/composition.py` & `dagster-1.7.1/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/config.py` & `dagster-1.7.1/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/configurable.py` & `dagster-1.7.1/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/data_time.py` & `dagster-1.7.1/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/data_version.py` & `dagster-1.7.1/dagster/_core/definitions/data_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -529,16 +529,14 @@
                 if not provenance.has_input_asset(dep_key.asset_key):
                     yield StaleCause(
                         key,
                         StaleCauseCategory.DEPENDENCIES,
                         f"has a new dependency on {dep_key.asset_key.to_user_string()}",
                         dep_key,
                     )
-                # Currently we exclude assets downstream of AllPartitionMappings from stale
-                # status logic due to potentially huge numbers of dependencies.
                 elif self._is_dep_updated(provenance, dep_key):
                     report_data_version = (
                         dep_asset.code_version is not None
                         or self._is_current_data_version_user_provided(key=dep_key)
                     )
                     yield StaleCause(
                         key,
@@ -690,43 +688,50 @@
             ancestors = self.asset_graph.get_ancestor_asset_keys(key.asset_key, include_self=True)
             self.instance_queryer.prefetch_asset_records(ancestors)
         return self.instance_queryer.get_latest_materialization_or_observation_record(
             asset_partition=key
         )
 
     # If a partition has greater than or equal to SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD
-    # of dependencies, it is not included in partition_deps. This is for performance reasons. This
-    # constraint can be removed when we have thoroughly tested performance for large upstream
-    # partition counts. At that time, the body of this method can just be replaced with a call to
-    # `asset_graph.get_parents_partitions`, which the logic here largely replicates.
+    # of dependencies, or is downstream of a time window partition with an AllPartitionsMapping,
+    # it is not included in partition_deps. This is for performance reasons. Besides this, the
+    # logic here largely replicates `asset_graph.get_parents_partitions`.
     #
-    # If an asset is self-dependent and has greater than or equal to
+    # Similarly, If an asset is self-dependent and has greater than or equal to
     # SKIP_PARTITION_DATA_VERSION_SELF_DEPENDENCY_THRESHOLD partitions, we don't check the
     # self-edge for updated data or propagate other stale causes through the edge. That is because
     # the current logic will recurse to the first partition, potentially throwing a recursion error.
-    # This constraint can be removed when we have thoroughly tested performance for large partition
-    # counts on self-dependent assets.
     @cached_method
     def _get_partition_dependencies(
         self, *, key: "AssetKeyPartitionKey"
     ) -> Sequence["AssetKeyPartitionKey"]:
+        from dagster import AllPartitionMapping
         from dagster._core.definitions.events import (
             AssetKeyPartitionKey,
         )
+        from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 
         asset_deps = self.asset_graph.get(key.asset_key).parent_keys
 
         deps = []
         for dep_asset_key in asset_deps:
-            if not self.asset_graph.get(dep_asset_key).is_partitioned:
+            dep_asset = self.asset_graph.get(dep_asset_key)
+            if not dep_asset.is_partitioned:
                 deps.append(AssetKeyPartitionKey(dep_asset_key, None))
             elif key.asset_key == dep_asset_key and self._exceeds_self_partition_limit(
                 key.asset_key
             ):
                 continue
+            elif isinstance(
+                dep_asset.partitions_def, TimeWindowPartitionsDefinition
+            ) and isinstance(
+                self.asset_graph.get_partition_mapping(key.asset_key, dep_asset_key),
+                AllPartitionMapping,
+            ):
+                continue
             else:
                 upstream_partition_keys = list(
                     self.asset_graph.get_parent_partition_keys_for_child(
                         key.partition_key,
                         dep_asset_key,
                         key.asset_key,
                         dynamic_partitions_store=self._instance,
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,16 +712,28 @@
                 fn,
                 ins or {},
                 deps=(
                     {dep.asset_key for dep in upstream_asset_deps} if upstream_asset_deps else set()
                 ),
             )
             output_tuples_by_asset_key = build_asset_outs(asset_out_map)
+
+            # validate that the asset_ins are a subset of the upstream asset_deps.
+            upstream_internal_asset_keys = set().union(*asset_deps.values())
+            asset_in_keys = set(asset_ins.keys())
+            if asset_deps and not asset_in_keys.issubset(upstream_internal_asset_keys):
+                invalid_asset_in_keys = asset_in_keys - upstream_internal_asset_keys
+                check.failed(
+                    f"Invalid asset dependencies: `{invalid_asset_in_keys}` specified as asset"
+                    " inputs, but are not specified in `internal_asset_deps`. Asset inputs must"
+                    " be associated with an output produced by the asset."
+                )
+
             # validate that the asset_deps make sense
-            valid_asset_deps = set(asset_ins.keys()) | set(output_tuples_by_asset_key.keys())
+            valid_asset_deps = asset_in_keys | set(output_tuples_by_asset_key.keys())
             for out_name, asset_keys in asset_deps.items():
                 if asset_out_map and out_name not in asset_out_map:
                     check.failed(
                         f"Invalid out key '{out_name}' supplied to `internal_asset_deps` argument"
                         f" for multi-asset {op_name}. Must be one of the outs for this multi-asset"
                         f" {list(asset_out_map.keys())[:20]}.",
                     )
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.1/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.1/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.1/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/dependency.py` & `dagster-1.7.1/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/events.py` & `dagster-1.7.1/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/external_asset.py` & `dagster-1.7.1/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_checks/last_update.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_checks/last_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 from dagster._annotations import experimental
 from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
 
 from ..asset_checks import AssetChecksDefinition
 from ..assets import AssetsDefinition, SourceAsset
 from ..events import CoercibleToAssetKey
+from .shared_builder import build_freshness_checks_for_assets
 from .utils import (
     DEFAULT_FRESHNESS_SEVERITY,
     DEFAULT_FRESHNESS_TIMEZONE,
-    build_freshness_checks_for_assets,
 )
 
 
 @experimental
 def build_last_update_freshness_checks(
     *,
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
@@ -46,14 +46,24 @@
     the most recently passed deadline, which is yesterday.
     Let's say I have an observable source asset on a data source which I expect should never be more
     than 3 hours out of date. In this case, there's no fixed schedule for when the data should be
     updated, so I would not provide a `deadline_cron`. Instead, I would set the `lower_bound_delta`
     parameter to "3 hours". This would mean that the check will expect the most recent observation
     record to indicate data no older than 3 hours, relative to the current time, regardless of when it runs.
 
+    The check result will contain the following metadata:
+    "dagster/freshness_params": A dictionary containing the parameters used to construct the
+    check
+    "dagster/last_updated_time": The time of the most recent update to the asset
+    "dagster/overdue_seconds": (Only present if asset is overdue) The number of seconds that the
+    asset is overdue by.
+    "dagster/overdue_deadline_timestamp": The timestamp that we are expecting the asset to have
+    arrived by. In the case of a provided deadline_cron, this is the timestamp of the most recent
+    tick of the cron schedule. In the case of no deadline_cron, this is the current time.
+
     Examples:
         .. code-block:: python
 
             # Example 1: Assets that are expected to be updated every day within 45 minutes of
             # 9:00 AM UTC
             from dagster import build_last_update_freshness_checks, AssetKey
             from .somewhere import my_daily_scheduled_assets_def
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_checks/sensor.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_checks/time_partition.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_checks/time_partition.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from dagster._annotations import experimental
 from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 
 from ..asset_checks import AssetChecksDefinition
 from ..assets import AssetsDefinition, SourceAsset
 from ..events import CoercibleToAssetKey
+from .shared_builder import build_freshness_checks_for_assets
 from .utils import (
     DEFAULT_FRESHNESS_SEVERITY,
     DEFAULT_FRESHNESS_TIMEZONE,
-    build_freshness_checks_for_assets,
 )
 
 
 @experimental
 def build_time_partition_freshness_checks(
     *,
     assets: Sequence[Union[SourceAsset, CoercibleToAssetKey, AssetsDefinition]],
@@ -43,14 +43,24 @@
 
     The timestamp of an observation record is the timestamp indicated by the
     "dagster/last_updated_timestamp" metadata key. The timestamp of a materialization record is the
     timestamp at which that record was created.
 
     The check will fail at runtime if a non-time-window partitioned asset is passed in.
 
+    The check result will contain the following metadata:
+    "dagster/freshness_params": A dictionary containing the parameters used to construct the
+    check.
+    "dagster/last_updated_time": (Only present if the asset has been observed/materialized before)
+    The time of the most recent update to the asset.
+    "dagster/overdue_seconds": (Only present if asset is overdue) The number of seconds that the
+    asset is overdue by.
+    "dagster/overdue_deadline_timestamp": The timestamp that we are expecting the asset to have
+    arrived by. This is the timestamp of the most recent tick of the cron schedule.
+
     Examples:
         .. code-block:: python
 
             from dagster import build_time_partition_freshness_checks, AssetKey
             # A daily partitioned asset that is expected to be updated every day within 45 minutes
             # of 9:00 AM UTC
             from .somewhere import my_daily_scheduled_assets_def
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.1/dagster/_core/execution/submit_asset_runs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,391 +1,333 @@
-import datetime
-import hashlib
-from typing import Callable, Iterable, Iterator, Optional, Sequence, Union, cast
-
-import pendulum
-
-from dagster import _check as check
-from dagster._core.definitions.asset_check_result import AssetCheckResult
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
-from dagster._core.definitions.asset_checks import AssetChecksDefinition
-from dagster._core.definitions.decorators.asset_check_decorator import (
-    multi_asset_check,
-)
-from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
-from dagster._core.event_api import AssetRecordsFilter, EventLogRecord
-from dagster._core.events import DagsterEventType
-from dagster._core.execution.context.compute import (
-    AssetCheckExecutionContext,
+import logging
+import time
+from typing import Dict, Iterator, List, NamedTuple, Optional, Sequence, Tuple, cast
+
+import dagster._check as check
+from dagster._core.definitions.asset_job import is_base_asset_job_name
+from dagster._core.definitions.events import AssetKey
+from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
+from dagster._core.definitions.run_request import RunRequest
+from dagster._core.definitions.selector import JobSubsetSelector
+from dagster._core.errors import (
+    DagsterCodeLocationLoadError,
+    DagsterInvalidSubsetError,
+    DagsterUserCodeUnreachableError,
 )
 from dagster._core.instance import DagsterInstance
-from dagster._utils.schedules import get_latest_completed_cron_tick, is_valid_cron_string
+from dagster._core.remote_representation import ExternalExecutionPlan, ExternalJob
+from dagster._core.snap import ExecutionPlanSnapshot
+from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
+from dagster._core.workspace.context import BaseWorkspaceRequestContext, IWorkspaceProcessContext
+from dagster._utils import SingleInstigatorDebugCrashFlags, check_for_debug_crash, hash_collection
 
-from ..assets import AssetsDefinition, SourceAsset
-from ..events import AssetKey, CoercibleToAssetKey
+EXECUTION_PLAN_CREATION_RETRIES = 1
 
-DEFAULT_FRESHNESS_SEVERITY = AssetCheckSeverity.WARN
-DEFAULT_FRESHNESS_TIMEZONE = "UTC"
-LOWER_BOUND_DELTA_METADATA_KEY = "dagster/lower_bound_delta"
-DEADLINE_CRON_METADATA_KEY = "dagster/deadline_cron"
-FRESHNESS_TIMEZONE_METADATA_KEY = "dagster/freshness_timezone"
-LAST_UPDATED_TIMESTAMP_METADATA_KEY = "dagster/last_updated_timestamp"
-FRESHNESS_PARAMS_METADATA_KEY = "dagster/freshness_params"
-
-
-def ensure_no_duplicate_assets(
-    assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
-) -> None:
-    """Finds duplicate assets in the provided list of assets, and errors if any are present.
 
-    Args:
-        assets (Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]): The assets to check for duplicates.
+class RunRequestExecutionData(NamedTuple):
+    external_job: ExternalJob
+    external_execution_plan: ExternalExecutionPlan
+    partitions_def: Optional[PartitionsDefinition]
 
-    Returns:
-        Sequence[AssetKey]: A list of the duplicate assets.
-    """
-    asset_keys = [
-        asset_key for asset in assets for asset_key in list(asset_to_keys_iterable(asset))
-    ]
-    duplicate_assets = [asset_key for asset_key in asset_keys if asset_keys.count(asset_key) > 1]
-    check.invariant(
-        len(duplicate_assets) == 0,
-        f"Found duplicate assets in the provided list of assets: {duplicate_assets}. Please ensure that each asset is unique.",
-    )
 
+def _get_implicit_job_name_for_assets(
+    asset_graph: RemoteAssetGraph, asset_keys: Sequence[AssetKey]
+) -> Optional[str]:
+    job_names = set(asset_graph.get_materialization_job_names(asset_keys[0]))
+    for asset_key in asset_keys[1:]:
+        job_names &= set(asset_graph.get_materialization_job_names(asset_key))
+
+    return next(job_name for job_name in job_names if is_base_asset_job_name(job_name))
+
+
+def _execution_plan_targets_asset_selection(
+    execution_plan_snapshot: ExecutionPlanSnapshot, asset_selection: Sequence[AssetKey]
+) -> bool:
+    output_asset_keys = set()
+    for step in execution_plan_snapshot.steps:
+        if step.key in execution_plan_snapshot.step_keys_to_execute:
+            for output in step.outputs:
+                asset_key = check.not_none(output.properties).asset_key
+                if asset_key:
+                    output_asset_keys.add(asset_key)
+    return all(key in output_asset_keys for key in asset_selection)
+
+
+def _get_job_execution_data_from_run_request(
+    asset_graph: RemoteAssetGraph,
+    run_request: RunRequest,
+    instance: DagsterInstance,
+    workspace: BaseWorkspaceRequestContext,
+    run_request_execution_data_cache: Dict[int, RunRequestExecutionData],
+) -> RunRequestExecutionData:
+    repo_handle = asset_graph.get_repository_handle(
+        cast(Sequence[AssetKey], run_request.asset_selection)[0]
+    )
+    location_name = repo_handle.code_location_origin.location_name
+    job_name = _get_implicit_job_name_for_assets(
+        asset_graph, cast(Sequence[AssetKey], run_request.asset_selection)
+    )
+    if job_name is None:
+        check.failed(
+            "Could not find an implicit asset job for the given assets:"
+            f" {run_request.asset_selection}"
+        )
 
-def asset_to_keys_iterable(
-    asset: Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset],
-) -> Iterator[AssetKey]:
-    """Converts the provided asset construct to a sequence of AssetKeys.
+    if not run_request.asset_selection:
+        check.failed("Expected RunRequest to have an asset selection")
 
-    Args:
-        asset (Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]): The asset to convert to a sequence of AssetKeys.
+    pipeline_selector = JobSubsetSelector(
+        location_name=location_name,
+        repository_name=repo_handle.repository_name,
+        job_name=job_name,
+        asset_selection=run_request.asset_selection,
+        asset_check_selection=run_request.asset_check_keys,
+        op_selection=None,
+    )
+
+    selector_id = hash_collection(pipeline_selector)
+
+    if selector_id not in run_request_execution_data_cache:
+        code_location = workspace.get_code_location(repo_handle.code_location_origin.location_name)
+        external_job = code_location.get_external_job(pipeline_selector)
+
+        external_execution_plan = code_location.get_external_execution_plan(
+            external_job,
+            {},
+            step_keys_to_execute=None,
+            known_state=None,
+            instance=instance,
+        )
 
-    Returns:
-        Sequence[AssetKey]: A sequence of AssetKeys.
-    """
-    if isinstance(asset, AssetsDefinition):
-        yield from asset.keys
-    elif isinstance(asset, SourceAsset):
-        yield asset.key
-    else:
-        yield AssetKey.from_coercible_or_definition(asset)
+        partitions_def = code_location.get_asset_job_partitions_def(external_job)
 
+        run_request_execution_data_cache[selector_id] = RunRequestExecutionData(
+            external_job,
+            external_execution_plan,
+            partitions_def,
+        )
 
-def ensure_no_duplicate_asset_checks(
-    asset_checks: Sequence[AssetChecksDefinition],
-) -> None:
-    asset_check_keys = [
-        asset_check_key
-        for asset_check in asset_checks
-        for asset_check_key in asset_check.check_keys
-    ]
-    duplicate_asset_checks = [
-        asset_check_key
-        for asset_check_key in asset_check_keys
-        if asset_check_keys.count(asset_check_key) > 1
-    ]
-    check.invariant(
-        len(duplicate_asset_checks) == 0,
-        f"Found duplicate asset checks in the provided list of asset checks: {duplicate_asset_checks}. Please ensure that each provided asset check is unique.",
-    )
+    return run_request_execution_data_cache[selector_id]
 
 
-def retrieve_latest_record(
+def _create_asset_run(
+    run_id: Optional[str],
+    run_request: RunRequest,
+    run_request_index: int,
     instance: DagsterInstance,
-    asset_key: AssetKey,
-    partition_key: Optional[str],
-) -> Optional[EventLogRecord]:
-    """Retrieve the latest materialization or observation record for the given asset.
-
-    If the asset is partitioned, the latest record for the latest partition will be returned.
+    run_request_execution_data_cache: Dict[int, RunRequestExecutionData],
+    asset_graph: RemoteAssetGraph,
+    workspace_process_context: IWorkspaceProcessContext,
+    debug_crash_flags: SingleInstigatorDebugCrashFlags,
+    logger: logging.Logger,
+) -> DagsterRun:
+    """Creates a run on the instance for the given run request. Ensures that the created run results
+    in an ExecutionPlan that targets the given asset selection. If it does not, attempts to create
+    a valid ExecutionPlan by reloading the workspace.
     """
-    materializations = instance.fetch_materializations(
-        records_filter=AssetRecordsFilter(
-            asset_key=asset_key, asset_partitions=[partition_key] if partition_key else None
-        ),
-        limit=1,
-    )
-    observations = instance.fetch_observations(
-        records_filter=AssetRecordsFilter(
-            asset_key=asset_key, asset_partitions=[partition_key] if partition_key else None
-        ),
-        limit=1,
-    )
-    if materializations.records and observations.records:
-        return max(
-            materializations.records[0],
-            observations.records[0],
-            key=lambda record: retrieve_timestamp_from_record(record),
-        )
-    else:
-        return (
-            materializations.records[0]
-            if materializations.records
-            else observations.records[0]
-            if observations.records
-            else None
-        )
-
-
-def retrieve_timestamp_from_record(asset_record: EventLogRecord) -> float:
-    """Retrieve the timestamp from the given materialization or observation record."""
-    check.inst_param(asset_record, "asset_record", EventLogRecord)
-    if asset_record.event_log_entry.dagster_event_type == DagsterEventType.ASSET_MATERIALIZATION:
-        return asset_record.timestamp
-    else:
-        metadata = check.not_none(asset_record.asset_observation).metadata
-        value = metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY].value
-        check.invariant(
-            isinstance(value, float),
-            f"Unexpected metadata value type for '{LAST_UPDATED_TIMESTAMP_METADATA_KEY}': "
-            f"{type(metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY])}",
-        )
-        return cast(float, value)
-
+    from dagster._daemon.controller import RELOAD_WORKSPACE_INTERVAL
 
-def get_last_updated_timestamp(record: Optional[EventLogRecord]) -> Optional[float]:
-    if record is None:
-        return None
-    if record.asset_materialization is not None:
-        return record.timestamp
-    elif record.asset_observation is not None:
-        metadata_value = record.asset_observation.metadata.get("dagster/last_updated_timestamp")
-        if metadata_value is not None:
-            return check.float_param(metadata_value.value, "last_updated_timestamp")
-        else:
-            return None
-    else:
-        check.failed("Expected record to be an observation or materialization")
+    if not run_request.asset_selection:
+        check.failed("Expected RunRequest to have an asset selection")
 
-
-def ensure_freshness_checks(checks: Sequence[AssetChecksDefinition]) -> None:
-    for check_def in checks:
-        for check_spec in check_def.check_specs:
-            check.invariant(
-                check_spec.metadata and check_spec.metadata.get(FRESHNESS_PARAMS_METADATA_KEY),
-                f"Asset check {check_spec.key} didn't have expected metadata. Please ensure that the asset check is a freshness check.",
+    for _ in range(EXECUTION_PLAN_CREATION_RETRIES + 1):
+        try:
+            # create a new request context for each run in case the code location server
+            # is swapped out in the middle of the submission process
+            workspace = workspace_process_context.create_request_context()
+            execution_data = _get_job_execution_data_from_run_request(
+                asset_graph,
+                run_request,
+                instance,
+                workspace=workspace,
+                run_request_execution_data_cache=run_request_execution_data_cache,
             )
+            check_for_debug_crash(debug_crash_flags, "EXECUTION_PLAN_CREATED")
+            check_for_debug_crash(debug_crash_flags, f"EXECUTION_PLAN_CREATED_{run_request_index}")
 
-
-def get_last_update_time_lower_bound(
-    deadline_cron: Optional[str],
-    current_timestamp: float,
-    lower_bound_delta: datetime.timedelta,
-    timezone: str,
-) -> datetime.datetime:
-    """Get the lower bound of the last_update_time for the given cron schedule."""
-    current_time_in_freshness_tz = pendulum.from_timestamp(current_timestamp, tz=timezone)
-    if deadline_cron:
-        return (
-            check.not_none(
-                get_latest_completed_cron_tick(
-                    cron_string=deadline_cron,
-                    current_time=current_time_in_freshness_tz,
-                    timezone=timezone,
+            # retry until the execution plan targets the asset selection
+            if _execution_plan_targets_asset_selection(
+                execution_data.external_execution_plan.execution_plan_snapshot,
+                check.not_none(run_request.asset_selection),
+            ):
+                external_job = execution_data.external_job
+                external_execution_plan = execution_data.external_execution_plan
+                partitions_def = execution_data.partitions_def
+
+                run = instance.create_run(
+                    job_snapshot=external_job.job_snapshot,
+                    execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
+                    parent_job_snapshot=external_job.parent_job_snapshot,
+                    job_name=external_job.name,
+                    run_id=run_id,
+                    resolved_op_selection=None,
+                    op_selection=None,
+                    run_config={},
+                    step_keys_to_execute=None,
+                    tags=run_request.tags,
+                    root_run_id=None,
+                    parent_run_id=None,
+                    status=DagsterRunStatus.NOT_STARTED,
+                    external_job_origin=external_job.get_external_origin(),
+                    job_code_origin=external_job.get_python_origin(),
+                    asset_selection=frozenset(run_request.asset_selection),
+                    asset_check_selection=None,
+                    asset_job_partitions_def=partitions_def,
                 )
-            )
-            - lower_bound_delta
-        )
-    else:
-        return current_time_in_freshness_tz - lower_bound_delta
-
 
-def get_latest_complete_partition_key(
-    deadline_cron: Optional[str],
-    current_timestamp: float,
-    timezone: str,
-    partitions_def: Optional[TimeWindowPartitionsDefinition],
-) -> Optional[str]:
-    """Get the latest complete partition key for the given cron schedule."""
-    if not partitions_def:
-        return None
-    current_time_in_freshness_tz = pendulum.from_timestamp(current_timestamp, tz=timezone)
-    latest_cron_tick_time = check.not_none(
-        get_latest_completed_cron_tick(
-            cron_string=deadline_cron,
-            current_time=current_time_in_freshness_tz,
-            timezone=timezone,
+                return run
+        except DagsterInvalidSubsetError:
+            pass
+
+        logger.warning(
+            "Execution plan is out of sync with the workspace. Pausing run submission for "
+            f"{RELOAD_WORKSPACE_INTERVAL} to allow the execution plan to rebuild with the updated workspace."
         )
+        # Sleep for RELOAD_WORKSPACE_INTERVAL seconds since the workspace can be refreshed
+        # at most once every interval
+        time.sleep(RELOAD_WORKSPACE_INTERVAL)
+        # Clear the execution plan cache as this data is no longer valid
+        run_request_execution_data_cache = {}
+
+        # If the execution plan does not targets the asset selection, the asset graph
+        # likely is outdated and targeting the wrong job, refetch the asset
+        # graph from the workspace
+        workspace = workspace_process_context.create_request_context()
+        asset_graph = workspace.asset_graph
+
+    check.failed(
+        f"Failed to target asset selection {run_request.asset_selection} in run after retrying."
     )
-    latest_cron_tick_time_in_partitions_def_tz = pendulum.from_timestamp(
-        latest_cron_tick_time.timestamp(), tz=partitions_def.timezone
-    )
-    time_window = check.not_none(
-        partitions_def.get_prev_partition_window(latest_cron_tick_time_in_partitions_def_tz)
-    )
-    return partitions_def.get_partition_key_range_for_time_window(time_window).start
 
 
-def build_freshness_multi_check(
-    asset_keys: Sequence[AssetKey],
-    deadline_cron: Optional[str],
-    timezone: str,
-    severity: AssetCheckSeverity,
-    lower_bound_delta: datetime.timedelta,
-    asset_property_enforcement_lambda: Optional[Callable[[AssetsDefinition], bool]],
-) -> AssetChecksDefinition:
-    params_metadata = {}
-    if deadline_cron:
-        params_metadata[DEADLINE_CRON_METADATA_KEY] = deadline_cron
-        params_metadata[FRESHNESS_TIMEZONE_METADATA_KEY] = timezone
-    if lower_bound_delta:
-        params_metadata[LOWER_BOUND_DELTA_METADATA_KEY] = lower_bound_delta.total_seconds()
-
-    @multi_asset_check(
-        specs=[
-            AssetCheckSpec(
-                "freshness_check",
-                asset=asset_key,
-                metadata={FRESHNESS_PARAMS_METADATA_KEY: params_metadata},
-                description="Evaluates freshness for targeted asset.",
-            )
-            for asset_key in asset_keys
-        ],
-        can_subset=True,
-        name=f"freshness_check_{unique_id_from_asset_keys(asset_keys)}",
-    )
-    def the_check(context: AssetCheckExecutionContext) -> Iterable[AssetCheckResult]:
-        for check_key in context.selected_asset_check_keys:
-            asset_key = check_key.asset_key
-            if asset_property_enforcement_lambda:
-                asset_property_enforcement_lambda(
-                    context.job_def.asset_layer.asset_graph.get(check_key.asset_key).assets_def
-                )
-            current_timestamp = pendulum.now("UTC").timestamp()
+def submit_asset_run(
+    run_id: Optional[str],
+    run_request: RunRequest,
+    run_request_index: int,
+    instance: DagsterInstance,
+    workspace_process_context: IWorkspaceProcessContext,
+    asset_graph: RemoteAssetGraph,
+    run_request_execution_data_cache: Dict[int, RunRequestExecutionData],
+    debug_crash_flags: SingleInstigatorDebugCrashFlags,
+    logger: logging.Logger,
+) -> DagsterRun:
+    """Submits a run for a run request that targets an asset selection. If the run already exists,
+    submits the existing run. If the run does not exist, creates a new run and submits it, ensuring
+    that the created run targets the given asset selection.
+    """
+    check.invariant(not run_request.run_config, "Asset run requests have no custom run config")
+    asset_keys = check.not_none(run_request.asset_selection)
 
-            # Explicit call to partitions def here will be replaced with AssetSlice reference once it's available.
-            partitions_def = cast(
-                Optional[TimeWindowPartitionsDefinition],
-                context.job_def.asset_layer.asset_graph.get(asset_key).partitions_def,
-            )
-            check.invariant(
-                partitions_def is None
-                or isinstance(partitions_def, TimeWindowPartitionsDefinition),
-                "Expected partitions_def to be time-windowed.",
-            )
+    check.invariant(len(asset_keys) > 0)
 
-            last_update_time_lower_bound = get_last_update_time_lower_bound(
-                deadline_cron=deadline_cron,
-                timezone=timezone,
-                current_timestamp=current_timestamp,
-                lower_bound_delta=lower_bound_delta,
-            )
-            expected_partition_key = get_latest_complete_partition_key(
-                deadline_cron=deadline_cron,
-                current_timestamp=current_timestamp,
-                timezone=timezone,
-                partitions_def=partitions_def,
-            )
-            latest_record = retrieve_latest_record(
-                instance=context.instance, asset_key=asset_key, partition_key=expected_partition_key
-            )
-            update_timestamp = get_last_updated_timestamp(latest_record)
-            passed = (
-                update_timestamp is not None
-                and update_timestamp >= last_update_time_lower_bound.timestamp()
+    # check if the run already exists
+    existing_run = instance.get_run_by_id(run_id) if run_id else None
+    if existing_run:
+        if existing_run.status != DagsterRunStatus.NOT_STARTED:
+            logger.warn(
+                f"Run {run_id} already submitted on a previously interrupted tick, skipping"
             )
 
-            yield AssetCheckResult(
-                passed=passed,
-                description=get_description_for_freshness_check_result(
-                    passed,
-                    update_timestamp,
-                    last_update_time_lower_bound,
-                    current_timestamp,
-                    expected_partition_key,
-                ),
-                severity=severity,
-                asset_key=asset_key,
+            check_for_debug_crash(debug_crash_flags, "RUN_SUBMITTED")
+            check_for_debug_crash(debug_crash_flags, f"RUN_SUBMITTED_{run_request_index}")
+
+            return existing_run
+        else:
+            logger.warn(
+                f"Run {run_id} already created on a previously interrupted tick, submitting"
             )
+            run_to_submit = existing_run
+    else:
+        run_to_submit = _create_asset_run(
+            run_id,
+            run_request,
+            run_request_index,
+            instance,
+            run_request_execution_data_cache,
+            asset_graph,
+            workspace_process_context,
+            debug_crash_flags,
+            logger,
+        )
 
-    return the_check
+    check_for_debug_crash(debug_crash_flags, "RUN_CREATED")
+    check_for_debug_crash(debug_crash_flags, f"RUN_CREATED_{run_request_index}")
 
+    instance.submit_run(run_to_submit.run_id, workspace_process_context.create_request_context())
 
-def get_description_for_freshness_check_result(
-    passed: bool,
-    update_timestamp: Optional[float],
-    last_update_time_lower_bound: datetime.datetime,
-    current_timestamp: float,
-    expected_partition_key: Optional[str],
-) -> str:
-    check.invariant(
-        (passed and update_timestamp is not None) or not passed,
-        "Should not be possible for check to pass without an update to the asset.",
-    )
-    update_time_delta_str = (
-        seconds_in_words(current_timestamp - update_timestamp) if update_timestamp else None
-    )
-    last_update_time_lower_bound_delta_str = seconds_in_words(
-        current_timestamp - last_update_time_lower_bound.timestamp()
-    )
-    return (
-        f"Partition {expected_partition_key} is fresh. Expected the partition to arrive within the last {last_update_time_lower_bound_delta_str}, and it arrived {update_time_delta_str} ago."
-        if passed and expected_partition_key
-        else f"Partition {expected_partition_key} is overdue. Expected the partition to arrive within the last {last_update_time_lower_bound_delta_str}."
-        if not passed and expected_partition_key
-        else f"Asset is fresh. Expected an update within the last {last_update_time_lower_bound_delta_str}, and found an update {update_time_delta_str} ago."
-        if passed and update_timestamp
-        else f"Asset is overdue. Expected an update within the last {last_update_time_lower_bound_delta_str}."
-    )
+    check_for_debug_crash(debug_crash_flags, "RUN_SUBMITTED")
+    check_for_debug_crash(debug_crash_flags, f"RUN_SUBMITTED_{run_request_index}")
 
+    asset_key_str = ", ".join([asset_key.to_user_string() for asset_key in asset_keys])
 
-def build_freshness_checks_for_assets(
-    assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
-    deadline_cron: Optional[str],
-    timezone: str,
-    severity: AssetCheckSeverity,
-    asset_property_enforcement_lambda: Optional[Callable[[AssetsDefinition], bool]] = None,
-    lower_bound_delta: datetime.timedelta = datetime.timedelta(minutes=0),
-) -> AssetChecksDefinition:
-    ensure_no_duplicate_assets(assets)
-    deadline_cron = check.opt_str_param(deadline_cron, "deadline_cron")
-    check.invariant(
-        is_valid_cron_string(deadline_cron) if deadline_cron else True,
-        "deadline_cron must be a valid cron string.",
-    )
-    severity = check.inst_param(severity, "severity", AssetCheckSeverity)
-    timezone = check.str_param(timezone, "timezone")
-    lower_bound_delta = check.inst_param(lower_bound_delta, "lower_bound_delta", datetime.timedelta)
-
-    return build_freshness_multi_check(
-        asset_keys=[asset_key for asset in assets for asset_key in asset_to_keys_iterable(asset)],
-        deadline_cron=deadline_cron,
-        timezone=timezone,
-        severity=severity,
-        lower_bound_delta=lower_bound_delta,
-        asset_property_enforcement_lambda=asset_property_enforcement_lambda,
+    logger.info(
+        f"Submitted run {run_to_submit.run_id} for assets {asset_key_str} with tags"
+        f" {run_request.tags}"
     )
 
+    return run_to_submit
 
-def seconds_in_words(delta: float) -> str:
-    """Converts the provided number of seconds to a human-readable string.
-
-    Return format is "X days, Y hours, Z minutes, A seconds".
-    """
-    days = int(delta // 86400)
-    hours = int(delta // 3600)
-    minutes = int((delta % 3600) // 60)
-    seconds = int(delta % 60)
-    return ", ".join(
-        filter(
-            None,
-            [
-                f"{days} days" if days else None,
-                f"{hours} hours" if hours else None,
-                f"{minutes} minutes" if minutes else None,
-                f"{seconds} seconds" if seconds else None,
-            ],
-        )
-    )
 
+class SubmitRunRequestChunkResult(NamedTuple):
+    chunk_submitted_runs: Sequence[Tuple[RunRequest, DagsterRun]]
+    retryable_error_raised: bool
 
-def unique_id_from_asset_keys(asset_keys: Sequence[AssetKey]) -> str:
-    """Generate a unique ID from the provided asset keys.
 
-    This is necessary to disambiguate between different ops underlying freshness checks without
-    forcing the user to provide a name for the underlying op.
+def submit_asset_runs_in_chunks(
+    run_requests: Sequence[RunRequest],
+    reserved_run_ids: Optional[Sequence[str]],
+    chunk_size: int,
+    instance: DagsterInstance,
+    workspace_process_context: IWorkspaceProcessContext,
+    asset_graph: RemoteAssetGraph,
+    debug_crash_flags: SingleInstigatorDebugCrashFlags,
+    logger: logging.Logger,
+    backfill_id: Optional[str] = None,
+) -> Iterator[Optional[SubmitRunRequestChunkResult]]:
+    """Submits runs for a sequence of run requests that target asset selections in chunks. Yields
+    None after each run is submitted to allow the daemon to heartbeat, and yields a list of tuples
+    of the run request and the submitted run after each chunk is submitted to allow the caller to
+    interrupt this process if needed.
     """
-    return hashlib.md5(",".join([str(asset_key) for asset_key in asset_keys]).encode()).hexdigest()[
-        :8
-    ]
+    if reserved_run_ids is not None:
+        check.invariant(len(run_requests) == len(reserved_run_ids))
+
+    run_request_execution_data_cache = {}
+    for chunk_start in range(0, len(run_requests), chunk_size):
+        run_request_chunk = run_requests[chunk_start : chunk_start + chunk_size]
+        chunk_submitted_runs: List[Tuple[RunRequest, DagsterRun]] = []
+        retryable_error_raised = False
+
+        logger.debug(f"{chunk_size}, {chunk_start}, {len(run_request_chunk)}")
+
+        # submit each run in the chunk
+        for chunk_idx, run_request in enumerate(run_request_chunk):
+            run_request_idx = chunk_start + chunk_idx
+            run_id = reserved_run_ids[run_request_idx] if reserved_run_ids else None
+            try:
+                submitted_run = submit_asset_run(
+                    run_id,
+                    run_request,
+                    run_request_idx,
+                    instance,
+                    workspace_process_context,
+                    asset_graph,
+                    run_request_execution_data_cache,
+                    debug_crash_flags,
+                    logger,
+                )
+                chunk_submitted_runs.append((run_request, submitted_run))
+                # allow the daemon to heartbeat while runs are submitted
+                yield None
+            except (DagsterUserCodeUnreachableError, DagsterCodeLocationLoadError) as e:
+                logger.warning(
+                    f"Unable to reach the user code server for assets {run_request.asset_selection}."
+                    f" Backfill {backfill_id} will resume execution once the server is available."
+                    f"User code server error: {e}"
+                )
+                retryable_error_raised = True
+                # Stop submitting runs if the user code server is unreachable for any
+                # given run request
+                break
+
+        yield SubmitRunRequestChunkResult(chunk_submitted_runs, retryable_error_raised)
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.1/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.1/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.1/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/inference.py` & `dagster-1.7.1/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/input.py` & `dagster-1.7.1/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.1/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/job_base.py` & `dagster-1.7.1/dagster/_core/definitions/job_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 from typing import TYPE_CHECKING, AbstractSet, Iterable, Optional
 
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.events import AssetKey
 
 if TYPE_CHECKING:
     from .job_definition import JobDefinition
+    from .repository_definition import RepositoryDefinition
 
 
 class IJob(ABC):
     """IJob is a wrapper interface for JobDefinitions to be used as parameters to Dagster's
     core execution APIs.  This enables these execution APIs to operate on both in memory job
     definitions to be executed in the current process (InMemoryJob) as well as definitions that
     can be reconstructed and executed in a different process (ReconstructableJob).
     """
 
     @abstractmethod
     def get_definition(self) -> "JobDefinition":
         pass
 
     @abstractmethod
+    def get_repository_definition(self) -> Optional["RepositoryDefinition"]:
+        pass
+
+    @abstractmethod
     def get_subset(
         self,
         *,
         op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         asset_check_selection: Optional[AbstractSet[AssetCheckKey]] = None,
     ) -> "IJob":
@@ -55,14 +60,17 @@
         job_def: "JobDefinition",
     ):
         self._job_def = job_def
 
     def get_definition(self) -> "JobDefinition":
         return self._job_def
 
+    def get_repository_definition(self) -> Optional["RepositoryDefinition"]:
+        return None
+
     def get_subset(
         self,
         *,
         op_selection: Optional[Iterable[str]] = None,
         asset_selection: Optional[AbstractSet[AssetKey]] = None,
         asset_check_selection: Optional[AbstractSet[AssetCheckKey]] = None,
     ) -> "InMemoryJob":
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/job_definition.py` & `dagster-1.7.1/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.1/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from importlib import import_module
 from types import ModuleType
-from typing import Iterable, Optional, Sequence, cast
+from typing import Iterable, Optional, Sequence, Set, cast
 
 import dagster._check as check
 from dagster._core.definitions.assets import AssetsDefinition
 
 from .asset_checks import AssetChecksDefinition, has_only_asset_checks
 from .asset_key import (
     CoercibleToAssetKeyPrefix,
@@ -16,18 +16,20 @@
     find_objects_in_module_of_types,
     prefix_assets,
 )
 
 
 def _checks_from_modules(modules: Iterable[ModuleType]) -> Sequence[AssetChecksDefinition]:
     checks = []
+    ids: Set[int] = set()
     for module in modules:
         for c in find_objects_in_module_of_types(module, AssetsDefinition):
-            if has_only_asset_checks(c):
+            if has_only_asset_checks(c) and id(c) not in ids:
                 checks.append(cast(AssetChecksDefinition, c))
+                ids.add(id(c))
     return checks
 
 
 def _checks_with_attributes(
     checks_defs: Sequence[AssetChecksDefinition],
     asset_key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
 ) -> Sequence[AssetChecksDefinition]:
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.1/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.1/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.1/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/materialize.py` & `dagster-1.7.1/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.1/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.1/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.1/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/node_container.py` & `dagster-1.7.1/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/node_definition.py` & `dagster-1.7.1/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/observe.py` & `dagster-1.7.1/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/op_definition.py` & `dagster-1.7.1/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.1/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/op_selection.py` & `dagster-1.7.1/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/output.py` & `dagster-1.7.1/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/partition.py` & `dagster-1.7.1/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.1/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.1/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.1/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/policy.py` & `dagster-1.7.1/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.1/dagster/_core/definitions/reconstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,19 +250,23 @@
         )
 
     def with_repository_load_data(
         self, metadata: Optional["RepositoryLoadData"]
     ) -> "ReconstructableJob":
         return self._replace(repository=self.repository.with_repository_load_data(metadata))
 
+    @lru_cache(maxsize=1)
+    def get_repository_definition(self) -> Optional["RepositoryDefinition"]:
+        return self.repository.get_definition()
+
     # Keep the most recent 1 definition (globally since this is a NamedTuple method)
     # This allows repeated calls to get_definition in execution paths to not reload the job
     @lru_cache(maxsize=1)
     def get_definition(self) -> "JobDefinition":
-        return self.repository.get_definition().get_maybe_subset_job_def(
+        return check.not_none(self.get_repository_definition()).get_maybe_subset_job_def(
             self.job_name,
             self.op_selection,
             self.asset_selection,
             self.asset_check_selection,
         )
 
     def get_reconstructable_repository(self) -> ReconstructableRepository:
```

### Comparing `dagster-1.7.0/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.1/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.1/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.1/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.1/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.1/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.1/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.1/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/result.py` & `dagster-1.7.1/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/run_config.py` & `dagster-1.7.1/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.1/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/run_request.py` & `dagster-1.7.1/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.1/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.1/dagster/_core/definitions/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.1/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/selector.py` & `dagster-1.7.1/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.1/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/source_asset.py` & `dagster-1.7.1/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.1/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/target.py` & `dagster-1.7.1/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.1/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.1/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.1/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/utils.py` & `dagster-1.7.1/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.1/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/errors.py` & `dagster-1.7.1/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/event_api.py` & `dagster-1.7.1/dagster/_core/event_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,14 +130,21 @@
     def asset_materialization(self) -> Optional[AssetMaterialization]:
         return self.event_log_entry.asset_materialization
 
     @property
     def asset_observation(self) -> Optional[AssetObservation]:
         return self.event_log_entry.asset_observation
 
+    @property
+    def event_type(self) -> DagsterEventType:
+        return check.not_none(
+            self.event_log_entry.dagster_event,
+            "Expected dagster_event property to be present if calling the event_type property",
+        ).event_type
+
 
 class EventRecordsResult(NamedTuple):
     """Return value for a query fetching event records from the instance.  Contains a list of event
     records, a cursor string, and a boolean indicating whether there are more records to fetch.
     """
 
     records: Sequence[EventLogRecord]
```

### Comparing `dagster-1.7.0/dagster/_core/events/__init__.py` & `dagster-1.7.1/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/events/log.py` & `dagster-1.7.1/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/events/utils.py` & `dagster-1.7.1/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/api.py` & `dagster-1.7.1/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.1/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/backfill.py` & `dagster-1.7.1/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/build_resources.py` & `dagster-1.7.1/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/compute_logs.py` & `dagster-1.7.1/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/compute.py` & `dagster-1.7.1/dagster/_core/execution/context/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     ExpectationResult,
     UserEvent,
 )
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
+from dagster._core.definitions.repository_definition.repository_definition import (
+    RepositoryDefinition,
+)
 from dagster._core.definitions.step_launcher import StepLauncher
 from dagster._core.definitions.time_window_partitions import TimeWindow
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidPropertyError,
     DagsterInvariantViolationError,
 )
@@ -92,14 +95,19 @@
     @property
     @abstractmethod
     def job_def(self) -> JobDefinition:
         """The job being executed."""
 
     @property
     @abstractmethod
+    def repository_def(self) -> RepositoryDefinition:
+        """The Dagster repository containing the job being executed."""
+
+    @property
+    @abstractmethod
     def run(self) -> DagsterRun:
         """The DagsterRun object corresponding to the execution."""
 
     @property
     @abstractmethod
     def resources(self) -> Any:
         """Resources available in the execution context."""
@@ -229,17 +237,22 @@
     def run_config(self) -> Mapping[str, object]:
         """dict: The run config for the current execution."""
         return self._step_execution_context.run_config
 
     @public
     @property
     def job_def(self) -> JobDefinition:
-        """JobDefinition: The currently executing pipeline."""
+        """JobDefinition: The currently executing job."""
         return self._step_execution_context.job_def
 
+    @property
+    def repository_def(self) -> RepositoryDefinition:
+        """RepositoryDefinition: The Dagster repository for the currently executing job."""
+        return self._step_execution_context.repository_def
+
     @public
     @property
     def job_name(self) -> str:
         """str: The name of the currently executing pipeline."""
         return self._step_execution_context.job_name
 
     @public
@@ -1437,14 +1450,19 @@
     def job_def(self) -> JobDefinition:
         """The definition for the currently executing job. Information like the job name, and job tags
         can be found on the JobDefinition.
         Returns: JobDefinition.
         """
         return self.op_execution_context.job_def
 
+    @property
+    def repository_def(self) -> RepositoryDefinition:
+        """RepositoryDefinition: The Dagster repository for the currently executing job."""
+        return self.op_execution_context.repository_def
+
     ######## Deprecated methods
 
     @deprecated(**_get_deprecation_kwargs("dagster_run"))
     @property
     @_copy_docs_from_op_execution_context
     def dagster_run(self) -> DagsterRun:
         return self.op_execution_context.dagster_run
@@ -1845,14 +1863,19 @@
     def job_def(self) -> JobDefinition:
         """The definition for the currently executing job. Information like the job name, and job tags
         can be found on the JobDefinition.
         Returns: JobDefinition.
         """
         return self.op_execution_context.job_def
 
+    @property
+    def repository_def(self) -> RepositoryDefinition:
+        """RepositoryDefinition: The Dagster repository for the currently executing job."""
+        return self.op_execution_context.repository_def
+
     #### check related
     @public
     @property
     @_copy_docs_from_op_execution_context
     def selected_asset_check_keys(self) -> AbstractSet[AssetCheckKey]:
         return self.op_execution_context.selected_asset_check_keys
```

### Comparing `dagster-1.7.0/dagster/_core/execution/context/hook.py` & `dagster-1.7.1/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/init.py` & `dagster-1.7.1/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/input.py` & `dagster-1.7.1/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/invocation.py` & `dagster-1.7.1/dagster/_core/execution/context/invocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     UserEvent,
 )
 from dagster._core.definitions.hook_definition import HookDefinition
 from dagster._core.definitions.job_definition import JobDefinition
 from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_definition import OpDefinition
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
+from dagster._core.definitions.repository_definition import RepositoryDefinition
 from dagster._core.definitions.resource_definition import (
     IContainsGenerator,
     ResourceDefinition,
     Resources,
     ScopedResourcesBuilder,
 )
 from dagster._core.definitions.resource_requirement import ensure_requirements_satisfied
@@ -442,14 +443,18 @@
         return run_config
 
     @property
     def job_def(self) -> JobDefinition:
         raise DagsterInvalidPropertyError(_property_msg("job_def", "property"))
 
     @property
+    def repository_def(self) -> RepositoryDefinition:
+        raise DagsterInvalidPropertyError(_property_msg("repository_def", "property"))
+
+    @property
     def job_name(self) -> str:
         raise DagsterInvalidPropertyError(_property_msg("job_name", "property"))
 
     @property
     def log(self) -> DagsterLogManager:
         """DagsterLogManager: A console manager constructed for this context."""
         return self._log
```

### Comparing `dagster-1.7.0/dagster/_core/execution/context/logger.py` & `dagster-1.7.1/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/output.py` & `dagster-1.7.1/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/context/system.py` & `dagster-1.7.1/dagster/_core/execution/context/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
 from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.partition_mapping import (
     PartitionMapping,
     infer_partition_mapping,
 )
 from dagster._core.definitions.policy import RetryPolicy
 from dagster._core.definitions.reconstruct import ReconstructableJob
+from dagster._core.definitions.repository_definition.repository_definition import (
+    RepositoryDefinition,
+)
 from dagster._core.definitions.resource_definition import ScopedResourcesBuilder
 from dagster._core.definitions.step_launcher import StepLauncher
 from dagster._core.definitions.time_window_partitions import (
     TimeWindow,
     TimeWindowPartitionsDefinition,
     has_one_dimension_time_window_partitioning,
 )
@@ -195,14 +198,15 @@
     This object contains information that requires access to user code, such as the pipeline
     definition and resources.
     """
 
     scoped_resources_builder: ScopedResourcesBuilder
     resolved_run_config: ResolvedRunConfig
     job_def: JobDefinition
+    repository_def: Optional[RepositoryDefinition]
 
 
 class IStepContext(IPlanContext):
     """Interface to represent data to be available during either step orchestration or execution."""
 
     @property
     @abstractmethod
@@ -344,14 +348,22 @@
         )
 
     @property
     def job_def(self) -> JobDefinition:
         return self._execution_data.job_def
 
     @property
+    def repository_def(self) -> RepositoryDefinition:
+        check.invariant(
+            self._execution_data.repository_def is not None,
+            "No repository definition was set on the step context",
+        )
+        return cast(RepositoryDefinition, self._execution_data.repository_def)
+
+    @property
     def resolved_run_config(self) -> ResolvedRunConfig:
         return self._execution_data.resolved_run_config
 
     @property
     def scoped_resources_builder(self) -> ScopedResourcesBuilder:
         return self._execution_data.scoped_resources_builder
 
@@ -624,14 +636,22 @@
         return self.op.definition
 
     @property
     def job_def(self) -> "JobDefinition":
         return self._execution_data.job_def
 
     @property
+    def repository_def(self) -> RepositoryDefinition:
+        check.invariant(
+            self._execution_data.repository_def is not None,
+            "No repository definition was set on the step context",
+        )
+        return cast(RepositoryDefinition, self._execution_data.repository_def)
+
+    @property
     def op(self) -> OpNode:
         return self.job_def.get_op(self._step.node_handle)
 
     @property
     def op_retry_policy(self) -> Optional[RetryPolicy]:
         return self.job_def.get_retry_policy_for_handle(self.node_handle)
 
@@ -1380,12 +1400,16 @@
 
     @public
     @property
     def job_def(self) -> "JobDefinition":
         """The underlying job definition being executed."""
         return super(DagsterTypeLoaderContext, self).job_def
 
+    @property
+    def repository_def(self) -> "RepositoryDefinition":
+        return super(DagsterTypeLoaderContext, self).repository_def
+
     @public
     @property
     def op_def(self) -> "OpDefinition":
         """The op for which type loading is occurring."""
         return super(DagsterTypeLoaderContext, self).op_def
```

### Comparing `dagster-1.7.0/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.1/dagster/_core/execution/context_creation_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     cast,
 )
 
 import dagster._check as check
 from dagster._core.definitions import ExecutorDefinition, JobDefinition
 from dagster._core.definitions.executor_definition import check_cross_process_constraints
 from dagster._core.definitions.job_base import IJob
+from dagster._core.definitions.repository_definition.repository_definition import (
+    RepositoryDefinition,
+)
 from dagster._core.definitions.resource_definition import ScopedResourcesBuilder
 from dagster._core.errors import DagsterError, DagsterUserCodeExecutionError
 from dagster._core.events import DagsterEvent, RunFailureReason
 from dagster._core.execution.memoization import validate_reexecution_memoization
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.execution.resources_init import (
     get_required_resource_keys_to_init,
@@ -90,14 +93,18 @@
     resource_keys_to_init: AbstractSet[str]
     execution_plan: ExecutionPlan
 
     @property
     def job_def(self) -> JobDefinition:
         return self.job.get_definition()
 
+    @property
+    def repository_def(self) -> Optional[RepositoryDefinition]:
+        return self.job.get_repository_definition()
+
 
 def create_context_creation_data(
     job: IJob,
     execution_plan: ExecutionPlan,
     run_config: Mapping[str, object],
     dagster_run: DagsterRun,
     instance: DagsterInstance,
@@ -135,14 +142,15 @@
     context_creation_data: "ContextCreationData",
     scoped_resources_builder: ScopedResourcesBuilder,
 ) -> ExecutionData:
     return ExecutionData(
         scoped_resources_builder=scoped_resources_builder,
         resolved_run_config=context_creation_data.resolved_run_config,
         job_def=context_creation_data.job_def,
+        repository_def=context_creation_data.repository_def,
     )
 
 
 TContextType = TypeVar("TContextType", bound=IPlanContext)
 
 
 class ExecutionContextManager(Generic[TContextType], ABC):
```

### Comparing `dagster-1.7.0/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.1/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.1/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/execution_result.py` & `dagster-1.7.1/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/host_mode.py` & `dagster-1.7.1/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/job_backfill.py` & `dagster-1.7.1/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.1/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/memoization.py` & `dagster-1.7.1/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/active.py` & `dagster-1.7.1/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/compute.py` & `dagster-1.7.1/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.1/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.1/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.1/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.1/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/handle.py` & `dagster-1.7.1/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.1/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.1/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.1/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/objects.py` & `dagster-1.7.1/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.1/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/plan.py` & `dagster-1.7.1/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/state.py` & `dagster-1.7.1/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/step.py` & `dagster-1.7.1/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/plan/utils.py` & `dagster-1.7.1/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.1/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.1/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/resources_init.py` & `dagster-1.7.1/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/retries.py` & `dagster-1.7.1/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.1/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/stats.py` & `dagster-1.7.1/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/tags.py` & `dagster-1.7.1/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.1/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.1/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/execution/with_resources.py` & `dagster-1.7.1/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/base.py` & `dagster-1.7.1/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.1/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/in_process.py` & `dagster-1.7.1/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/init.py` & `dagster-1.7.1/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/multiprocess.py` & `dagster-1.7.1/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.1/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.1/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/instance/__init__.py` & `dagster-1.7.1/dagster/_core/instance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Dict,
-    Final,
     Generic,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
     Set,
@@ -100,21 +99,14 @@
 # Our internal guts can handle empty strings for job name and run id
 # However making these named constants for documentation, to encode where we are making the assumption,
 # and to allow us to change this more easily in the future, provided we are disciplined about
 # actually using this constants.
 RUNLESS_RUN_ID = ""
 RUNLESS_JOB_NAME = ""
 
-# Sets the number of events that will be buffered before being written to the event log. Only
-# applies to explicitly batched events. Currently this defaults to 0, which turns off batching
-# entirely (multiple store_event calls are made instead of store_event_batch). This makes batching
-# opt-in.
-EVENT_BATCH_SIZE: Final = int(os.getenv("DAGSTER_EVENT_BATCH_SIZE", "0"))
-
-
 if TYPE_CHECKING:
     from dagster._core.debug import DebugRunPayload
     from dagster._core.definitions.asset_check_spec import AssetCheckKey
     from dagster._core.definitions.job_definition import (
         JobDefinition,
     )
     from dagster._core.definitions.partition import PartitionsDefinition
@@ -187,16 +179,27 @@
     from dagster._core.workspace.workspace import IWorkspace
     from dagster._daemon.types import DaemonHeartbeat, DaemonStatus
 
 
 DagsterInstanceOverrides: TypeAlias = Mapping[str, Any]
 
 
+# Sets the number of events that will be buffered before being written to the event log. Only
+# applies to explicitly batched events. Currently this defaults to 0, which turns off batching
+# entirely (multiple store_event calls are made instead of store_event_batch). This makes batching
+# opt-in.
+#
+# Note that we don't store the value in the constant so that it can be changed without a process
+# restart.
+def _get_event_batch_size() -> int:
+    return int(os.getenv("DAGSTER_EVENT_BATCH_SIZE", "0"))
+
+
 def _is_batch_writing_enabled() -> bool:
-    return EVENT_BATCH_SIZE > 0
+    return _get_event_batch_size() > 0
 
 
 def _check_run_equality(
     pipeline_run: DagsterRun, candidate_run: DagsterRun
 ) -> Mapping[str, Tuple[Any, Any]]:
     field_diff: Dict[str, Tuple[Any, Any]] = {}
     for field in pipeline_run._fields:
@@ -2381,29 +2384,29 @@
         batch_metadata: Optional["DagsterEventBatchMetadata"] = None,
     ) -> None:
         """Handle a new event by storing it and notifying subscribers.
 
         Events may optionally be sent with `batch_metadata`. If batch writing is enabled, then
         events sent with `batch_metadata` will not trigger an immediate write. Instead, they will be
         kept in a batch-specific buffer (identified by `batch_metadata.id`) until either the buffer
-        reaches the EVENT_BATCH_SIZE or the end of the batch is reached (signaled by
+        reaches the event batch size or the end of the batch is reached (signaled by
         `batch_metadata.is_end`). When this point is reached, all events in the buffer will be sent
         to the storage layer in a single batch. If an error occurrs during batch writing, then we
         fall back to iterative individual event writes.
 
         Args:
             event (EventLogEntry): The event to handle.
             batch_metadata (Optional[DagsterEventBatchMetadata]): Metadata for batch writing.
         """
         if batch_metadata is None or not _is_batch_writing_enabled():
             events = [event]
         else:
             batch_id, is_batch_end = batch_metadata.id, batch_metadata.is_end
             self._event_buffer[batch_id].append(event)
-            if is_batch_end or len(self._event_buffer[batch_id]) == EVENT_BATCH_SIZE:
+            if is_batch_end or len(self._event_buffer[batch_id]) == _get_event_batch_size():
                 events = self._event_buffer[batch_id]
                 del self._event_buffer[batch_id]
             else:
                 return
 
         if len(events) == 1:
             self._event_storage.store_event(events[0])
```

### Comparing `dagster-1.7.0/dagster/_core/instance/config.py` & `dagster-1.7.1/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/instance/ref.py` & `dagster-1.7.1/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/instance_for_test.py` & `dagster-1.7.1/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/launcher/base.py` & `dagster-1.7.1/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.1/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.1/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/log_manager.py` & `dagster-1.7.1/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/nux.py` & `dagster-1.7.1/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.1/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/origin.py` & `dagster-1.7.1/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/pipes/client.py` & `dagster-1.7.1/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/pipes/context.py` & `dagster-1.7.1/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/pipes/subprocess.py` & `dagster-1.7.1/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/pipes/utils.py` & `dagster-1.7.1/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.1/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.1/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/external.py` & `dagster-1.7.1/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.1/dagster/_core/remote_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1226,36 +1226,44 @@
         "_ExternalAssetCheck",
         [
             ("name", str),
             ("asset_key", AssetKey),
             ("description", Optional[str]),
             ("execution_set_identifier", Optional[str]),
             ("job_names", Sequence[str]),
+            ("blocking", bool),
+            ("additional_asset_keys", Sequence[AssetKey]),
         ],
     )
 ):
     """Serializable data associated with an asset check."""
 
     def __new__(
         cls,
         name: str,
         asset_key: AssetKey,
         description: Optional[str],
         execution_set_identifier: Optional[str] = None,
         job_names: Optional[Sequence[str]] = None,
+        blocking: bool = False,
+        additional_asset_keys: Optional[Sequence[AssetKey]] = None,
     ):
         return super(ExternalAssetCheck, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             asset_key=check.inst_param(asset_key, "asset_key", AssetKey),
             description=check.opt_str_param(description, "description"),
             execution_set_identifier=check.opt_str_param(
                 execution_set_identifier, "execution_set_identifier"
             ),
             job_names=check.opt_sequence_param(job_names, "job_names", of_type=str),
+            blocking=check.bool_param(blocking, "blocking"),
+            additional_asset_keys=check.opt_sequence_param(
+                additional_asset_keys, "additional_asset_keys", of_type=AssetKey
+            ),
         )
 
     @property
     def key(self) -> AssetCheckKey:
         return AssetCheckKey(asset_key=self.asset_key, name=self.name)
 
 
@@ -1644,14 +1652,16 @@
         external_checks.append(
             ExternalAssetCheck(
                 name=check_key.name,
                 asset_key=check_key.asset_key,
                 description=spec.description,
                 execution_set_identifier=execution_set_identifier,
                 job_names=job_names_by_check_key[check_key],
+                blocking=spec.blocking,
+                additional_asset_keys=[dep.asset_key for dep in spec.additional_deps],
             )
         )
 
     return sorted(external_checks, key=lambda check: (check.asset_key, check.name))
 
 
 def external_asset_nodes_from_defs(
```

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.1/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.1/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.1/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/handle.py` & `dagster-1.7.1/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/historical.py` & `dagster-1.7.1/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.1/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/origin.py` & `dagster-1.7.1/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/remote_representation/represented.py` & `dagster-1.7.1/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/run_coordinator/base.py` & `dagster-1.7.1/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.1/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.1/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/scheduler/__init__.py` & `dagster-1.7.1/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/scheduler/execution.py` & `dagster-1.7.1/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/scheduler/instigation.py` & `dagster-1.7.1/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.1/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/secrets/env_file.py` & `dagster-1.7.1/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/selector/subset_selector.py` & `dagster-1.7.1/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/__init__.py` & `dagster-1.7.1/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/dagster_types.py` & `dagster-1.7.1/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.1/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.1/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.1/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/mode.py` & `dagster-1.7.1/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/node.py` & `dagster-1.7.1/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.1/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.1/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/README.md` & `dagster-1.7.1/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/env.py` & `dagster-1.7.1/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.1/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.1/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.1/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/base_storage.py` & `dagster-1.7.1/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.1/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.1/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.1/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/config.py` & `dagster-1.7.1/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/dagster_run.py` & `dagster-1.7.1/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.1/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/base.py` & `dagster-1.7.1/dagster/_core/storage/event_log/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.1/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.1/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.1/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.1/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.1/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.1/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/file_manager.py` & `dagster-1.7.1/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/input_manager.py` & `dagster-1.7.1/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/io_manager.py` & `dagster-1.7.1/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.1/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.1/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.1/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/migration/utils.py` & `dagster-1.7.1/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.1/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/output_manager.py` & `dagster-1.7.1/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.1/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/root.py` & `dagster-1.7.1/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/base.py` & `dagster-1.7.1/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.1/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/migration.py` & `dagster-1.7.1/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/schema.py` & `dagster-1.7.1/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.1/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.1/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.1/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/base.py` & `dagster-1.7.1/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.1/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.1/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.1/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.1/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.1/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/sql.py` & `dagster-1.7.1/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.1/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/sqlite.py` & `dagster-1.7.1/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.1/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/tags.py` & `dagster-1.7.1/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.1/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.1/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.1/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/system_config/objects.py` & `dagster-1.7.1/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/telemetry.py` & `dagster-1.7.1/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/telemetry_upload.py` & `dagster-1.7.1/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/test_utils.py` & `dagster-1.7.1/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.1/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/config_schema.py` & `dagster-1.7.1/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/dagster_type.py` & `dagster-1.7.1/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/decorator.py` & `dagster-1.7.1/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.1/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.1/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/python_dict.py` & `dagster-1.7.1/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/python_set.py` & `dagster-1.7.1/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/python_tuple.py` & `dagster-1.7.1/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/types/transform_typing.py` & `dagster-1.7.1/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/utility_ops.py` & `dagster-1.7.1/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/utils.py` & `dagster-1.7.1/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.1/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/config_schema.py` & `dagster-1.7.1/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/context.py` & `dagster-1.7.1/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/load.py` & `dagster-1.7.1/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/load_target.py` & `dagster-1.7.1/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/permissions.py` & `dagster-1.7.1/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_core/workspace/workspace.py` & `dagster-1.7.1/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/__init__.py` & `dagster-1.7.1/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/asset_daemon.py` & `dagster-1.7.1/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.1/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.1/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/backfill.py` & `dagster-1.7.1/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/cli/__init__.py` & `dagster-1.7.1/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/controller.py` & `dagster-1.7.1/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/daemon.py` & `dagster-1.7.1/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.1/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.1/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.1/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/sensor.py` & `dagster-1.7.1/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/types.py` & `dagster-1.7.1/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/utils.py` & `dagster-1.7.1/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_daemon/workspace.py` & `dagster-1.7.1/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_generate/download.py` & `dagster-1.7.1/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_generate/generate.py` & `dagster-1.7.1/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.1/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.1/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/__init__.py` & `dagster-1.7.1/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/client.py` & `dagster-1.7.1/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/compile.py` & `dagster-1.7.1/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/impl.py` & `dagster-1.7.1/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/protos/api.proto` & `dagster-1.7.1/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/proxy_server.py` & `dagster-1.7.1/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/server.py` & `dagster-1.7.1/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/server_watcher.py` & `dagster-1.7.1/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/types.py` & `dagster-1.7.1/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_grpc/utils.py` & `dagster-1.7.1/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_loggers/__init__.py` & `dagster-1.7.1/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_model/__init__.py` & `dagster-1.7.1/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_module_alias_map.py` & `dagster-1.7.1/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_scheduler/scheduler.py` & `dagster-1.7.1/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_scheduler/stale.py` & `dagster-1.7.1/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_serdes/__init__.py` & `dagster-1.7.1/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_serdes/config_class.py` & `dagster-1.7.1/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_serdes/ipc.py` & `dagster-1.7.1/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_serdes/serdes.py` & `dagster-1.7.1/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_serdes/utils.py` & `dagster-1.7.1/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_seven/__init__.py` & `dagster-1.7.1/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_seven/abc.py` & `dagster-1.7.1/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_seven/compat/pendulum.py` & `dagster-1.7.1/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/__init__.py` & `dagster-1.7.1/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/alert.py` & `dagster-1.7.1/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/backoff.py` & `dagster-1.7.1/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/cached_method.py` & `dagster-1.7.1/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.1/dagster/_utils/caching_instance_queryer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/concurrency.py` & `dagster-1.7.1/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/container.py` & `dagster-1.7.1/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/dagster_type.py` & `dagster-1.7.1/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/env.py` & `dagster-1.7.1/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/error.py` & `dagster-1.7.1/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/external.py` & `dagster-1.7.1/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/forked_pdb.py` & `dagster-1.7.1/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/hosted_user_process.py` & `dagster-1.7.1/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/indenting_printer.py` & `dagster-1.7.1/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/internal_init.py` & `dagster-1.7.1/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/interrupts.py` & `dagster-1.7.1/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/log.py` & `dagster-1.7.1/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/merger.py` & `dagster-1.7.1/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/net.py` & `dagster-1.7.1/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/schedules.py` & `dagster-1.7.1/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/tags.py` & `dagster-1.7.1/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/temp_file.py` & `dagster-1.7.1/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/test/__init__.py` & `dagster-1.7.1/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/test/data_versions.py` & `dagster-1.7.1/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.1/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.1/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.1/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/timing.py` & `dagster-1.7.1/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/typed_dict.py` & `dagster-1.7.1/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/typing_api.py` & `dagster-1.7.1/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/warnings.py` & `dagster-1.7.1/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster/_utils/yaml_utils.py` & `dagster-1.7.1/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.0/dagster.egg-info/PKG-INFO` & `dagster-1.7.1/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.0
+Version: 1.7.1
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -117,15 +117,15 @@
 ```
 
 This installs two packages:
 
 - `dagster`: The core programming model.
 - `dagster-webserver`: The server that hosts Dagster's web UI for developing and operating Dagster jobs and assets.
 
-Running on Using a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
+Running on a Mac with an Apple silicon chip? Check the [install details here](https://docs.dagster.io/getting-started/install#installing-dagster-into-an-existing-python-environment).
 
 ## Documentation
 
 You can find the full Dagster documentation [here](https://docs.dagster.io), including the ['getting started' guide](https://docs.dagster.io/getting-started).
 
 <hr/>
```

### Comparing `dagster-1.7.0/dagster.egg-info/SOURCES.txt` & `dagster-1.7.1/dagster.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
 dagster/_core/definitions/decorators/repository_decorator.py
 dagster/_core/definitions/decorators/schedule_decorator.py
 dagster/_core/definitions/decorators/sensor_decorator.py
 dagster/_core/definitions/decorators/source_asset_decorator.py
 dagster/_core/definitions/freshness_checks/__init__.py
 dagster/_core/definitions/freshness_checks/last_update.py
 dagster/_core/definitions/freshness_checks/sensor.py
+dagster/_core/definitions/freshness_checks/shared_builder.py
 dagster/_core/definitions/freshness_checks/time_partition.py
 dagster/_core/definitions/freshness_checks/utils.py
 dagster/_core/definitions/metadata/__init__.py
 dagster/_core/definitions/metadata/table.py
 dagster/_core/definitions/repository_definition/__init__.py
 dagster/_core/definitions/repository_definition/caching_index.py
 dagster/_core/definitions/repository_definition/repository_data.py
```

### Comparing `dagster-1.7.0/dagster.egg-info/requires.txt` & `dagster-1.7.1/dagster.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 structlog
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
-dagster-pipes==1.7.0
+dagster-pipes==1.7.1
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.0/setup.py` & `dagster-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         'pywin32!=226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
-        "dagster-pipes==1.7.0",
+        "dagster-pipes==1.7.1",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

