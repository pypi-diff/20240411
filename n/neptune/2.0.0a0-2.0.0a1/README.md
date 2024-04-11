# Comparing `tmp/neptune-2.0.0a0.tar.gz` & `tmp/neptune-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-2.0.0a0.tar", max compression
+gzip compressed data, was "neptune-2.0.0a1.tar", max compression
```

## Comparing `neptune-2.0.0a0.tar` & `neptune-2.0.0a1.tar`

### file list

```diff
@@ -1,280 +1,280 @@
--rw-r--r--   0        0        0    43968 2024-04-10 07:14:20.632583 neptune-2.0.0a0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-10 07:14:20.632583 neptune-2.0.0a0/LICENSE
--rw-r--r--   0        0        0    12786 2024-04-10 07:14:20.632583 neptune-2.0.0a0/README.md
--rw-r--r--   0        0        0    10949 2024-04-10 07:14:30.776590 neptune-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/__init__.py
--rw-r--r--   0        0        0     2768 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/field_visitor.py
--rw-r--r--   0        0        0    19028 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/models.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
--rw-r--r--   0        0        0     1642 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
--rw-r--r--   0        0        0     6126 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
--rw-r--r--   0        0        0    17492 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
--rw-r--r--   0        0        0      990 2024-04-10 07:14:20.632583 neptune-2.0.0a0/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     8193 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2105 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1923 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2446 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2665 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2139 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3023 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4585 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2594 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4432 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3505 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2057 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5391 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     5220 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10813 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5167 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/cli/utils.py
--rw-r--r--   0        0        0     1087 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2573 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/envs.py
--rw-r--r--   0        0        0    42022 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/exceptions.py
--rw-r--r--   0        0        0    32661 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      775 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0      796 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      784 2024-04-10 07:14:20.636583 neptune-2.0.0a0/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      781 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      790 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      795 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/mosaicml/__init__.py
--rw-r--r--   0        0        0      784 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0     3633 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pandas/__init__.py
--rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3026 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0      814 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      784 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0      799 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0      814 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0      812 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0      864 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      787 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5141 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2377 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     6311 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9567 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6338 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18056 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    45673 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9535 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    32992 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     2894 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     5864 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3948 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5005 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13843 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5658 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    15904 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1517 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1134 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2349 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      859 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/envs.py
--rw-r--r--   0        0        0    15028 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1725 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3216 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-04-10 07:14:20.640583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2031 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1772 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1756 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5122 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3496 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1681 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      949 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2323 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2512 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/hardware/system/system_monitor.py
--rw-r--r--   0        0        0      933 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0     4784 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/oauth.py
--rw-r--r--   0        0        0    17298 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13129 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3936 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
--rw-r--r--   0        0        0     3070 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1422 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1146 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2443 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      886 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/patches/bravado.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2883 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1663 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4899 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1789 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/state.py
--rw-r--r--   0        0        0     1130 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/__init__.py
--rw-r--r--   0        0        0     3227 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/datastream.py
--rw-r--r--   0        0        0     7330 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/storage/storage_utils.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1999 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3066 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5581 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4586 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2409 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2116 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5746 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2300 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0     2490 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/git_info.py
--rw-r--r--   0        0        0      849 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10577 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1152 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/iso_dates.py
--rw-r--r--   0        0        0     1288 2024-04-10 07:14:20.644583 neptune-2.0.0a0/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2972 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0      726 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/patterns.py
--rw-r--r--   0        0        0     2187 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1168 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/requirement_check.py
--rw-r--r--   0        0        0     1566 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2266 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2001 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     7575 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/utils/utils.py
--rw-r--r--   0        0        0     4442 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0     3284 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/warnings.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3591 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2638 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     5210 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1231 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0     4795 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    44742 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2021 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      923 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/__init__.py
--rw-r--r--   0        0        0     2351 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/abstract.py
--rw-r--r--   0        0        0    15938 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/model.py
--rw-r--r--   0        0        0    13843 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/model_version.py
--rw-r--r--   0        0        0    26824 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/neptune_object.py
--rw-r--r--   0        0        0    19268 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/project.py
--rw-r--r--   0        0        0    26572 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/run.py
--rw-r--r--   0        0        0     1576 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/structure_version.py
--rw-r--r--   0        0        0     4043 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/objects/utils.py
--rw-r--r--   0        0        0     5783 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/table.py
--rw-r--r--   0        0        0     1071 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    12157 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3854 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-04-10 07:14:20.648583 neptune-2.0.0a0/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3210 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/typing.py
--rw-r--r--   0        0        0     4252 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     1431 2024-04-10 07:14:20.652583 neptune-2.0.0a0/src/neptune/version.py
--rw-r--r--   0        0        0    16631 1970-01-01 00:00:00.000000 neptune-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    44436 2024-04-11 15:36:18.970295 neptune-2.0.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-11 15:36:18.970295 neptune-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0    12786 2024-04-11 15:36:18.970295 neptune-2.0.0a1/README.md
+-rw-r--r--   0        0        0    10951 2024-04-11 15:36:28.874262 neptune-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-11 15:36:18.970295 neptune-2.0.0a1/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     2768 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/field_visitor.py
+-rw-r--r--   0        0        0    19028 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/models.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
+-rw-r--r--   0        0        0     1642 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
+-rw-r--r--   0        0        0     6126 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
+-rw-r--r--   0        0        0    17492 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
+-rw-r--r--   0        0        0      990 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     7771 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2105 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     1923 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2446 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2665 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2139 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3023 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4585 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2594 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4432 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2656 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3505 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2627 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2057 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5391 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     5220 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10813 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5167 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0     1087 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2573 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/envs.py
+-rw-r--r--   0        0        0    42022 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    32876 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      775 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      795 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/mosaicml/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0     3633 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pandas/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3026 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4810 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5141 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2377 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     6311 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9567 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6714 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18056 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    46218 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     9535 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    32992 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2894 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     5864 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3948 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5005 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13843 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5658 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    15994 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1517 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1134 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2349 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      859 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/envs.py
+-rw-r--r--   0        0        0    15028 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1725 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3216 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2031 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1772 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1756 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5122 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3496 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1681 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      949 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2323 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2512 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0      933 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0     4784 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/oauth.py
+-rw-r--r--   0        0        0    17298 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13129 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3936 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
+-rw-r--r--   0        0        0     3070 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1422 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1146 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2443 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      886 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/patches/bravado.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2883 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1663 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4899 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1789 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/state.py
+-rw-r--r--   0        0        0     1130 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/__init__.py
+-rw-r--r--   0        0        0     3227 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/datastream.py
+-rw-r--r--   0        0        0     7330 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/storage_utils.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3066 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5581 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2409 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2116 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5746 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2300 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0     2490 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/git_info.py
+-rw-r--r--   0        0        0      849 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10577 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1152 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/iso_dates.py
+-rw-r--r--   0        0        0     1288 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2972 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0      726 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/patterns.py
+-rw-r--r--   0        0        0     2187 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1168 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/requirement_check.py
+-rw-r--r--   0        0        0     1566 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1340 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2266 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2001 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     7575 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/utils.py
+-rw-r--r--   0        0        0     4442 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0     3284 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/warnings.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3591 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2638 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     5210 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1231 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0     4795 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    44742 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2021 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      923 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/abstract.py
+-rw-r--r--   0        0        0    15915 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/model.py
+-rw-r--r--   0        0        0    13820 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/model_version.py
+-rw-r--r--   0        0        0    26780 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/neptune_object.py
+-rw-r--r--   0        0        0    19245 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/project.py
+-rw-r--r--   0        0        0    26549 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/run.py
+-rw-r--r--   0        0        0     1576 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/structure_version.py
+-rw-r--r--   0        0        0     4043 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/utils.py
+-rw-r--r--   0        0        0     5783 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/table.py
+-rw-r--r--   0        0        0     1071 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    12157 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3854 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3089 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/typing.py
+-rw-r--r--   0        0        0     4310 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     1431 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/version.py
+-rw-r--r--   0        0        0    16631 1970-01-01 00:00:00.000000 neptune-2.0.0a1/PKG-INFO
```

### Comparing `neptune-2.0.0a0/CHANGELOG.md` & `neptune-2.0.0a1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 - Renamed `metadata_containers` to `objects` ([#1696](https://github.com/neptune-ai/neptune-client/pull/1696))
 - Removed `neptune-client` ([#1699](https://github.com/neptune-ai/neptune-client/pull/1699))
 - Deleted `neptune.logging` package ([#1698](https://github.com/neptune-ai/neptune-client/pull/1698))
 - Disabled `Model` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1701))
 - Disabled `ModelVersion` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1708))
 - Disabled `Project` ([#1709](https://github.com/neptune-ai/neptune-client/pull/1709))
 - Disabled `neptune command-line tool` ([#1718](https://github.com/neptune-ai/neptune-client/pull/1718))
+- Disabled deleting fields in `Handler` ([#1729](https://github.com/neptune-ai/neptune-client/pull/1729))
+- Removed `AbstractNeptuneObject` ([#1725](https://github.com/neptune-ai/neptune-client/pull/1725))
 
 ### Changes
 - Stop sending `X-Neptune-LegacyClient` header ([#1715](https://github.com/neptune-ai/neptune-client/pull/1715))
 - Use `tqdm.auto` ([#1717](https://github.com/neptune-ai/neptune-client/pull/1717))
 - Fields DTO conversion reworked ([#1722](https://github.com/neptune-ai/neptune-client/pull/1722))
 - Added support for Protocol Buffers ([#1728](https://github.com/neptune-ai/neptune-client/pull/1728))
 
 ### Features
 - ?
 
 ### Fixes
 - Fixed `tqdm.notebook` import only in Notebook environment ([#1716](https://github.com/neptune-ai/neptune-client/pull/1716))
 - Added `setuptools` to dependencies for `python >= 3.12` ([#1721](https://github.com/neptune-ai/neptune-client/pull/1721))
+- Fixed compatibility checks with pre-release versions ([#1730](https://github.com/neptune-ai/neptune-client/pull/1730))
+- Added `Accept` and `Accept-Encoding` headers to protocol buffer requests ([#1736](https://github.com/neptune-ai/neptune-client/pull/1736))
 
 
 ## neptune 1.10.0
 
 ### Features
 - Added `get_workspace_status()` method to management API ([#1662](https://github.com/neptune-ai/neptune-client/pull/1662))
 - Added auto-scaling pixel values for image logging ([#1664](https://github.com/neptune-ai/neptune-client/pull/1664))
```

### Comparing `neptune-2.0.0a0/LICENSE` & `neptune-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/README.md` & `neptune-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/pyproject.toml` & `neptune-2.0.0a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "2.0.0-alpha"
+version = "2.0.0-alpha.1"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-2.0.0a0/src/neptune/__init__.py` & `neptune-2.0.0a1/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/__init__.py` & `neptune-2.0.0a1/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/field_visitor.py` & `neptune-2.0.0a1/src/neptune/api/field_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/models.py` & `neptune-2.0.0a1/src/neptune/api/models.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/__init__.py` & `neptune-2.0.0a1/src/neptune/api/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/__init__.py` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/__init__.py` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/__init__.py` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi` & `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/requests_utils.py` & `neptune-2.0.0a1/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/api/searching_entries.py` & `neptune-2.0.0a1/src/neptune/api/searching_entries.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     Any,
     Dict,
     Generator,
     Iterable,
     Optional,
 )
 
-from bravado.client import construct_request  # type: ignore
-from bravado.config import RequestConfig  # type: ignore
 from bravado.exception import HTTPBadRequest  # type: ignore
 from typing_extensions import (
     Literal,
     TypeAlias,
 )
 
 from neptune.api.field_visitor import FieldToValueVisitor
@@ -37,15 +35,18 @@
     Field,
     FieldType,
     LeaderboardEntriesSearchResult,
     LeaderboardEntry,
 )
 from neptune.api.proto.neptune_pb.api.model.leaderboard_entries_pb2 import ProtoLeaderboardEntriesSearchResultDTO
 from neptune.exceptions import NeptuneInvalidQueryException
-from neptune.internal.backends.hosted_client import DEFAULT_REQUEST_KWARGS
+from neptune.internal.backends.hosted_client import (
+    DEFAULT_PROTO_REQUEST_KWARGS,
+    DEFAULT_REQUEST_KWARGS,
+)
 from neptune.internal.backends.nql import (
     NQLAggregator,
     NQLAttributeOperator,
     NQLAttributeType,
     NQLEmptyQuery,
     NQLQuery,
     NQLQueryAggregate,
@@ -139,31 +140,22 @@
             "query": {"query": str(normalized_query)},
             "pagination": {"limit": limit, "offset": offset},
         },
     }
 
     try:
         if use_proto:
-            result = client.api.searchLeaderboardEntriesProto(**params).response().result
+            result = (
+                client.api.searchLeaderboardEntriesProto(**params, **DEFAULT_PROTO_REQUEST_KWARGS).response().result
+            )
             proto_data = ProtoLeaderboardEntriesSearchResultDTO.FromString(result)
             return LeaderboardEntriesSearchResult.from_proto(proto_data)
         else:
-            request_options = DEFAULT_REQUEST_KWARGS.get("_request_options", {})
-            request_config = RequestConfig(request_options, True)
-            request_params = construct_request(client.api.searchLeaderboardEntries, request_options, **params)
-
-            http_client = client.swagger_spec.http_client
-
-            json_data = (
-                http_client.request(request_params, operation=None, request_config=request_config)
-                .response()
-                .incoming_response.json()
-            )
-
-            return LeaderboardEntriesSearchResult.from_dict(json_data)
+            model_data = client.api.searchLeaderboardEntries(**params, **DEFAULT_REQUEST_KWARGS).response().result
+            return LeaderboardEntriesSearchResult.from_model(model_data)
     except HTTPBadRequest as e:
         title = e.response.json().get("title")
         if title == "Syntax error":
             raise NeptuneInvalidQueryException(nql_query=str(normalized_query))
         raise e
```

### Comparing `neptune-2.0.0a0/src/neptune/attributes/__init__.py` & `neptune-2.0.0a1/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/__init__.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/artifact.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/atom.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/boolean.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/datetime.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/file.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/float.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/git_ref.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/integer.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/run_state.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/atoms/string.py` & `neptune-2.0.0a1/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/attribute.py` & `neptune-2.0.0a1/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/constants.py` & `neptune-2.0.0a1/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/file_set.py` & `neptune-2.0.0a1/src/neptune/attributes/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/namespace.py` & `neptune-2.0.0a1/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/__init__.py` & `neptune-2.0.0a1/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/fetchable_series.py` & `neptune-2.0.0a1/src/neptune/attributes/series/fetchable_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/file_series.py` & `neptune-2.0.0a1/src/neptune/attributes/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/float_series.py` & `neptune-2.0.0a1/src/neptune/attributes/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/series.py` & `neptune-2.0.0a1/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/series/string_series.py` & `neptune-2.0.0a1/src/neptune/attributes/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/sets/__init__.py` & `neptune-2.0.0a1/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/sets/set.py` & `neptune-2.0.0a1/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/sets/string_set.py` & `neptune-2.0.0a1/src/neptune/attributes/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/attributes/utils.py` & `neptune-2.0.0a1/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/__init__.py` & `neptune-2.0.0a1/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/__main__.py` & `neptune-2.0.0a1/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/clear.py` & `neptune-2.0.0a1/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/collect.py` & `neptune-2.0.0a1/src/neptune/cli/collect.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/commands.py` & `neptune-2.0.0a1/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/containers.py` & `neptune-2.0.0a1/src/neptune/cli/containers.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/path_option.py` & `neptune-2.0.0a1/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/status.py` & `neptune-2.0.0a1/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/sync.py` & `neptune-2.0.0a1/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/cli/utils.py` & `neptune-2.0.0a1/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/constants.py` & `neptune-2.0.0a1/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/__init__.py` & `neptune-2.0.0a1/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/__init__.py` & `neptune-2.0.0a1/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/abstract.py` & `neptune-2.0.0a1/src/neptune/core/components/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/metadata_file.py` & `neptune-2.0.0a1/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/operation_storage.py` & `neptune-2.0.0a1/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/queue/__init__.py` & `neptune-2.0.0a1/src/neptune/core/components/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/queue/disk_queue.py` & `neptune-2.0.0a1/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/queue/json_file_splitter.py` & `neptune-2.0.0a1/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/queue/log_file.py` & `neptune-2.0.0a1/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/core/components/queue/sync_offset_file.py` & `neptune-2.0.0a1/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/envs.py` & `neptune-2.0.0a1/src/neptune/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/exceptions.py` & `neptune-2.0.0a1/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/handler.py` & `neptune-2.0.0a1/src/neptune/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from neptune.attributes.series import FileSeries
 from neptune.attributes.series.float_series import FloatSeries
 from neptune.attributes.series.string_series import StringSeries
 from neptune.attributes.sets.string_set import StringSet
 from neptune.exceptions import (
     MissingFieldException,
     NeptuneCannotChangeStageManually,
+    NeptuneUnsupportedFunctionalityException,
     NeptuneUserApiInputException,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.types.stringify_value import StringifyValue
 from neptune.internal.utils import (
     is_collection,
     is_dict_like,
@@ -463,16 +464,15 @@
         with self._container.lock():
             attr = self._container.get_attribute(self._path)
             if attr is None:
                 attr = StringSet(self._container, parse_path(self._path))
                 self._container.set_attribute(self._path, attr)
             attr.add(values, wait=wait)
 
-    @check_protected_paths
-    def pop(self, path: str = None, *, wait: bool = False) -> None:
+    def _delete_item(self, path: str = None, *, wait: bool = False) -> None:
         with self._container.lock():
             handler = self
             if path:
                 verify_type("path", path, str)
                 handler = self[path]
                 path = join_paths(self._path, path)
                 # extra check: check_protected_paths decorator does not catch flow with non-null path
@@ -726,15 +726,19 @@
             if attr is None:
                 attr = Artifact(self._container, parse_path(self._path))
                 self._container.set_attribute(self._path, attr)
 
             attr.track_files(path=path, destination=destination, wait=wait)
 
     def __delitem__(self, path) -> None:
-        self.pop(path)
+        raise NeptuneUnsupportedFunctionalityException()
+
+    @check_protected_paths
+    def pop(self, path: str = None, *, wait: bool = False) -> None:
+        raise NeptuneUnsupportedFunctionalityException()
 
 
 class ExtendUtils:
     @staticmethod
     def transform_to_extend_format(value):
         """Preserves the nested structure created by `Namespaces` and `dict_like` objects,
         but replaces all other values with single-element lists,
```

### Comparing `neptune-2.0.0a0/src/neptune/integrations/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/aws/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/detectron2/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/fastai/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/kedro/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/lightgbm/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/mosaicml/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/mosaicml/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/optuna/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/pandas/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/prophet/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/python_logger.py` & `neptune-2.0.0a1/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/pytorch/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/sacred/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/sklearn/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/tensorboard/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/transformers/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/utils.py` & `neptune-2.0.0a1/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/integrations/xgboost/__init__.py` & `neptune-2.0.0a1/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/local.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/file_hasher.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/types.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/artifacts/utils.py` & `neptune-2.0.0a1/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/api_model.py` & `neptune-2.0.0a1/src/neptune/internal/backends/api_model.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/factory.py` & `neptune-2.0.0a1/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-2.0.0a1/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/hosted_client.py` & `neptune-2.0.0a1/src/neptune/internal/backends/hosted_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = [
     "DEFAULT_REQUEST_KWARGS",
+    "DEFAULT_PROTO_REQUEST_KWARGS",
     "create_http_client_with_auth",
     "create_backend_client",
     "create_leaderboard_client",
     "create_artifacts_client",
 ]
 
 import os
@@ -61,14 +62,25 @@
     "_request_options": {
         "connect_timeout": CONNECT_TIMEOUT,
         "timeout": REQUEST_TIMEOUT,
         "headers": {},
     }
 }
 
+DEFAULT_PROTO_REQUEST_KWARGS = {
+    "_request_options": {
+        **DEFAULT_REQUEST_KWARGS["_request_options"],
+        "headers": {
+            **DEFAULT_REQUEST_KWARGS["_request_options"]["headers"],
+            "Accept": "application/x-protobuf,application/json",
+            "Accept-Encoding": "gzip, deflate, br",
+        },
+    }
+}
+
 
 def _close_connections_on_fork(session: requests.Session):
     try:
         os.register_at_fork(before=session.close, after_in_child=session.close, after_in_parent=session.close)
     except AttributeError:
         pass
```

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-2.0.0a1/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-2.0.0a1/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 from neptune.internal.backends.hosted_artifact_operations import (
     get_artifact_attribute,
     list_artifact_files,
     track_to_existing_artifact,
     track_to_new_artifact,
 )
 from neptune.internal.backends.hosted_client import (
+    DEFAULT_PROTO_REQUEST_KWARGS,
     DEFAULT_REQUEST_KWARGS,
     create_artifacts_client,
     create_backend_client,
     create_http_client_with_auth,
     create_leaderboard_client,
 )
 from neptune.internal.backends.hosted_file_operations import (
@@ -1134,24 +1135,37 @@
         container_type: ContainerType,
         use_proto: Optional[bool] = None,
     ) -> List[FieldDefinition]:
         use_proto = use_proto if use_proto is not None else self.use_proto
 
         params = {
             "experimentIdentifier": container_id,
-            **DEFAULT_REQUEST_KWARGS,
         }
 
         try:
             if use_proto:
-                result = self.leaderboard_client.api.queryAttributeDefinitionsProto(**params).response().result
+                result = (
+                    self.leaderboard_client.api.queryAttributeDefinitionsProto(
+                        **params,
+                        **DEFAULT_PROTO_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
                 data = ProtoAttributesSearchResultDTO.FromString(result)
                 return [FieldDefinition.from_proto(field_def) for field_def in data.entries]
             else:
-                data = self.leaderboard_client.api.queryAttributeDefinitions(**params).response().result
+                data = (
+                    self.leaderboard_client.api.queryAttributeDefinitions(
+                        **params,
+                        **DEFAULT_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
                 return [FieldDefinition.from_model(field_def) for field_def in data.entries]
         except HTTPNotFound as e:
             raise ContainerUUIDNotFound(
                 container_id=container_id,
                 container_type=container_type,
             ) from e
 
@@ -1167,15 +1181,22 @@
                 "attributePathsFilter": paths,
             },
             **DEFAULT_REQUEST_KWARGS,
         }
 
         try:
             if use_proto:
-                result = self.leaderboard_client.api.getAttributesWithPathsFilterProto(**params).response().result
+                result = (
+                    self.leaderboard_client.api.getAttributesWithPathsFilterProto(
+                        **params,
+                        **DEFAULT_PROTO_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
                 data = ProtoAttributesDTO.FromString(result)
                 return [Field.from_proto(field) for field in data.attributes]
             else:
                 data = self.leaderboard_client.api.getAttributesWithPathsFilter(**params).response().result
                 return [Field.from_model(field) for field in data.attributes]
         except HTTPNotFound as e:
             raise ContainerUUIDNotFound(
```

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend.py` & `neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/nql.py` & `neptune-2.0.0a1/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-2.0.0a1/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-2.0.0a1/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-2.0.0a1/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-2.0.0a1/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/project_name_lookup.py` & `neptune-2.0.0a1/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-2.0.0a1/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/backends/utils.py` & `neptune-2.0.0a1/src/neptune/internal/backends/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,26 +272,34 @@
             formats=[uuid_format],
         ),
         http_client=http_client,
     )
 
 
 def verify_client_version(client_config: ClientConfig, version: Version):
+    base_version = Version(f"{version.major}.{version.minor}.{version.micro}")
     version_with_patch_0 = Version(replace_patch_version(str(version)))
-    if client_config.version_info.min_compatible and client_config.version_info.min_compatible > version:
+
+    min_compatible = client_config.version_info.min_compatible
+    max_compatible = client_config.version_info.max_compatible
+    min_recommended = client_config.version_info.min_recommended
+
+    if min_compatible and min_compatible > base_version:
         raise NeptuneClientUpgradeRequiredError(version, min_version=client_config.version_info.min_compatible)
-    if client_config.version_info.max_compatible and client_config.version_info.max_compatible < version_with_patch_0:
+
+    if max_compatible and max_compatible < version_with_patch_0:
         raise NeptuneClientUpgradeRequiredError(version, max_version=client_config.version_info.max_compatible)
-    if client_config.version_info.min_recommended and client_config.version_info.min_recommended > version:
+
+    if min_recommended and min_recommended > version:
         logger.warning(
             "WARNING: Your version of the Neptune client library (%s) is deprecated,"
             " and soon will no longer be supported by the Neptune server."
             " We recommend upgrading to at least version %s.",
             version,
-            client_config.version_info.min_recommended,
+            min_recommended,
         )
 
 
 def update_session_proxies(session: Session, proxies: Optional[Dict[str, str]]):
     if proxies:
         try:
             session.proxies.update(proxies)
```

### Comparing `neptune-2.0.0a0/src/neptune/internal/backgroud_job_list.py` & `neptune-2.0.0a1/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/background_job.py` & `neptune-2.0.0a1/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/constants.py` & `neptune-2.0.0a1/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/container_structure.py` & `neptune-2.0.0a1/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/container_type.py` & `neptune-2.0.0a1/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/credentials.py` & `neptune-2.0.0a1/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/envs.py` & `neptune-2.0.0a1/src/neptune/internal/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/exceptions.py` & `neptune-2.0.0a1/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/extensions.py` & `neptune-2.0.0a1/src/neptune/internal/extensions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/cgroup/cgroup_monitor.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/constants.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/cpu.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_factory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gauge_mode.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/gpu.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gauges/memory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metric.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_container.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/metrics_factory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_report.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/metrics/service/metric_service_factory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/resources/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/resources/system_resource_info_factory.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/system/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/hardware/system/system_monitor.py` & `neptune-2.0.0a1/src/neptune/internal/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/id_formats.py` & `neptune-2.0.0a1/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/init/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/init/parameters.py` & `neptune-2.0.0a1/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/notebooks/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/notebooks/comm.py` & `neptune-2.0.0a1/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/notebooks/notebooks.py` & `neptune-2.0.0a1/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/oauth.py` & `neptune-2.0.0a1/src/neptune/internal/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation.py` & `neptune-2.0.0a1/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/factory.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_logger.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_processors/utils.py` & `neptune-2.0.0a1/src/neptune/internal/operation_processors/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/operation_visitor.py` & `neptune-2.0.0a1/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/patches/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/patches/bravado.py` & `neptune-2.0.0a1/src/neptune/internal/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/signals_processing/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/signals_processing/background_job.py` & `neptune-2.0.0a1/src/neptune/internal/signals_processing/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/signals_processing/signals.py` & `neptune-2.0.0a1/src/neptune/internal/signals_processing/signals.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/signals_processing/signals_processor.py` & `neptune-2.0.0a1/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/signals_processing/utils.py` & `neptune-2.0.0a1/src/neptune/internal/signals_processing/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/state.py` & `neptune-2.0.0a1/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/storage/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/storage/datastream.py` & `neptune-2.0.0a1/src/neptune/internal/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/storage/storage_utils.py` & `neptune-2.0.0a1/src/neptune/internal/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/streams/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-2.0.0a1/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-2.0.0a1/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/threading/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/threading/daemon.py` & `neptune-2.0.0a1/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/types/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/types/file_types.py` & `neptune-2.0.0a1/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/types/stringify_value.py` & `neptune-2.0.0a1/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/types/utils.py` & `neptune-2.0.0a1/src/neptune/internal/types/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/dependency_tracking.py` & `neptune-2.0.0a1/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/deprecation.py` & `neptune-2.0.0a1/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/disk_utilization.py` & `neptune-2.0.0a1/src/neptune/internal/utils/disk_utilization.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-2.0.0a1/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/git.py` & `neptune-2.0.0a1/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/git_info.py` & `neptune-2.0.0a1/src/neptune/internal/utils/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/hashing.py` & `neptune-2.0.0a1/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/images.py` & `neptune-2.0.0a1/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/iso_dates.py` & `neptune-2.0.0a1/src/neptune/internal/utils/iso_dates.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/iteration.py` & `neptune-2.0.0a1/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/limits.py` & `neptune-2.0.0a1/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/logger.py` & `neptune-2.0.0a1/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/paths.py` & `neptune-2.0.0a1/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/patterns.py` & `neptune-2.0.0a1/src/neptune/internal/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/ping_background_job.py` & `neptune-2.0.0a1/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/process_killer.py` & `neptune-2.0.0a1/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/requirement_check.py` & `neptune-2.0.0a1/src/neptune/internal/utils/requirement_check.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/run_state.py` & `neptune-2.0.0a1/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/runningmode.py` & `neptune-2.0.0a1/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/s3.py` & `neptune-2.0.0a1/src/neptune/internal/utils/s3.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/source_code.py` & `neptune-2.0.0a1/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/traceback_job.py` & `neptune-2.0.0a1/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-2.0.0a1/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/utils/utils.py` & `neptune-2.0.0a1/src/neptune/internal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-2.0.0a1/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/warnings.py` & `neptune-2.0.0a1/src/neptune/internal/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/websockets/__init__.py` & `neptune-2.0.0a1/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/websockets/reconnecting_websocket.py` & `neptune-2.0.0a1/src/neptune/internal/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/websockets/websocket_client_adapter.py` & `neptune-2.0.0a1/src/neptune/internal/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-2.0.0a1/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/internal/websockets/websockets_factory.py` & `neptune-2.0.0a1/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/__init__.py` & `neptune-2.0.0a1/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/exceptions.py` & `neptune-2.0.0a1/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/internal/__init__.py` & `neptune-2.0.0a1/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/internal/api.py` & `neptune-2.0.0a1/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/internal/dto.py` & `neptune-2.0.0a1/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/internal/types.py` & `neptune-2.0.0a1/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/management/internal/utils.py` & `neptune-2.0.0a1/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/objects/__init__.py` & `neptune-2.0.0a1/src/neptune/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/objects/abstract.py` & `neptune-2.0.0a1/src/neptune/objects/abstract.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,26 +9,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["SupportsNamespaces", "AbstractNeptuneObject", "NeptuneObjectCallback"]
+__all__ = ["SupportsNamespaces"]
 
 from abc import (
     ABC,
     abstractmethod,
 )
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Optional,
-    Union,
-)
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from neptune.handler import Handler
 
 
 class SupportsNamespaces(ABC):
     """
@@ -61,15 +56,7 @@
     def __setitem__(self, key: str, value) -> None: ...
 
     @abstractmethod
     def __delitem__(self, path) -> None: ...
 
     @abstractmethod
     def get_root_object(self) -> "SupportsNamespaces": ...
-
-
-class AbstractNeptuneObject(SupportsNamespaces, ABC):
-    @abstractmethod
-    def stop(self, *, seconds: Optional[Union[float, int]] = None) -> None: ...
-
-
-NeptuneObjectCallback = Callable[[AbstractNeptuneObject], None]
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/model.py` & `neptune-2.0.0a1/src/neptune/objects/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,18 @@
     DEFAULT_FLUSH_PERIOD,
     DEFAULT_NAME,
     OFFLINE_PROJECT_QUALIFIED_NAME,
 )
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import verify_type
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
-from neptune.objects.abstract import NeptuneObjectCallback
-from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.neptune_object import (
+    NeptuneObject,
+    NeptuneObjectCallback,
+)
 from neptune.objects.utils import build_raw_query
 from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.typing import (
     ProgressBarCallback,
     ProgressBarType,
 )
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/model_version.py` & `neptune-2.0.0a1/src/neptune/objects/model_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,18 @@
     DEFAULT_NAME,
     OFFLINE_PROJECT_QUALIFIED_NAME,
 )
 from neptune.internal.operation_processors.offline_operation_processor import OfflineOperationProcessor
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import verify_type
 from neptune.internal.utils.ping_background_job import PingBackgroundJob
-from neptune.objects.abstract import NeptuneObjectCallback
-from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.neptune_object import (
+    NeptuneObject,
+    NeptuneObjectCallback,
+)
 from neptune.types.mode import Mode
 from neptune.types.model_version_stage import ModelVersionStage
 
 if TYPE_CHECKING:
     from neptune.internal.background_job import BackgroundJob
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/neptune_object.py` & `neptune-2.0.0a1/src/neptune/objects/neptune_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     partial,
     wraps,
 )
 from queue import Queue
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Union,
 )
 
@@ -89,38 +90,37 @@
     get_logger,
 )
 from neptune.internal.utils.paths import parse_path
 from neptune.internal.utils.uncaught_exception_handler import instance as uncaught_exception_handler
 from neptune.internal.utils.utils import reset_internal_ssl_state
 from neptune.internal.value_to_attribute_visitor import ValueToAttributeVisitor
 from neptune.internal.warnings import warn_about_unsupported_type
-from neptune.objects.abstract import (
-    AbstractNeptuneObject,
-    NeptuneObjectCallback,
-)
 from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.types.type_casting import cast_value
 from neptune.typing import ProgressBarType
 from neptune.utils import stop_synchronization_callback
 
 if TYPE_CHECKING:
     from neptune.internal.signals_processing.signals import Signal
 
 
+NeptuneObjectCallback = Callable[["NeptuneObject"], None]
+
+
 def ensure_not_stopped(fun):
     @wraps(fun)
     def inner_fun(self: "NeptuneObject", *args, **kwargs):
         self._raise_if_stopped()
         return fun(self, *args, **kwargs)
 
     return inner_fun
 
 
-class NeptuneObject(AbstractContextManager, AbstractNeptuneObject):
+class NeptuneObject(AbstractContextManager):
     container_type: ContainerType
 
     def __init__(
         self,
         *,
         project: Optional[str] = None,
         api_token: Optional[str] = None,
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/project.py` & `neptune-2.0.0a1/src/neptune/objects/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 from neptune.internal.state import ContainerState
 from neptune.internal.utils import (
     as_list,
     verify_collection_type,
     verify_type,
     verify_value,
 )
-from neptune.objects.abstract import NeptuneObjectCallback
-from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.neptune_object import (
+    NeptuneObject,
+    NeptuneObjectCallback,
+)
 from neptune.objects.utils import (
     build_raw_query,
     prepare_nql_query,
 )
 from neptune.table import Table
 from neptune.types.mode import Mode
 from neptune.typing import (
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/run.py` & `neptune-2.0.0a1/src/neptune/objects/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,18 @@
 from neptune.internal.utils.source_code import upload_source_code
 from neptune.internal.utils.traceback_job import TracebackJob
 from neptune.internal.warnings import (
     NeptuneWarning,
     warn_once,
 )
 from neptune.internal.websockets.websocket_signals_background_job import WebsocketSignalsBackgroundJob
-from neptune.objects.abstract import NeptuneObjectCallback
-from neptune.objects.neptune_object import NeptuneObject
+from neptune.objects.neptune_object import (
+    NeptuneObject,
+    NeptuneObjectCallback,
+)
 from neptune.types import (
     GitRef,
     StringSeries,
 )
 from neptune.types.atoms.git_ref import GitRefDisabled
 from neptune.types.mode import Mode
```

### Comparing `neptune-2.0.0a0/src/neptune/objects/structure_version.py` & `neptune-2.0.0a1/src/neptune/objects/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/objects/utils.py` & `neptune-2.0.0a1/src/neptune/objects/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/table.py` & `neptune-2.0.0a1/src/neptune/table.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/__init__.py` & `neptune-2.0.0a1/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/__init__.py` & `neptune-2.0.0a1/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/artifact.py` & `neptune-2.0.0a1/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/atom.py` & `neptune-2.0.0a1/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/boolean.py` & `neptune-2.0.0a1/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/datetime.py` & `neptune-2.0.0a1/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/file.py` & `neptune-2.0.0a1/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/float.py` & `neptune-2.0.0a1/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/git_ref.py` & `neptune-2.0.0a1/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/integer.py` & `neptune-2.0.0a1/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/atoms/string.py` & `neptune-2.0.0a1/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/file_set.py` & `neptune-2.0.0a1/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/mode.py` & `neptune-2.0.0a1/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/model_version_stage.py` & `neptune-2.0.0a1/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/namespace.py` & `neptune-2.0.0a1/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/__init__.py` & `neptune-2.0.0a1/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/file_series.py` & `neptune-2.0.0a1/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/float_series.py` & `neptune-2.0.0a1/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/series.py` & `neptune-2.0.0a1/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/series_value.py` & `neptune-2.0.0a1/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/series/string_series.py` & `neptune-2.0.0a1/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/sets/__init__.py` & `neptune-2.0.0a1/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/sets/set.py` & `neptune-2.0.0a1/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/sets/string_set.py` & `neptune-2.0.0a1/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/type_casting.py` & `neptune-2.0.0a1/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/value.py` & `neptune-2.0.0a1/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/value_copy.py` & `neptune-2.0.0a1/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/types/value_visitor.py` & `neptune-2.0.0a1/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/typing.py` & `neptune-2.0.0a1/src/neptune/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = [
     "SupportsNamespaces",
-    "AbstractNeptuneObject",
-    "NeptuneObjectCallback",
     "ProgressBarCallback",
     "ProgressBarType",
 ]
 
 import abc
 import contextlib
 from typing import (
@@ -28,19 +26,15 @@
     Optional,
     Type,
     Union,
 )
 
 from typing_extensions import TypeAlias
 
-from neptune.objects.abstract import (
-    AbstractNeptuneObject,
-    NeptuneObjectCallback,
-    SupportsNamespaces,
-)
+from neptune.objects.abstract import SupportsNamespaces
 
 
 class ProgressBarCallback(contextlib.AbstractContextManager):
     """Abstract base class for progress bar callbacks.
 
     You can use this class to implement your own progress bar callback that will be invoked in table fetching methods:
```

### Comparing `neptune-2.0.0a0/src/neptune/utils.py` & `neptune-2.0.0a1/src/neptune/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,31 @@
     "stop_synchronization_callback",
     "TqdmProgressBar",
     "NullProgressBar",
 ]
 
 from types import TracebackType
 from typing import (
+    TYPE_CHECKING,
     Any,
     Mapping,
     MutableMapping,
     Optional,
     Type,
     Union,
 )
 
 from neptune.internal.init.parameters import DEFAULT_STOP_TIMEOUT
 from neptune.internal.types.stringify_value import StringifyValue
 from neptune.internal.utils.logger import get_logger
-from neptune.typing import (
-    AbstractNeptuneObject,
-    ProgressBarCallback,
-)
+from neptune.typing import ProgressBarCallback
+
+if TYPE_CHECKING:
+    from neptune.objects.neptune_object import NeptuneObject
+
 
 logger = get_logger()
 
 
 def stringify_unsupported(value: Any) -> Union[StringifyValue, Mapping]:
     """Helper function that converts unsupported values in a collection or dictionary to strings.
 
@@ -59,15 +61,15 @@
     """
     if isinstance(value, MutableMapping):
         return {str(k): stringify_unsupported(v) for k, v in value.items()}
 
     return StringifyValue(value=value)
 
 
-def stop_synchronization_callback(neptune_object: AbstractNeptuneObject) -> None:
+def stop_synchronization_callback(neptune_object: "NeptuneObject") -> None:
     """Default callback function that stops a Neptune object's synchronization with the server.
 
     Args:
         neptune_object: A Neptune object (Run, Model, ModelVersion, or Project) to be stopped.
 
     Example:
         >>> import neptune
```

### Comparing `neptune-2.0.0a0/src/neptune/vendor/lib_programname.py` & `neptune-2.0.0a1/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/vendor/pynvml.py` & `neptune-2.0.0a1/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/src/neptune/version.py` & `neptune-2.0.0a1/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a0/PKG-INFO` & `neptune-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neptune Version: 2.0.0a0 Summary: Neptune Client
+Metadata-Version: 2.1 Name: neptune Version: 2.0.0a1 Summary: Neptune Client
 Home-page: https://neptune.ai/ License: Apache-2.0 Keywords: MLOps,ML
 Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store Author:
 neptune.ai Author-email: contact@neptune.ai Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
```

