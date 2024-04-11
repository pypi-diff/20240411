# Comparing `tmp/types-tensorflow-2.15.0.20240314.tar.gz` & `tmp/types-tensorflow-2.15.0.20240411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.15.0.20240314.tar", last modified: Thu Mar 14 02:13:10 2024, max compression
+gzip compressed data, was "types-tensorflow-2.15.0.20240411.tar", last modified: Thu Apr 11 02:17:31 2024, max compression
```

## Comparing `types-tensorflow-2.15.0.20240314.tar` & `types-tensorflow-2.15.0.20240411.tar`

### file list

```diff
@@ -1,206 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-03-14 02:13:09.000000 types-tensorflow-2.15.0.20240314/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.539885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/_aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/autodiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.539885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/autograph/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/autograph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/autograph/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/bitwise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.535885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.543885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.543885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (127)    79860 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    82279 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.543885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/config/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.535885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.543885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.547885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15300 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.551885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    74698 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26278 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28815 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27569 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27150 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19691 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    51282 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    15097 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/data/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/distribute/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/distribute/experimental/coordinator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/experimental/dtensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.555885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/losses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/linalg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/nn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 02:13:09.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/distribute/distribute_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/framework/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/trackable/ressource.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.535885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/training/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/training/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/training/tracking/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/random.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/raw_ops.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/saved_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/saved_model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/saved_model/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/sparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/summary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.559885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/train/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/train/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/train/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.539885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26251 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20061 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12744 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24682 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/tensorflow-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-14 02:12:47.000000 types-tensorflow-2.15.0.20240314/tensorflow-stubs/types/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 02:13:10.563885 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 02:13:10.000000 types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.537975 types-tensorflow-2.15.0.20240411/
+-rw-r--r--   0 runner    (1001) docker     (127)     7980 2024-04-11 02:17:30.000000 types-tensorflow-2.15.0.20240411/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 02:17:30.000000 types-tensorflow-2.15.0.20240411/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-11 02:17:31.537975 types-tensorflow-2.15.0.20240411/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 02:17:31.537975 types-tensorflow-2.15.0.20240411/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-11 02:17:30.000000 types-tensorflow-2.15.0.20240411/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.513975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-11 02:17:30.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/_aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/autodiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.513975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/autograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/autograph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/autograph/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/bitwise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.509975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.513975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.513975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.513975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/config/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.509975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.517975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.521975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/data/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/distribute/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.525975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/distribute/experimental/coordinator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/experimental/dtensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/linalg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/nn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 02:17:30.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/distribute/distribute_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/framework/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.529976 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/trackable/ressource.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.509975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/training/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/training/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/training/tracking/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/raw_ops.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/saved_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/saved_model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/saved_model/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/sparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/summary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/train/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/train/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.509975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.533975 types-tensorflow-2.15.0.20240411/tensorflow-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-11 02:17:07.000000 types-tensorflow-2.15.0.20240411/tensorflow-stubs/types/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 02:17:31.537975 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-11 02:17:31.000000 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-11 02:17:31.000000 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 02:17:31.000000 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 02:17:31.000000 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 02:17:31.000000 types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.15.0.20240314/CHANGELOG.md` & `types-tensorflow-2.15.0.20240411/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.15.0.20240411 (2024-04-11)
+
+Bump mypy-protobuf in sync_tensorflow script and improve generation scripts (#11740)
+
 ## 2.15.0.20240314 (2024-03-14)
 
 `tensorflow`: Add `tensorflow.keras.models.Model` (#11334)
 
 Based on:
 
 - https://github.com/hmc-cs-mdrissi/tensorflow_stubs/blob/main/stubs/tensorflow/saved_model/__init__.pyi
```

### Comparing `types-tensorflow-2.15.0.20240314/PKG-INFO` & `types-tensorflow-2.15.0.20240411/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240314
+Version: 2.15.0.20240411
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a1bfd65e9fa92e1bb61a475c7622ba0376d936d5` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-tensorflow-2.15.0.20240314/setup.py` & `types-tensorflow-2.15.0.20240411/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a1bfd65e9fa92e1bb61a475c7622ba0376d936d5` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.20240314",
+      version="2.15.0.20240411",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf', 'types-requests', 'numpy>=1.20'],
       packages=['tensorflow-stubs'],
-      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'audio.pyi', 'autodiff.pyi', 'autograph/__init__.pyi', 'autograph/experimental.pyi', 'bitwise.pyi', 'compiler/xla/autotune_results_pb2.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/service/metrics_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'config/__init__.pyi', 'config/experimental.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/dataset_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/optimized_function_graph_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/rpc_options_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'distribute/__init__.pyi', 'distribute/experimental/coordinator.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'experimental/dtensor.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/callbacks.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers/__init__.pyi', 'keras/layers/experimental/preprocessing.pyi', 'keras/layers/preprocessing/__init__.pyi', 'keras/layers/preprocessing/index_lookup.pyi', 'keras/losses.pyi', 'keras/metrics.pyi', 'keras/models.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'linalg.pyi', 'math.pyi', 'nn.pyi', 'python/__init__.pyi', 'python/distribute/distribute_lib.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/framework/dtypes.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'python/trackable/resource.pyi', 'python/trackable/ressource.pyi', 'python/training/tracking/autotrackable.pyi', 'random.pyi', 'raw_ops.pyi', 'saved_model/__init__.pyi', 'saved_model/experimental.pyi', 'sparse.pyi', 'strings.pyi', 'summary.pyi', 'train/__init__.pyi', 'train/experimental.pyi', 'tsl/protobuf/autotuning_pb2.pyi', 'tsl/protobuf/bfc_memory_map_pb2.pyi', 'tsl/protobuf/coordination_config_pb2.pyi', 'tsl/protobuf/coordination_service_pb2.pyi', 'tsl/protobuf/distributed_runtime_payloads_pb2.pyi', 'tsl/protobuf/dnn_pb2.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'tsl/protobuf/rpc_options_pb2.pyi', 'tsl/protobuf/test_log_pb2.pyi', 'types/experimental.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'audio.pyi', 'autodiff.pyi', 'autograph/__init__.pyi', 'autograph/experimental.pyi', 'bitwise.pyi', 'compiler/xla/autotune_results_pb2.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/service/metrics_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'config/__init__.pyi', 'config/experimental.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/dataset_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/optimized_function_graph_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/rpc_options_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'distribute/__init__.pyi', 'distribute/experimental/coordinator.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'experimental/dtensor.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/callbacks.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers/__init__.pyi', 'keras/layers/experimental/preprocessing.pyi', 'keras/layers/preprocessing/__init__.pyi', 'keras/layers/preprocessing/index_lookup.pyi', 'keras/losses.pyi', 'keras/metrics.pyi', 'keras/models.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'linalg.pyi', 'math.pyi', 'nn.pyi', 'python/__init__.pyi', 'python/distribute/distribute_lib.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/framework/dtypes.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'python/trackable/resource.pyi', 'python/trackable/ressource.pyi', 'python/training/tracking/autotrackable.pyi', 'random.pyi', 'raw_ops.pyi', 'saved_model/__init__.pyi', 'saved_model/experimental.pyi', 'sparse.pyi', 'strings.pyi', 'summary.pyi', 'train/__init__.pyi', 'train/experimental.pyi', 'tsl/protobuf/autotuning_pb2.pyi', 'tsl/protobuf/bfc_memory_map_pb2.pyi', 'tsl/protobuf/coordination_config_pb2.pyi', 'tsl/protobuf/coordination_service_pb2.pyi', 'tsl/protobuf/distributed_runtime_payloads_pb2.pyi', 'tsl/protobuf/dnn_pb2.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'tsl/protobuf/rpc_options_pb2.pyi', 'tsl/protobuf/test_log_pb2.pyi', 'types/experimental.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/autodiff.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/autodiff.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/autograph/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/autograph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/autograph/experimental.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/autograph/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/bitwise.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/bitwise.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.tsl.protobuf.autotuning_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class AutotuneResults(google.protobuf.message.Message):
     """A collection of algorithms for particular dot/convs.  Usually this is "the
     best" algorithm for the particular dot/conv, although that's not strictly
     required.
 
     Users don't interact with this proto directly.  It's used internally to
     facilitate ahead-of-time autotuning -- The string used by
@@ -39,15 +40,15 @@
     proto.
 
     LINT.IfChange
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Entry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         DEVICE_FIELD_NUMBER: builtins.int
         HLO_FIELD_NUMBER: builtins.int
         RESULT_FIELD_NUMBER: builtins.int
         device: builtins.str
@@ -56,23 +57,24 @@
         def result(self) -> tensorflow.tsl.protobuf.autotuning_pb2.AutotuneResult:
             """nb: These results are always tied to a particular version of
             cublas/cudnn, but this is *especially* true for cublasLt results.  For
             cublasLt gemms, the result is an index into the list of candidate
             algorithms returned by cublasLt.  Different version of cublasLt ->
             different list of algos -> different interpretation of results!
             """
+
         def __init__(
             self,
             *,
             device: builtins.str | None = ...,
             hlo: builtins.str | None = ...,
             result: tensorflow.tsl.protobuf.autotuning_pb2.AutotuneResult | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["result", b"result"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "hlo", b"hlo", "result", b"result"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["result", b"result"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["device", b"device", "hlo", b"hlo", "result", b"result"]) -> None: ...
 
     VERSION_FIELD_NUMBER: builtins.int
     DOTS_FIELD_NUMBER: builtins.int
     CONVS_FIELD_NUMBER: builtins.int
     version: builtins.int
     @property
     def dots(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AutotuneResults.Entry]: ...
@@ -81,10 +83,10 @@
     def __init__(
         self,
         *,
         version: builtins.int | None = ...,
         dots: collections.abc.Iterable[global___AutotuneResults.Entry] | None = ...,
         convs: collections.abc.Iterable[global___AutotuneResults.Entry] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["convs", b"convs", "dots", b"dots", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["convs", b"convs", "dots", b"dots", "version", b"version"]) -> None: ...
 
 global___AutotuneResults = AutotuneResults
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 FIELD NAMES ARE IMPORTANT
 
 Unlike most protos, you can't safely change the names of fields, even if you
 keep the numeric ids the same. This is because we sometimes serialize these
 protos as JSON, which includes the field names in the serialization.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -210,23 +211,23 @@
 """
 MAY_ALIAS: Kind.ValueType  # 1
 """The buffers may or may not alias at runtime."""
 MUST_ALIAS: Kind.ValueType  # 2
 """The buffers must alias at runtime."""
 global___Kind = Kind
 
-@typing_extensions.final
+@typing.final
 class HloInstructionProto(google.protobuf.message.Message):
     """Serialization of HloInstruction.
     Next ID: 81
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class SliceDimensions(google.protobuf.message.Message):
         """Describes the [begin, end) index range and stride for slices."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         START_FIELD_NUMBER: builtins.int
         LIMIT_FIELD_NUMBER: builtins.int
@@ -237,15 +238,15 @@
         def __init__(
             self,
             *,
             start: builtins.int | None = ...,
             limit: builtins.int | None = ...,
             stride: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["limit", b"limit", "start", b"start", "stride", b"stride"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["limit", b"limit", "start", b"start", "stride", b"stride"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     OPCODE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     LITERAL_FIELD_NUMBER: builtins.int
     PARAMETER_NUMBER_FIELD_NUMBER: builtins.int
@@ -309,59 +310,29 @@
     CROSS_PROGRAM_PREFETCH_INDEX_FIELD_NUMBER: builtins.int
     PADDING_TYPE_FIELD_NUMBER: builtins.int
     CUSTOM_CALL_API_VERSION_FIELD_NUMBER: builtins.int
     ASYNC_GROUP_ID_FIELD_NUMBER: builtins.int
     ASYNC_EXECUTION_THREAD_FIELD_NUMBER: builtins.int
     name: builtins.str
     opcode: builtins.str
-    @property
-    def shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ShapeProto: ...
-    @property
-    def metadata(self) -> tensorflow.compiler.xla.xla_data_pb2.OpMetadata: ...
-    @property
-    def literal(self) -> tensorflow.compiler.xla.xla_data_pb2.LiteralProto:
-        """Literal, only present for kConstant."""
     parameter_number: builtins.int
     """Parameter number is only present for kParameter."""
     fusion_kind: builtins.str
     """Fusion state, only present for kFusion."""
     tuple_index: builtins.int
     """Index for kGetTupleElement."""
-    @property
-    def dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """Dimensions present for some operations that require reshaping or
-        broadcasting, including Reshape, Reduce, ReduceWindow, and Reverse.
-        """
-    @property
-    def window(self) -> tensorflow.compiler.xla.xla_data_pb2.Window:
-        """Describes the window in a windowed operation such as convolution."""
-    @property
-    def convolution_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.ConvolutionDimensionNumbers:
-        """Describes the dimension numbers used for a convolution."""
     feature_group_count: builtins.int
     """The number of feature groups. Used for a convolution. Must be a divisor of
     the input feature dimension and output feature dimension. If not specified,
     it will use a default value of 1.
     """
     batch_group_count: builtins.int
-    @property
-    def slice_dimensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloInstructionProto.SliceDimensions]: ...
     exponent_bits: builtins.int
     """The bit sizes for a reduce-precision operation."""
     mantissa_bits: builtins.int
-    @property
-    def dynamic_slice_sizes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """Describes the [start, start + size) range size for a dynamic slice
-        ('start' is specified dynamically in the second operand of the operation).
-        """
-    @property
-    def padding_config(self) -> tensorflow.compiler.xla.xla_data_pb2.PaddingConfig:
-        """The padding configuration that describes the edge padding and interior
-        padding of this pad instruction. Only set for pad instructions.
-        """
     outfeed_config: builtins.bytes
     """Outfeed configuration information, only present for kOutfeed."""
     distribution: tensorflow.compiler.xla.xla_data_pb2.RandomDistribution.ValueType
     """The distribution requested for random number generation.
     Only present for kRng.
     """
     epsilon: builtins.float
@@ -381,47 +352,22 @@
     """
     infeed_config: builtins.bytes
     """The string representation of the infeed configuration."""
     custom_call_target: builtins.str
     """Name of a external target (eg, global symbol) to call, only present for
     kCustomCall.
     """
-    @property
-    def outfeed_shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ShapeProto:
-        """Shape of outfeed request."""
-    @property
-    def dot_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.DotDimensionNumbers:
-        """Describes the dimension numbers used for a dot operation"""
     fft_type: tensorflow.compiler.xla.xla_data_pb2.FftType.ValueType
     """FFT type (FFT, IFFT, etc)."""
-    @property
-    def fft_length(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """FFT length."""
     comparison_direction: builtins.str
     """Comparison direction only used for kCompare."""
-    @property
-    def gather_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.GatherDimensionNumbers:
-        """Gather dimension numbers."""
-    @property
-    def gather_slice_sizes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     id: builtins.int
     """The id of this instruction."""
-    @property
-    def operand_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def control_predecessor_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def called_computation_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
     backend_config: builtins.bytes
     """Backend configuration for the instruction. Has backend-specific meaning."""
-    @property
-    def replica_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.ReplicaGroup]:
-        """Cross replica op fields."""
     all_reduce_id: builtins.int
     """Deprecated, but keeping it for backward compatibility. Use channel_id.
     Non-positive all_reduce_id is equivalent to no all_reduce_id.
     """
     use_global_device_ids: builtins.bool
     """If true, interprets ids in ReplicaGroup as global device ids, which is
     a linearized id of `replica_id * partition_count + partition_id`.
@@ -429,66 +375,34 @@
     is_host_transfer: builtins.bool
     """Whether this Send/Recv instruction transfers data to/from the host. Only
     present for Send and Recv instructions and their SendDone and RecvDone
     partners.
     """
     is_stable: builtins.bool
     """Whether this Sort instruction should be stable."""
-    @property
-    def scatter_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.ScatterDimensionNumbers: ...
-    @property
-    def precision_config(self) -> tensorflow.compiler.xla.xla_data_pb2.PrecisionConfig:
-        """Precision configuration for the instruction. Has backend-specific meaning."""
-    @property
-    def source_target_pairs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.SourceTarget]:
-        """Collective permute field."""
-    @property
-    def domain_entry_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding:
-        """Sharding for kDomain instructions."""
-    @property
-    def domain_exit_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
     constrain_layout: builtins.bool
     """For custom call this indicates that the layouts are constrained. If
     constrain_layout is true then the 'shape' field must contain a layout, and
     'operand_shapes_with_layout' must contain a shape with layout for each
     operand.
     """
-    @property
-    def operand_shapes_with_layout(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.ShapeProto]: ...
-    @property
-    def triangular_solve_options(self) -> tensorflow.compiler.xla.xla_data_pb2.TriangularSolveOptions:
-        """Options for TriangularSolve"""
-    @property
-    def cholesky_options(self) -> tensorflow.compiler.xla.xla_data_pb2.CholeskyOptions:
-        """Options for Cholesky"""
-    @property
-    def parameter_replication(self) -> tensorflow.compiler.xla.xla_data_pb2.ParameterReplication:
-        """Describes how parameters behave with regards to replicas."""
     custom_call_has_side_effect: builtins.bool
     """Whether the kCustomCall instruction has side-effects, only present for
     kCustomCall.
     """
-    @property
-    def output_operand_aliasing(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.OutputOperandAliasing]:
-        """A list of OutputOperandAliasing pairs that specifies aliasing buffers
-        between output and operands for kCustomCall and kFusion.
-        """
     custom_call_schedule: global___CustomCallSchedule.ValueType
     """Specifies the desired schedule for the custom-call. The field is only
     present for custom-call.
     """
     delta: builtins.int
     """The delta value for kRngGetAndUpdateState."""
     indices_are_sorted: builtins.bool
     """Specifies if the gather/scatter indices are guaranteed to be sorted by the
     caller.
     """
-    @property
-    def frontend_attributes(self) -> tensorflow.compiler.xla.xla_data_pb2.FrontendAttributes:
-        """Frontend attributes to pass to the XLA backend."""
     unique_indices: builtins.bool
     """Specifies if all elements updated are guaranteed to be unique by
     the caller.
     """
     rng_algorithm: tensorflow.compiler.xla.xla_data_pb2.RandomAlgorithm.ValueType
     """RNG algorithm used by kRngBitGenerator."""
     comparison_type: builtins.str
@@ -512,14 +426,120 @@
     Negative async_group_id is equivalent to no async group id.
     """
     async_execution_thread: builtins.str
     """Represents a unique execution thread name for one or more async groups.
     Each HLO module may contain a main thread and one or more parallel threads.
     Empty async_execution_thread is equivalent to main thread.
     """
+    @property
+    def shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ShapeProto: ...
+    @property
+    def metadata(self) -> tensorflow.compiler.xla.xla_data_pb2.OpMetadata: ...
+    @property
+    def literal(self) -> tensorflow.compiler.xla.xla_data_pb2.LiteralProto:
+        """Literal, only present for kConstant."""
+
+    @property
+    def dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Dimensions present for some operations that require reshaping or
+        broadcasting, including Reshape, Reduce, ReduceWindow, and Reverse.
+        """
+
+    @property
+    def window(self) -> tensorflow.compiler.xla.xla_data_pb2.Window:
+        """Describes the window in a windowed operation such as convolution."""
+
+    @property
+    def convolution_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.ConvolutionDimensionNumbers:
+        """Describes the dimension numbers used for a convolution."""
+
+    @property
+    def slice_dimensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloInstructionProto.SliceDimensions]: ...
+    @property
+    def dynamic_slice_sizes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """Describes the [start, start + size) range size for a dynamic slice
+        ('start' is specified dynamically in the second operand of the operation).
+        """
+
+    @property
+    def padding_config(self) -> tensorflow.compiler.xla.xla_data_pb2.PaddingConfig:
+        """The padding configuration that describes the edge padding and interior
+        padding of this pad instruction. Only set for pad instructions.
+        """
+
+    @property
+    def outfeed_shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ShapeProto:
+        """Shape of outfeed request."""
+
+    @property
+    def dot_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.DotDimensionNumbers:
+        """Describes the dimension numbers used for a dot operation"""
+
+    @property
+    def fft_length(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """FFT length."""
+
+    @property
+    def gather_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.GatherDimensionNumbers:
+        """Gather dimension numbers."""
+
+    @property
+    def gather_slice_sizes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def operand_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def control_predecessor_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def called_computation_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
+    @property
+    def replica_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.ReplicaGroup]:
+        """Cross replica op fields."""
+
+    @property
+    def scatter_dimension_numbers(self) -> tensorflow.compiler.xla.xla_data_pb2.ScatterDimensionNumbers: ...
+    @property
+    def precision_config(self) -> tensorflow.compiler.xla.xla_data_pb2.PrecisionConfig:
+        """Precision configuration for the instruction. Has backend-specific meaning."""
+
+    @property
+    def source_target_pairs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.SourceTarget]:
+        """Collective permute field."""
+
+    @property
+    def domain_entry_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding:
+        """Sharding for kDomain instructions."""
+
+    @property
+    def domain_exit_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
+    @property
+    def operand_shapes_with_layout(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.ShapeProto]: ...
+    @property
+    def triangular_solve_options(self) -> tensorflow.compiler.xla.xla_data_pb2.TriangularSolveOptions:
+        """Options for TriangularSolve"""
+
+    @property
+    def cholesky_options(self) -> tensorflow.compiler.xla.xla_data_pb2.CholeskyOptions:
+        """Options for Cholesky"""
+
+    @property
+    def parameter_replication(self) -> tensorflow.compiler.xla.xla_data_pb2.ParameterReplication:
+        """Describes how parameters behave with regards to replicas."""
+
+    @property
+    def output_operand_aliasing(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.OutputOperandAliasing]:
+        """A list of OutputOperandAliasing pairs that specifies aliasing buffers
+        between output and operands for kCustomCall and kFusion.
+        """
+
+    @property
+    def frontend_attributes(self) -> tensorflow.compiler.xla.xla_data_pb2.FrontendAttributes:
+        """Frontend attributes to pass to the XLA backend."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         opcode: builtins.str | None = ...,
         shape: tensorflow.compiler.xla.xla_data_pb2.ShapeProto | None = ...,
         metadata: tensorflow.compiler.xla.xla_data_pb2.OpMetadata | None = ...,
@@ -584,127 +604,130 @@
         is_cross_program_prefetch: builtins.bool | None = ...,
         cross_program_prefetch_index: builtins.int | None = ...,
         padding_type: tensorflow.compiler.xla.xla_data_pb2.PaddingType.ValueType | None = ...,
         custom_call_api_version: global___CustomCallApiVersion.ValueType | None = ...,
         async_group_id: builtins.int | None = ...,
         async_execution_thread: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cholesky_options", b"cholesky_options", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "frontend_attributes", b"frontend_attributes", "gather_dimension_numbers", b"gather_dimension_numbers", "literal", b"literal", "metadata", b"metadata", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_shape", b"outfeed_shape", "padding_config", b"padding_config", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "triangular_solve_options", b"triangular_solve_options", "window", b"window"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_reduce_id", b"all_reduce_id", "async_execution_thread", b"async_execution_thread", "async_group_id", b"async_group_id", "backend_config", b"backend_config", "batch_group_count", b"batch_group_count", "called_computation_ids", b"called_computation_ids", "channel_id", b"channel_id", "cholesky_options", b"cholesky_options", "comparison_direction", b"comparison_direction", "comparison_type", b"comparison_type", "constrain_layout", b"constrain_layout", "control_predecessor_ids", b"control_predecessor_ids", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "custom_call_api_version", b"custom_call_api_version", "custom_call_has_side_effect", b"custom_call_has_side_effect", "custom_call_schedule", b"custom_call_schedule", "custom_call_target", b"custom_call_target", "delta", b"delta", "dimensions", b"dimensions", "distribution", b"distribution", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "dynamic_slice_sizes", b"dynamic_slice_sizes", "epsilon", b"epsilon", "exponent_bits", b"exponent_bits", "feature_group_count", b"feature_group_count", "feature_index", b"feature_index", "fft_length", b"fft_length", "fft_type", b"fft_type", "frontend_attributes", b"frontend_attributes", "fusion_kind", b"fusion_kind", "gather_dimension_numbers", b"gather_dimension_numbers", "gather_slice_sizes", b"gather_slice_sizes", "id", b"id", "indices_are_sorted", b"indices_are_sorted", "infeed_config", b"infeed_config", "is_cross_program_prefetch", b"is_cross_program_prefetch", "is_host_transfer", b"is_host_transfer", "is_stable", b"is_stable", "literal", b"literal", "mantissa_bits", b"mantissa_bits", "metadata", b"metadata", "name", b"name", "opcode", b"opcode", "operand_ids", b"operand_ids", "operand_shapes_with_layout", b"operand_shapes_with_layout", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_config", b"outfeed_config", "outfeed_shape", b"outfeed_shape", "output_operand_aliasing", b"output_operand_aliasing", "padding_config", b"padding_config", "padding_type", b"padding_type", "parameter_number", b"parameter_number", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "replica_groups", b"replica_groups", "rng_algorithm", b"rng_algorithm", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "slice_dimensions", b"slice_dimensions", "source_target_pairs", b"source_target_pairs", "triangular_solve_options", b"triangular_solve_options", "tuple_index", b"tuple_index", "unique_indices", b"unique_indices", "use_global_device_ids", b"use_global_device_ids", "window", b"window"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index"]) -> typing_extensions.Literal["cross_program_prefetch_index"] | None: ...
+    def HasField(self, field_name: typing.Literal["cholesky_options", b"cholesky_options", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "frontend_attributes", b"frontend_attributes", "gather_dimension_numbers", b"gather_dimension_numbers", "literal", b"literal", "metadata", b"metadata", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_shape", b"outfeed_shape", "padding_config", b"padding_config", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "triangular_solve_options", b"triangular_solve_options", "window", b"window"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_reduce_id", b"all_reduce_id", "async_execution_thread", b"async_execution_thread", "async_group_id", b"async_group_id", "backend_config", b"backend_config", "batch_group_count", b"batch_group_count", "called_computation_ids", b"called_computation_ids", "channel_id", b"channel_id", "cholesky_options", b"cholesky_options", "comparison_direction", b"comparison_direction", "comparison_type", b"comparison_type", "constrain_layout", b"constrain_layout", "control_predecessor_ids", b"control_predecessor_ids", "convolution_dimension_numbers", b"convolution_dimension_numbers", "cross_program_prefetch_index", b"cross_program_prefetch_index", "custom_call_api_version", b"custom_call_api_version", "custom_call_has_side_effect", b"custom_call_has_side_effect", "custom_call_schedule", b"custom_call_schedule", "custom_call_target", b"custom_call_target", "delta", b"delta", "dimensions", b"dimensions", "distribution", b"distribution", "domain_entry_sharding", b"domain_entry_sharding", "domain_exit_sharding", b"domain_exit_sharding", "dot_dimension_numbers", b"dot_dimension_numbers", "dynamic_slice_sizes", b"dynamic_slice_sizes", "epsilon", b"epsilon", "exponent_bits", b"exponent_bits", "feature_group_count", b"feature_group_count", "feature_index", b"feature_index", "fft_length", b"fft_length", "fft_type", b"fft_type", "frontend_attributes", b"frontend_attributes", "fusion_kind", b"fusion_kind", "gather_dimension_numbers", b"gather_dimension_numbers", "gather_slice_sizes", b"gather_slice_sizes", "id", b"id", "indices_are_sorted", b"indices_are_sorted", "infeed_config", b"infeed_config", "is_cross_program_prefetch", b"is_cross_program_prefetch", "is_host_transfer", b"is_host_transfer", "is_stable", b"is_stable", "literal", b"literal", "mantissa_bits", b"mantissa_bits", "metadata", b"metadata", "name", b"name", "opcode", b"opcode", "operand_ids", b"operand_ids", "operand_shapes_with_layout", b"operand_shapes_with_layout", "optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index", "outfeed_config", b"outfeed_config", "outfeed_shape", b"outfeed_shape", "output_operand_aliasing", b"output_operand_aliasing", "padding_config", b"padding_config", "padding_type", b"padding_type", "parameter_number", b"parameter_number", "parameter_replication", b"parameter_replication", "precision_config", b"precision_config", "replica_groups", b"replica_groups", "rng_algorithm", b"rng_algorithm", "scatter_dimension_numbers", b"scatter_dimension_numbers", "shape", b"shape", "sharding", b"sharding", "slice_dimensions", b"slice_dimensions", "source_target_pairs", b"source_target_pairs", "triangular_solve_options", b"triangular_solve_options", "tuple_index", b"tuple_index", "unique_indices", b"unique_indices", "use_global_device_ids", b"use_global_device_ids", "window", b"window"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_cross_program_prefetch_index", b"optional_cross_program_prefetch_index"]) -> typing.Literal["cross_program_prefetch_index"] | None: ...
 
 global___HloInstructionProto = HloInstructionProto
 
-@typing_extensions.final
+@typing.final
 class HloComputationProto(google.protobuf.message.Message):
     """Serialization of HloComputation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     INSTRUCTIONS_FIELD_NUMBER: builtins.int
     PROGRAM_SHAPE_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
     ROOT_ID_FIELD_NUMBER: builtins.int
     IS_FUSION_COMPUTATION_FIELD_NUMBER: builtins.int
     EXECUTION_THREAD_FIELD_NUMBER: builtins.int
     name: builtins.str
-    @property
-    def instructions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloInstructionProto]:
-        """The array of instructions is always in a valid dependency order, where
-        operands appear before their users.
-        """
-    @property
-    def program_shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ProgramShapeProto:
-        """The program shape (with layout) of this computation."""
     id: builtins.int
     """The id of this computation."""
     root_id: builtins.int
     """The id of the root of the computation."""
     is_fusion_computation: builtins.bool
     """Whether this is a fusion computation. Fusion computations should use this
     to determine whether they are a fusion in CreateFromProto since the
     parent fusion_instruction_ may get removed and be nullptr.
     """
     execution_thread: builtins.str
     """The name of execution thread this computation belongs to."""
+    @property
+    def instructions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloInstructionProto]:
+        """The array of instructions is always in a valid dependency order, where
+        operands appear before their users.
+        """
+
+    @property
+    def program_shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ProgramShapeProto:
+        """The program shape (with layout) of this computation."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         instructions: collections.abc.Iterable[global___HloInstructionProto] | None = ...,
         program_shape: tensorflow.compiler.xla.xla_data_pb2.ProgramShapeProto | None = ...,
         id: builtins.int | None = ...,
         root_id: builtins.int | None = ...,
         is_fusion_computation: builtins.bool | None = ...,
         execution_thread: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["program_shape", b"program_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["execution_thread", b"execution_thread", "id", b"id", "instructions", b"instructions", "is_fusion_computation", b"is_fusion_computation", "name", b"name", "program_shape", b"program_shape", "root_id", b"root_id"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["program_shape", b"program_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["execution_thread", b"execution_thread", "id", b"id", "instructions", b"instructions", "is_fusion_computation", b"is_fusion_computation", "name", b"name", "program_shape", b"program_shape", "root_id", b"root_id"]) -> None: ...
 
 global___HloComputationProto = HloComputationProto
 
-@typing_extensions.final
+@typing.final
 class HloScheduleProto(google.protobuf.message.Message):
     """Serialization of an HLO schedule. An HLO schedule contains a total order of
     instructions for each non-fusion computation in the module.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class InstructionSequence(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         INSTRUCTION_IDS_FIELD_NUMBER: builtins.int
         @property
         def instruction_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
         def __init__(
             self,
             *,
             instruction_ids: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["instruction_ids", b"instruction_ids"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["instruction_ids", b"instruction_ids"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class SequencesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
         def value(self) -> global___HloScheduleProto.InstructionSequence: ...
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: global___HloScheduleProto.InstructionSequence | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     SEQUENCES_FIELD_NUMBER: builtins.int
     @property
     def sequences(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___HloScheduleProto.InstructionSequence]:
         """Map from computation id to sequence."""
+
     def __init__(
         self,
         *,
         sequences: collections.abc.Mapping[builtins.int, global___HloScheduleProto.InstructionSequence] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sequences", b"sequences"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sequences", b"sequences"]) -> None: ...
 
 global___HloScheduleProto = HloScheduleProto
 
-@typing_extensions.final
+@typing.final
 class HloInputOutputAliasProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AliasEntryProto(google.protobuf.message.Message):
         """The following proto describes a pair of aliased an input
         (described by parameter number and a ShapeIndex of the parameter)
         and an output (described by a ShapeIndex of the root
         instruction). For example:
 
         entry = {
@@ -719,51 +742,53 @@
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         OUTPUT_SHAPE_INDEX_FIELD_NUMBER: builtins.int
         PARAMETER_NUMBER_FIELD_NUMBER: builtins.int
         PARAMETER_SHAPE_INDEX_FIELD_NUMBER: builtins.int
         KIND_FIELD_NUMBER: builtins.int
+        parameter_number: builtins.int
+        """Number of the parameter in entry computation."""
+        kind: global___Kind.ValueType
+        """The kind of alias to be setup."""
         @property
         def output_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
             """ShapeIndex of the root hlo."""
-        parameter_number: builtins.int
-        """Number of the parameter in entry computation."""
+
         @property
         def parameter_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
             """ShapeIndex of the parameter instruction."""
-        kind: global___Kind.ValueType
-        """The kind of alias to be setup."""
+
         def __init__(
             self,
             *,
             output_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
             parameter_number: builtins.int | None = ...,
             parameter_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
             kind: global___Kind.ValueType | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["kind", b"kind", "output_shape_index", b"output_shape_index", "parameter_number", b"parameter_number", "parameter_shape_index", b"parameter_shape_index"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["kind", b"kind", "output_shape_index", b"output_shape_index", "parameter_number", b"parameter_number", "parameter_shape_index", b"parameter_shape_index"]) -> None: ...
 
     ENTRIES_FIELD_NUMBER: builtins.int
     @property
     def entries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloInputOutputAliasProto.AliasEntryProto]: ...
     def __init__(
         self,
         *,
         entries: collections.abc.Iterable[global___HloInputOutputAliasProto.AliasEntryProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["entries", b"entries"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["entries", b"entries"]) -> None: ...
 
 global___HloInputOutputAliasProto = HloInputOutputAliasProto
 
-@typing_extensions.final
+@typing.final
 class DynamicParameterBindingProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Binding(google.protobuf.message.Message):
         """A list of bindings which indicates that the `target_param_dim_num` in
         the subshape `target_param_index` of parameter `target_param_num`
         is a dynamic dimension and its real dynamic size is represented
         by `dynamic_param_index` in parameter `dynamic_param_num`.
 
         As an example, imagine we have a program:
@@ -790,66 +815,66 @@
 
         DYNAMIC_PARAM_NUM_FIELD_NUMBER: builtins.int
         DYNAMIC_PARAM_INDEX_FIELD_NUMBER: builtins.int
         TARGET_PARAM_NUM_FIELD_NUMBER: builtins.int
         TARGET_PARAM_INDEX_FIELD_NUMBER: builtins.int
         TARGET_PARAM_DIM_NUM_FIELD_NUMBER: builtins.int
         dynamic_param_num: builtins.int
+        target_param_num: builtins.int
+        target_param_dim_num: builtins.int
         @property
         def dynamic_param_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-        target_param_num: builtins.int
         @property
         def target_param_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-        target_param_dim_num: builtins.int
         def __init__(
             self,
             *,
             dynamic_param_num: builtins.int | None = ...,
             dynamic_param_index: collections.abc.Iterable[builtins.int] | None = ...,
             target_param_num: builtins.int | None = ...,
             target_param_index: collections.abc.Iterable[builtins.int] | None = ...,
             target_param_dim_num: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["dynamic_param_index", b"dynamic_param_index", "dynamic_param_num", b"dynamic_param_num", "target_param_dim_num", b"target_param_dim_num", "target_param_index", b"target_param_index", "target_param_num", b"target_param_num"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["dynamic_param_index", b"dynamic_param_index", "dynamic_param_num", b"dynamic_param_num", "target_param_dim_num", b"target_param_dim_num", "target_param_index", b"target_param_index", "target_param_num", b"target_param_num"]) -> None: ...
 
     ENTRIES_FIELD_NUMBER: builtins.int
     @property
     def entries(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DynamicParameterBindingProto.Binding]: ...
     def __init__(
         self,
         *,
         entries: collections.abc.Iterable[global___DynamicParameterBindingProto.Binding] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["entries", b"entries"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["entries", b"entries"]) -> None: ...
 
 global___DynamicParameterBindingProto = DynamicParameterBindingProto
 
-@typing_extensions.final
+@typing.final
 class CrossProgramPrefetch(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PARAMETER_FIELD_NUMBER: builtins.int
     INDEX_FIELD_NUMBER: builtins.int
     OFFSET_FIELD_NUMBER: builtins.int
     parameter: builtins.int
+    offset: builtins.int
     @property
     def index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    offset: builtins.int
     def __init__(
         self,
         *,
         parameter: builtins.int | None = ...,
         index: collections.abc.Iterable[builtins.int] | None = ...,
         offset: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["index", b"index", "offset", b"offset", "parameter", b"parameter"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["index", b"index", "offset", b"offset", "parameter", b"parameter"]) -> None: ...
 
 global___CrossProgramPrefetch = CrossProgramPrefetch
 
-@typing_extensions.final
+@typing.final
 class HloModuleProto(google.protobuf.message.Message):
     """Serialization of HloModule."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ProfileType:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -868,15 +893,15 @@
 
     INVALID: HloModuleProto.ProfileType.ValueType  # 0
     FLAG: HloModuleProto.ProfileType.ValueType  # 1
     FUSION: HloModuleProto.ProfileType.ValueType  # 2
     LAYOUT: HloModuleProto.ProfileType.ValueType  # 3
     DOT: HloModuleProto.ProfileType.ValueType  # 4
 
-    @typing_extensions.final
+    @typing.final
     class ProfileInfo(google.protobuf.message.Message):
         """Information about the optimization profile that this module contains."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PROFILE_TYPE_FIELD_NUMBER: builtins.int
         RELATIVE_SPEEDUP_FIELD_NUMBER: builtins.int
@@ -894,15 +919,15 @@
             self,
             *,
             profile_type: global___HloModuleProto.ProfileType.ValueType | None = ...,
             relative_speedup: builtins.float | None = ...,
             profile_source: tensorflow.compiler.xla.xla_data_pb2.ProfileSource.ValueType | None = ...,
             compilation_event: tensorflow.compiler.xla.xla_data_pb2.CompilationEvent.ValueType | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["compilation_event", b"compilation_event", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["compilation_event", b"compilation_event", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     ENTRY_COMPUTATION_NAME_FIELD_NUMBER: builtins.int
     ENTRY_COMPUTATION_ID_FIELD_NUMBER: builtins.int
     COMPUTATIONS_FIELD_NUMBER: builtins.int
     HOST_PROGRAM_SHAPE_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
@@ -915,48 +940,54 @@
     SPMD_PARAMETERS_SHARDINGS_FIELD_NUMBER: builtins.int
     USE_AUTO_SPMD_PARTITIONING_FIELD_NUMBER: builtins.int
     PROFILE_INFO_FIELD_NUMBER: builtins.int
     DEVICE_ASSIGNMENT_FIELD_NUMBER: builtins.int
     name: builtins.str
     entry_computation_name: builtins.str
     entry_computation_id: builtins.int
+    id: builtins.int
+    """The id of this module."""
+    is_dynamic: builtins.bool
+    """True if the module contains dynamic computation."""
+    use_auto_spmd_partitioning: builtins.bool
+    """Uses AutoSharding pass or not."""
     @property
     def computations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloComputationProto]:
         """The array of computations is always in a valid dependency order, where
         callees appear before their callers.
         """
+
     @property
     def host_program_shape(self) -> tensorflow.compiler.xla.xla_data_pb2.ProgramShapeProto:
         """The host program shape (with layout) of the entry computation."""
-    id: builtins.int
-    """The id of this module."""
+
     @property
     def schedule(self) -> global___HloScheduleProto:
         """The schedule for this module."""
+
     @property
     def input_output_alias(self) -> global___HloInputOutputAliasProto:
         """Describes alias information between inputs and outputs."""
+
     @property
     def dynamic_parameter_binding(self) -> global___DynamicParameterBindingProto: ...
     @property
     def cross_program_prefetches(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CrossProgramPrefetch]: ...
-    is_dynamic: builtins.bool
-    """True if the module contains dynamic computation."""
     @property
     def spmd_output_sharding(self) -> tensorflow.compiler.xla.xla_data_pb2.OpSharding: ...
     @property
     def spmd_parameters_shardings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.OpSharding]: ...
-    use_auto_spmd_partitioning: builtins.bool
-    """Uses AutoSharding pass or not."""
     @property
     def profile_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloModuleProto.ProfileInfo]:
         """Profile information for the HLO module."""
+
     @property
     def device_assignment(self) -> tensorflow.compiler.xla.xla_data_pb2.DeviceAssignmentProto:
         """DeviceAssignment object information."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         entry_computation_name: builtins.str | None = ...,
         entry_computation_id: builtins.int | None = ...,
         computations: collections.abc.Iterable[global___HloComputationProto] | None = ...,
@@ -969,26 +1000,26 @@
         is_dynamic: builtins.bool | None = ...,
         spmd_output_sharding: tensorflow.compiler.xla.xla_data_pb2.OpSharding | None = ...,
         spmd_parameters_shardings: collections.abc.Iterable[tensorflow.compiler.xla.xla_data_pb2.OpSharding] | None = ...,
         use_auto_spmd_partitioning: builtins.bool | None = ...,
         profile_info: collections.abc.Iterable[global___HloModuleProto.ProfileInfo] | None = ...,
         device_assignment: tensorflow.compiler.xla.xla_data_pb2.DeviceAssignmentProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "host_program_shape", b"host_program_shape", "input_output_alias", b"input_output_alias", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["computations", b"computations", "cross_program_prefetches", b"cross_program_prefetches", "device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "entry_computation_id", b"entry_computation_id", "entry_computation_name", b"entry_computation_name", "host_program_shape", b"host_program_shape", "id", b"id", "input_output_alias", b"input_output_alias", "is_dynamic", b"is_dynamic", "name", b"name", "profile_info", b"profile_info", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding", "spmd_parameters_shardings", b"spmd_parameters_shardings", "use_auto_spmd_partitioning", b"use_auto_spmd_partitioning"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "host_program_shape", b"host_program_shape", "input_output_alias", b"input_output_alias", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["computations", b"computations", "cross_program_prefetches", b"cross_program_prefetches", "device_assignment", b"device_assignment", "dynamic_parameter_binding", b"dynamic_parameter_binding", "entry_computation_id", b"entry_computation_id", "entry_computation_name", b"entry_computation_name", "host_program_shape", b"host_program_shape", "id", b"id", "input_output_alias", b"input_output_alias", "is_dynamic", b"is_dynamic", "name", b"name", "profile_info", b"profile_info", "schedule", b"schedule", "spmd_output_sharding", b"spmd_output_sharding", "spmd_parameters_shardings", b"spmd_parameters_shardings", "use_auto_spmd_partitioning", b"use_auto_spmd_partitioning"]) -> None: ...
 
 global___HloModuleProto = HloModuleProto
 
-@typing_extensions.final
+@typing.final
 class LogicalBufferProto(google.protobuf.message.Message):
     """Serialization of LogicalBuffer."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Location(google.protobuf.message.Message):
         """Location represents an instruction and its shape index, which uniquely
         identifies a point where a buffer is needed.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1003,46 +1034,47 @@
         def __init__(
             self,
             *,
             instruction_name: builtins.str | None = ...,
             instruction_id: builtins.int | None = ...,
             shape_index: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["instruction_id", b"instruction_id", "instruction_name", b"instruction_name", "shape_index", b"shape_index"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["instruction_id", b"instruction_id", "instruction_name", b"instruction_name", "shape_index", b"shape_index"]) -> None: ...
 
     ID_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     DEFINED_AT_FIELD_NUMBER: builtins.int
     COLOR_FIELD_NUMBER: builtins.int
     id: builtins.int
     size: builtins.int
+    color: builtins.int
     @property
     def defined_at(self) -> global___LogicalBufferProto.Location:
         """The location where the buffer is defined."""
-    color: builtins.int
+
     def __init__(
         self,
         *,
         id: builtins.int | None = ...,
         size: builtins.int | None = ...,
         defined_at: global___LogicalBufferProto.Location | None = ...,
         color: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["defined_at", b"defined_at"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["color", b"color", "defined_at", b"defined_at", "id", b"id", "size", b"size"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["defined_at", b"defined_at"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["color", b"color", "defined_at", b"defined_at", "id", b"id", "size", b"size"]) -> None: ...
 
 global___LogicalBufferProto = LogicalBufferProto
 
-@typing_extensions.final
+@typing.final
 class BufferAllocationProto(google.protobuf.message.Message):
     """Serialization of BufferAllocation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Assigned(google.protobuf.message.Message):
         """Assigned represents a single LogicalBuffer that is assigned to this
         BufferAllocation.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1055,15 +1087,15 @@
         def __init__(
             self,
             *,
             logical_buffer_id: builtins.int | None = ...,
             offset: builtins.int | None = ...,
             size: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["logical_buffer_id", b"logical_buffer_id", "offset", b"offset", "size", b"size"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["logical_buffer_id", b"logical_buffer_id", "offset", b"offset", "size", b"size"]) -> None: ...
 
     INDEX_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     IS_THREAD_LOCAL_FIELD_NUMBER: builtins.int
     IS_TUPLE_FIELD_NUMBER: builtins.int
     IS_ENTRY_COMPUTATION_PARAMETER_FIELD_NUMBER: builtins.int
     IS_CONSTANT_FIELD_NUMBER: builtins.int
@@ -1075,19 +1107,19 @@
     index: builtins.int
     size: builtins.int
     is_thread_local: builtins.bool
     is_tuple: builtins.bool
     is_entry_computation_parameter: builtins.bool
     is_constant: builtins.bool
     parameter_number: builtins.int
-    @property
-    def parameter_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     maybe_live_out: builtins.bool
     color: builtins.int
     @property
+    def parameter_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
     def assigned(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BufferAllocationProto.Assigned]: ...
     def __init__(
         self,
         *,
         index: builtins.int | None = ...,
         size: builtins.int | None = ...,
         is_thread_local: builtins.bool | None = ...,
@@ -1096,25 +1128,25 @@
         is_constant: builtins.bool | None = ...,
         parameter_number: builtins.int | None = ...,
         parameter_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
         maybe_live_out: builtins.bool | None = ...,
         color: builtins.int | None = ...,
         assigned: collections.abc.Iterable[global___BufferAllocationProto.Assigned] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["assigned", b"assigned", "color", b"color", "index", b"index", "is_constant", b"is_constant", "is_entry_computation_parameter", b"is_entry_computation_parameter", "is_thread_local", b"is_thread_local", "is_tuple", b"is_tuple", "maybe_live_out", b"maybe_live_out", "parameter_number", b"parameter_number", "parameter_shape_index", b"parameter_shape_index", "size", b"size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["assigned", b"assigned", "color", b"color", "index", b"index", "is_constant", b"is_constant", "is_entry_computation_parameter", b"is_entry_computation_parameter", "is_thread_local", b"is_thread_local", "is_tuple", b"is_tuple", "maybe_live_out", b"maybe_live_out", "parameter_number", b"parameter_number", "parameter_shape_index", b"parameter_shape_index", "size", b"size"]) -> None: ...
 
 global___BufferAllocationProto = BufferAllocationProto
 
-@typing_extensions.final
+@typing.final
 class HeapSimulatorTrace(google.protobuf.message.Message):
     """A trace of a HeapSimulator run."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Event(google.protobuf.message.Message):
         """The trace includes a list of events, where each event describes one action
         performed by the heap simulator.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1172,35 +1204,35 @@
             *,
             kind: global___HeapSimulatorTrace.Event.Kind.ValueType | None = ...,
             buffer_id: builtins.int | None = ...,
             computation_name: builtins.str | None = ...,
             instruction_name: builtins.str | None = ...,
             share_with_canonical_id: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["buffer_id", b"buffer_id", "computation_name", b"computation_name", "instruction_name", b"instruction_name", "kind", b"kind", "share_with_canonical_id", b"share_with_canonical_id"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["buffer_id", b"buffer_id", "computation_name", b"computation_name", "instruction_name", b"instruction_name", "kind", b"kind", "share_with_canonical_id", b"share_with_canonical_id"]) -> None: ...
 
     EVENTS_FIELD_NUMBER: builtins.int
     WHOLE_MODULE_SIMULATION_FIELD_NUMBER: builtins.int
     BUFFER_ALLOCATION_INDEX_FIELD_NUMBER: builtins.int
-    @property
-    def events(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HeapSimulatorTrace.Event]: ...
     whole_module_simulation: builtins.bool
     buffer_allocation_index: builtins.int
+    @property
+    def events(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HeapSimulatorTrace.Event]: ...
     def __init__(
         self,
         *,
         events: collections.abc.Iterable[global___HeapSimulatorTrace.Event] | None = ...,
         whole_module_simulation: builtins.bool | None = ...,
         buffer_allocation_index: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer_allocation_index", b"buffer_allocation_index", "events", b"events", "whole_module_simulation", b"whole_module_simulation"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["buffer_allocation_index", b"buffer_allocation_index", "events", b"events", "whole_module_simulation", b"whole_module_simulation"]) -> None: ...
 
 global___HeapSimulatorTrace = HeapSimulatorTrace
 
-@typing_extensions.final
+@typing.final
 class HloModuleGroupProto(google.protobuf.message.Message):
     """An abstraction representing a set of HLO module built to run concurrently
     across different devices.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1211,25 +1243,25 @@
     def hlo_modules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloModuleProto]: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         hlo_modules: collections.abc.Iterable[global___HloModuleProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["hlo_modules", b"hlo_modules", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["hlo_modules", b"hlo_modules", "name", b"name"]) -> None: ...
 
 global___HloModuleGroupProto = HloModuleGroupProto
 
-@typing_extensions.final
+@typing.final
 class BufferAssignmentProto(google.protobuf.message.Message):
     """Serialization of BufferAssignment."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class BufferAlias(google.protobuf.message.Message):
         """Alias represents a source LogicalBuffer, and the buffer location that
         aliases it.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1240,16 +1272,16 @@
         def location(self) -> global___LogicalBufferProto.Location: ...
         def __init__(
             self,
             *,
             source_buffer_id: builtins.int | None = ...,
             location: global___LogicalBufferProto.Location | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["location", b"location"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["location", b"location", "source_buffer_id", b"source_buffer_id"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["location", b"location"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["location", b"location", "source_buffer_id", b"source_buffer_id"]) -> None: ...
 
     LOGICAL_BUFFERS_FIELD_NUMBER: builtins.int
     BUFFER_ALIASES_FIELD_NUMBER: builtins.int
     BUFFER_ALLOCATIONS_FIELD_NUMBER: builtins.int
     HEAP_SIMULATOR_TRACES_FIELD_NUMBER: builtins.int
     @property
     def logical_buffers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LogicalBufferProto]: ...
@@ -1263,19 +1295,19 @@
         self,
         *,
         logical_buffers: collections.abc.Iterable[global___LogicalBufferProto] | None = ...,
         buffer_aliases: collections.abc.Iterable[global___BufferAssignmentProto.BufferAlias] | None = ...,
         buffer_allocations: collections.abc.Iterable[global___BufferAllocationProto] | None = ...,
         heap_simulator_traces: collections.abc.Iterable[global___HeapSimulatorTrace] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer_aliases", b"buffer_aliases", "buffer_allocations", b"buffer_allocations", "heap_simulator_traces", b"heap_simulator_traces", "logical_buffers", b"logical_buffers"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["buffer_aliases", b"buffer_aliases", "buffer_allocations", b"buffer_allocations", "heap_simulator_traces", b"heap_simulator_traces", "logical_buffers", b"logical_buffers"]) -> None: ...
 
 global___BufferAssignmentProto = BufferAssignmentProto
 
-@typing_extensions.final
+@typing.final
 class HloProto(google.protobuf.message.Message):
     """Grouping message that contains all of the information above."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HLO_MODULE_FIELD_NUMBER: builtins.int
     BUFFER_ASSIGNMENT_FIELD_NUMBER: builtins.int
@@ -1285,57 +1317,60 @@
     def buffer_assignment(self) -> global___BufferAssignmentProto: ...
     def __init__(
         self,
         *,
         hlo_module: global___HloModuleProto | None = ...,
         buffer_assignment: global___BufferAssignmentProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["buffer_assignment", b"buffer_assignment", "hlo_module", b"hlo_module"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffer_assignment", b"buffer_assignment", "hlo_module", b"hlo_module"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["buffer_assignment", b"buffer_assignment", "hlo_module", b"hlo_module"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["buffer_assignment", b"buffer_assignment", "hlo_module", b"hlo_module"]) -> None: ...
 
 global___HloProto = HloProto
 
-@typing_extensions.final
+@typing.final
 class HloSnapshot(google.protobuf.message.Message):
     """Encapsulates HloProto together with the arguments, result, and
     execution_platform. This message is used for purposes such as
     analysis/replay/file-storage.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HLO_FIELD_NUMBER: builtins.int
     ARGUMENTS_FIELD_NUMBER: builtins.int
     RESULT_FIELD_NUMBER: builtins.int
     EXECUTION_PLATFORM_FIELD_NUMBER: builtins.int
+    execution_platform: builtins.str
+    """The name of the platform used to run the graph."""
     @property
     def hlo(self) -> global___HloProto:
         """The hlo graph."""
+
     @property
     def arguments(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.xla_data_pb2.LiteralProto]:
         """The arguments passed to the graph."""
+
     @property
     def result(self) -> tensorflow.compiler.xla.xla_data_pb2.LiteralProto:
         """The result of the graph."""
-    execution_platform: builtins.str
-    """The name of the platform used to run the graph."""
+
     def __init__(
         self,
         *,
         hlo: global___HloProto | None = ...,
         arguments: collections.abc.Iterable[tensorflow.compiler.xla.xla_data_pb2.LiteralProto] | None = ...,
         result: tensorflow.compiler.xla.xla_data_pb2.LiteralProto | None = ...,
         execution_platform: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["hlo", b"hlo", "result", b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arguments", b"arguments", "execution_platform", b"execution_platform", "hlo", b"hlo", "result", b"result"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["hlo", b"hlo", "result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["arguments", b"arguments", "execution_platform", b"execution_platform", "hlo", b"hlo", "result", b"result"]) -> None: ...
 
 global___HloSnapshot = HloSnapshot
 
-@typing_extensions.final
+@typing.final
 class HloModuleMetadataProto(google.protobuf.message.Message):
     """Metadata for an HLO module. Dumped after HLO passes and before LLO lowering
     with filename module_####.metadata.textproto, where #### is
     canonical_module_id.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -1358,31 +1393,33 @@
     if applicable.
     """
     @property
     def partitioned_module_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The canonical module ids of the modules that this one is partitioned into,
         if applicable.
         """
+
     @property
     def pass_metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___HloPassMetadata]:
         """Metadata for the HLO passes that are run on the module."""
+
     def __init__(
         self,
         *,
         canonical_module_id: builtins.int | None = ...,
         module_group_name: builtins.str | None = ...,
         original_module_id: builtins.int | None = ...,
         partitioned_module_ids: collections.abc.Iterable[builtins.int] | None = ...,
         pass_metadata: collections.abc.Iterable[global___HloPassMetadata] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["canonical_module_id", b"canonical_module_id", "module_group_name", b"module_group_name", "original_module_id", b"original_module_id", "partitioned_module_ids", b"partitioned_module_ids", "pass_metadata", b"pass_metadata"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["canonical_module_id", b"canonical_module_id", "module_group_name", b"module_group_name", "original_module_id", b"original_module_id", "partitioned_module_ids", b"partitioned_module_ids", "pass_metadata", b"pass_metadata"]) -> None: ...
 
 global___HloModuleMetadataProto = HloModuleMetadataProto
 
-@typing_extensions.final
+@typing.final
 class HloPassMetadata(google.protobuf.message.Message):
     """Metadata for one run of an HLO pass on a module. Provides more information
     when processing debug dumps of HloProtos about the order of HLO passes and
     various other stats like duration. `pass_id` may also be used to identify a
     particular run of a pass in debug info that propagates through stages of
     compilation.
     """
@@ -1403,78 +1440,80 @@
     that module. Note that a pass_id may not always refer to the same pass
     because the order of passes during compilation may change. For finding
     metadata for a particular pass, pass_name and pipeline_name would be more
     reliable, although note that they may not be unique.
     """
     pass_name: builtins.str
     pipeline_name: builtins.str
-    @property
-    def dump_filenames(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Filenames of the dumps of the module after this pass ran. Module may be
-        dumped in multiple formats, and the order of formats in this field will
-        stay consistent across passes.
-        """
     module_changed: builtins.bool
     """Return value of pass.Run(). True if this pass changed the module, or, in
     the case where the module was run through this pass as part of a module
     group, true if this pass changed any module in the same module group.
     """
     module_id: builtins.int
     """The unique_id of the module that this pass is run on. May be different from
     the canonical_module_id of the HloModuleMetadata that this HloPassMetadata
     is inside.
     """
+    start_timestamp_usec: builtins.int
+    """Timestamp before and after the pass is run. Note they may be equal."""
+    end_timestamp_usec: builtins.int
+    @property
+    def dump_filenames(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Filenames of the dumps of the module after this pass ran. Module may be
+        dumped in multiple formats, and the order of formats in this field will
+        stay consistent across passes.
+        """
+
     @property
     def module_group_module_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """If the module went through this pass as part of a module group, this is
         set as the ids of all the modules in the module group. Empty otherwise.
         """
-    start_timestamp_usec: builtins.int
-    """Timestamp before and after the pass is run. Note they may be equal."""
-    end_timestamp_usec: builtins.int
+
     def __init__(
         self,
         *,
         pass_id: builtins.int | None = ...,
         pass_name: builtins.str | None = ...,
         pipeline_name: builtins.str | None = ...,
         dump_filenames: collections.abc.Iterable[builtins.str] | None = ...,
         module_changed: builtins.bool | None = ...,
         module_id: builtins.int | None = ...,
         module_group_module_ids: collections.abc.Iterable[builtins.int] | None = ...,
         start_timestamp_usec: builtins.int | None = ...,
         end_timestamp_usec: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dump_filenames", b"dump_filenames", "end_timestamp_usec", b"end_timestamp_usec", "module_changed", b"module_changed", "module_group_module_ids", b"module_group_module_ids", "module_id", b"module_id", "pass_id", b"pass_id", "pass_name", b"pass_name", "pipeline_name", b"pipeline_name", "start_timestamp_usec", b"start_timestamp_usec"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dump_filenames", b"dump_filenames", "end_timestamp_usec", b"end_timestamp_usec", "module_changed", b"module_changed", "module_group_module_ids", b"module_group_module_ids", "module_id", b"module_id", "pass_id", b"pass_id", "pass_name", b"pass_name", "pipeline_name", b"pipeline_name", "start_timestamp_usec", b"start_timestamp_usec"]) -> None: ...
 
 global___HloPassMetadata = HloPassMetadata
 
-@typing_extensions.final
+@typing.final
 class EntryFunctionAttributes(google.protobuf.message.Message):
     """Encodes attributes for an entry function."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ShapeIndex(google.protobuf.message.Message):
         """Acts as the underlying container for an xla::ShapeIndex."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         INDICES_FIELD_NUMBER: builtins.int
         @property
         def indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
         def __init__(
             self,
             *,
             indices: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["indices", b"indices"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["indices", b"indices"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class BufferParameterAttributes(google.protobuf.message.Message):
         """Encodes attributes for a single buffer parameter."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         LMHLO_PARAMS_FIELD_NUMBER: builtins.int
         LMHLO_PARAMS_PRESENT_FIELD_NUMBER: builtins.int
@@ -1484,77 +1523,79 @@
         LMHLO_OUTPUT_INDEX_FIELD_NUMBER: builtins.int
         lmhlo_params: builtins.int
         """Represents an lmhlo.params function argument attribute."""
         lmhlo_params_present: builtins.bool
         """TODO(hanbinyoon): Deprecate when optional fields are available in proto3
         (Protocol Buffers v3.15.0).
         """
-        @property
-        def lmhlo_param_shape_index(self) -> global___EntryFunctionAttributes.ShapeIndex:
-            """Represents an lmhlo.param_shape_index function argument attribute."""
         lmhlo_constant_name: builtins.str
         """Represents an lmhlo.constant_name function argument attribute."""
         lmhlo_must_alias: builtins.bool
         """Represents an lmhlo.must_alias function argument attribute."""
         @property
+        def lmhlo_param_shape_index(self) -> global___EntryFunctionAttributes.ShapeIndex:
+            """Represents an lmhlo.param_shape_index function argument attribute."""
+
+        @property
         def lmhlo_output_index(self) -> global___EntryFunctionAttributes.ShapeIndex:
             """Represents an lmhlo.params function argument attribute."""
+
         def __init__(
             self,
             *,
             lmhlo_params: builtins.int | None = ...,
             lmhlo_params_present: builtins.bool | None = ...,
             lmhlo_param_shape_index: global___EntryFunctionAttributes.ShapeIndex | None = ...,
             lmhlo_constant_name: builtins.str | None = ...,
             lmhlo_must_alias: builtins.bool | None = ...,
             lmhlo_output_index: global___EntryFunctionAttributes.ShapeIndex | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["lmhlo_constant_name", b"lmhlo_constant_name", "lmhlo_must_alias", b"lmhlo_must_alias", "lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index", "lmhlo_params", b"lmhlo_params", "lmhlo_params_present", b"lmhlo_params_present"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["lmhlo_constant_name", b"lmhlo_constant_name", "lmhlo_must_alias", b"lmhlo_must_alias", "lmhlo_output_index", b"lmhlo_output_index", "lmhlo_param_shape_index", b"lmhlo_param_shape_index", "lmhlo_params", b"lmhlo_params", "lmhlo_params_present", b"lmhlo_params_present"]) -> None: ...
 
     BUFFERS_FIELD_NUMBER: builtins.int
     RESULT_XLA_SHAPE_FIELD_NUMBER: builtins.int
-    @property
-    def buffers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntryFunctionAttributes.BufferParameterAttributes]: ...
     result_xla_shape: builtins.str
     """xla::Shape in string format."""
+    @property
+    def buffers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EntryFunctionAttributes.BufferParameterAttributes]: ...
     def __init__(
         self,
         *,
         buffers: collections.abc.Iterable[global___EntryFunctionAttributes.BufferParameterAttributes] | None = ...,
         result_xla_shape: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["buffers", b"buffers", "result_xla_shape", b"result_xla_shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["buffers", b"buffers", "result_xla_shape", b"result_xla_shape"]) -> None: ...
 
 global___EntryFunctionAttributes = EntryFunctionAttributes
 
-@typing_extensions.final
+@typing.final
 class XlaRuntimeExecutableProto(google.protobuf.message.Message):
     """Encodes the underlying Xla runtime executable compiled from the XLA module."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HLO_MODULE_PROTO_FIELD_NUMBER: builtins.int
     OBJ_FILE_FIELD_NUMBER: builtins.int
     MLIR_MODULE_FIELD_NUMBER: builtins.int
-    @property
-    def hlo_module_proto(self) -> global___HloModuleProto: ...
     obj_file: builtins.bytes
     """TODO(b/232263665)): Serialized executable has to know what APIs it has to
     be linked with, including the version. For example Gpu executable must be
     linked with a runtime layer that abstracts over CUDA.
 
     Serialized object file compiled from the XLA module.
     """
     mlir_module: builtins.str
     """Serialized MLIR module corresponding to compiled object file."""
+    @property
+    def hlo_module_proto(self) -> global___HloModuleProto: ...
     def __init__(
         self,
         *,
         hlo_module_proto: global___HloModuleProto | None = ...,
         obj_file: builtins.bytes | None = ...,
         mlir_module: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["hlo_module_proto", b"hlo_module_proto"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["hlo_module_proto", b"hlo_module_proto", "mlir_module", b"mlir_module", "obj_file", b"obj_file"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["hlo_module_proto", b"hlo_module_proto"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["hlo_module_proto", b"hlo_module_proto", "mlir_module", b"mlir_module", "obj_file", b"obj_file"]) -> None: ...
 
 global___XlaRuntimeExecutableProto = XlaRuntimeExecutableProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.enum_type_wrapper
@@ -15,15 +16,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CompilationLogEntry(google.protobuf.message.Message):
     """Defines XLA compilation metrics."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CompilationStage:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -46,29 +47,31 @@
     CODE_GENERATION: CompilationLogEntry.CompilationStage.ValueType  # 3
     BACKEND_PASSES: CompilationLogEntry.CompilationStage.ValueType  # 4
 
     TIMESTAMP_FIELD_NUMBER: builtins.int
     STAGE_FIELD_NUMBER: builtins.int
     DURATION_FIELD_NUMBER: builtins.int
     TASK_INDEX_FIELD_NUMBER: builtins.int
+    stage: global___CompilationLogEntry.CompilationStage.ValueType
+    """Compilation stage recorded by this log entry."""
+    task_index: builtins.int
+    """Task index from which this log entry was recorded."""
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Time when the event captured by this log entry occurred."""
-    stage: global___CompilationLogEntry.CompilationStage.ValueType
-    """Compilation stage recorded by this log entry."""
+
     @property
     def duration(self) -> google.protobuf.duration_pb2.Duration:
         """Duration of the given compilation stage."""
-    task_index: builtins.int
-    """Task index from which this log entry was recorded."""
+
     def __init__(
         self,
         *,
         timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         stage: global___CompilationLogEntry.CompilationStage.ValueType | None = ...,
         duration: google.protobuf.duration_pb2.Duration | None = ...,
         task_index: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["duration", b"duration", "timestamp", b"timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["duration", b"duration", "stage", b"stage", "task_index", b"task_index", "timestamp", b"timestamp"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["duration", b"duration", "timestamp", b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["duration", b"duration", "stage", b"stage", "task_index", b"task_index", "timestamp", b"timestamp"]) -> None: ...
 
 global___CompilationLogEntry = CompilationLogEntry
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -373,23 +374,23 @@
 RNG_DEFAULT: RandomAlgorithm.ValueType  # 0
 """Backend dependent default algorithm."""
 RNG_THREE_FRY: RandomAlgorithm.ValueType  # 1
 RNG_PHILOX: RandomAlgorithm.ValueType  # 2
 """Next: 2"""
 global___RandomAlgorithm = RandomAlgorithm
 
-@typing_extensions.final
+@typing.final
 class PaddingConfig(google.protobuf.message.Message):
     """Describes the padding configuration for Pad operation. The padding amount on
     both edges as well as between the elements are specified for each dimension.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class PaddingConfigDimension(google.protobuf.message.Message):
         """Describes the padding configuration for a dimension."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         EDGE_PADDING_LOW_FIELD_NUMBER: builtins.int
         EDGE_PADDING_HIGH_FIELD_NUMBER: builtins.int
@@ -405,30 +406,31 @@
         def __init__(
             self,
             *,
             edge_padding_low: builtins.int | None = ...,
             edge_padding_high: builtins.int | None = ...,
             interior_padding: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["edge_padding_high", b"edge_padding_high", "edge_padding_low", b"edge_padding_low", "interior_padding", b"interior_padding"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["edge_padding_high", b"edge_padding_high", "edge_padding_low", b"edge_padding_low", "interior_padding", b"interior_padding"]) -> None: ...
 
     DIMENSIONS_FIELD_NUMBER: builtins.int
     @property
     def dimensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PaddingConfig.PaddingConfigDimension]:
         """The padding configuration for all dimensions."""
+
     def __init__(
         self,
         *,
         dimensions: collections.abc.Iterable[global___PaddingConfig.PaddingConfigDimension] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dimensions", b"dimensions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dimensions", b"dimensions"]) -> None: ...
 
 global___PaddingConfig = PaddingConfig
 
-@typing_extensions.final
+@typing.final
 class TileProto(google.protobuf.message.Message):
     """Describes a tile used in tiling-based layout. Refer to
     g3doc/third_party/tensorflow/compiler/xla/g3doc/tiled_layout.md for
     details about tiling-based layout.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -437,24 +439,25 @@
     @property
     def dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Number of elements in each dimension of the tile. It's ordered from the
         most major dimension of the tile to the most minor dimension of the tile.
         The dimensions correspond to a suffix of the dimensions of the shape being
         tiled.
         """
+
     def __init__(
         self,
         *,
         dimensions: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dimensions", b"dimensions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dimensions", b"dimensions"]) -> None: ...
 
 global___TileProto = TileProto
 
-@typing_extensions.final
+@typing.final
 class LayoutProto(google.protobuf.message.Message):
     """A layout describes how the array is placed in (1D) memory space.  This
     includes the minor-to-major ordering of dimensions within a shape.
 
     Clients must specify the layouts of input Literals to the
     computation. Layouts specified in interior operations which take Shapes (for
     example, Convert) are ignored.
@@ -472,88 +475,93 @@
     MINOR_TO_MAJOR_FIELD_NUMBER: builtins.int
     TILES_FIELD_NUMBER: builtins.int
     MEMORY_SPACE_FIELD_NUMBER: builtins.int
     INDEX_PRIMITIVE_TYPE_FIELD_NUMBER: builtins.int
     POINTER_PRIMITIVE_TYPE_FIELD_NUMBER: builtins.int
     PHYSICAL_SHAPE_FIELD_NUMBER: builtins.int
     DYNAMIC_SHAPE_METADATA_PREFIX_BYTES_FIELD_NUMBER: builtins.int
+    memory_space: builtins.int
+    """Memory space where this array resides. The integer field is interpreted in
+    a backend-specific manner.
+    """
+    index_primitive_type: global___PrimitiveType.ValueType
+    """The integer types to be used for indices and pointers.  These fields must
+    not be used unless the layout represents a sparse array.  The PrimitiveType
+    must correspond to an unsigned integer (U8, U16, U32, or U64).
+    If not provided, the compiler will use the largest unsigned integer
+    that is naturally supported by the target device (U32 or U64 in currently
+    supported devices).
+    """
+    pointer_primitive_type: global___PrimitiveType.ValueType
+    dynamic_shape_metadata_prefix_bytes: builtins.int
+    """The dynamic shape metadata size in bytes in front of the shape data. The
+    field may be non-zero for a static shape whose associated buffer is for a
+    dynamic shape, e.g. a result of SliceToDynamic.
+    """
     @property
     def dim_level_types(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___DimLevelType.ValueType]:
         """The dimension level type list for this array, specifying the way in which
         each array dimension is represented in memory. If this list is empty, the
         array is assumed to be dense.
         """
+
     @property
     def dim_unique(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]:
         """Whether each dimension is unique or ordered.  Each of the following lists
         must be empty, or have one entry for each entry of dim_level_types.  If
         either list is empty, all dimensions are assumed to be unique and ordered,
         respectively.  Entries in this list may not be false for some DimLevelType
         values (such as DIM_DENSE in particular).
         """
+
     @property
     def dim_ordered(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]: ...
     @property
     def minor_to_major(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Sequence of dimension numbers, from minor (fastest varying index) to major
         (slowest varying index). This field is required.
         """
+
     @property
     def tiles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TileProto]:
         """A sequence of tiles, starting from the tile that's applied first to the
         Shape.
 
         TODO(b/119839262): implement tiling in each backend or add Unimplemented
         error.
         """
-    memory_space: builtins.int
-    """Memory space where this array resides. The integer field is interpreted in
-    a backend-specific manner.
-    """
-    index_primitive_type: global___PrimitiveType.ValueType
-    """The integer types to be used for indices and pointers.  These fields must
-    not be used unless the layout represents a sparse array.  The PrimitiveType
-    must correspond to an unsigned integer (U8, U16, U32, or U64).
-    If not provided, the compiler will use the largest unsigned integer
-    that is naturally supported by the target device (U32 or U64 in currently
-    supported devices).
-    """
-    pointer_primitive_type: global___PrimitiveType.ValueType
+
     @property
     def physical_shape(self) -> global___ShapeProto:
         """The physical, on-device shape used to represent the shape this layout
         belongs to. Only used for sparse arrays.
         The layout(s) contained within the physical shape should not also contain
         a physical shape.
         """
-    dynamic_shape_metadata_prefix_bytes: builtins.int
-    """The dynamic shape metadata size in bytes in front of the shape data. The
-    field may be non-zero for a static shape whose associated buffer is for a
-    dynamic shape, e.g. a result of SliceToDynamic.
-    """
+
     def __init__(
         self,
         *,
         dim_level_types: collections.abc.Iterable[global___DimLevelType.ValueType] | None = ...,
         dim_unique: collections.abc.Iterable[builtins.bool] | None = ...,
         dim_ordered: collections.abc.Iterable[builtins.bool] | None = ...,
         minor_to_major: collections.abc.Iterable[builtins.int] | None = ...,
         tiles: collections.abc.Iterable[global___TileProto] | None = ...,
         memory_space: builtins.int | None = ...,
         index_primitive_type: global___PrimitiveType.ValueType | None = ...,
         pointer_primitive_type: global___PrimitiveType.ValueType | None = ...,
         physical_shape: global___ShapeProto | None = ...,
         dynamic_shape_metadata_prefix_bytes: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["physical_shape", b"physical_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dim_level_types", b"dim_level_types", "dim_ordered", b"dim_ordered", "dim_unique", b"dim_unique", "dynamic_shape_metadata_prefix_bytes", b"dynamic_shape_metadata_prefix_bytes", "index_primitive_type", b"index_primitive_type", "memory_space", b"memory_space", "minor_to_major", b"minor_to_major", "physical_shape", b"physical_shape", "pointer_primitive_type", b"pointer_primitive_type", "tiles", b"tiles"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["physical_shape", b"physical_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dim_level_types", b"dim_level_types", "dim_ordered", b"dim_ordered", "dim_unique", b"dim_unique", "dynamic_shape_metadata_prefix_bytes", b"dynamic_shape_metadata_prefix_bytes", "index_primitive_type", b"index_primitive_type", "memory_space", b"memory_space", "minor_to_major", b"minor_to_major", "physical_shape", b"physical_shape", "pointer_primitive_type", b"pointer_primitive_type", "tiles", b"tiles"]) -> None: ...
 
 global___LayoutProto = LayoutProto
 
-@typing_extensions.final
+@typing.final
 class ShapeProto(google.protobuf.message.Message):
     """A shape describes the number of dimensions in the array, the size of each
     dimension, and the primitive component type.
 
     Tuples are a special case in that they have rank zero and have tuple_shapes
     defined.
 
@@ -578,42 +586,46 @@
         to N-1 for an N-dimensional array. The first element of 'dimensions' is the
         size of dimension 0, the second element is the size of dimension 1, and so
         forth.  Empty list indicates a scalar.
 
         If the respective element in 'is_dimension_dynamic' is true then the value
         in this field represents an upper bound on the size of the dimension.
         """
+
     @property
     def tuple_shapes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ShapeProto]:
         """For tuples only, the shapes of constituent shapes in the tuple sequence."""
+
     @property
     def layout(self) -> global___LayoutProto:
         """The layout used to back this shape."""
+
     @property
     def is_dynamic_dimension(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]:
         """For arrays, this indicates whether or not each dimension is
         dynamically-sized. The number of elements in this repeated field should be
         zero (indicating that no dimensions are dynamic) or equal to the number of
         elements in the 'dimensions' field.
         """
+
     def __init__(
         self,
         *,
         element_type: global___PrimitiveType.ValueType | None = ...,
         dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         tuple_shapes: collections.abc.Iterable[global___ShapeProto] | None = ...,
         layout: global___LayoutProto | None = ...,
         is_dynamic_dimension: collections.abc.Iterable[builtins.bool] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["layout", b"layout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dimensions", b"dimensions", "element_type", b"element_type", "is_dynamic_dimension", b"is_dynamic_dimension", "layout", b"layout", "tuple_shapes", b"tuple_shapes"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["layout", b"layout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dimensions", b"dimensions", "element_type", b"element_type", "is_dynamic_dimension", b"is_dynamic_dimension", "layout", b"layout", "tuple_shapes", b"tuple_shapes"]) -> None: ...
 
 global___ShapeProto = ShapeProto
 
-@typing_extensions.final
+@typing.final
 class ProgramShapeProto(google.protobuf.message.Message):
     """Shape of the parameters and output of a computation (like a traditional
     function signature).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -629,20 +641,20 @@
     def __init__(
         self,
         *,
         parameters: collections.abc.Iterable[global___ShapeProto] | None = ...,
         result: global___ShapeProto | None = ...,
         parameter_names: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["result", b"result"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["parameter_names", b"parameter_names", "parameters", b"parameters", "result", b"result"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["result", b"result"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["parameter_names", b"parameter_names", "parameters", b"parameters", "result", b"result"]) -> None: ...
 
 global___ProgramShapeProto = ProgramShapeProto
 
-@typing_extensions.final
+@typing.final
 class ComputationStats(google.protobuf.message.Message):
     """Statistics of a computation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FLOP_COUNT_FIELD_NUMBER: builtins.int
     TRANSCENDENTAL_COUNT_FIELD_NUMBER: builtins.int
@@ -652,58 +664,59 @@
     """The number of transcendental operations (e.g., exp) in the computation."""
     def __init__(
         self,
         *,
         flop_count: builtins.float | None = ...,
         transcendental_count: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["flop_count", b"flop_count", "transcendental_count", b"transcendental_count"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["flop_count", b"flop_count", "transcendental_count", b"transcendental_count"]) -> None: ...
 
 global___ComputationStats = ComputationStats
 
-@typing_extensions.final
+@typing.final
 class OpMetadata(google.protobuf.message.Message):
     """Symbolization metadata for HLO Instructions.
 
     This metadata is used for debugging XLA code generation, as well as
     performance profiling of XLA-generated executables.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ProfileInfo(google.protobuf.message.Message):
         """Information about the optimization profile that this operation contains."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PROFILE_TYPE_FIELD_NUMBER: builtins.int
         RELATIVE_SPEEDUP_FIELD_NUMBER: builtins.int
         PROFILE_SOURCE_FIELD_NUMBER: builtins.int
         COMPILATION_EVENT_FIELD_NUMBER: builtins.int
-        @property
-        def profile_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___ProfileType.ValueType]:
-            """The type of optimization profiles that this operation contains."""
         relative_speedup: builtins.float
         """Speedup of tuned config compared to default config.
         TODO(b/203817882) Set the relative_speedup.
         """
         profile_source: global___ProfileSource.ValueType
         """The source of the optimization profiles that this operation contains."""
         compilation_event: global___CompilationEvent.ValueType
         """The compilation event that triggered the use of the profiles."""
+        @property
+        def profile_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___ProfileType.ValueType]:
+            """The type of optimization profiles that this operation contains."""
+
         def __init__(
             self,
             *,
             profile_type: collections.abc.Iterable[global___ProfileType.ValueType] | None = ...,
             relative_speedup: builtins.float | None = ...,
             profile_source: global___ProfileSource.ValueType | None = ...,
             compilation_event: global___CompilationEvent.ValueType | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["compilation_event", b"compilation_event", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["compilation_event", b"compilation_event", "profile_source", b"profile_source", "profile_type", b"profile_type", "relative_speedup", b"relative_speedup"]) -> None: ...
 
     OP_TYPE_FIELD_NUMBER: builtins.int
     OP_NAME_FIELD_NUMBER: builtins.int
     SOURCE_FILE_FIELD_NUMBER: builtins.int
     SOURCE_LINE_FIELD_NUMBER: builtins.int
     PROFILE_TYPE_FIELD_NUMBER: builtins.int
     CREATION_PASS_ID_FIELD_NUMBER: builtins.int
@@ -728,17 +741,14 @@
     """
     source_file: builtins.str
     """Indicate a file and line that this op is associated to in a user's program.
 
     e.g. it could be the file and line of user code that generated the op.
     """
     source_line: builtins.int
-    @property
-    def profile_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___ProfileType.ValueType]:
-        """Deprecated, use [ProfileInfo][profile_type] instead."""
     creation_pass_id: builtins.int
     """HloPassMetadata.pass_id of the pass that created this HLO instruction
     object. Should never be copied between HLO instructions. Zero if unset and
     -1 if the instruction was created before HLO passes began.
     """
     logical_creation_pass_id: builtins.int
     """HloPassMetadata.pass_id of the pass that created the logical functionality
@@ -749,36 +759,41 @@
     size_of_generated_code_in_bytes: builtins.int
     """The footprint of the generated code for the instruction."""
     size_of_memory_working_set_in_bytes: builtins.int
     """The size of the working set, i.e., the amount of memory, used by the
     instruction in a compiler-managed fast device memory.
     """
     @property
+    def profile_type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___ProfileType.ValueType]:
+        """Deprecated, use [ProfileInfo][profile_type] instead."""
+
+    @property
     def profile_info(self) -> global___OpMetadata.ProfileInfo:
         """Profile information for the Op."""
+
     def __init__(
         self,
         *,
         op_type: builtins.str | None = ...,
         op_name: builtins.str | None = ...,
         source_file: builtins.str | None = ...,
         source_line: builtins.int | None = ...,
         profile_type: collections.abc.Iterable[global___ProfileType.ValueType] | None = ...,
         creation_pass_id: builtins.int | None = ...,
         logical_creation_pass_id: builtins.int | None = ...,
         size_of_generated_code_in_bytes: builtins.int | None = ...,
         size_of_memory_working_set_in_bytes: builtins.int | None = ...,
         profile_info: global___OpMetadata.ProfileInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["profile_info", b"profile_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_pass_id", b"creation_pass_id", "logical_creation_pass_id", b"logical_creation_pass_id", "op_name", b"op_name", "op_type", b"op_type", "profile_info", b"profile_info", "profile_type", b"profile_type", "size_of_generated_code_in_bytes", b"size_of_generated_code_in_bytes", "size_of_memory_working_set_in_bytes", b"size_of_memory_working_set_in_bytes", "source_file", b"source_file", "source_line", b"source_line"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["profile_info", b"profile_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["creation_pass_id", b"creation_pass_id", "logical_creation_pass_id", b"logical_creation_pass_id", "op_name", b"op_name", "op_type", b"op_type", "profile_info", b"profile_info", "profile_type", b"profile_type", "size_of_generated_code_in_bytes", b"size_of_generated_code_in_bytes", "size_of_memory_working_set_in_bytes", b"size_of_memory_working_set_in_bytes", "source_file", b"source_file", "source_line", b"source_line"]) -> None: ...
 
 global___OpMetadata = OpMetadata
 
-@typing_extensions.final
+@typing.final
 class ExecutionProfile(google.protobuf.message.Message):
     """Profile data from the execution of a computation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMPILATION_CACHE_HIT_FIELD_NUMBER: builtins.int
     COMPILE_TIME_MS_FIELD_NUMBER: builtins.int
@@ -820,38 +835,38 @@
         compile_time_ms: builtins.int | None = ...,
         compute_cycle_count: builtins.int | None = ...,
         compute_time_ns: builtins.int | None = ...,
         compute_and_transfer_time_ns: builtins.int | None = ...,
         executable_size_in_bytes: builtins.int | None = ...,
         profile_cache_hit: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compilation_cache_hit", b"compilation_cache_hit", "compile_time_ms", b"compile_time_ms", "compute_and_transfer_time_ns", b"compute_and_transfer_time_ns", "compute_cycle_count", b"compute_cycle_count", "compute_time_ns", b"compute_time_ns", "executable_size_in_bytes", b"executable_size_in_bytes", "profile_cache_hit", b"profile_cache_hit"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["compilation_cache_hit", b"compilation_cache_hit", "compile_time_ms", b"compile_time_ms", "compute_and_transfer_time_ns", b"compute_and_transfer_time_ns", "compute_cycle_count", b"compute_cycle_count", "compute_time_ns", b"compute_time_ns", "executable_size_in_bytes", b"executable_size_in_bytes", "profile_cache_hit", b"profile_cache_hit"]) -> None: ...
 
 global___ExecutionProfile = ExecutionProfile
 
-@typing_extensions.final
+@typing.final
 class ExecutionHandle(google.protobuf.message.Message):
     """Handle given to a user that represents an execution that the user launched
     asynchronously on the device.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HANDLE_FIELD_NUMBER: builtins.int
     handle: builtins.int
     def __init__(
         self,
         *,
         handle: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle"]) -> None: ...
 
 global___ExecutionHandle = ExecutionHandle
 
-@typing_extensions.final
+@typing.final
 class GlobalDataHandle(google.protobuf.message.Message):
     """Handle given to a user that represents a globally accessible allocation.
     Contrast this against a ComputationDataHandle, which is not globally
     accessible, since it only exists within a specific computation.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -859,19 +874,19 @@
     HANDLE_FIELD_NUMBER: builtins.int
     handle: builtins.int
     def __init__(
         self,
         *,
         handle: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle"]) -> None: ...
 
 global___GlobalDataHandle = GlobalDataHandle
 
-@typing_extensions.final
+@typing.final
 class DeviceHandle(google.protobuf.message.Message):
     """Handle given to a user that represents a replicated virtual device. Each
     replicated device represents N physical devices for execution where N is the
     number of replicas.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -885,19 +900,19 @@
     """
     def __init__(
         self,
         *,
         handle: builtins.int | None = ...,
         device_count: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_count", b"device_count", "handle", b"handle"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device_count", b"device_count", "handle", b"handle"]) -> None: ...
 
 global___DeviceHandle = DeviceHandle
 
-@typing_extensions.final
+@typing.final
 class ChannelHandle(google.protobuf.message.Message):
     """Handle given to a user to represent a channel between two computations
     via a Send and Recv instruction pair. Channels are unbuffered, so Send
     Send instructions will be blocked until the data is transferred.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -941,28 +956,28 @@
     type: global___ChannelHandle.ChannelType.ValueType
     def __init__(
         self,
         *,
         handle: builtins.int | None = ...,
         type: global___ChannelHandle.ChannelType.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle", "type", b"type"]) -> None: ...
 
 global___ChannelHandle = ChannelHandle
 
-@typing_extensions.final
+@typing.final
 class DeviceAssignmentProto(google.protobuf.message.Message):
     """DeviceAssignmentProto is a serialized form of DeviceAssignment class, which
     represents the device ids assigned to a set of replicated computations.
     See xla::DeviceAssignment class comment for more details.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ComputationDevice(google.protobuf.message.Message):
         """Each logical computation runs on replica_count physical devices.
         ComputationDevice represents the device ids assinged to the replicas.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -970,15 +985,15 @@
         @property
         def replica_device_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
         def __init__(
             self,
             *,
             replica_device_ids: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["replica_device_ids", b"replica_device_ids"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["replica_device_ids", b"replica_device_ids"]) -> None: ...
 
     REPLICA_COUNT_FIELD_NUMBER: builtins.int
     COMPUTATION_COUNT_FIELD_NUMBER: builtins.int
     COMPUTATION_DEVICES_FIELD_NUMBER: builtins.int
     replica_count: builtins.int
     computation_count: builtins.int
     @property
@@ -986,19 +1001,19 @@
     def __init__(
         self,
         *,
         replica_count: builtins.int | None = ...,
         computation_count: builtins.int | None = ...,
         computation_devices: collections.abc.Iterable[global___DeviceAssignmentProto.ComputationDevice] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["computation_count", b"computation_count", "computation_devices", b"computation_devices", "replica_count", b"replica_count"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["computation_count", b"computation_count", "computation_devices", b"computation_devices", "replica_count", b"replica_count"]) -> None: ...
 
 global___DeviceAssignmentProto = DeviceAssignmentProto
 
-@typing_extensions.final
+@typing.final
 class LiteralProto(google.protobuf.message.Message):
     """Literals are used when the server and client need to exchange materialized
     data / results. Literals are also used to describe constants used in
     computations.
 
     Transfers to/from the client are encoded in literal form, and the structure
     of the repeated fields is implied by the shape.
@@ -1022,20 +1037,27 @@
     F16S_FIELD_NUMBER: builtins.int
     BF16S_FIELD_NUMBER: builtins.int
     U16S_FIELD_NUMBER: builtins.int
     S16S_FIELD_NUMBER: builtins.int
     F8E5M2S_FIELD_NUMBER: builtins.int
     F8E4M3FNS_FIELD_NUMBER: builtins.int
     SPARSE_INDICES_FIELD_NUMBER: builtins.int
+    s8s: builtins.bytes
+    u8s: builtins.bytes
+    f16s: builtins.bytes
+    """The F16s, BF16s, U16s and S16s are encoded in little endian byte order"""
+    bf16s: builtins.bytes
+    u16s: builtins.bytes
+    s16s: builtins.bytes
+    f8e5m2s: builtins.bytes
+    f8e4m3fns: builtins.bytes
     @property
     def shape(self) -> global___ShapeProto: ...
     @property
     def preds(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]: ...
-    s8s: builtins.bytes
-    u8s: builtins.bytes
     @property
     def s32s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
     def s64s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
     def u32s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
@@ -1043,29 +1065,25 @@
     @property
     def f32s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     @property
     def f64s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     @property
     def c64s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Stored as interleaved real, imag floats."""
+
     @property
     def c128s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Stored as interleaved real, imag doubles."""
+
     @property
     def tuple_literals(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___LiteralProto]: ...
-    f16s: builtins.bytes
-    """The F16s, BF16s, U16s and S16s are encoded in little endian byte order"""
-    bf16s: builtins.bytes
-    u16s: builtins.bytes
-    s16s: builtins.bytes
-    f8e5m2s: builtins.bytes
-    f8e4m3fns: builtins.bytes
     @property
     def sparse_indices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Next = 21"""
+
     def __init__(
         self,
         *,
         shape: global___ShapeProto | None = ...,
         preds: collections.abc.Iterable[builtins.bool] | None = ...,
         s8s: builtins.bytes | None = ...,
         u8s: builtins.bytes | None = ...,
@@ -1082,20 +1100,20 @@
         bf16s: builtins.bytes | None = ...,
         u16s: builtins.bytes | None = ...,
         s16s: builtins.bytes | None = ...,
         f8e5m2s: builtins.bytes | None = ...,
         f8e4m3fns: builtins.bytes | None = ...,
         sparse_indices: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bf16s", b"bf16s", "c128s", b"c128s", "c64s", b"c64s", "f16s", b"f16s", "f32s", b"f32s", "f64s", b"f64s", "f8e4m3fns", b"f8e4m3fns", "f8e5m2s", b"f8e5m2s", "preds", b"preds", "s16s", b"s16s", "s32s", b"s32s", "s64s", b"s64s", "s8s", b"s8s", "shape", b"shape", "sparse_indices", b"sparse_indices", "tuple_literals", b"tuple_literals", "u16s", b"u16s", "u32s", b"u32s", "u64s", b"u64s", "u8s", b"u8s"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bf16s", b"bf16s", "c128s", b"c128s", "c64s", b"c64s", "f16s", b"f16s", "f32s", b"f32s", "f64s", b"f64s", "f8e4m3fns", b"f8e4m3fns", "f8e5m2s", b"f8e5m2s", "preds", b"preds", "s16s", b"s16s", "s32s", b"s32s", "s64s", b"s64s", "s8s", b"s8s", "shape", b"shape", "sparse_indices", b"sparse_indices", "tuple_literals", b"tuple_literals", "u16s", b"u16s", "u32s", b"u32s", "u64s", b"u64s", "u8s", b"u8s"]) -> None: ...
 
 global___LiteralProto = LiteralProto
 
-@typing_extensions.final
+@typing.final
 class WindowDimension(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SIZE_FIELD_NUMBER: builtins.int
     STRIDE_FIELD_NUMBER: builtins.int
     PADDING_LOW_FIELD_NUMBER: builtins.int
     PADDING_HIGH_FIELD_NUMBER: builtins.int
@@ -1149,19 +1167,19 @@
         stride: builtins.int | None = ...,
         padding_low: builtins.int | None = ...,
         padding_high: builtins.int | None = ...,
         window_dilation: builtins.int | None = ...,
         base_dilation: builtins.int | None = ...,
         window_reversal: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["base_dilation", b"base_dilation", "padding_high", b"padding_high", "padding_low", b"padding_low", "size", b"size", "stride", b"stride", "window_dilation", b"window_dilation", "window_reversal", b"window_reversal"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["base_dilation", b"base_dilation", "padding_high", b"padding_high", "padding_low", b"padding_low", "size", b"size", "stride", b"stride", "window_dilation", b"window_dilation", "window_reversal", b"window_reversal"]) -> None: ...
 
 global___WindowDimension = WindowDimension
 
-@typing_extensions.final
+@typing.final
 class Window(google.protobuf.message.Message):
     """Describes the windowing in an operation such as convolution.
 
     The window is moved across a base area and for each position of the
     window a computation is performed. The field below describes the
     window and the movement of the window across a base area.
     """
@@ -1172,32 +1190,36 @@
     @property
     def dimensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___WindowDimension]: ...
     def __init__(
         self,
         *,
         dimensions: collections.abc.Iterable[global___WindowDimension] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dimensions", b"dimensions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dimensions", b"dimensions"]) -> None: ...
 
 global___Window = Window
 
-@typing_extensions.final
+@typing.final
 class GatherDimensionNumbers(google.protobuf.message.Message):
     """Describes the dimension numbers for a gather operation.
 
     See https://www.tensorflow.org/performance/xla/operation_semantics#gather for
     more details.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OFFSET_DIMS_FIELD_NUMBER: builtins.int
     COLLAPSED_SLICE_DIMS_FIELD_NUMBER: builtins.int
     START_INDEX_MAP_FIELD_NUMBER: builtins.int
     INDEX_VECTOR_DIM_FIELD_NUMBER: builtins.int
+    index_vector_dim: builtins.int
+    """The dimension in the start_indices input that contains the starting
+    indices.
+    """
     @property
     def offset_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """"Window indices" is a term for a set of indices that index into the
         interior of a dynamic-slice from the input tensor, the starting indices for
         which were computed from output_gather_dims (see the operation semantic for
         how this is defined) and the start_indices tensor.
 
@@ -1206,74 +1228,74 @@
          i = 0
          for (k : [0, input_tensor_shape.rank))
            window_indices[k] =
              if k in collapsed_slice_dims
              then 0
              else Out[offset_dims[i++]]
         """
+
     @property
     def collapsed_slice_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
     def start_index_map(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """This is interpreted as a map from i to start_index_map[i]. It
         transforms the gather index looked up from the start_indices tensor into
         the starting index in the input space.
         """
-    index_vector_dim: builtins.int
-    """The dimension in the start_indices input that contains the starting
-    indices.
-    """
+
     def __init__(
         self,
         *,
         offset_dims: collections.abc.Iterable[builtins.int] | None = ...,
         collapsed_slice_dims: collections.abc.Iterable[builtins.int] | None = ...,
         start_index_map: collections.abc.Iterable[builtins.int] | None = ...,
         index_vector_dim: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["collapsed_slice_dims", b"collapsed_slice_dims", "index_vector_dim", b"index_vector_dim", "offset_dims", b"offset_dims", "start_index_map", b"start_index_map"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["collapsed_slice_dims", b"collapsed_slice_dims", "index_vector_dim", b"index_vector_dim", "offset_dims", b"offset_dims", "start_index_map", b"start_index_map"]) -> None: ...
 
 global___GatherDimensionNumbers = GatherDimensionNumbers
 
-@typing_extensions.final
+@typing.final
 class ScatterDimensionNumbers(google.protobuf.message.Message):
     """Describes the dimension numbers for a scatter operation.
 
     All the fields are similar to the corresponding fields in
     GatherDimensionNumbers. Differences are noted below.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     UPDATE_WINDOW_DIMS_FIELD_NUMBER: builtins.int
     INSERTED_WINDOW_DIMS_FIELD_NUMBER: builtins.int
     SCATTER_DIMS_TO_OPERAND_DIMS_FIELD_NUMBER: builtins.int
     INDEX_VECTOR_DIM_FIELD_NUMBER: builtins.int
+    index_vector_dim: builtins.int
     @property
     def update_window_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The set of dimensions in the updates shape that are window dimensions."""
+
     @property
     def inserted_window_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The set of window dimensions that must be inserted into the updates shape."""
+
     @property
     def scatter_dims_to_operand_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    index_vector_dim: builtins.int
     def __init__(
         self,
         *,
         update_window_dims: collections.abc.Iterable[builtins.int] | None = ...,
         inserted_window_dims: collections.abc.Iterable[builtins.int] | None = ...,
         scatter_dims_to_operand_dims: collections.abc.Iterable[builtins.int] | None = ...,
         index_vector_dim: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["index_vector_dim", b"index_vector_dim", "inserted_window_dims", b"inserted_window_dims", "scatter_dims_to_operand_dims", b"scatter_dims_to_operand_dims", "update_window_dims", b"update_window_dims"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["index_vector_dim", b"index_vector_dim", "inserted_window_dims", b"inserted_window_dims", "scatter_dims_to_operand_dims", b"scatter_dims_to_operand_dims", "update_window_dims", b"update_window_dims"]) -> None: ...
 
 global___ScatterDimensionNumbers = ScatterDimensionNumbers
 
-@typing_extensions.final
+@typing.final
 class ConvolutionDimensionNumbers(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INPUT_BATCH_DIMENSION_FIELD_NUMBER: builtins.int
     INPUT_FEATURE_DIMENSION_FIELD_NUMBER: builtins.int
     INPUT_SPATIAL_DIMENSIONS_FIELD_NUMBER: builtins.int
     KERNEL_INPUT_FEATURE_DIMENSION_FIELD_NUMBER: builtins.int
@@ -1282,92 +1304,99 @@
     OUTPUT_BATCH_DIMENSION_FIELD_NUMBER: builtins.int
     OUTPUT_FEATURE_DIMENSION_FIELD_NUMBER: builtins.int
     OUTPUT_SPATIAL_DIMENSIONS_FIELD_NUMBER: builtins.int
     input_batch_dimension: builtins.int
     """The number of the dimension that represents batch in the input."""
     input_feature_dimension: builtins.int
     """The number of the dimension that represents features in the input."""
-    @property
-    def input_spatial_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-        """The dimension numbers for the spatial dimensions that the window
-        moves through in the input.
-        """
     kernel_input_feature_dimension: builtins.int
     """The number of the dimension that represents input features in the
     convolutional kernel (rhs).
     """
     kernel_output_feature_dimension: builtins.int
     """The number of the dimension that represents output features in
     the convolutional kernel (rhs).
     """
+    output_batch_dimension: builtins.int
+    """The number of the dimension that represents batch in the output."""
+    output_feature_dimension: builtins.int
+    """The number of the dimension that represents features in the output."""
+    @property
+    def input_spatial_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+        """The dimension numbers for the spatial dimensions that the window
+        moves through in the input.
+        """
+
     @property
     def kernel_spatial_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers for the spatial dimensions that the window
         moves through in the kernel (rhs). window.strides(0) is the
         stride in the kernel_spatial_dimensions(0) dimension.
         """
-    output_batch_dimension: builtins.int
-    """The number of the dimension that represents batch in the output."""
-    output_feature_dimension: builtins.int
-    """The number of the dimension that represents features in the output."""
+
     @property
     def output_spatial_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers for the spatial dimensions that the window
         moves through in the output.
         """
+
     def __init__(
         self,
         *,
         input_batch_dimension: builtins.int | None = ...,
         input_feature_dimension: builtins.int | None = ...,
         input_spatial_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         kernel_input_feature_dimension: builtins.int | None = ...,
         kernel_output_feature_dimension: builtins.int | None = ...,
         kernel_spatial_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         output_batch_dimension: builtins.int | None = ...,
         output_feature_dimension: builtins.int | None = ...,
         output_spatial_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["input_batch_dimension", b"input_batch_dimension", "input_feature_dimension", b"input_feature_dimension", "input_spatial_dimensions", b"input_spatial_dimensions", "kernel_input_feature_dimension", b"kernel_input_feature_dimension", "kernel_output_feature_dimension", b"kernel_output_feature_dimension", "kernel_spatial_dimensions", b"kernel_spatial_dimensions", "output_batch_dimension", b"output_batch_dimension", "output_feature_dimension", b"output_feature_dimension", "output_spatial_dimensions", b"output_spatial_dimensions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["input_batch_dimension", b"input_batch_dimension", "input_feature_dimension", b"input_feature_dimension", "input_spatial_dimensions", b"input_spatial_dimensions", "kernel_input_feature_dimension", b"kernel_input_feature_dimension", "kernel_output_feature_dimension", b"kernel_output_feature_dimension", "kernel_spatial_dimensions", b"kernel_spatial_dimensions", "output_batch_dimension", b"output_batch_dimension", "output_feature_dimension", b"output_feature_dimension", "output_spatial_dimensions", b"output_spatial_dimensions"]) -> None: ...
 
 global___ConvolutionDimensionNumbers = ConvolutionDimensionNumbers
 
-@typing_extensions.final
+@typing.final
 class DotDimensionNumbers(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LHS_CONTRACTING_DIMENSIONS_FIELD_NUMBER: builtins.int
     RHS_CONTRACTING_DIMENSIONS_FIELD_NUMBER: builtins.int
     LHS_BATCH_DIMENSIONS_FIELD_NUMBER: builtins.int
     RHS_BATCH_DIMENSIONS_FIELD_NUMBER: builtins.int
     @property
     def lhs_contracting_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers that represent the 'lhs' contracting dimensions."""
+
     @property
     def rhs_contracting_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers that represent the 'rhs' contracting dimensions."""
+
     @property
     def lhs_batch_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers that represent the 'lhs' batch dimensions."""
+
     @property
     def rhs_batch_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimension numbers that represent the 'rhs' batch dimensions."""
+
     def __init__(
         self,
         *,
         lhs_contracting_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         rhs_contracting_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         lhs_batch_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         rhs_batch_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lhs_batch_dimensions", b"lhs_batch_dimensions", "lhs_contracting_dimensions", b"lhs_contracting_dimensions", "rhs_batch_dimensions", b"rhs_batch_dimensions", "rhs_contracting_dimensions", b"rhs_contracting_dimensions"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["lhs_batch_dimensions", b"lhs_batch_dimensions", "lhs_contracting_dimensions", b"lhs_contracting_dimensions", "rhs_batch_dimensions", b"rhs_batch_dimensions", "rhs_contracting_dimensions", b"rhs_contracting_dimensions"]) -> None: ...
 
 global___DotDimensionNumbers = DotDimensionNumbers
 
-@typing_extensions.final
+@typing.final
 class TriangularSolveOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Transpose:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -1407,73 +1436,73 @@
         self,
         *,
         left_side: builtins.bool | None = ...,
         lower: builtins.bool | None = ...,
         unit_diagonal: builtins.bool | None = ...,
         transpose_a: global___TriangularSolveOptions.Transpose.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["left_side", b"left_side", "lower", b"lower", "transpose_a", b"transpose_a", "unit_diagonal", b"unit_diagonal"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["left_side", b"left_side", "lower", b"lower", "transpose_a", b"transpose_a", "unit_diagonal", b"unit_diagonal"]) -> None: ...
 
 global___TriangularSolveOptions = TriangularSolveOptions
 
-@typing_extensions.final
+@typing.final
 class CholeskyOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOWER_FIELD_NUMBER: builtins.int
     lower: builtins.bool
     """If true, uses the lower triangle of `a`. If false, uses the upper triangle
     of `a`.
     """
     def __init__(
         self,
         *,
         lower: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lower", b"lower"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["lower", b"lower"]) -> None: ...
 
 global___CholeskyOptions = CholeskyOptions
 
-@typing_extensions.final
+@typing.final
 class FrontendAttributes(google.protobuf.message.Message):
     """Generic map of attributes used to pass hints / configuration options from
     the Python frontend to the XLA backend.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class MapEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     MAP_FIELD_NUMBER: builtins.int
     @property
     def map(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     def __init__(
         self,
         *,
         map: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["map", b"map"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["map", b"map"]) -> None: ...
 
 global___FrontendAttributes = FrontendAttributes
 
-@typing_extensions.final
+@typing.final
 class OpSharding(google.protobuf.message.Message):
     """LINT.IfChange"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -1517,99 +1546,106 @@
     TILE_ASSIGNMENT_DIMENSIONS_FIELD_NUMBER: builtins.int
     TILE_ASSIGNMENT_DEVICES_FIELD_NUMBER: builtins.int
     TUPLE_SHARDINGS_FIELD_NUMBER: builtins.int
     REPLICATE_ON_LAST_TILE_DIM_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     LAST_TILE_DIMS_FIELD_NUMBER: builtins.int
     type: global___OpSharding.Type.ValueType
+    replicate_on_last_tile_dim: builtins.bool
+    """Only used for OTHER type. If true, data is sharded according to other
+    dimensions of tile_assignment(), but replicated across devices along the
+    last dimension. (Experimental)
+    """
     @property
     def tile_shape(self) -> global___ShapeProto:
         """The shape of the sharded tile."""
+
     @property
     def tile_assignment_dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The shape of the tile assignment tensor - this must be the same rank as
         tile_shape and the product of its dimensions must equal
         tile_assignment_devices.size().
         """
+
     @property
     def tile_assignment_devices(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Flattened list of device IDs. The order of flattening is the same as used
         by IndexUtil::MultiToLinearIndex(tile_assignment_shape).
         """
+
     @property
     def tuple_shardings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpSharding]:
         """If type == TUPLE, the sub-shardings, one per leaf node in the tuple shape,
         in pre-order. The tuple shape could be nested; here we store just a
         flattened list of all leaves in the tuple shape. Note that the tuple shape
         is not stored here; shardings do not store the shapes to which they are
         applied, this is inferred from the instruction this sharding gets attached
         to.
         """
-    replicate_on_last_tile_dim: builtins.bool
-    """Only used for OTHER type. If true, data is sharded according to other
-    dimensions of tile_assignment(), but replicated across devices along the
-    last dimension. (Experimental)
-    """
+
     @property
     def metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpMetadata]:
         """This field is used to track the source of this sharding, usually derived
         from instructions. Multple metadata may be populated if sharding is
         combined with other shardings.  Metadata are to not be populated when
         type == TUPLE and instead metadata should be set on individual tuple
         elements.
         """
+
     @property
     def last_tile_dims(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___OpSharding.Type.ValueType]:
         """This field is used to represented the sharding type of each subgroup.
         For example, sharding={devices=[2,2,2,2]0,1,2,...,15 last_tile_dims={
         replicate, manual, unreduced}} means that each of the last 3 dimensions
         in [2,2,2,2] represents a subgrouping in replicate, manual,
         unreduced sharding type respectively.
         """
+
     def __init__(
         self,
         *,
         type: global___OpSharding.Type.ValueType | None = ...,
         tile_shape: global___ShapeProto | None = ...,
         tile_assignment_dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         tile_assignment_devices: collections.abc.Iterable[builtins.int] | None = ...,
         tuple_shardings: collections.abc.Iterable[global___OpSharding] | None = ...,
         replicate_on_last_tile_dim: builtins.bool | None = ...,
         metadata: collections.abc.Iterable[global___OpMetadata] | None = ...,
         last_tile_dims: collections.abc.Iterable[global___OpSharding.Type.ValueType] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tile_shape", b"tile_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["last_tile_dims", b"last_tile_dims", "metadata", b"metadata", "replicate_on_last_tile_dim", b"replicate_on_last_tile_dim", "tile_assignment_devices", b"tile_assignment_devices", "tile_assignment_dimensions", b"tile_assignment_dimensions", "tile_shape", b"tile_shape", "tuple_shardings", b"tuple_shardings", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tile_shape", b"tile_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["last_tile_dims", b"last_tile_dims", "metadata", b"metadata", "replicate_on_last_tile_dim", b"replicate_on_last_tile_dim", "tile_assignment_devices", b"tile_assignment_devices", "tile_assignment_dimensions", b"tile_assignment_dimensions", "tile_shape", b"tile_shape", "tuple_shardings", b"tuple_shardings", "type", b"type"]) -> None: ...
 
 global___OpSharding = OpSharding
 
-@typing_extensions.final
+@typing.final
 class ReplicaGroup(google.protobuf.message.Message):
     """Describes the replica groups in a cross replica op (e.g., all-reduce and
     all-to-all).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REPLICA_IDS_FIELD_NUMBER: builtins.int
     @property
     def replica_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The ids of the replicas that belongs to the same group. The ordering of the
         ids matters in some ops (e.g., all-to-all).
         """
+
     def __init__(
         self,
         *,
         replica_ids: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["replica_ids", b"replica_ids"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["replica_ids", b"replica_ids"]) -> None: ...
 
 global___ReplicaGroup = ReplicaGroup
 
-@typing_extensions.final
+@typing.final
 class SourceTarget(google.protobuf.message.Message):
     """Describes the source target pair in the collective permute op."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
@@ -1617,19 +1653,19 @@
     target: builtins.int
     def __init__(
         self,
         *,
         source: builtins.int | None = ...,
         target: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["source", b"source", "target", b"target"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["source", b"source", "target", b"target"]) -> None: ...
 
 global___SourceTarget = SourceTarget
 
-@typing_extensions.final
+@typing.final
 class PrecisionConfig(google.protobuf.message.Message):
     """Used to indicate the precision configuration. It has backend specific
     meaning.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1656,19 +1692,19 @@
     @property
     def operand_precision(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___PrecisionConfig.Precision.ValueType]: ...
     def __init__(
         self,
         *,
         operand_precision: collections.abc.Iterable[global___PrecisionConfig.Precision.ValueType] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["operand_precision", b"operand_precision"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["operand_precision", b"operand_precision"]) -> None: ...
 
 global___PrecisionConfig = PrecisionConfig
 
-@typing_extensions.final
+@typing.final
 class ParameterReplication(google.protobuf.message.Message):
     """Describes whether all data-parallelism replicas will receive the same
     parameter data at each buffer.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -1678,85 +1714,87 @@
         """A list of boolean values for the flattened leaf buffers. Each value
         indicates whether the corresponding leaf buffer is replicated.
 
         If this field is empty, it means no buffer is replicated. Otherwise, the
         number of elements in this field must match the number of leaf buffers in
         the HLO instruction's shape.
         """
+
     def __init__(
         self,
         *,
         replicated_at_leaf_buffers: collections.abc.Iterable[builtins.bool] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["replicated_at_leaf_buffers", b"replicated_at_leaf_buffers"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["replicated_at_leaf_buffers", b"replicated_at_leaf_buffers"]) -> None: ...
 
 global___ParameterReplication = ParameterReplication
 
-@typing_extensions.final
+@typing.final
 class WhileLoopBackendConfig(google.protobuf.message.Message):
     """A backend-config for kWhile loops that stores the loop's trip count, if it is
     known.
 
     This is useful for backends that can implement a `for i in 0..N` loop more
     efficiently than a `while` loop.  For example, on GPUs, we can implement a
     `for i in 0..N` loop by enqueueing the kernels for the loop body N times,
     whereas implementing a `while` loop requires a host-device sync on each
     iteration.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class KnownTripCount(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         N_FIELD_NUMBER: builtins.int
         n: builtins.int
         def __init__(
             self,
             *,
             n: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["n", b"n"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["n", b"n"]) -> None: ...
 
     KNOWN_TRIP_COUNT_FIELD_NUMBER: builtins.int
     @property
     def known_trip_count(self) -> global___WhileLoopBackendConfig.KnownTripCount:
         """This indirection lets us distinguish between known-trip-count == 0 and
         unknown-trip-count.
         """
+
     def __init__(
         self,
         *,
         known_trip_count: global___WhileLoopBackendConfig.KnownTripCount | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["known_trip_count", b"known_trip_count"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["known_trip_count", b"known_trip_count"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["known_trip_count", b"known_trip_count"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["known_trip_count", b"known_trip_count"]) -> None: ...
 
 global___WhileLoopBackendConfig = WhileLoopBackendConfig
 
-@typing_extensions.final
+@typing.final
 class OutputOperandAliasing(google.protobuf.message.Message):
     """Specifies a pair of output/operand buffers that alias each other for
     kCustomCall and kFusion
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OUTPUT_SHAPE_INDEX_FIELD_NUMBER: builtins.int
     OPERAND_INDEX_FIELD_NUMBER: builtins.int
     OPERAND_SHAPE_INDEX_FIELD_NUMBER: builtins.int
+    operand_index: builtins.int
     @property
     def output_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    operand_index: builtins.int
     @property
     def operand_shape_index(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         output_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
         operand_index: builtins.int | None = ...,
         operand_shape_index: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["operand_index", b"operand_index", "operand_shape_index", b"operand_shape_index", "output_shape_index", b"output_shape_index"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["operand_index", b"operand_index", "operand_shape_index", b"operand_shape_index", "output_shape_index", b"output_shape_index"]) -> None: ...
 
 global___OutputOperandAliasing = OutputOperandAliasing
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/config/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/config/experimental.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/config/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol messages for describing the configuration of the ExampleParserOp."""
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class VarLenFeatureProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     VALUES_OUTPUT_TENSOR_NAME_FIELD_NUMBER: builtins.int
     INDICES_OUTPUT_TENSOR_NAME_FIELD_NUMBER: builtins.int
     SHAPES_OUTPUT_TENSOR_NAME_FIELD_NUMBER: builtins.int
@@ -31,46 +32,46 @@
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         values_output_tensor_name: builtins.str | None = ...,
         indices_output_tensor_name: builtins.str | None = ...,
         shapes_output_tensor_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "indices_output_tensor_name", b"indices_output_tensor_name", "shapes_output_tensor_name", b"shapes_output_tensor_name", "values_output_tensor_name", b"values_output_tensor_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "indices_output_tensor_name", b"indices_output_tensor_name", "shapes_output_tensor_name", b"shapes_output_tensor_name", "values_output_tensor_name", b"values_output_tensor_name"]) -> None: ...
 
 global___VarLenFeatureProto = VarLenFeatureProto
 
-@typing_extensions.final
+@typing.final
 class FixedLenFeatureProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DEFAULT_VALUE_FIELD_NUMBER: builtins.int
     VALUES_OUTPUT_TENSOR_NAME_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
+    values_output_tensor_name: builtins.str
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     @property
     def default_value(self) -> tensorflow.core.framework.tensor_pb2.TensorProto: ...
-    values_output_tensor_name: builtins.str
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         default_value: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
         values_output_tensor_name: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["default_value", b"default_value", "shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["default_value", b"default_value", "dtype", b"dtype", "shape", b"shape", "values_output_tensor_name", b"values_output_tensor_name"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["default_value", b"default_value", "shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["default_value", b"default_value", "dtype", b"dtype", "shape", b"shape", "values_output_tensor_name", b"values_output_tensor_name"]) -> None: ...
 
 global___FixedLenFeatureProto = FixedLenFeatureProto
 
-@typing_extensions.final
+@typing.final
 class FeatureConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FIXED_LEN_FEATURE_FIELD_NUMBER: builtins.int
     VAR_LEN_FEATURE_FIELD_NUMBER: builtins.int
     @property
     def fixed_len_feature(self) -> global___FixedLenFeatureProto: ...
@@ -78,46 +79,46 @@
     def var_len_feature(self) -> global___VarLenFeatureProto: ...
     def __init__(
         self,
         *,
         fixed_len_feature: global___FixedLenFeatureProto | None = ...,
         var_len_feature: global___VarLenFeatureProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "fixed_len_feature", b"fixed_len_feature", "var_len_feature", b"var_len_feature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "fixed_len_feature", b"fixed_len_feature", "var_len_feature", b"var_len_feature"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config", b"config"]) -> typing_extensions.Literal["fixed_len_feature", "var_len_feature"] | None: ...
+    def HasField(self, field_name: typing.Literal["config", b"config", "fixed_len_feature", b"fixed_len_feature", "var_len_feature", b"var_len_feature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["config", b"config", "fixed_len_feature", b"fixed_len_feature", "var_len_feature", b"var_len_feature"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["config", b"config"]) -> typing.Literal["fixed_len_feature", "var_len_feature"] | None: ...
 
 global___FeatureConfiguration = FeatureConfiguration
 
-@typing_extensions.final
+@typing.final
 class ExampleParserConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FeatureMapEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___FeatureConfiguration: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___FeatureConfiguration | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FEATURE_MAP_FIELD_NUMBER: builtins.int
     @property
     def feature_map(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FeatureConfiguration]: ...
     def __init__(
         self,
         *,
         feature_map: collections.abc.Mapping[builtins.str, global___FeatureConfiguration] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["feature_map", b"feature_map"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["feature_map", b"feature_map"]) -> None: ...
 
 global___ExampleParserConfiguration = ExampleParserConfiguration
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol messages for describing input data Examples for machine learning
 model training or inference.
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.example.feature_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Example(google.protobuf.message.Message):
     """An Example is a mostly-normalized data format for storing data for
     training and inference.  It contains a key-value store (features); where
     each key (string) maps to a Feature message (which is oneof packed BytesList,
     FloatList, or Int64List).  This flexible and compact format allows the
     storage of large amounts of typed data, but requires that the data shape
     and use be determined by the configuration files and parsers that are used to
@@ -95,20 +96,20 @@
     @property
     def features(self) -> tensorflow.core.example.feature_pb2.Features: ...
     def __init__(
         self,
         *,
         features: tensorflow.core.example.feature_pb2.Features | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["features", b"features"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["features", b"features"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["features", b"features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["features", b"features"]) -> None: ...
 
 global___Example = Example
 
-@typing_extensions.final
+@typing.final
 class SequenceExample(google.protobuf.message.Message):
     """A SequenceExample is an Example representing one or more sequences, and
     some context.  The context contains features which apply to the entire
     example. The feature_lists contain a key, value map where each key is
     associated with a repeated set of Features (a FeatureList).
     A FeatureList thus represents the values of a feature identified by its key
     over time / frames.
@@ -323,11 +324,11 @@
     def feature_lists(self) -> tensorflow.core.example.feature_pb2.FeatureLists: ...
     def __init__(
         self,
         *,
         context: tensorflow.core.example.feature_pb2.Features | None = ...,
         feature_lists: tensorflow.core.example.feature_pb2.FeatureLists | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["context", b"context", "feature_lists", b"feature_lists"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["context", b"context", "feature_lists", b"feature_lists"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["context", b"context", "feature_lists", b"feature_lists"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["context", b"context", "feature_lists", b"feature_lists"]) -> None: ...
 
 global___SequenceExample = SequenceExample
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -51,25 +51,26 @@
   feature {
     key: "purchase_price"
     value { float_list {
       value: 9.99
     }}
   }
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class BytesList(google.protobuf.message.Message):
     """LINT.IfChange
     Containers to hold repeated fundamental values.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -77,51 +78,51 @@
     @property
     def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]: ...
     def __init__(
         self,
         *,
         value: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
 global___BytesList = BytesList
 
-@typing_extensions.final
+@typing.final
 class FloatList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
     def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     def __init__(
         self,
         *,
         value: collections.abc.Iterable[builtins.float] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
 global___FloatList = FloatList
 
-@typing_extensions.final
+@typing.final
 class Int64List(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
     def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         value: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
 global___Int64List = Int64List
 
-@typing_extensions.final
+@typing.final
 class Feature(google.protobuf.message.Message):
     """Containers for non-sequential data."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BYTES_LIST_FIELD_NUMBER: builtins.int
     FLOAT_LIST_FIELD_NUMBER: builtins.int
@@ -135,56 +136,57 @@
     def __init__(
         self,
         *,
         bytes_list: global___BytesList | None = ...,
         float_list: global___FloatList | None = ...,
         int64_list: global___Int64List | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["bytes_list", "float_list", "int64_list"] | None: ...
+    def HasField(self, field_name: typing.Literal["bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["bytes_list", "float_list", "int64_list"] | None: ...
 
 global___Feature = Feature
 
-@typing_extensions.final
+@typing.final
 class Features(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FeatureEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___Feature: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___Feature | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FEATURE_FIELD_NUMBER: builtins.int
     @property
     def feature(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___Feature]:
         """Map from feature name to feature."""
+
     def __init__(
         self,
         *,
         feature: collections.abc.Mapping[builtins.str, global___Feature] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["feature", b"feature"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["feature", b"feature"]) -> None: ...
 
 global___Features = Features
 
-@typing_extensions.final
+@typing.final
 class FeatureList(google.protobuf.message.Message):
     """Containers for sequential data.
 
     A FeatureList contains lists of Features.  These may hold zero or more
     Feature values.
 
     FeatureLists are organized into categories by name.  The FeatureLists message
@@ -197,45 +199,46 @@
     @property
     def feature(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Feature]: ...
     def __init__(
         self,
         *,
         feature: collections.abc.Iterable[global___Feature] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["feature", b"feature"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["feature", b"feature"]) -> None: ...
 
 global___FeatureList = FeatureList
 
-@typing_extensions.final
+@typing.final
 class FeatureLists(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FeatureListEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___FeatureList: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___FeatureList | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FEATURE_LIST_FIELD_NUMBER: builtins.int
     @property
     def feature_list(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___FeatureList]:
         """Map from feature name to feature list."""
+
     def __init__(
         self,
         *,
         feature_list: collections.abc.Mapping[builtins.str, global___FeatureList] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["feature_list", b"feature_list"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["feature_list", b"feature_list"]) -> None: ...
 
 global___FeatureLists = FeatureLists
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class AllocationDescription(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     REQUESTED_BYTES_FIELD_NUMBER: builtins.int
     ALLOCATED_BYTES_FIELD_NUMBER: builtins.int
     ALLOCATOR_NAME_FIELD_NUMBER: builtins.int
     ALLOCATION_ID_FIELD_NUMBER: builtins.int
@@ -38,10 +39,10 @@
         requested_bytes: builtins.int | None = ...,
         allocated_bytes: builtins.int | None = ...,
         allocator_name: builtins.str | None = ...,
         allocation_id: builtins.int | None = ...,
         has_single_reference: builtins.bool | None = ...,
         ptr: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocated_bytes", b"allocated_bytes", "allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "has_single_reference", b"has_single_reference", "ptr", b"ptr", "requested_bytes", b"requested_bytes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allocated_bytes", b"allocated_bytes", "allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "has_single_reference", b"has_single_reference", "ptr", b"ptr", "requested_bytes", b"requested_bytes"]) -> None: ...
 
 global___AllocationDescription = AllocationDescription
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Defines the text format for including per-op API definition and
 overrides for client language op code generators.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -18,15 +19,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ApiDef(google.protobuf.message.Message):
     """Used to specify and override the default API & behavior in the
     generated code for client languages, from what you would get from
     the OpDef alone. There will be a set of ApiDefs that are common
     to all client languages, and another set per client language.
     The per-client-language ApiDefs will inherit values from the
     common ApiDefs which it can either replace or modify.
@@ -77,15 +78,15 @@
     set to 'SKIP', other fields are ignored for this op.
     """
     HIDDEN: ApiDef.Visibility.ValueType  # 3
     """Hide this op by putting it into an internal namespace (or whatever
     is appropriate in the target language).
     """
 
-    @typing_extensions.final
+    @typing.final
     class Endpoint(google.protobuf.message.Message):
         """If you specify any endpoint, this will replace all of the
         inherited endpoints.  The first endpoint should be the
         "canonical" endpoint, and should not be deprecated (unless all
         endpoints are deprecated).
         """
 
@@ -112,17 +113,17 @@
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             deprecated: builtins.bool | None = ...,
             deprecation_version: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "deprecation_version", b"deprecation_version", "name", b"name"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["deprecated", b"deprecated", "deprecation_version", b"deprecation_version", "name", b"name"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Arg(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         RENAME_TO_FIELD_NUMBER: builtins.int
         DESCRIPTION_FIELD_NUMBER: builtins.int
         name: builtins.str
@@ -139,17 +140,17 @@
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             rename_to: builtins.str | None = ...,
             description: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "name", b"name", "rename_to", b"rename_to"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["description", b"description", "name", b"name", "rename_to", b"rename_to"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Attr(google.protobuf.message.Message):
         """Description of the graph-construction-time configuration of this
         Op.  That is to say, this describes the attr fields that will
         be specified in the NodeDef.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -160,35 +161,36 @@
         DESCRIPTION_FIELD_NUMBER: builtins.int
         name: builtins.str
         rename_to: builtins.str
         """Change the name used to access this attr in the API from what
         is used in the GraphDef.  Note that these names in `backticks`
         will also be replaced in the summary & description fields.
         """
+        description: builtins.str
+        """Note: this will replace any inherited attr doc, there is no current
+        way of modifying attr descriptions as can be done with op descriptions.
+        """
         @property
         def default_value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue:
             """Specify a new default value to use for this attr.  This default
             will be used when creating new graphs, as opposed to the
             default in the OpDef, which will be used when interpreting old
             GraphDefs.
             """
-        description: builtins.str
-        """Note: this will replace any inherited attr doc, there is no current
-        way of modifying attr descriptions as can be done with op descriptions.
-        """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             rename_to: builtins.str | None = ...,
             default_value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
             description: builtins.str | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["default_value", b"default_value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["default_value", b"default_value", "description", b"description", "name", b"name", "rename_to", b"rename_to"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["default_value", b"default_value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["default_value", b"default_value", "description", b"description", "name", b"name", "rename_to", b"rename_to"]) -> None: ...
 
     GRAPH_OP_NAME_FIELD_NUMBER: builtins.int
     DEPRECATION_MESSAGE_FIELD_NUMBER: builtins.int
     DEPRECATION_VERSION_FIELD_NUMBER: builtins.int
     VISIBILITY_FIELD_NUMBER: builtins.int
     ENDPOINT_FIELD_NUMBER: builtins.int
     IN_ARG_FIELD_NUMBER: builtins.int
@@ -208,37 +210,38 @@
     """
     deprecation_version: builtins.int
     """Major version when the op will be deleted. For e.g. set this
     value to 2 if op API should be removed in TensorFlow 2.0 and
     deprecated in versions before that.
     """
     visibility: global___ApiDef.Visibility.ValueType
+    summary: builtins.str
+    """One-line human-readable description of what the Op does."""
+    description: builtins.str
+    """Additional, longer human-readable description of what the Op does."""
+    description_prefix: builtins.str
+    """Modify an existing/inherited description by adding text to the beginning
+    or end.
+    """
+    description_suffix: builtins.str
     @property
     def endpoint(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiDef.Endpoint]: ...
     @property
     def in_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiDef.Arg]: ...
     @property
     def out_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiDef.Arg]: ...
     @property
     def arg_order(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of original in_arg names to specify new argument order.
         Length of arg_order should be either empty to keep current order
         or match size of in_arg.
         """
+
     @property
     def attr(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiDef.Attr]: ...
-    summary: builtins.str
-    """One-line human-readable description of what the Op does."""
-    description: builtins.str
-    """Additional, longer human-readable description of what the Op does."""
-    description_prefix: builtins.str
-    """Modify an existing/inherited description by adding text to the beginning
-    or end.
-    """
-    description_suffix: builtins.str
     def __init__(
         self,
         *,
         graph_op_name: builtins.str | None = ...,
         deprecation_message: builtins.str | None = ...,
         deprecation_version: builtins.int | None = ...,
         visibility: global___ApiDef.Visibility.ValueType | None = ...,
@@ -248,26 +251,26 @@
         arg_order: collections.abc.Iterable[builtins.str] | None = ...,
         attr: collections.abc.Iterable[global___ApiDef.Attr] | None = ...,
         summary: builtins.str | None = ...,
         description: builtins.str | None = ...,
         description_prefix: builtins.str | None = ...,
         description_suffix: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arg_order", b"arg_order", "attr", b"attr", "deprecation_message", b"deprecation_message", "deprecation_version", b"deprecation_version", "description", b"description", "description_prefix", b"description_prefix", "description_suffix", b"description_suffix", "endpoint", b"endpoint", "graph_op_name", b"graph_op_name", "in_arg", b"in_arg", "out_arg", b"out_arg", "summary", b"summary", "visibility", b"visibility"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["arg_order", b"arg_order", "attr", b"attr", "deprecation_message", b"deprecation_message", "deprecation_version", b"deprecation_version", "description", b"description", "description_prefix", b"description_prefix", "description_suffix", b"description_suffix", "endpoint", b"endpoint", "graph_op_name", b"graph_op_name", "in_arg", b"in_arg", "out_arg", b"out_arg", "summary", b"summary", "visibility", b"visibility"]) -> None: ...
 
 global___ApiDef = ApiDef
 
-@typing_extensions.final
+@typing.final
 class ApiDefs(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OP_FIELD_NUMBER: builtins.int
     @property
     def op(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiDef]: ...
     def __init__(
         self,
         *,
         op: collections.abc.Iterable[global___ApiDef] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["op", b"op"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["op", b"op"]) -> None: ...
 
 global___ApiDefs = ApiDefs
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class AttrValue(google.protobuf.message.Message):
     """Protocol buffer representing the value for an attr used to configure an Op.
     Comment indicates the corresponding attr type.  Only the field matching the
     attr type may be filled.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ListValue(google.protobuf.message.Message):
         """LINT.IfChange"""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         S_FIELD_NUMBER: builtins.int
         I_FIELD_NUMBER: builtins.int
@@ -37,48 +38,56 @@
         TYPE_FIELD_NUMBER: builtins.int
         SHAPE_FIELD_NUMBER: builtins.int
         TENSOR_FIELD_NUMBER: builtins.int
         FUNC_FIELD_NUMBER: builtins.int
         @property
         def s(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]:
             """"list(string)" """
+
         @property
         def i(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
             """"list(int)" """
+
         @property
         def f(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
             """"list(float)" """
+
         @property
         def b(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]:
             """"list(bool)" """
+
         @property
         def type(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[tensorflow.core.framework.types_pb2.DataType.ValueType]:
             """"list(type)" """
+
         @property
         def shape(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto]:
             """"list(shape)" """
+
         @property
         def tensor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_pb2.TensorProto]:
             """"list(tensor)" """
+
         @property
         def func(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NameAttrList]:
             """"list(attr)" """
+
         def __init__(
             self,
             *,
             s: collections.abc.Iterable[builtins.bytes] | None = ...,
             i: collections.abc.Iterable[builtins.int] | None = ...,
             f: collections.abc.Iterable[builtins.float] | None = ...,
             b: collections.abc.Iterable[builtins.bool] | None = ...,
             type: collections.abc.Iterable[tensorflow.core.framework.types_pb2.DataType.ValueType] | None = ...,
             shape: collections.abc.Iterable[tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto] | None = ...,
             tensor: collections.abc.Iterable[tensorflow.core.framework.tensor_pb2.TensorProto] | None = ...,
             func: collections.abc.Iterable[global___NameAttrList] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type"]) -> None: ...
 
     S_FIELD_NUMBER: builtins.int
     I_FIELD_NUMBER: builtins.int
     F_FIELD_NUMBER: builtins.int
     B_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
@@ -92,92 +101,96 @@
     """"int" """
     f: builtins.float
     """"float" """
     b: builtins.bool
     """"bool" """
     type: tensorflow.core.framework.types_pb2.DataType.ValueType
     """"type" """
+    placeholder: builtins.str
+    """This is a placeholder only used in nodes defined inside a
+    function.  It indicates the attr value will be supplied when
+    the function is instantiated.  For example, let us suppose a
+    node "N" in function "FN". "N" has an attr "A" with value
+    placeholder = "foo". When FN is instantiated with attr "foo"
+    set to "bar", the instantiated node N's attr A will have been
+    given the value "bar".
+    """
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """"shape" """
+
     @property
     def tensor(self) -> tensorflow.core.framework.tensor_pb2.TensorProto:
         """"tensor" """
+
     @property
     def list(self) -> global___AttrValue.ListValue:
         """any "list(...)" """
+
     @property
     def func(self) -> global___NameAttrList:
         """"func" represents a function. func.name is a function's name or
         a primitive op's name. func.attr.first is the name of an attr
         defined for that function. func.attr.second is the value for
         that attr in the instantiation.
         """
-    placeholder: builtins.str
-    """This is a placeholder only used in nodes defined inside a
-    function.  It indicates the attr value will be supplied when
-    the function is instantiated.  For example, let us suppose a
-    node "N" in function "FN". "N" has an attr "A" with value
-    placeholder = "foo". When FN is instantiated with attr "foo"
-    set to "bar", the instantiated node N's attr A will have been
-    given the value "bar".
-    """
+
     def __init__(
         self,
         *,
         s: builtins.bytes | None = ...,
         i: builtins.int | None = ...,
         f: builtins.float | None = ...,
         b: builtins.bool | None = ...,
         type: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         tensor: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
         list: global___AttrValue.ListValue | None = ...,
         func: global___NameAttrList | None = ...,
         placeholder: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "list", b"list", "placeholder", b"placeholder", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type", "value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "list", b"list", "placeholder", b"placeholder", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type", "value", b"value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["value", b"value"]) -> typing_extensions.Literal["s", "i", "f", "b", "type", "shape", "tensor", "list", "func", "placeholder"] | None: ...
+    def HasField(self, field_name: typing.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "list", b"list", "placeholder", b"placeholder", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type", "value", b"value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["b", b"b", "f", b"f", "func", b"func", "i", b"i", "list", b"list", "placeholder", b"placeholder", "s", b"s", "shape", b"shape", "tensor", b"tensor", "type", b"type", "value", b"value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["value", b"value"]) -> typing.Literal["s", "i", "f", "b", "type", "shape", "tensor", "list", "func", "placeholder"] | None: ...
 
 global___AttrValue = AttrValue
 
-@typing_extensions.final
+@typing.final
 class NameAttrList(google.protobuf.message.Message):
     """A list of attr names and their values. The whole list is attached
     with a string name.  E.g., MatMul[T=float].
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AttrEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___AttrValue: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___AttrValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     ATTR_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def attr(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___AttrValue]: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         attr: collections.abc.Mapping[builtins.str, global___AttrValue] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["attr", b"attr", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["attr", b"attr", "name", b"name"]) -> None: ...
 
 global___NameAttrList = NameAttrList
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CostGraphDef(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Node(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class InputInfo(google.protobuf.message.Message):
             """Inputs of this node. They must be executed before this node can be
             executed. An input is a particular output of another node, specified
             by the node id and the output index.
             """
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -37,17 +38,17 @@
             preceding_port: builtins.int
             def __init__(
                 self,
                 *,
                 preceding_node: builtins.int | None = ...,
                 preceding_port: builtins.int | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["preceding_node", b"preceding_node", "preceding_port", b"preceding_port"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["preceding_node", b"preceding_node", "preceding_port", b"preceding_port"]) -> None: ...
 
-        @typing_extensions.final
+        @typing.final
         class OutputInfo(google.protobuf.message.Message):
             """Outputs of this node."""
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             SIZE_FIELD_NUMBER: builtins.int
             ALIAS_INPUT_PORT_FIELD_NUMBER: builtins.int
@@ -55,27 +56,27 @@
             DTYPE_FIELD_NUMBER: builtins.int
             size: builtins.int
             alias_input_port: builtins.int
             """If >= 0, the output is an alias of an input. Note that an alias input
             may itself be an alias. The algorithm will therefore need to follow
             those pointers.
             """
+            dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
             @property
             def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
-            dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
             def __init__(
                 self,
                 *,
                 size: builtins.int | None = ...,
                 alias_input_port: builtins.int | None = ...,
                 shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
                 dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
             ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal["alias_input_port", b"alias_input_port", "dtype", b"dtype", "shape", b"shape", "size", b"size"]) -> None: ...
+            def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing.Literal["alias_input_port", b"alias_input_port", "dtype", b"dtype", "shape", b"shape", "size", b"size"]) -> None: ...
 
         NAME_FIELD_NUMBER: builtins.int
         DEVICE_FIELD_NUMBER: builtins.int
         ID_FIELD_NUMBER: builtins.int
         INPUT_INFO_FIELD_NUMBER: builtins.int
         OUTPUT_INFO_FIELD_NUMBER: builtins.int
         TEMPORARY_MEMORY_SIZE_FIELD_NUMBER: builtins.int
@@ -93,18 +94,14 @@
         """The name of the node. Names are globally unique."""
         device: builtins.str
         """The device of the node. Can be empty if the node is mapped to the
         default partition or partitioning hasn't been run yet.
         """
         id: builtins.int
         """The id of the node. Node ids are only unique inside a partition."""
-        @property
-        def input_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.Node.InputInfo]: ...
-        @property
-        def output_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.Node.OutputInfo]: ...
         temporary_memory_size: builtins.int
         """Temporary memory used by this node."""
         persistent_memory_size: builtins.int
         """Persistent memory used by this node."""
         host_temp_memory_size: builtins.int
         device_temp_memory_size: builtins.int
         device_persistent_memory_size: builtins.int
@@ -118,19 +115,24 @@
         """Analytical estimate of the memory access cost of this node, in
         microseconds.
         """
         is_final: builtins.bool
         """If true, the output is permanent: it can't be discarded, because this
         node is part of the "final output". Nodes may depend on final nodes.
         """
+        inaccurate: builtins.bool
+        """Are the costs inaccurate?"""
+        @property
+        def input_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.Node.InputInfo]: ...
+        @property
+        def output_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.Node.OutputInfo]: ...
         @property
         def control_input(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
             """Ids of the control inputs for this node."""
-        inaccurate: builtins.bool
-        """Are the costs inaccurate?"""
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             device: builtins.str | None = ...,
             id: builtins.int | None = ...,
             input_info: collections.abc.Iterable[global___CostGraphDef.Node.InputInfo] | None = ...,
@@ -143,17 +145,17 @@
             compute_cost: builtins.int | None = ...,
             compute_time: builtins.int | None = ...,
             memory_time: builtins.int | None = ...,
             is_final: builtins.bool | None = ...,
             control_input: collections.abc.Iterable[builtins.int] | None = ...,
             inaccurate: builtins.bool | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["compute_cost", b"compute_cost", "compute_time", b"compute_time", "control_input", b"control_input", "device", b"device", "device_persistent_memory_size", b"device_persistent_memory_size", "device_temp_memory_size", b"device_temp_memory_size", "host_temp_memory_size", b"host_temp_memory_size", "id", b"id", "inaccurate", b"inaccurate", "input_info", b"input_info", "is_final", b"is_final", "memory_time", b"memory_time", "name", b"name", "output_info", b"output_info", "persistent_memory_size", b"persistent_memory_size", "temporary_memory_size", b"temporary_memory_size"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["compute_cost", b"compute_cost", "compute_time", b"compute_time", "control_input", b"control_input", "device", b"device", "device_persistent_memory_size", b"device_persistent_memory_size", "device_temp_memory_size", b"device_temp_memory_size", "host_temp_memory_size", b"host_temp_memory_size", "id", b"id", "inaccurate", b"inaccurate", "input_info", b"input_info", "is_final", b"is_final", "memory_time", b"memory_time", "name", b"name", "output_info", b"output_info", "persistent_memory_size", b"persistent_memory_size", "temporary_memory_size", b"temporary_memory_size"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class AggregatedCost(google.protobuf.message.Message):
         """Total cost of this graph, typically used for balancing decisions."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         COST_FIELD_NUMBER: builtins.int
         DIMENSION_FIELD_NUMBER: builtins.int
@@ -163,24 +165,24 @@
         """Aggregated cost dimension (e.g. 'memory', 'compute', 'network')."""
         def __init__(
             self,
             *,
             cost: builtins.float | None = ...,
             dimension: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["cost", b"cost", "dimension", b"dimension"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["cost", b"cost", "dimension", b"dimension"]) -> None: ...
 
     NODE_FIELD_NUMBER: builtins.int
     COST_FIELD_NUMBER: builtins.int
     @property
     def node(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.Node]: ...
     @property
     def cost(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CostGraphDef.AggregatedCost]: ...
     def __init__(
         self,
         *,
         node: collections.abc.Iterable[global___CostGraphDef.Node] | None = ...,
         cost: collections.abc.Iterable[global___CostGraphDef.AggregatedCost] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cost", b"cost", "node", b"node"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cost", b"cost", "node", b"node"]) -> None: ...
 
 global___CostGraphDef = CostGraphDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -84,15 +85,15 @@
     """Represents how to handle external state during serialization."""
 
 POLICY_WARN: ExternalStatePolicy.ValueType  # 0
 POLICY_IGNORE: ExternalStatePolicy.ValueType  # 1
 POLICY_FAIL: ExternalStatePolicy.ValueType  # 2
 global___ExternalStatePolicy = ExternalStatePolicy
 
-@typing_extensions.final
+@typing.final
 class AutotuneOptions(google.protobuf.message.Message):
     """next: 5"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENABLED_FIELD_NUMBER: builtins.int
     CPU_BUDGET_FIELD_NUMBER: builtins.int
@@ -106,28 +107,28 @@
         self,
         *,
         enabled: builtins.bool | None = ...,
         cpu_budget: builtins.int | None = ...,
         ram_budget: builtins.int | None = ...,
         autotune_algorithm: tensorflow.core.framework.model_pb2.AutotuneAlgorithm.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["autotune_algorithm", b"autotune_algorithm", "cpu_budget", b"cpu_budget", "enabled", b"enabled", "optional_autotune_algorithm", b"optional_autotune_algorithm", "optional_cpu_budget", b"optional_cpu_budget", "optional_enabled", b"optional_enabled", "optional_ram_budget", b"optional_ram_budget", "ram_budget", b"ram_budget"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["autotune_algorithm", b"autotune_algorithm", "cpu_budget", b"cpu_budget", "enabled", b"enabled", "optional_autotune_algorithm", b"optional_autotune_algorithm", "optional_cpu_budget", b"optional_cpu_budget", "optional_enabled", b"optional_enabled", "optional_ram_budget", b"optional_ram_budget", "ram_budget", b"ram_budget"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["autotune_algorithm", b"autotune_algorithm", "cpu_budget", b"cpu_budget", "enabled", b"enabled", "optional_autotune_algorithm", b"optional_autotune_algorithm", "optional_cpu_budget", b"optional_cpu_budget", "optional_enabled", b"optional_enabled", "optional_ram_budget", b"optional_ram_budget", "ram_budget", b"ram_budget"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["autotune_algorithm", b"autotune_algorithm", "cpu_budget", b"cpu_budget", "enabled", b"enabled", "optional_autotune_algorithm", b"optional_autotune_algorithm", "optional_cpu_budget", b"optional_cpu_budget", "optional_enabled", b"optional_enabled", "optional_ram_budget", b"optional_ram_budget", "ram_budget", b"ram_budget"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_autotune_algorithm", b"optional_autotune_algorithm"]) -> typing_extensions.Literal["autotune_algorithm"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_autotune_algorithm", b"optional_autotune_algorithm"]) -> typing.Literal["autotune_algorithm"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_cpu_budget", b"optional_cpu_budget"]) -> typing_extensions.Literal["cpu_budget"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_cpu_budget", b"optional_cpu_budget"]) -> typing.Literal["cpu_budget"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_enabled", b"optional_enabled"]) -> typing_extensions.Literal["enabled"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_enabled", b"optional_enabled"]) -> typing.Literal["enabled"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_ram_budget", b"optional_ram_budget"]) -> typing_extensions.Literal["ram_budget"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_ram_budget", b"optional_ram_budget"]) -> typing.Literal["ram_budget"] | None: ...
 
 global___AutotuneOptions = AutotuneOptions
 
-@typing_extensions.final
+@typing.final
 class CardinalityOptions(google.protobuf.message.Message):
     """next: 2"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ComputeLevel:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -165,19 +166,19 @@
     COMPUTE_LEVEL_FIELD_NUMBER: builtins.int
     compute_level: global___CardinalityOptions.ComputeLevel.ValueType
     def __init__(
         self,
         *,
         compute_level: global___CardinalityOptions.ComputeLevel.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compute_level", b"compute_level"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["compute_level", b"compute_level"]) -> None: ...
 
 global___CardinalityOptions = CardinalityOptions
 
-@typing_extensions.final
+@typing.final
 class DistributeOptions(google.protobuf.message.Message):
     """next: 3"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     AUTO_SHARD_POLICY_FIELD_NUMBER: builtins.int
     NUM_DEVICES_FIELD_NUMBER: builtins.int
@@ -185,21 +186,21 @@
     num_devices: builtins.int
     def __init__(
         self,
         *,
         auto_shard_policy: global___AutoShardPolicy.ValueType | None = ...,
         num_devices: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["num_devices", b"num_devices", "optional_num_devices", b"optional_num_devices"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["auto_shard_policy", b"auto_shard_policy", "num_devices", b"num_devices", "optional_num_devices", b"optional_num_devices"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_num_devices", b"optional_num_devices"]) -> typing_extensions.Literal["num_devices"] | None: ...
+    def HasField(self, field_name: typing.Literal["num_devices", b"num_devices", "optional_num_devices", b"optional_num_devices"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["auto_shard_policy", b"auto_shard_policy", "num_devices", b"num_devices", "optional_num_devices", b"optional_num_devices"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_num_devices", b"optional_num_devices"]) -> typing.Literal["num_devices"] | None: ...
 
 global___DistributeOptions = DistributeOptions
 
-@typing_extensions.final
+@typing.final
 class OptimizationOptions(google.protobuf.message.Message):
     """next: 20"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLY_DEFAULT_OPTIMIZATIONS_FIELD_NUMBER: builtins.int
     FILTER_FUSION_FIELD_NUMBER: builtins.int
@@ -234,42 +235,42 @@
         map_parallelization: builtins.bool | None = ...,
         noop_elimination: builtins.bool | None = ...,
         parallel_batch: builtins.bool | None = ...,
         shuffle_and_repeat_fusion: builtins.bool | None = ...,
         filter_parallelization: builtins.bool | None = ...,
         inject_prefetch: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["apply_default_optimizations", b"apply_default_optimizations", "filter_fusion", b"filter_fusion", "filter_parallelization", b"filter_parallelization", "inject_prefetch", b"inject_prefetch", "map_and_batch_fusion", b"map_and_batch_fusion", "map_and_filter_fusion", b"map_and_filter_fusion", "map_fusion", b"map_fusion", "map_parallelization", b"map_parallelization", "noop_elimination", b"noop_elimination", "optional_apply_default_optimizations", b"optional_apply_default_optimizations", "optional_filter_fusion", b"optional_filter_fusion", "optional_filter_parallelization", b"optional_filter_parallelization", "optional_inject_prefetch", b"optional_inject_prefetch", "optional_map_and_batch_fusion", b"optional_map_and_batch_fusion", "optional_map_and_filter_fusion", b"optional_map_and_filter_fusion", "optional_map_fusion", b"optional_map_fusion", "optional_map_parallelization", b"optional_map_parallelization", "optional_noop_elimination", b"optional_noop_elimination", "optional_parallel_batch", b"optional_parallel_batch", "optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion", "parallel_batch", b"parallel_batch", "shuffle_and_repeat_fusion", b"shuffle_and_repeat_fusion"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_apply_default_optimizations", b"optional_apply_default_optimizations"]) -> typing_extensions.Literal["apply_default_optimizations"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_apply_default_optimizations", b"optional_apply_default_optimizations"]) -> typing.Literal["apply_default_optimizations"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_filter_fusion", b"optional_filter_fusion"]) -> typing_extensions.Literal["filter_fusion"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_filter_fusion", b"optional_filter_fusion"]) -> typing.Literal["filter_fusion"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_filter_parallelization", b"optional_filter_parallelization"]) -> typing_extensions.Literal["filter_parallelization"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_filter_parallelization", b"optional_filter_parallelization"]) -> typing.Literal["filter_parallelization"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_inject_prefetch", b"optional_inject_prefetch"]) -> typing_extensions.Literal["inject_prefetch"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_inject_prefetch", b"optional_inject_prefetch"]) -> typing.Literal["inject_prefetch"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_map_and_batch_fusion", b"optional_map_and_batch_fusion"]) -> typing_extensions.Literal["map_and_batch_fusion"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_map_and_batch_fusion", b"optional_map_and_batch_fusion"]) -> typing.Literal["map_and_batch_fusion"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_map_and_filter_fusion", b"optional_map_and_filter_fusion"]) -> typing_extensions.Literal["map_and_filter_fusion"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_map_and_filter_fusion", b"optional_map_and_filter_fusion"]) -> typing.Literal["map_and_filter_fusion"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_map_fusion", b"optional_map_fusion"]) -> typing_extensions.Literal["map_fusion"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_map_fusion", b"optional_map_fusion"]) -> typing.Literal["map_fusion"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_map_parallelization", b"optional_map_parallelization"]) -> typing_extensions.Literal["map_parallelization"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_map_parallelization", b"optional_map_parallelization"]) -> typing.Literal["map_parallelization"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_noop_elimination", b"optional_noop_elimination"]) -> typing_extensions.Literal["noop_elimination"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_noop_elimination", b"optional_noop_elimination"]) -> typing.Literal["noop_elimination"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_parallel_batch", b"optional_parallel_batch"]) -> typing_extensions.Literal["parallel_batch"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_parallel_batch", b"optional_parallel_batch"]) -> typing.Literal["parallel_batch"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion"]) -> typing_extensions.Literal["shuffle_and_repeat_fusion"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_shuffle_and_repeat_fusion", b"optional_shuffle_and_repeat_fusion"]) -> typing.Literal["shuffle_and_repeat_fusion"] | None: ...
 
 global___OptimizationOptions = OptimizationOptions
 
-@typing_extensions.final
+@typing.final
 class ThreadingOptions(google.protobuf.message.Message):
     """next: 3"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAX_INTRA_OP_PARALLELISM_FIELD_NUMBER: builtins.int
     PRIVATE_THREADPOOL_SIZE_FIELD_NUMBER: builtins.int
@@ -277,24 +278,24 @@
     private_threadpool_size: builtins.int
     def __init__(
         self,
         *,
         max_intra_op_parallelism: builtins.int | None = ...,
         private_threadpool_size: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["max_intra_op_parallelism", b"max_intra_op_parallelism", "optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism", "optional_private_threadpool_size", b"optional_private_threadpool_size", "private_threadpool_size", b"private_threadpool_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_intra_op_parallelism", b"max_intra_op_parallelism", "optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism", "optional_private_threadpool_size", b"optional_private_threadpool_size", "private_threadpool_size", b"private_threadpool_size"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["max_intra_op_parallelism", b"max_intra_op_parallelism", "optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism", "optional_private_threadpool_size", b"optional_private_threadpool_size", "private_threadpool_size", b"private_threadpool_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["max_intra_op_parallelism", b"max_intra_op_parallelism", "optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism", "optional_private_threadpool_size", b"optional_private_threadpool_size", "private_threadpool_size", b"private_threadpool_size"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism"]) -> typing_extensions.Literal["max_intra_op_parallelism"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_max_intra_op_parallelism", b"optional_max_intra_op_parallelism"]) -> typing.Literal["max_intra_op_parallelism"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_private_threadpool_size", b"optional_private_threadpool_size"]) -> typing_extensions.Literal["private_threadpool_size"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_private_threadpool_size", b"optional_private_threadpool_size"]) -> typing.Literal["private_threadpool_size"] | None: ...
 
 global___ThreadingOptions = ThreadingOptions
 
-@typing_extensions.final
+@typing.final
 class Options(google.protobuf.message.Message):
     """Message stored with Dataset objects to control how datasets are processed and
     optimized.
 
     next: 9
     """
 
@@ -305,46 +306,50 @@
     DISTRIBUTE_OPTIONS_FIELD_NUMBER: builtins.int
     OPTIMIZATION_OPTIONS_FIELD_NUMBER: builtins.int
     SLACK_FIELD_NUMBER: builtins.int
     THREADING_OPTIONS_FIELD_NUMBER: builtins.int
     EXTERNAL_STATE_POLICY_FIELD_NUMBER: builtins.int
     SYMBOLIC_CHECKPOINT_FIELD_NUMBER: builtins.int
     deterministic: builtins.bool
+    slack: builtins.bool
+    external_state_policy: global___ExternalStatePolicy.ValueType
+    symbolic_checkpoint: builtins.bool
     @property
     def autotune_options(self) -> global___AutotuneOptions:
         """The distribution strategy options associated with the dataset."""
+
     @property
     def distribute_options(self) -> global___DistributeOptions:
         """The distribution strategy options associated with the dataset."""
+
     @property
     def optimization_options(self) -> global___OptimizationOptions:
         """The optimization options associated with the dataset."""
-    slack: builtins.bool
+
     @property
     def threading_options(self) -> global___ThreadingOptions:
         """The threading options associated with the dataset."""
-    external_state_policy: global___ExternalStatePolicy.ValueType
-    symbolic_checkpoint: builtins.bool
+
     def __init__(
         self,
         *,
         deterministic: builtins.bool | None = ...,
         autotune_options: global___AutotuneOptions | None = ...,
         distribute_options: global___DistributeOptions | None = ...,
         optimization_options: global___OptimizationOptions | None = ...,
         slack: builtins.bool | None = ...,
         threading_options: global___ThreadingOptions | None = ...,
         external_state_policy: global___ExternalStatePolicy.ValueType | None = ...,
         symbolic_checkpoint: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["autotune_options", b"autotune_options", "deterministic", b"deterministic", "distribute_options", b"distribute_options", "external_state_policy", b"external_state_policy", "optimization_options", b"optimization_options", "optional_deterministic", b"optional_deterministic", "optional_external_state_policy", b"optional_external_state_policy", "optional_slack", b"optional_slack", "optional_symbolic_checkpoint", b"optional_symbolic_checkpoint", "slack", b"slack", "symbolic_checkpoint", b"symbolic_checkpoint", "threading_options", b"threading_options"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_deterministic", b"optional_deterministic"]) -> typing_extensions.Literal["deterministic"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_deterministic", b"optional_deterministic"]) -> typing.Literal["deterministic"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_external_state_policy", b"optional_external_state_policy"]) -> typing_extensions.Literal["external_state_policy"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_external_state_policy", b"optional_external_state_policy"]) -> typing.Literal["external_state_policy"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_slack", b"optional_slack"]) -> typing_extensions.Literal["slack"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_slack", b"optional_slack"]) -> typing.Literal["slack"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_symbolic_checkpoint", b"optional_symbolic_checkpoint"]) -> typing_extensions.Literal["symbolic_checkpoint"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_symbolic_checkpoint", b"optional_symbolic_checkpoint"]) -> typing.Literal["symbolic_checkpoint"] | None: ...
 
 global___Options = Options
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/dataset_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/dataset_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CompressedComponentMetadata(google.protobuf.message.Message):
     """This file contains protocol buffers for working with tf.data Datasets.
 
     Metadata describing a compressed component of a dataset element.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -28,74 +29,77 @@
     TENSOR_SHAPE_FIELD_NUMBER: builtins.int
     UNCOMPRESSED_BYTES_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     """The dtype of the component tensor."""
     @property
     def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """The shape of the component tensor."""
+
     @property
     def uncompressed_bytes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The amount of uncompressed tensor data.
         - For string tensors, there is an element for each string indicating the
         size of the string.
         - For all other tensors, there is a single element indicating the size of
         the tensor.
         """
+
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         tensor_shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         uncompressed_bytes: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "tensor_shape", b"tensor_shape", "uncompressed_bytes", b"uncompressed_bytes"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "tensor_shape", b"tensor_shape", "uncompressed_bytes", b"uncompressed_bytes"]) -> None: ...
 
 global___CompressedComponentMetadata = CompressedComponentMetadata
 
-@typing_extensions.final
+@typing.final
 class CompressedElement(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_FIELD_NUMBER: builtins.int
     COMPONENT_METADATA_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     data: builtins.bytes
     """Compressed tensor bytes for all components of the element."""
-    @property
-    def component_metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CompressedComponentMetadata]:
-        """Metadata for the components of the element."""
     version: builtins.int
     """Version of the CompressedElement. CompressedElements may be stored on disk
     and read back by later versions of code, so we store a version number to
     help readers understand which version they are reading. When you add a new
     field to this proto, you need to increment kCompressedElementVersion in
     tensorflow/core/data/compression_utils.cc.
     """
+    @property
+    def component_metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CompressedComponentMetadata]:
+        """Metadata for the components of the element."""
+
     def __init__(
         self,
         *,
         data: builtins.bytes | None = ...,
         component_metadata: collections.abc.Iterable[global___CompressedComponentMetadata] | None = ...,
         version: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["component_metadata", b"component_metadata", "data", b"data", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["component_metadata", b"component_metadata", "data", b"data", "version", b"version"]) -> None: ...
 
 global___CompressedElement = CompressedElement
 
-@typing_extensions.final
+@typing.final
 class UncompressedElement(google.protobuf.message.Message):
     """An uncompressed dataset element."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     COMPONENTS_FIELD_NUMBER: builtins.int
     @property
     def components(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_pb2.TensorProto]: ...
     def __init__(
         self,
         *,
         components: collections.abc.Iterable[tensorflow.core.framework.tensor_pb2.TensorProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["components", b"components"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["components", b"components"]) -> None: ...
 
 global___UncompressedElement = UncompressedElement
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class InterconnectLink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEVICE_ID_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     STRENGTH_FIELD_NUMBER: builtins.int
     device_id: builtins.int
@@ -25,35 +26,35 @@
     def __init__(
         self,
         *,
         device_id: builtins.int | None = ...,
         type: builtins.str | None = ...,
         strength: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_id", b"device_id", "strength", b"strength", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device_id", b"device_id", "strength", b"strength", "type", b"type"]) -> None: ...
 
 global___InterconnectLink = InterconnectLink
 
-@typing_extensions.final
+@typing.final
 class LocalLinks(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LINK_FIELD_NUMBER: builtins.int
     @property
     def link(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___InterconnectLink]: ...
     def __init__(
         self,
         *,
         link: collections.abc.Iterable[global___InterconnectLink] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["link", b"link"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["link", b"link"]) -> None: ...
 
 global___LocalLinks = LocalLinks
 
-@typing_extensions.final
+@typing.final
 class DeviceLocality(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BUS_ID_FIELD_NUMBER: builtins.int
     NUMA_NODE_FIELD_NUMBER: builtins.int
     LINKS_FIELD_NUMBER: builtins.int
     bus_id: builtins.int
@@ -61,27 +62,28 @@
     no specific locality.  Specific localities are indexed from 1.
     """
     numa_node: builtins.int
     """Optional NUMA locality of device."""
     @property
     def links(self) -> global___LocalLinks:
         """Optional local interconnect links to other devices."""
+
     def __init__(
         self,
         *,
         bus_id: builtins.int | None = ...,
         numa_node: builtins.int | None = ...,
         links: global___LocalLinks | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["links", b"links"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bus_id", b"bus_id", "links", b"links", "numa_node", b"numa_node"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["links", b"links"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bus_id", b"bus_id", "links", b"links", "numa_node", b"numa_node"]) -> None: ...
 
 global___DeviceLocality = DeviceLocality
 
-@typing_extensions.final
+@typing.final
 class DeviceAttributes(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     DEVICE_TYPE_FIELD_NUMBER: builtins.int
     MEMORY_LIMIT_FIELD_NUMBER: builtins.int
     LOCALITY_FIELD_NUMBER: builtins.int
@@ -90,38 +92,39 @@
     XLA_GLOBAL_ID_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Fully specified name of the device within a cluster."""
     device_type: builtins.str
     """String representation of device_type."""
     memory_limit: builtins.int
     """Memory capacity of device in bytes."""
-    @property
-    def locality(self) -> global___DeviceLocality:
-        """Platform-specific data about device that may be useful
-        for supporting efficient data transfers.
-        """
     incarnation: builtins.int
     """A device is assigned a global unique number each time it is
     initialized. "incarnation" should never be 0.
     """
     physical_device_desc: builtins.str
     """String representation of the physical device that this device maps to."""
     xla_global_id: builtins.int
     """A physical device ID for use in XLA DeviceAssignments, unique across
     clients in a multi-client setup. Set to -1 if unavailable, non-negative
     otherwise.
     """
+    @property
+    def locality(self) -> global___DeviceLocality:
+        """Platform-specific data about device that may be useful
+        for supporting efficient data transfers.
+        """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         device_type: builtins.str | None = ...,
         memory_limit: builtins.int | None = ...,
         locality: global___DeviceLocality | None = ...,
         incarnation: builtins.int | None = ...,
         physical_device_desc: builtins.str | None = ...,
         xla_global_id: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["locality", b"locality"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_type", b"device_type", "incarnation", b"incarnation", "locality", b"locality", "memory_limit", b"memory_limit", "name", b"name", "physical_device_desc", b"physical_device_desc", "xla_global_id", b"xla_global_id"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["locality", b"locality"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["device_type", b"device_type", "incarnation", b"incarnation", "locality", b"locality", "memory_limit", b"memory_limit", "name", b"name", "physical_device_desc", b"physical_device_desc", "xla_global_id", b"xla_global_id"]) -> None: ...
 
 global___DeviceAttributes = DeviceAttributes
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -569,15 +570,15 @@
 """The equivalent of a Tensor with DT_VARIANT dtype, kept here to simplify
 translation. This type should not normally appear after type inference.
 Note that LEGACY_VARIANT != ANY: TENSOR[INT32] is a subtype of ANY, but is
 not a subtype of LEGACY_VARIANT.
 """
 global___FullTypeId = FullTypeId
 
-@typing_extensions.final
+@typing.final
 class FullTypeDef(google.protobuf.message.Message):
     """Highly experimental and very likely to change.
     This encoding uses tags instead of dedicated messages for regularity. In
     particular the encoding imposes no restrictions on what the parameters of any
     type should be, which in particular needs to be true for type symbols.
     """
 
@@ -588,25 +589,25 @@
     S_FIELD_NUMBER: builtins.int
     I_FIELD_NUMBER: builtins.int
     type_id: global___FullTypeId.ValueType
     """The principal type represented by this object. This may be a concrete type
     (Tensor, Dataset) a type variable (used for dependent types) a type
     symbol (Any, Union). See FullTypeId for details.
     """
-    @property
-    def args(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FullTypeDef]: ...
     s: builtins.str
     i: builtins.int
     """TODO(mdan): list/tensor, map? Need to reconcile with TFT_RECORD, etc."""
+    @property
+    def args(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FullTypeDef]: ...
     def __init__(
         self,
         *,
         type_id: global___FullTypeId.ValueType | None = ...,
         args: collections.abc.Iterable[global___FullTypeDef] | None = ...,
         s: builtins.str | None = ...,
         i: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["attr", b"attr", "i", b"i", "s", b"s"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["args", b"args", "attr", b"attr", "i", b"i", "s", b"s", "type_id", b"type_id"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["attr", b"attr"]) -> typing_extensions.Literal["s", "i"] | None: ...
+    def HasField(self, field_name: typing.Literal["attr", b"attr", "i", b"i", "s", b"s"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["args", b"args", "attr", b"attr", "i", b"i", "s", b"s", "type_id", b"type_id"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["attr", b"attr"]) -> typing.Literal["s", "i"] | None: ...
 
 global___FullTypeDef = FullTypeDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.attr_value_pb2
 import tensorflow.core.framework.node_def_pb2
 import tensorflow.core.framework.op_def_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class FunctionDefLibrary(google.protobuf.message.Message):
     """A library is a set of named functions."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FUNCTION_FIELD_NUMBER: builtins.int
     GRADIENT_FIELD_NUMBER: builtins.int
@@ -33,216 +34,222 @@
     def __init__(
         self,
         *,
         function: collections.abc.Iterable[global___FunctionDef] | None = ...,
         gradient: collections.abc.Iterable[global___GradientDef] | None = ...,
         registered_gradients: collections.abc.Iterable[global___RegisteredGradient] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["function", b"function", "gradient", b"gradient", "registered_gradients", b"registered_gradients"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["function", b"function", "gradient", b"gradient", "registered_gradients", b"registered_gradients"]) -> None: ...
 
 global___FunctionDefLibrary = FunctionDefLibrary
 
-@typing_extensions.final
+@typing.final
 class FunctionDef(google.protobuf.message.Message):
     """A function can be instantiated when the runtime can bind every attr
     with a value. When a GraphDef has a call to a function, it must
     have binding for every attr defined in the signature.
 
     TODO(zhifengc):
       * device spec, etc.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AttrEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ArgAttrs(google.protobuf.message.Message):
         """Attributes for function arguments. These attributes are the same set of
         valid attributes as to _Arg nodes.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class AttrEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: builtins.str
             @property
             def value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue: ...
             def __init__(
                 self,
                 *,
                 key: builtins.str | None = ...,
                 value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
             ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+            def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         ATTR_FIELD_NUMBER: builtins.int
         @property
         def attr(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue]: ...
         def __init__(
             self,
             *,
             attr: collections.abc.Mapping[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["attr", b"attr"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["attr", b"attr"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ArgAttrEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
         def value(self) -> global___FunctionDef.ArgAttrs: ...
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: global___FunctionDef.ArgAttrs | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ResourceArgUniqueIdEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         value: builtins.int
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class RetEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ControlRetEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     SIGNATURE_FIELD_NUMBER: builtins.int
     ATTR_FIELD_NUMBER: builtins.int
     ARG_ATTR_FIELD_NUMBER: builtins.int
     RESOURCE_ARG_UNIQUE_ID_FIELD_NUMBER: builtins.int
     NODE_DEF_FIELD_NUMBER: builtins.int
     RET_FIELD_NUMBER: builtins.int
     CONTROL_RET_FIELD_NUMBER: builtins.int
     @property
     def signature(self) -> tensorflow.core.framework.op_def_pb2.OpDef:
         """The definition of the function's name, arguments, return values,
         attrs etc.
         """
+
     @property
     def attr(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue]:
         """Attributes specific to this function definition."""
+
     @property
     def arg_attr(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___FunctionDef.ArgAttrs]: ...
     @property
     def resource_arg_unique_id(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.int]:
         """Unique IDs for each resource argument, used to track aliasing resources. If
         Argument A and Argument B alias each other, then
         resource_arg_unique_ids[A.index] == resource_arg_unique_ids[B.index].
 
         If this field is empty, none of the arguments could alias; otherwise, every
         resource argument should have an entry in this field.
 
         When instantiated, the unique IDs will be attached to the _Arg nodes'
         "_resource_arg_unique_id" attribute.
         """
+
     @property
     def node_def(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.node_def_pb2.NodeDef]:
         """The body of the function.  Unlike the NodeDefs in a GraphDef, attrs
         may have values of type `placeholder` and the `input` field uses
         the "output" format above.
 
         By convention, "op" in node_def is resolved by consulting with a
         user-defined library first. If not resolved, "func" is assumed to
         be a builtin op.
         """
+
     @property
     def ret(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """A mapping from the output arg names from `signature` to the
         outputs from `node_def` that should be returned by the function.
         """
+
     @property
     def control_ret(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """A mapping from control output names from `signature` to node names in
         `node_def` which should be control outputs of this function.
         """
+
     def __init__(
         self,
         *,
         signature: tensorflow.core.framework.op_def_pb2.OpDef | None = ...,
         attr: collections.abc.Mapping[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue] | None = ...,
         arg_attr: collections.abc.Mapping[builtins.int, global___FunctionDef.ArgAttrs] | None = ...,
         resource_arg_unique_id: collections.abc.Mapping[builtins.int, builtins.int] | None = ...,
         node_def: collections.abc.Iterable[tensorflow.core.framework.node_def_pb2.NodeDef] | None = ...,
         ret: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         control_ret: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["signature", b"signature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arg_attr", b"arg_attr", "attr", b"attr", "control_ret", b"control_ret", "node_def", b"node_def", "resource_arg_unique_id", b"resource_arg_unique_id", "ret", b"ret", "signature", b"signature"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["signature", b"signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["arg_attr", b"arg_attr", "attr", b"attr", "control_ret", b"control_ret", "node_def", b"node_def", "resource_arg_unique_id", b"resource_arg_unique_id", "ret", b"ret", "signature", b"signature"]) -> None: ...
 
 global___FunctionDef = FunctionDef
 
-@typing_extensions.final
+@typing.final
 class GradientDef(google.protobuf.message.Message):
     """GradientDef defines the gradient function of a function defined in
     a function library.
 
     A gradient function g (specified by gradient_func) for a function f
     (specified by function_name) must follow the following:
 
@@ -270,19 +277,19 @@
     """The gradient function's name."""
     def __init__(
         self,
         *,
         function_name: builtins.str | None = ...,
         gradient_func: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["function_name", b"function_name", "gradient_func", b"gradient_func"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["function_name", b"function_name", "gradient_func", b"gradient_func"]) -> None: ...
 
 global___GradientDef = GradientDef
 
-@typing_extensions.final
+@typing.final
 class RegisteredGradient(google.protobuf.message.Message):
     """RegisteredGradient stores a gradient function that is registered in the
     gradients library and used in the ops of a function in the function library.
     Unlike GradientDef, these gradients are identified by op type, and not
     directly linked to any function.
     """
 
@@ -296,10 +303,10 @@
     """The gradient function's registered op type."""
     def __init__(
         self,
         *,
         gradient_func: builtins.str | None = ...,
         registered_op_type: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["gradient_func", b"gradient_func", "registered_op_type", b"registered_op_type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["gradient_func", b"gradient_func", "registered_op_type", b"registered_op_type"]) -> None: ...
 
 global___RegisteredGradient = RegisteredGradient
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.function_pb2
 import tensorflow.core.framework.node_def_pb2
 import tensorflow.core.framework.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GraphDef(google.protobuf.message.Message):
     """Represents the graph of operations"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_FIELD_NUMBER: builtins.int
     VERSIONS_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     LIBRARY_FIELD_NUMBER: builtins.int
+    version: builtins.int
+    """Deprecated single version field; use versions above instead.  Since all
+    GraphDef changes before "versions" was introduced were forward
+    compatible, this field is entirely ignored.
+    """
     @property
     def node(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.node_def_pb2.NodeDef]: ...
     @property
     def versions(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
         """Compatibility versions of the graph.  See core/public/version.h for version
         history.  The GraphDef version is distinct from the TensorFlow version, and
         each release of TensorFlow will support a range of GraphDef versions.
         """
-    version: builtins.int
-    """Deprecated single version field; use versions above instead.  Since all
-    GraphDef changes before "versions" was introduced were forward
-    compatible, this field is entirely ignored.
-    """
+
     @property
     def library(self) -> tensorflow.core.framework.function_pb2.FunctionDefLibrary:
         """"library" provides user-defined functions.
 
         Naming:
           * library.function.name are in a flat namespace.
             NOTE: We may need to change it to be hierarchical to support
@@ -63,19 +65,20 @@
 
           * The consumer of return values may start executing as soon as
             the return values the consumer depends on are ready.  The
             consumer may want to use Tuple() mechanism to ensure the
             consumer does not start until all return values of the callee
             function are ready.
         """
+
     def __init__(
         self,
         *,
         node: collections.abc.Iterable[tensorflow.core.framework.node_def_pb2.NodeDef] | None = ...,
         versions: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
         version: builtins.int | None = ...,
         library: tensorflow.core.framework.function_pb2.FunctionDefLibrary | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["library", b"library", "versions", b"versions"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["library", b"library", "node", b"node", "version", b"version", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["library", b"library", "versions", b"versions"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["library", b"library", "node", b"node", "version", b"version", "versions", b"versions"]) -> None: ...
 
 global___GraphDef = GraphDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -16,33 +17,33 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GraphTransferNodeInput(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_ID_FIELD_NUMBER: builtins.int
     OUTPUT_PORT_FIELD_NUMBER: builtins.int
     node_id: builtins.int
     output_port: builtins.int
     def __init__(
         self,
         *,
         node_id: builtins.int | None = ...,
         output_port: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["node_id", b"node_id", "output_port", b"output_port"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["node_id", b"node_id", "output_port", b"output_port"]) -> None: ...
 
 global___GraphTransferNodeInput = GraphTransferNodeInput
 
-@typing_extensions.final
+@typing.final
 class GraphTransferNodeInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     NODE_ID_FIELD_NUMBER: builtins.int
     TYPE_NAME_FIELD_NUMBER: builtins.int
     SOC_OP_ID_FIELD_NUMBER: builtins.int
@@ -63,129 +64,129 @@
         node_id: builtins.int | None = ...,
         type_name: builtins.str | None = ...,
         soc_op_id: builtins.int | None = ...,
         padding_id: builtins.int | None = ...,
         input_count: builtins.int | None = ...,
         output_count: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["input_count", b"input_count", "name", b"name", "node_id", b"node_id", "output_count", b"output_count", "padding_id", b"padding_id", "soc_op_id", b"soc_op_id", "type_name", b"type_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["input_count", b"input_count", "name", b"name", "node_id", b"node_id", "output_count", b"output_count", "padding_id", b"padding_id", "soc_op_id", b"soc_op_id", "type_name", b"type_name"]) -> None: ...
 
 global___GraphTransferNodeInfo = GraphTransferNodeInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferConstNodeInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     NODE_ID_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     node_id: builtins.int
-    @property
-    def shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     data: builtins.bytes
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
+    @property
+    def shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         node_id: builtins.int | None = ...,
         shape: collections.abc.Iterable[builtins.int] | None = ...,
         data: builtins.bytes | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "dtype", b"dtype", "name", b"name", "node_id", b"node_id", "shape", b"shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data", "dtype", b"dtype", "name", b"name", "node_id", b"node_id", "shape", b"shape"]) -> None: ...
 
 global___GraphTransferConstNodeInfo = GraphTransferConstNodeInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferNodeInputInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_ID_FIELD_NUMBER: builtins.int
     NODE_INPUT_FIELD_NUMBER: builtins.int
     node_id: builtins.int
     @property
     def node_input(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferNodeInput]: ...
     def __init__(
         self,
         *,
         node_id: builtins.int | None = ...,
         node_input: collections.abc.Iterable[global___GraphTransferNodeInput] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["node_id", b"node_id", "node_input", b"node_input"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["node_id", b"node_id", "node_input", b"node_input"]) -> None: ...
 
 global___GraphTransferNodeInputInfo = GraphTransferNodeInputInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferNodeOutputInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_ID_FIELD_NUMBER: builtins.int
     MAX_BYTE_SIZE_FIELD_NUMBER: builtins.int
     node_id: builtins.int
     @property
     def max_byte_size(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         node_id: builtins.int | None = ...,
         max_byte_size: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_byte_size", b"max_byte_size", "node_id", b"node_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_byte_size", b"max_byte_size", "node_id", b"node_id"]) -> None: ...
 
 global___GraphTransferNodeOutputInfo = GraphTransferNodeOutputInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferGraphInputNodeInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         shape: collections.abc.Iterable[builtins.int] | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
 
 global___GraphTransferGraphInputNodeInfo = GraphTransferGraphInputNodeInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferGraphOutputNodeInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         shape: collections.abc.Iterable[builtins.int] | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
 
 global___GraphTransferGraphOutputNodeInfo = GraphTransferGraphOutputNodeInfo
 
-@typing_extensions.final
+@typing.final
 class GraphTransferInfo(google.protobuf.message.Message):
     """Protocol buffer representing a handle to a tensorflow resource. Handles are
     not valid across executions, but can be serialized back and forth from within
     a single run.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -206,36 +207,37 @@
     NODE_INFO_FIELD_NUMBER: builtins.int
     CONST_NODE_INFO_FIELD_NUMBER: builtins.int
     NODE_INPUT_INFO_FIELD_NUMBER: builtins.int
     NODE_OUTPUT_INFO_FIELD_NUMBER: builtins.int
     GRAPH_INPUT_NODE_INFO_FIELD_NUMBER: builtins.int
     GRAPH_OUTPUT_NODE_INFO_FIELD_NUMBER: builtins.int
     DESTINATION_FIELD_NUMBER: builtins.int
+    destination: global___GraphTransferInfo.Destination.ValueType
+    """Destination of graph transfer"""
     @property
     def node_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferNodeInfo]: ...
     @property
     def const_node_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferConstNodeInfo]: ...
     @property
     def node_input_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferNodeInputInfo]: ...
     @property
     def node_output_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferNodeOutputInfo]: ...
     @property
     def graph_input_node_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferGraphInputNodeInfo]:
         """Input Node parameters of transferred graph"""
+
     @property
     def graph_output_node_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphTransferGraphOutputNodeInfo]: ...
-    destination: global___GraphTransferInfo.Destination.ValueType
-    """Destination of graph transfer"""
     def __init__(
         self,
         *,
         node_info: collections.abc.Iterable[global___GraphTransferNodeInfo] | None = ...,
         const_node_info: collections.abc.Iterable[global___GraphTransferConstNodeInfo] | None = ...,
         node_input_info: collections.abc.Iterable[global___GraphTransferNodeInputInfo] | None = ...,
         node_output_info: collections.abc.Iterable[global___GraphTransferNodeOutputInfo] | None = ...,
         graph_input_node_info: collections.abc.Iterable[global___GraphTransferGraphInputNodeInfo] | None = ...,
         graph_output_node_info: collections.abc.Iterable[global___GraphTransferGraphOutputNodeInfo] | None = ...,
         destination: global___GraphTransferInfo.Destination.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["const_node_info", b"const_node_info", "destination", b"destination", "graph_input_node_info", b"graph_input_node_info", "graph_output_node_info", b"graph_output_node_info", "node_info", b"node_info", "node_input_info", b"node_input_info", "node_output_info", b"node_output_info"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["const_node_info", b"const_node_info", "destination", b"destination", "graph_input_node_info", b"graph_input_node_info", "graph_output_node_info", b"graph_output_node_info", "node_info", b"node_info", "node_input_info", b"node_input_info", "node_output_info", b"node_output_info"]) -> None: ...
 
 global___GraphTransferInfo = GraphTransferInfo
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,102 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.attr_value_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class KernelDef(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AttrConstraint(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         ALLOWED_VALUES_FIELD_NUMBER: builtins.int
         name: builtins.str
         """Name of an attr from the Op."""
         @property
         def allowed_values(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue:
             """A list of values that this kernel supports for this attr.
             Like OpDef.AttrDef.allowed_values, except for kernels instead of Ops.
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             allowed_values: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["allowed_values", b"allowed_values"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["allowed_values", b"allowed_values", "name", b"name"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["allowed_values", b"allowed_values"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["allowed_values", b"allowed_values", "name", b"name"]) -> None: ...
 
     OP_FIELD_NUMBER: builtins.int
     DEVICE_TYPE_FIELD_NUMBER: builtins.int
     CONSTRAINT_FIELD_NUMBER: builtins.int
     HOST_MEMORY_ARG_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
     PRIORITY_FIELD_NUMBER: builtins.int
     op: builtins.str
     """Must match the name of an Op."""
     device_type: builtins.str
     """Type of device this kernel runs on."""
-    @property
-    def constraint(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___KernelDef.AttrConstraint]: ...
-    @property
-    def host_memory_arg(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Names of the Op's input_/output_args that reside in host memory
-        instead of device memory.
-        """
     label: builtins.str
     """This allows experimental kernels to be registered for an op that
     won't be used unless the user specifies a "_kernel" attr with
     value matching this.
     """
     priority: builtins.int
     """Prioritization of kernel amongst different devices. By default we assume
     priority is 0. The higher the priority the better. By default (i.e. if
     this is not set), we prefer GPU kernels over CPU.
     """
+    @property
+    def constraint(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___KernelDef.AttrConstraint]: ...
+    @property
+    def host_memory_arg(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Names of the Op's input_/output_args that reside in host memory
+        instead of device memory.
+        """
+
     def __init__(
         self,
         *,
         op: builtins.str | None = ...,
         device_type: builtins.str | None = ...,
         constraint: collections.abc.Iterable[global___KernelDef.AttrConstraint] | None = ...,
         host_memory_arg: collections.abc.Iterable[builtins.str] | None = ...,
         label: builtins.str | None = ...,
         priority: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["constraint", b"constraint", "device_type", b"device_type", "host_memory_arg", b"host_memory_arg", "label", b"label", "op", b"op", "priority", b"priority"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["constraint", b"constraint", "device_type", b"device_type", "host_memory_arg", b"host_memory_arg", "label", b"label", "op", b"op", "priority", b"priority"]) -> None: ...
 
 global___KernelDef = KernelDef
 
-@typing_extensions.final
+@typing.final
 class KernelList(google.protobuf.message.Message):
     """A collection of KernelDefs"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KERNEL_FIELD_NUMBER: builtins.int
     @property
     def kernel(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___KernelDef]: ...
     def __init__(
         self,
         *,
         kernel: collections.abc.Iterable[global___KernelDef] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kernel", b"kernel"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["kernel", b"kernel"]) -> None: ...
 
 global___KernelList = KernelList
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.framework.tensor_description_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class MemoryLogStep(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STEP_ID_FIELD_NUMBER: builtins.int
     HANDLE_FIELD_NUMBER: builtins.int
     step_id: builtins.int
     """Process-unique step id."""
@@ -23,19 +24,19 @@
     """Handle describing the feeds and fetches of the step."""
     def __init__(
         self,
         *,
         step_id: builtins.int | None = ...,
         handle: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["handle", b"handle", "step_id", b"step_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["handle", b"handle", "step_id", b"step_id"]) -> None: ...
 
 global___MemoryLogStep = MemoryLogStep
 
-@typing_extensions.final
+@typing.final
 class MemoryLogTensorAllocation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STEP_ID_FIELD_NUMBER: builtins.int
     KERNEL_NAME_FIELD_NUMBER: builtins.int
     TENSOR_FIELD_NUMBER: builtins.int
     step_id: builtins.int
@@ -43,27 +44,28 @@
     kernel_name: builtins.str
     """Name of the kernel making the allocation as set in GraphDef,
     e.g., "affine2/weights/Assign".
     """
     @property
     def tensor(self) -> tensorflow.core.framework.tensor_description_pb2.TensorDescription:
         """Allocated tensor details."""
+
     def __init__(
         self,
         *,
         step_id: builtins.int | None = ...,
         kernel_name: builtins.str | None = ...,
         tensor: tensorflow.core.framework.tensor_description_pb2.TensorDescription | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor", b"tensor"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kernel_name", b"kernel_name", "step_id", b"step_id", "tensor", b"tensor"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor", b"tensor"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["kernel_name", b"kernel_name", "step_id", b"step_id", "tensor", b"tensor"]) -> None: ...
 
 global___MemoryLogTensorAllocation = MemoryLogTensorAllocation
 
-@typing_extensions.final
+@typing.final
 class MemoryLogTensorDeallocation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOCATION_ID_FIELD_NUMBER: builtins.int
     ALLOCATOR_NAME_FIELD_NUMBER: builtins.int
     allocation_id: builtins.int
     """Id of the tensor buffer being deallocated, used to match to a
@@ -73,19 +75,19 @@
     """Name of the allocator used."""
     def __init__(
         self,
         *,
         allocation_id: builtins.int | None = ...,
         allocator_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name"]) -> None: ...
 
 global___MemoryLogTensorDeallocation = MemoryLogTensorDeallocation
 
-@typing_extensions.final
+@typing.final
 class MemoryLogTensorOutput(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STEP_ID_FIELD_NUMBER: builtins.int
     KERNEL_NAME_FIELD_NUMBER: builtins.int
     INDEX_FIELD_NUMBER: builtins.int
     TENSOR_FIELD_NUMBER: builtins.int
@@ -96,28 +98,29 @@
     "affine2/weights/Assign".
     """
     index: builtins.int
     """Index of the output being set."""
     @property
     def tensor(self) -> tensorflow.core.framework.tensor_description_pb2.TensorDescription:
         """Output tensor details."""
+
     def __init__(
         self,
         *,
         step_id: builtins.int | None = ...,
         kernel_name: builtins.str | None = ...,
         index: builtins.int | None = ...,
         tensor: tensorflow.core.framework.tensor_description_pb2.TensorDescription | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor", b"tensor"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["index", b"index", "kernel_name", b"kernel_name", "step_id", b"step_id", "tensor", b"tensor"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor", b"tensor"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["index", b"index", "kernel_name", b"kernel_name", "step_id", b"step_id", "tensor", b"tensor"]) -> None: ...
 
 global___MemoryLogTensorOutput = MemoryLogTensorOutput
 
-@typing_extensions.final
+@typing.final
 class MemoryLogRawAllocation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STEP_ID_FIELD_NUMBER: builtins.int
     OPERATION_FIELD_NUMBER: builtins.int
     NUM_BYTES_FIELD_NUMBER: builtins.int
     PTR_FIELD_NUMBER: builtins.int
@@ -143,19 +146,19 @@
         step_id: builtins.int | None = ...,
         operation: builtins.str | None = ...,
         num_bytes: builtins.int | None = ...,
         ptr: builtins.int | None = ...,
         allocation_id: builtins.int | None = ...,
         allocator_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "num_bytes", b"num_bytes", "operation", b"operation", "ptr", b"ptr", "step_id", b"step_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "num_bytes", b"num_bytes", "operation", b"operation", "ptr", b"ptr", "step_id", b"step_id"]) -> None: ...
 
 global___MemoryLogRawAllocation = MemoryLogRawAllocation
 
-@typing_extensions.final
+@typing.final
 class MemoryLogRawDeallocation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STEP_ID_FIELD_NUMBER: builtins.int
     OPERATION_FIELD_NUMBER: builtins.int
     ALLOCATION_ID_FIELD_NUMBER: builtins.int
     ALLOCATOR_NAME_FIELD_NUMBER: builtins.int
@@ -179,10 +182,10 @@
         *,
         step_id: builtins.int | None = ...,
         operation: builtins.str | None = ...,
         allocation_id: builtins.int | None = ...,
         allocator_name: builtins.str | None = ...,
         deferred: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "deferred", b"deferred", "operation", b"operation", "step_id", b"step_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allocation_id", b"allocation_id", "allocator_name", b"allocator_name", "deferred", b"deferred", "operation", b"operation", "step_id", b"step_id"]) -> None: ...
 
 global___MemoryLogRawDeallocation = MemoryLogRawDeallocation
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -63,29 +64,29 @@
 DEFAULT: AutotuneAlgorithm.ValueType  # 0
 HILL_CLIMB: AutotuneAlgorithm.ValueType  # 1
 GRADIENT_DESCENT: AutotuneAlgorithm.ValueType  # 2
 MAX_PARALLELISM: AutotuneAlgorithm.ValueType  # 3
 STAGE_BASED: AutotuneAlgorithm.ValueType  # 4
 global___AutotuneAlgorithm = AutotuneAlgorithm
 
-@typing_extensions.final
+@typing.final
 class ModelProto(google.protobuf.message.Message):
     """Protocol buffer representing the data used by the autotuning modeling
     framework.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Node(google.protobuf.message.Message):
         """General representation of a node in the model."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class Parameter(google.protobuf.message.Message):
             """Represents a node parameter."""
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             NAME_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
@@ -113,15 +114,15 @@
                 name: builtins.str | None = ...,
                 value: builtins.float | None = ...,
                 state_value: builtins.float | None = ...,
                 min: builtins.float | None = ...,
                 max: builtins.float | None = ...,
                 tunable: builtins.bool | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["max", b"max", "min", b"min", "name", b"name", "state_value", b"state_value", "tunable", b"tunable", "value", b"value"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["max", b"max", "min", b"min", "name", b"name", "state_value", b"state_value", "tunable", b"tunable", "value", b"value"]) -> None: ...
 
         ID_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         AUTOTUNE_FIELD_NUMBER: builtins.int
         BUFFERED_BYTES_FIELD_NUMBER: builtins.int
         BUFFERED_ELEMENTS_FIELD_NUMBER: builtins.int
         BYTES_CONSUMED_FIELD_NUMBER: builtins.int
@@ -154,33 +155,35 @@
         """The number of elements produced by the node."""
         processing_time: builtins.int
         """The aggregate processing time spent in this node in nanoseconds."""
         record_metrics: builtins.bool
         """An indication whether this node records metrics about produced and
         consumed elements.
         """
-        @property
-        def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ModelProto.Node.Parameter]:
-            """Parameters of this node."""
         input_processing_time_sum: builtins.float
         """Statistic of inputs processing time history."""
         input_processing_time_count: builtins.int
-        @property
-        def inputs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-            """IDs of inputs of this node."""
         node_class: global___NodeClass.ValueType
         """Class of this node."""
         ratio: builtins.float
         """Ratio of input to output elements. This is only used by KNOWN_RATIO and
         ASYNC_KNOWN_RATIO nodes.
         """
         memory_ratio: builtins.float
         """Ratio identifies how many parallelism calls are introduced by one
         buffered element. This is only used by ASYNC_KNOWN_RATIO nodes.
         """
+        @property
+        def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ModelProto.Node.Parameter]:
+            """Parameters of this node."""
+
+        @property
+        def inputs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """IDs of inputs of this node."""
+
         def __init__(
             self,
             *,
             id: builtins.int | None = ...,
             name: builtins.str | None = ...,
             autotune: builtins.bool | None = ...,
             buffered_bytes: builtins.int | None = ...,
@@ -194,35 +197,35 @@
             input_processing_time_sum: builtins.float | None = ...,
             input_processing_time_count: builtins.int | None = ...,
             inputs: collections.abc.Iterable[builtins.int] | None = ...,
             node_class: global___NodeClass.ValueType | None = ...,
             ratio: builtins.float | None = ...,
             memory_ratio: builtins.float | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["autotune", b"autotune", "buffered_bytes", b"buffered_bytes", "buffered_elements", b"buffered_elements", "bytes_consumed", b"bytes_consumed", "bytes_produced", b"bytes_produced", "id", b"id", "input_processing_time_count", b"input_processing_time_count", "input_processing_time_sum", b"input_processing_time_sum", "inputs", b"inputs", "memory_ratio", b"memory_ratio", "name", b"name", "node_class", b"node_class", "num_elements", b"num_elements", "parameters", b"parameters", "processing_time", b"processing_time", "ratio", b"ratio", "record_metrics", b"record_metrics"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["autotune", b"autotune", "buffered_bytes", b"buffered_bytes", "buffered_elements", b"buffered_elements", "bytes_consumed", b"bytes_consumed", "bytes_produced", b"bytes_produced", "id", b"id", "input_processing_time_count", b"input_processing_time_count", "input_processing_time_sum", b"input_processing_time_sum", "inputs", b"inputs", "memory_ratio", b"memory_ratio", "name", b"name", "node_class", b"node_class", "num_elements", b"num_elements", "parameters", b"parameters", "processing_time", b"processing_time", "ratio", b"ratio", "record_metrics", b"record_metrics"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class NodesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
         def value(self) -> global___ModelProto.Node: ...
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: global___ModelProto.Node | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class OptimizationParams(google.protobuf.message.Message):
         """Contains parameters of the model autotuning optimization."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ALGORITHM_FIELD_NUMBER: builtins.int
         CPU_BUDGET_FIELD_NUMBER: builtins.int
@@ -242,34 +245,35 @@
             self,
             *,
             algorithm: global___AutotuneAlgorithm.ValueType | None = ...,
             cpu_budget: builtins.int | None = ...,
             ram_budget: builtins.int | None = ...,
             model_input_time: builtins.float | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "cpu_budget", b"cpu_budget", "model_input_time", b"model_input_time", "ram_budget", b"ram_budget"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "cpu_budget", b"cpu_budget", "model_input_time", b"model_input_time", "ram_budget", b"ram_budget"]) -> None: ...
 
     NODES_FIELD_NUMBER: builtins.int
     OUTPUT_FIELD_NUMBER: builtins.int
     ID_COUNTER_FIELD_NUMBER: builtins.int
     OPTIMIZATION_PARAMS_FIELD_NUMBER: builtins.int
-    @property
-    def nodes(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___ModelProto.Node]:
-        """Map of node IDs to nodes of this model."""
     output: builtins.int
     """ID of the output node of this model."""
     id_counter: builtins.int
     """Counter for node IDs of this model."""
     @property
+    def nodes(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___ModelProto.Node]:
+        """Map of node IDs to nodes of this model."""
+
+    @property
     def optimization_params(self) -> global___ModelProto.OptimizationParams: ...
     def __init__(
         self,
         *,
         nodes: collections.abc.Mapping[builtins.int, global___ModelProto.Node] | None = ...,
         output: builtins.int | None = ...,
         id_counter: builtins.int | None = ...,
         optimization_params: global___ModelProto.OptimizationParams | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["optimization_params", b"optimization_params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id_counter", b"id_counter", "nodes", b"nodes", "optimization_params", b"optimization_params", "output", b"output"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["optimization_params", b"optimization_params"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["id_counter", b"id_counter", "nodes", b"nodes", "optimization_params", b"optimization_params", "output", b"output"]) -> None: ...
 
 global___ModelProto = ModelProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.attr_value_pb2
 import tensorflow.core.framework.full_type_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class NodeDef(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class AttrEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ExperimentalDebugInfo(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ORIGINAL_NODE_NAMES_FIELD_NUMBER: builtins.int
         ORIGINAL_FUNC_NAMES_FIELD_NUMBER: builtins.int
         @property
         def original_node_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
@@ -48,31 +49,33 @@
 
             This is intended to store the list of names of the nodes from the
             original graph that this node was derived. For example if this node, say
             C, was result of a fusion of 2 nodes A and B, then 'original_node' would
             be {A, B}. This information can be used to map errors originating at the
             current node to some top level source code.
             """
+
         @property
         def original_func_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
             """This is intended to store the list of names of the functions from the
             original graph that this node was derived. For example if this node, say
             C, was result of a fusion of node A in function FA and node B in function
             FB, then `original_funcs` would be {FA, FB}. If the node is in the top
             level graph, the `original_func` is empty. This information, with the
             `original_node_names` can be used to map errors originating at the
             current ndoe to some top level source code.
             """
+
         def __init__(
             self,
             *,
             original_node_names: collections.abc.Iterable[builtins.str] | None = ...,
             original_func_names: collections.abc.Iterable[builtins.str] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["original_func_names", b"original_func_names", "original_node_names", b"original_node_names"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["original_func_names", b"original_func_names", "original_node_names", b"original_node_names"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     OP_FIELD_NUMBER: builtins.int
     INPUT_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     ATTR_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_DEBUG_INFO_FIELD_NUMBER: builtins.int
@@ -82,22 +85,14 @@
     logging, visualization, etc.  Unique within a single GraphDef.
     Must match the regexp "[A-Za-z0-9.][A-Za-z0-9_>./]*".
     """
     op: builtins.str
     """The operation name.  There may be custom parameters in attrs.
     Op names starting with an underscore are reserved for internal use.
     """
-    @property
-    def input(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Each input is "node:src_output" with "node" being a string name and
-        "src_output" indicating which output tensor to use from "node". If
-        "src_output" is 0 the ":0" suffix can be omitted.  Regular inputs
-        may optionally be followed by control inputs that have the format
-        "^node".
-        """
     device: builtins.str
     """A (possibly partial) specification for the device on which this
     node should be placed.
     The expected syntax for this string is as follows:
 
     DEVICE_SPEC ::= PARTIAL_SPEC
 
@@ -113,46 +108,58 @@
     * ""                                    (no specification)
 
     If the constraints do not resolve to a single device (or if this
     field is empty or not present), the runtime will attempt to
     choose a device automatically.
     """
     @property
+    def input(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Each input is "node:src_output" with "node" being a string name and
+        "src_output" indicating which output tensor to use from "node". If
+        "src_output" is 0 the ":0" suffix can be omitted.  Regular inputs
+        may optionally be followed by control inputs that have the format
+        "^node".
+        """
+
+    @property
     def attr(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue]:
         """Operation-specific graph-construction-time configuration.
         Note that this should include all attrs defined in the
         corresponding OpDef, including those with a value matching
         the default -- this allows the default to change and makes
         NodeDefs easier to interpret on their own.  However, if
         an attr with a default is not specified in this list, the
         default will be used.
         The "names" (keys) must match the regexp "[a-z][a-z0-9_]+" (and
         one of the names from the corresponding OpDef's attr field).
         The values must have a type matching the corresponding OpDef
         attr's type field.
         TODO(josh11b): Add some examples here showing best practices.
         """
+
     @property
     def experimental_debug_info(self) -> global___NodeDef.ExperimentalDebugInfo:
         """This stores debug information associated with the node."""
+
     @property
     def experimental_type(self) -> tensorflow.core.framework.full_type_pb2.FullTypeDef:
         """The complete type of this node. Experimental and subject to change.
         Currently, the field only contains the return types of the node. That will
         extend in the future to contain the entire signature of the node, as a
         function type.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         op: builtins.str | None = ...,
         input: collections.abc.Iterable[builtins.str] | None = ...,
         device: builtins.str | None = ...,
         attr: collections.abc.Mapping[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue] | None = ...,
         experimental_debug_info: global___NodeDef.ExperimentalDebugInfo | None = ...,
         experimental_type: tensorflow.core.framework.full_type_pb2.FullTypeDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["experimental_debug_info", b"experimental_debug_info", "experimental_type", b"experimental_type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["attr", b"attr", "device", b"device", "experimental_debug_info", b"experimental_debug_info", "experimental_type", b"experimental_type", "input", b"input", "name", b"name", "op", b"op"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["experimental_debug_info", b"experimental_debug_info", "experimental_type", b"experimental_type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["attr", b"attr", "device", b"device", "experimental_debug_info", b"experimental_debug_info", "experimental_type", b"experimental_type", "input", b"input", "name", b"name", "op", b"op"]) -> None: ...
 
 global___NodeDef = NodeDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.attr_value_pb2
 import tensorflow.core.framework.full_type_pb2
 import tensorflow.core.framework.resource_handle_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class OpDef(google.protobuf.message.Message):
     """Defines an operation. A NodeDef in a GraphDef specifies an Op by
     using the "op" field which should match the name of a OpDef.
     LINT.IfChange
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ArgDef(google.protobuf.message.Message):
         """For describing inputs and outputs."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         DESCRIPTION_FIELD_NUMBER: builtins.int
@@ -60,51 +61,53 @@
         """if specified, attr must have type "type" """
         number_attr: builtins.str
         """if specified, attr must have type "int" """
         type_list_attr: builtins.str
         """If specified, attr must have type "list(type)", and none of
         type, type_attr, and number_attr may be specified.
         """
-        @property
-        def handle_data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.resource_handle_pb2.ResourceHandleProto.DtypeAndShape]:
-            """The handle data for resource inputs."""
         is_ref: builtins.bool
         """For inputs: if true, the inputs are required to be refs.
           By default, inputs can be either refs or non-refs.
         For outputs: if true, outputs are refs, otherwise they are not.
         """
         @property
+        def handle_data(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.resource_handle_pb2.ResourceHandleProto.DtypeAndShape]:
+            """The handle data for resource inputs."""
+
+        @property
         def experimental_full_type(self) -> tensorflow.core.framework.full_type_pb2.FullTypeDef:
             """Experimental. Full type declaration for this argument.
             The full type specification combines type, type_attr, type_list_attr,
             etc. into a unified representation.
             This declaration may contain non-concrete types (for example,
             Tensor<TypeVar<'T'>> is a valid type declaration.
 
             Note: this is a transient field. The long-term aim is to represent the
             entire OpDef as a single type: a callable. In that context, this field is
             just the type of a single argument.
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             description: builtins.str | None = ...,
             type: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
             type_attr: builtins.str | None = ...,
             number_attr: builtins.str | None = ...,
             type_list_attr: builtins.str | None = ...,
             handle_data: collections.abc.Iterable[tensorflow.core.framework.resource_handle_pb2.ResourceHandleProto.DtypeAndShape] | None = ...,
             is_ref: builtins.bool | None = ...,
             experimental_full_type: tensorflow.core.framework.full_type_pb2.FullTypeDef | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["experimental_full_type", b"experimental_full_type"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "experimental_full_type", b"experimental_full_type", "handle_data", b"handle_data", "is_ref", b"is_ref", "name", b"name", "number_attr", b"number_attr", "type", b"type", "type_attr", b"type_attr", "type_list_attr", b"type_list_attr"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["experimental_full_type", b"experimental_full_type"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["description", b"description", "experimental_full_type", b"experimental_full_type", "handle_data", b"handle_data", "is_ref", b"is_ref", "name", b"name", "number_attr", b"number_attr", "type", b"type", "type_attr", b"type_attr", "type_list_attr", b"type_list_attr"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class AttrDef(google.protobuf.message.Message):
         """Description of the graph-construction-time configuration of this
         Op.  That is to say, this describes the attr fields that will
         be specified in the NodeDef.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -121,52 +124,54 @@
         Python client, as a keyword argument name, and so should match
         the regexp "[a-z][a-z0-9_]+".
         """
         type: builtins.str
         """One of the type names from attr_value.proto ("string", "list(string)",
         "int", etc.).
         """
-        @property
-        def default_value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue:
-            """A reasonable default for this attribute if the user does not supply
-            a value.  If not specified, the user must supply a value.
-            """
         description: builtins.str
         """Human-readable description."""
         has_minimum: builtins.bool
         """--- Constraints ---
         These constraints are only in effect if specified.  Default is no
         constraints.
 
         For type == "int", this is a minimum value.  For "list(___)"
         types, this is the minimum length.
         """
         minimum: builtins.int
         @property
+        def default_value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue:
+            """A reasonable default for this attribute if the user does not supply
+            a value.  If not specified, the user must supply a value.
+            """
+
+        @property
         def allowed_values(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue:
             """The set of allowed values.  Has type that is the "list" version
             of the "type" field above (uses the "list" field of AttrValue).
             If type == "type" or "list(type)" above, then the "type" field
             of "allowed_values.list" has the set of allowed DataTypes.
             If type == "string" or "list(string)", then the "s" field of
             "allowed_values.list" has the set of allowed strings.
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             type: builtins.str | None = ...,
             default_value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
             description: builtins.str | None = ...,
             has_minimum: builtins.bool | None = ...,
             minimum: builtins.int | None = ...,
             allowed_values: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["allowed_values", b"allowed_values", "default_value", b"default_value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["allowed_values", b"allowed_values", "default_value", b"default_value", "description", b"description", "has_minimum", b"has_minimum", "minimum", b"minimum", "name", b"name", "type", b"type"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["allowed_values", b"allowed_values", "default_value", b"default_value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["allowed_values", b"allowed_values", "default_value", b"default_value", "description", b"description", "has_minimum", b"has_minimum", "minimum", b"minimum", "name", b"name", "type", b"type"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     INPUT_ARG_FIELD_NUMBER: builtins.int
     OUTPUT_ARG_FIELD_NUMBER: builtins.int
     CONTROL_OUTPUT_FIELD_NUMBER: builtins.int
     ATTR_FIELD_NUMBER: builtins.int
     DEPRECATION_FIELD_NUMBER: builtins.int
@@ -177,30 +182,14 @@
     IS_STATEFUL_FIELD_NUMBER: builtins.int
     ALLOWS_UNINITIALIZED_INPUT_FIELD_NUMBER: builtins.int
     IS_DISTRIBUTED_COMMUNICATION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Op names starting with an underscore are reserved for internal use.
     Names should be CamelCase and match the regexp "[A-Z][a-zA-Z0-9>_]*".
     """
-    @property
-    def input_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.ArgDef]:
-        """Description of the input(s)."""
-    @property
-    def output_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.ArgDef]:
-        """Description of the output(s)."""
-    @property
-    def control_output(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Named control outputs for this operation. Useful only for composite
-        operations (i.e. functions) which want to name different control outputs.
-        """
-    @property
-    def attr(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.AttrDef]: ...
-    @property
-    def deprecation(self) -> global___OpDeprecation:
-        """Optional deprecation based on GraphDef versions."""
     summary: builtins.str
     """One-line human-readable description of what the Op does."""
     description: builtins.str
     """Additional, longer human-readable description of what the Op does."""
     is_commutative: builtins.bool
     """-------------------------------------------------------------------------
     Which optimizations this operation can participate in.
@@ -246,14 +235,34 @@
     for Assign, etc.
     """
     is_distributed_communication: builtins.bool
     """Indicates whether the op implementation uses distributed communication.
     If True, the op is allowed to return errors for network disconnection and
     trigger TF network failure handling logics.
     """
+    @property
+    def input_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.ArgDef]:
+        """Description of the input(s)."""
+
+    @property
+    def output_arg(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.ArgDef]:
+        """Description of the output(s)."""
+
+    @property
+    def control_output(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Named control outputs for this operation. Useful only for composite
+        operations (i.e. functions) which want to name different control outputs.
+        """
+
+    @property
+    def attr(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef.AttrDef]: ...
+    @property
+    def deprecation(self) -> global___OpDeprecation:
+        """Optional deprecation based on GraphDef versions."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         input_arg: collections.abc.Iterable[global___OpDef.ArgDef] | None = ...,
         output_arg: collections.abc.Iterable[global___OpDef.ArgDef] | None = ...,
         control_output: collections.abc.Iterable[builtins.str] | None = ...,
@@ -263,20 +272,20 @@
         description: builtins.str | None = ...,
         is_commutative: builtins.bool | None = ...,
         is_aggregate: builtins.bool | None = ...,
         is_stateful: builtins.bool | None = ...,
         allows_uninitialized_input: builtins.bool | None = ...,
         is_distributed_communication: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deprecation", b"deprecation"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allows_uninitialized_input", b"allows_uninitialized_input", "attr", b"attr", "control_output", b"control_output", "deprecation", b"deprecation", "description", b"description", "input_arg", b"input_arg", "is_aggregate", b"is_aggregate", "is_commutative", b"is_commutative", "is_distributed_communication", b"is_distributed_communication", "is_stateful", b"is_stateful", "name", b"name", "output_arg", b"output_arg", "summary", b"summary"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["deprecation", b"deprecation"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allows_uninitialized_input", b"allows_uninitialized_input", "attr", b"attr", "control_output", b"control_output", "deprecation", b"deprecation", "description", b"description", "input_arg", b"input_arg", "is_aggregate", b"is_aggregate", "is_commutative", b"is_commutative", "is_distributed_communication", b"is_distributed_communication", "is_stateful", b"is_stateful", "name", b"name", "output_arg", b"output_arg", "summary", b"summary"]) -> None: ...
 
 global___OpDef = OpDef
 
-@typing_extensions.final
+@typing.final
 class OpDeprecation(google.protobuf.message.Message):
     """Information about version-dependent deprecation of an op"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VERSION_FIELD_NUMBER: builtins.int
     EXPLANATION_FIELD_NUMBER: builtins.int
@@ -286,28 +295,28 @@
     """Explanation of why it was deprecated and what to use instead."""
     def __init__(
         self,
         *,
         version: builtins.int | None = ...,
         explanation: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["explanation", b"explanation", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["explanation", b"explanation", "version", b"version"]) -> None: ...
 
 global___OpDeprecation = OpDeprecation
 
-@typing_extensions.final
+@typing.final
 class OpList(google.protobuf.message.Message):
     """A collection of OpDefs"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OP_FIELD_NUMBER: builtins.int
     @property
     def op(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___OpDef]: ...
     def __init__(
         self,
         *,
         op: collections.abc.Iterable[global___OpDef] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["op", b"op"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["op", b"op"]) -> None: ...
 
 global___OpList = OpList
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.graph_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class OptimizedFunctionGraph(google.protobuf.message.Message):
     """Optimized function graph after instantiation-related graph optimization
     passes (up till before graph partitioning). The first half of the proto is
     representing a GraphDef and the rest of the fields are extra information from
     graph optimizations.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class NodeNameToControlRetEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     FUNCTION_GRAPH_FIELD_NUMBER: builtins.int
     NODE_NAME_TO_CONTROL_RET_FIELD_NUMBER: builtins.int
     RET_TYPES_FIELD_NUMBER: builtins.int
     NUM_RETURN_NODES_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Function name. It can be a human-readable SignatureDef's method name, or a
     FunctionDef name.
     """
+    num_return_nodes: builtins.int
+    """Number of return nodes. This is an output of graph preprocessing."""
     @property
     def function_graph(self) -> tensorflow.core.framework.graph_pb2.GraphDef:
         """Optimized function graph."""
+
     @property
     def node_name_to_control_ret(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Maps from node name to control ret. This is an output from running TF/XLA
         bridge.
         """
+
     @property
     def ret_types(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[tensorflow.core.framework.types_pb2.DataType.ValueType]:
         """Return node types of the function. This is an output of graph
         preprocessing.
         """
-    num_return_nodes: builtins.int
-    """Number of return nodes. This is an output of graph preprocessing."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         function_graph: tensorflow.core.framework.graph_pb2.GraphDef | None = ...,
         node_name_to_control_ret: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         ret_types: collections.abc.Iterable[tensorflow.core.framework.types_pb2.DataType.ValueType] | None = ...,
         num_return_nodes: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["function_graph", b"function_graph"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["function_graph", b"function_graph", "name", b"name", "node_name_to_control_ret", b"node_name_to_control_ret", "num_return_nodes", b"num_return_nodes", "ret_types", b"ret_types"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["function_graph", b"function_graph"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["function_graph", b"function_graph", "name", b"name", "node_name_to_control_ret", b"node_name_to_control_ret", "num_return_nodes", b"num_return_nodes", "ret_types", b"ret_types"]) -> None: ...
 
 global___OptimizedFunctionGraph = OptimizedFunctionGraph
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ReaderBaseState(google.protobuf.message.Message):
     """For serializing and restoring the state of ReaderBase, see
     reader_base.h for details.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -30,10 +31,10 @@
         self,
         *,
         work_started: builtins.int | None = ...,
         work_finished: builtins.int | None = ...,
         num_records_produced: builtins.int | None = ...,
         current_work: builtins.bytes | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["current_work", b"current_work", "num_records_produced", b"num_records_produced", "work_finished", b"work_finished", "work_started", b"work_started"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["current_work", b"current_work", "num_records_produced", b"num_records_produced", "work_finished", b"work_finished", "work_started", b"work_started"]) -> None: ...
 
 global___ReaderBaseState = ReaderBaseState
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ResourceHandleProto(google.protobuf.message.Message):
     """Protocol buffer representing a handle to a tensorflow resource. Handles are
     not valid across executions, but can be serialized back and forth from within
     a single run.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class DtypeAndShape(google.protobuf.message.Message):
         """Protocol buffer representing a pair of (data type, tensor shape)."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         DTYPE_FIELD_NUMBER: builtins.int
         SHAPE_FIELD_NUMBER: builtins.int
@@ -36,16 +37,16 @@
         def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
         def __init__(
             self,
             *,
             dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
             shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
 
     DEVICE_FIELD_NUMBER: builtins.int
     CONTAINER_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     HASH_CODE_FIELD_NUMBER: builtins.int
     MAYBE_TYPE_NAME_FIELD_NUMBER: builtins.int
     DTYPES_AND_SHAPES_FIELD_NUMBER: builtins.int
@@ -62,20 +63,21 @@
     maybe_type_name: builtins.str
     """For debug-only, the name of the type pointed to by this handle, if
     available.
     """
     @property
     def dtypes_and_shapes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceHandleProto.DtypeAndShape]:
         """Data types and shapes for the underlying resource."""
+
     def __init__(
         self,
         *,
         device: builtins.str | None = ...,
         container: builtins.str | None = ...,
         name: builtins.str | None = ...,
         hash_code: builtins.int | None = ...,
         maybe_type_name: builtins.str | None = ...,
         dtypes_and_shapes: collections.abc.Iterable[global___ResourceHandleProto.DtypeAndShape] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["container", b"container", "device", b"device", "dtypes_and_shapes", b"dtypes_and_shapes", "hash_code", b"hash_code", "maybe_type_name", b"maybe_type_name", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["container", b"container", "device", b"device", "dtypes_and_shapes", b"dtypes_and_shapes", "hash_code", b"hash_code", "maybe_type_name", b"maybe_type_name", "name", b"name"]) -> None: ...
 
 global___ResourceHandleProto = ResourceHandleProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.allocation_description_pb2
 import tensorflow.core.framework.tensor_description_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class AllocationRecord(google.protobuf.message.Message):
     """An allocation/de-allocation operation performed by the allocator."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOC_MICROS_FIELD_NUMBER: builtins.int
     ALLOC_BYTES_FIELD_NUMBER: builtins.int
@@ -28,19 +29,19 @@
     """Number of bytes allocated, or de-allocated if negative."""
     def __init__(
         self,
         *,
         alloc_micros: builtins.int | None = ...,
         alloc_bytes: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["alloc_bytes", b"alloc_bytes", "alloc_micros", b"alloc_micros"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["alloc_bytes", b"alloc_bytes", "alloc_micros", b"alloc_micros"]) -> None: ...
 
 global___AllocationRecord = AllocationRecord
 
-@typing_extensions.final
+@typing.final
 class AllocatorMemoryUsed(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOCATOR_NAME_FIELD_NUMBER: builtins.int
     TOTAL_BYTES_FIELD_NUMBER: builtins.int
     PEAK_BYTES_FIELD_NUMBER: builtins.int
     LIVE_BYTES_FIELD_NUMBER: builtins.int
@@ -48,36 +49,37 @@
     ALLOCATOR_BYTES_IN_USE_FIELD_NUMBER: builtins.int
     allocator_name: builtins.str
     total_bytes: builtins.int
     """These are per-node allocator memory stats."""
     peak_bytes: builtins.int
     live_bytes: builtins.int
     """The bytes that are not deallocated."""
-    @property
-    def allocation_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AllocationRecord]:
-        """The allocation and deallocation timeline."""
     allocator_bytes_in_use: builtins.int
     """These are snapshots of the overall allocator memory stats.
     The number of live bytes currently allocated by the allocator.
     """
+    @property
+    def allocation_records(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AllocationRecord]:
+        """The allocation and deallocation timeline."""
+
     def __init__(
         self,
         *,
         allocator_name: builtins.str | None = ...,
         total_bytes: builtins.int | None = ...,
         peak_bytes: builtins.int | None = ...,
         live_bytes: builtins.int | None = ...,
         allocation_records: collections.abc.Iterable[global___AllocationRecord] | None = ...,
         allocator_bytes_in_use: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocation_records", b"allocation_records", "allocator_bytes_in_use", b"allocator_bytes_in_use", "allocator_name", b"allocator_name", "live_bytes", b"live_bytes", "peak_bytes", b"peak_bytes", "total_bytes", b"total_bytes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allocation_records", b"allocation_records", "allocator_bytes_in_use", b"allocator_bytes_in_use", "allocator_name", b"allocator_name", "live_bytes", b"live_bytes", "peak_bytes", b"peak_bytes", "total_bytes", b"total_bytes"]) -> None: ...
 
 global___AllocatorMemoryUsed = AllocatorMemoryUsed
 
-@typing_extensions.final
+@typing.final
 class NodeOutput(google.protobuf.message.Message):
     """Output sizes recorded for a single execution of a graph node."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SLOT_FIELD_NUMBER: builtins.int
     TENSOR_DESCRIPTION_FIELD_NUMBER: builtins.int
@@ -86,54 +88,54 @@
     def tensor_description(self) -> tensorflow.core.framework.tensor_description_pb2.TensorDescription: ...
     def __init__(
         self,
         *,
         slot: builtins.int | None = ...,
         tensor_description: tensorflow.core.framework.tensor_description_pb2.TensorDescription | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_description", b"tensor_description"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["slot", b"slot", "tensor_description", b"tensor_description"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_description", b"tensor_description"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["slot", b"slot", "tensor_description", b"tensor_description"]) -> None: ...
 
 global___NodeOutput = NodeOutput
 
-@typing_extensions.final
+@typing.final
 class MemoryStats(google.protobuf.message.Message):
     """For memory tracking."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TEMP_MEMORY_SIZE_FIELD_NUMBER: builtins.int
     PERSISTENT_MEMORY_SIZE_FIELD_NUMBER: builtins.int
     PERSISTENT_TENSOR_ALLOC_IDS_FIELD_NUMBER: builtins.int
     DEVICE_TEMP_MEMORY_SIZE_FIELD_NUMBER: builtins.int
     DEVICE_PERSISTENT_MEMORY_SIZE_FIELD_NUMBER: builtins.int
     DEVICE_PERSISTENT_TENSOR_ALLOC_IDS_FIELD_NUMBER: builtins.int
     temp_memory_size: builtins.int
     persistent_memory_size: builtins.int
-    @property
-    def persistent_tensor_alloc_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     device_temp_memory_size: builtins.int
     device_persistent_memory_size: builtins.int
     @property
+    def persistent_tensor_alloc_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
     def device_persistent_tensor_alloc_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         temp_memory_size: builtins.int | None = ...,
         persistent_memory_size: builtins.int | None = ...,
         persistent_tensor_alloc_ids: collections.abc.Iterable[builtins.int] | None = ...,
         device_temp_memory_size: builtins.int | None = ...,
         device_persistent_memory_size: builtins.int | None = ...,
         device_persistent_tensor_alloc_ids: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_persistent_memory_size", b"device_persistent_memory_size", "device_persistent_tensor_alloc_ids", b"device_persistent_tensor_alloc_ids", "device_temp_memory_size", b"device_temp_memory_size", "persistent_memory_size", b"persistent_memory_size", "persistent_tensor_alloc_ids", b"persistent_tensor_alloc_ids", "temp_memory_size", b"temp_memory_size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device_persistent_memory_size", b"device_persistent_memory_size", "device_persistent_tensor_alloc_ids", b"device_persistent_tensor_alloc_ids", "device_temp_memory_size", b"device_temp_memory_size", "persistent_memory_size", b"persistent_memory_size", "persistent_tensor_alloc_ids", b"persistent_tensor_alloc_ids", "temp_memory_size", b"temp_memory_size"]) -> None: ...
 
 global___MemoryStats = MemoryStats
 
-@typing_extensions.final
+@typing.final
 class NodeExecStats(google.protobuf.message.Message):
     """Time/size stats recorded for a single execution of a graph node."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_NAME_FIELD_NUMBER: builtins.int
     ALL_START_MICROS_FIELD_NUMBER: builtins.int
@@ -158,30 +160,30 @@
     global id (cost_id?) for each node, or we should use a hash of
     the name.
     """
     all_start_micros: builtins.int
     op_start_rel_micros: builtins.int
     op_end_rel_micros: builtins.int
     all_end_rel_micros: builtins.int
-    @property
-    def memory(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AllocatorMemoryUsed]: ...
-    @property
-    def output(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NodeOutput]: ...
     timeline_label: builtins.str
     scheduled_micros: builtins.int
     thread_id: builtins.int
-    @property
-    def referenced_tensor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.allocation_description_pb2.AllocationDescription]: ...
-    @property
-    def memory_stats(self) -> global___MemoryStats: ...
     all_start_nanos: builtins.int
     op_start_rel_nanos: builtins.int
     op_end_rel_nanos: builtins.int
     all_end_rel_nanos: builtins.int
     scheduled_nanos: builtins.int
+    @property
+    def memory(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AllocatorMemoryUsed]: ...
+    @property
+    def output(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NodeOutput]: ...
+    @property
+    def referenced_tensor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.allocation_description_pb2.AllocationDescription]: ...
+    @property
+    def memory_stats(self) -> global___MemoryStats: ...
     def __init__(
         self,
         *,
         node_name: builtins.str | None = ...,
         all_start_micros: builtins.int | None = ...,
         op_start_rel_micros: builtins.int | None = ...,
         op_end_rel_micros: builtins.int | None = ...,
@@ -195,67 +197,68 @@
         memory_stats: global___MemoryStats | None = ...,
         all_start_nanos: builtins.int | None = ...,
         op_start_rel_nanos: builtins.int | None = ...,
         op_end_rel_nanos: builtins.int | None = ...,
         all_end_rel_nanos: builtins.int | None = ...,
         scheduled_nanos: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["memory_stats", b"memory_stats"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["all_end_rel_micros", b"all_end_rel_micros", "all_end_rel_nanos", b"all_end_rel_nanos", "all_start_micros", b"all_start_micros", "all_start_nanos", b"all_start_nanos", "memory", b"memory", "memory_stats", b"memory_stats", "node_name", b"node_name", "op_end_rel_micros", b"op_end_rel_micros", "op_end_rel_nanos", b"op_end_rel_nanos", "op_start_rel_micros", b"op_start_rel_micros", "op_start_rel_nanos", b"op_start_rel_nanos", "output", b"output", "referenced_tensor", b"referenced_tensor", "scheduled_micros", b"scheduled_micros", "scheduled_nanos", b"scheduled_nanos", "thread_id", b"thread_id", "timeline_label", b"timeline_label"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["memory_stats", b"memory_stats"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["all_end_rel_micros", b"all_end_rel_micros", "all_end_rel_nanos", b"all_end_rel_nanos", "all_start_micros", b"all_start_micros", "all_start_nanos", b"all_start_nanos", "memory", b"memory", "memory_stats", b"memory_stats", "node_name", b"node_name", "op_end_rel_micros", b"op_end_rel_micros", "op_end_rel_nanos", b"op_end_rel_nanos", "op_start_rel_micros", b"op_start_rel_micros", "op_start_rel_nanos", b"op_start_rel_nanos", "output", b"output", "referenced_tensor", b"referenced_tensor", "scheduled_micros", b"scheduled_micros", "scheduled_nanos", b"scheduled_nanos", "thread_id", b"thread_id", "timeline_label", b"timeline_label"]) -> None: ...
 
 global___NodeExecStats = NodeExecStats
 
-@typing_extensions.final
+@typing.final
 class DeviceStepStats(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ThreadNamesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     DEVICE_FIELD_NUMBER: builtins.int
     NODE_STATS_FIELD_NUMBER: builtins.int
     THREAD_NAMES_FIELD_NUMBER: builtins.int
     device: builtins.str
     @property
     def node_stats(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NodeExecStats]: ...
     @property
     def thread_names(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.str]:
         """Its key is thread id."""
+
     def __init__(
         self,
         *,
         device: builtins.str | None = ...,
         node_stats: collections.abc.Iterable[global___NodeExecStats] | None = ...,
         thread_names: collections.abc.Mapping[builtins.int, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "node_stats", b"node_stats", "thread_names", b"thread_names"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device", b"device", "node_stats", b"node_stats", "thread_names", b"thread_names"]) -> None: ...
 
 global___DeviceStepStats = DeviceStepStats
 
-@typing_extensions.final
+@typing.final
 class StepStats(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEV_STATS_FIELD_NUMBER: builtins.int
     @property
     def dev_stats(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeviceStepStats]: ...
     def __init__(
         self,
         *,
         dev_stats: collections.abc.Iterable[global___DeviceStepStats] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dev_stats", b"dev_stats"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dev_stats", b"dev_stats"]) -> None: ...
 
 global___StepStats = StepStats
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -65,15 +66,15 @@
 """
 DATA_CLASS_BLOB_SEQUENCE: DataClass.ValueType  # 3
 """Blob sequence time series. Each `Value` for the corresponding tag must
 have `tensor` set to a rank-1 tensor of bytestring dtype.
 """
 global___DataClass = DataClass
 
-@typing_extensions.final
+@typing.final
 class SummaryDescription(google.protobuf.message.Message):
     """Metadata associated with a series of Summary data"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_HINT_FIELD_NUMBER: builtins.int
     type_hint: builtins.str
@@ -81,27 +82,27 @@
     Supported values include "scalar", "histogram", "image", "audio"
     """
     def __init__(
         self,
         *,
         type_hint: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["type_hint", b"type_hint"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["type_hint", b"type_hint"]) -> None: ...
 
 global___SummaryDescription = SummaryDescription
 
-@typing_extensions.final
+@typing.final
 class SummaryMetadata(google.protobuf.message.Message):
     """A SummaryMetadata encapsulates information on which plugins are able to make
     use of a certain summary value.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class PluginData(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PLUGIN_NAME_FIELD_NUMBER: builtins.int
         CONTENT_FIELD_NUMBER: builtins.int
         plugin_name: builtins.str
         """The name of the plugin this data pertains to."""
@@ -111,59 +112,60 @@
         """
         def __init__(
             self,
             *,
             plugin_name: builtins.str | None = ...,
             content: builtins.bytes | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["content", b"content", "plugin_name", b"plugin_name"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["content", b"content", "plugin_name", b"plugin_name"]) -> None: ...
 
     PLUGIN_DATA_FIELD_NUMBER: builtins.int
     DISPLAY_NAME_FIELD_NUMBER: builtins.int
     SUMMARY_DESCRIPTION_FIELD_NUMBER: builtins.int
     DATA_CLASS_FIELD_NUMBER: builtins.int
-    @property
-    def plugin_data(self) -> global___SummaryMetadata.PluginData:
-        """Data that associates a summary with a certain plugin."""
     display_name: builtins.str
     """Display name for viewing in TensorBoard."""
     summary_description: builtins.str
     """Longform readable description of the summary sequence. Markdown supported."""
     data_class: global___DataClass.ValueType
     """Class of data stored in this time series. Required for compatibility with
     TensorBoard's generic data facilities (`DataProvider`, et al.). This value
     imposes constraints on the dtype and shape of the corresponding tensor
     values. See `DataClass` docs for details.
     """
+    @property
+    def plugin_data(self) -> global___SummaryMetadata.PluginData:
+        """Data that associates a summary with a certain plugin."""
+
     def __init__(
         self,
         *,
         plugin_data: global___SummaryMetadata.PluginData | None = ...,
         display_name: builtins.str | None = ...,
         summary_description: builtins.str | None = ...,
         data_class: global___DataClass.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["plugin_data", b"plugin_data"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data_class", b"data_class", "display_name", b"display_name", "plugin_data", b"plugin_data", "summary_description", b"summary_description"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["plugin_data", b"plugin_data"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data_class", b"data_class", "display_name", b"display_name", "plugin_data", b"plugin_data", "summary_description", b"summary_description"]) -> None: ...
 
 global___SummaryMetadata = SummaryMetadata
 
-@typing_extensions.final
+@typing.final
 class Summary(google.protobuf.message.Message):
     """A Summary is a set of named values to be displayed by the
     visualizer.
 
     Summaries are produced regularly during training, as controlled by
     the "summary_interval_secs" attribute of the training operation.
     Summaries are also produced at the end of an evaluation.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Image(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         HEIGHT_FIELD_NUMBER: builtins.int
         WIDTH_FIELD_NUMBER: builtins.int
         COLORSPACE_FIELD_NUMBER: builtins.int
         ENCODED_IMAGE_STRING_FIELD_NUMBER: builtins.int
@@ -187,17 +189,17 @@
             self,
             *,
             height: builtins.int | None = ...,
             width: builtins.int | None = ...,
             colorspace: builtins.int | None = ...,
             encoded_image_string: builtins.bytes | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["colorspace", b"colorspace", "encoded_image_string", b"encoded_image_string", "height", b"height", "width", b"width"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["colorspace", b"colorspace", "encoded_image_string", b"encoded_image_string", "height", b"height", "width", b"width"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Audio(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         SAMPLE_RATE_FIELD_NUMBER: builtins.int
         NUM_CHANNELS_FIELD_NUMBER: builtins.int
         LENGTH_FRAMES_FIELD_NUMBER: builtins.int
         ENCODED_AUDIO_STRING_FIELD_NUMBER: builtins.int
@@ -218,17 +220,17 @@
             *,
             sample_rate: builtins.float | None = ...,
             num_channels: builtins.int | None = ...,
             length_frames: builtins.int | None = ...,
             encoded_audio_string: builtins.bytes | None = ...,
             content_type: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["content_type", b"content_type", "encoded_audio_string", b"encoded_audio_string", "length_frames", b"length_frames", "num_channels", b"num_channels", "sample_rate", b"sample_rate"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["content_type", b"content_type", "encoded_audio_string", b"encoded_audio_string", "length_frames", b"length_frames", "num_channels", b"num_channels", "sample_rate", b"sample_rate"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Value(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NODE_NAME_FIELD_NUMBER: builtins.int
         TAG_FIELD_NUMBER: builtins.int
         METADATA_FIELD_NUMBER: builtins.int
         SIMPLE_VALUE_FIELD_NUMBER: builtins.int
@@ -240,24 +242,25 @@
         node_name: builtins.str
         """This field is deprecated and will not be set."""
         tag: builtins.str
         """Tag name for the data. Used by TensorBoard plugins to organize data. Tags
         are often organized by scope (which contains slashes to convey
         hierarchy). For example: foo/bar/0
         """
+        simple_value: builtins.float
+        obsolete_old_style_histogram: builtins.bytes
         @property
         def metadata(self) -> global___SummaryMetadata:
             """Contains metadata on the summary value such as which plugins may use it.
             Take note that many summary values may lack a metadata field. This is
             because the FileWriter only keeps a metadata object on the first summary
             value with a certain tag for each tag. TensorBoard then remembers which
             tags are associated with which plugins. This saves space.
             """
-        simple_value: builtins.float
-        obsolete_old_style_histogram: builtins.bytes
+
         @property
         def image(self) -> global___Summary.Image: ...
         @property
         def histo(self) -> tensorflow.tsl.protobuf.histogram_pb2.HistogramProto: ...
         @property
         def audio(self) -> global___Summary.Audio: ...
         @property
@@ -271,23 +274,24 @@
             simple_value: builtins.float | None = ...,
             obsolete_old_style_histogram: builtins.bytes | None = ...,
             image: global___Summary.Image | None = ...,
             histo: tensorflow.tsl.protobuf.histogram_pb2.HistogramProto | None = ...,
             audio: global___Summary.Audio | None = ...,
             tensor: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["audio", b"audio", "histo", b"histo", "image", b"image", "metadata", b"metadata", "obsolete_old_style_histogram", b"obsolete_old_style_histogram", "simple_value", b"simple_value", "tensor", b"tensor", "value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["audio", b"audio", "histo", b"histo", "image", b"image", "metadata", b"metadata", "node_name", b"node_name", "obsolete_old_style_histogram", b"obsolete_old_style_histogram", "simple_value", b"simple_value", "tag", b"tag", "tensor", b"tensor", "value", b"value"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["value", b"value"]) -> typing_extensions.Literal["simple_value", "obsolete_old_style_histogram", "image", "histo", "audio", "tensor"] | None: ...
+        def HasField(self, field_name: typing.Literal["audio", b"audio", "histo", b"histo", "image", b"image", "metadata", b"metadata", "obsolete_old_style_histogram", b"obsolete_old_style_histogram", "simple_value", b"simple_value", "tensor", b"tensor", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["audio", b"audio", "histo", b"histo", "image", b"image", "metadata", b"metadata", "node_name", b"node_name", "obsolete_old_style_histogram", b"obsolete_old_style_histogram", "simple_value", b"simple_value", "tag", b"tag", "tensor", b"tensor", "value", b"value"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing.Literal["value", b"value"]) -> typing.Literal["simple_value", "obsolete_old_style_histogram", "image", "histo", "audio", "tensor"] | None: ...
 
     VALUE_FIELD_NUMBER: builtins.int
     @property
     def value(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Summary.Value]:
         """Set of values for the summary."""
+
     def __init__(
         self,
         *,
         value: collections.abc.Iterable[global___Summary.Value] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
 global___Summary = Summary
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.framework.allocation_description_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TensorDescription(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     ALLOCATION_DESCRIPTION_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     """Data type of tensor elements"""
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """Shape of the tensor."""
+
     @property
     def allocation_description(self) -> tensorflow.core.framework.allocation_description_pb2.AllocationDescription:
         """Information about the size and allocator used for the data"""
+
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         allocation_description: tensorflow.core.framework.allocation_description_pb2.AllocationDescription | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["allocation_description", b"allocation_description", "shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocation_description", b"allocation_description", "dtype", b"dtype", "shape", b"shape"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["allocation_description", b"allocation_description", "shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allocation_description", b"allocation_description", "dtype", b"dtype", "shape", b"shape"]) -> None: ...
 
 global___TensorDescription = TensorDescription
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.resource_handle_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TensorProto(google.protobuf.message.Message):
     """Protocol buffer representing a tensor."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     TENSOR_SHAPE_FIELD_NUMBER: builtins.int
@@ -36,17 +37,14 @@
     DCOMPLEX_VAL_FIELD_NUMBER: builtins.int
     RESOURCE_HANDLE_VAL_FIELD_NUMBER: builtins.int
     VARIANT_VAL_FIELD_NUMBER: builtins.int
     UINT32_VAL_FIELD_NUMBER: builtins.int
     UINT64_VAL_FIELD_NUMBER: builtins.int
     FLOAT8_VAL_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
-    @property
-    def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
-        """Shape of the tensor.  TODO(touts): sort out the 0-rank issues."""
     version_number: builtins.int
     """Only one of the representations below is set, one of "tensor_contents" and
     the "xxx_val" attributes.  We are not using oneof because as oneofs cannot
     contain repeated fields it would require another extra set of messages.
 
     Version number.
 
@@ -57,68 +55,85 @@
     tensor_content: builtins.bytes
     """Serialized raw tensor content from either Tensor::AsProtoTensorContent or
     memcpy in tensorflow::grpc::EncodeTensorToByteBuffer. This representation
     can be used for all tensor types. The purpose of this representation is to
     reduce serialization overhead during RPC call by avoiding serialization of
     many repeated small items.
     """
+    float8_val: builtins.bytes
+    """DT_FLOAT8_*, use variable-sized set of bytes
+    (i.e. the equivalent of repeated uint8, if such a thing existed).
+    """
+    @property
+    def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
+        """Shape of the tensor.  TODO(touts): sort out the 0-rank issues."""
+
     @property
     def half_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Type specific representations that make it easy to create tensor protos in
         all languages.  Only the representation corresponding to "dtype" can
         be set.  The values hold the flattened representation of the tensor in
         row major order.
 
         DT_HALF, DT_BFLOAT16. Note that since protobuf has no int16 type, we'll
         have some pointless zero padding for each value here.
         """
+
     @property
     def float_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """DT_FLOAT."""
+
     @property
     def double_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """DT_DOUBLE."""
+
     @property
     def int_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """DT_INT32, DT_INT16, DT_UINT16, DT_INT8, DT_UINT8."""
+
     @property
     def string_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]:
         """DT_STRING"""
+
     @property
     def scomplex_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """DT_COMPLEX64. scomplex_val(2*i) and scomplex_val(2*i+1) are real
         and imaginary parts of i-th single precision complex.
         """
+
     @property
     def int64_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """DT_INT64"""
+
     @property
     def bool_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bool]:
         """DT_BOOL"""
+
     @property
     def dcomplex_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """DT_COMPLEX128. dcomplex_val(2*i) and dcomplex_val(2*i+1) are real
         and imaginary parts of i-th double precision complex.
         """
+
     @property
     def resource_handle_val(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.resource_handle_pb2.ResourceHandleProto]:
         """DT_RESOURCE"""
+
     @property
     def variant_val(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___VariantTensorDataProto]:
         """DT_VARIANT"""
+
     @property
     def uint32_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """DT_UINT32"""
+
     @property
     def uint64_val(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """DT_UINT64"""
-    float8_val: builtins.bytes
-    """DT_FLOAT8_*, use variable-sized set of bytes
-    (i.e. the equivalent of repeated uint8, if such a thing existed).
-    """
+
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         tensor_shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         version_number: builtins.int | None = ...,
         tensor_content: builtins.bytes | None = ...,
@@ -133,20 +148,20 @@
         dcomplex_val: collections.abc.Iterable[builtins.float] | None = ...,
         resource_handle_val: collections.abc.Iterable[tensorflow.core.framework.resource_handle_pb2.ResourceHandleProto] | None = ...,
         variant_val: collections.abc.Iterable[global___VariantTensorDataProto] | None = ...,
         uint32_val: collections.abc.Iterable[builtins.int] | None = ...,
         uint64_val: collections.abc.Iterable[builtins.int] | None = ...,
         float8_val: builtins.bytes | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bool_val", b"bool_val", "dcomplex_val", b"dcomplex_val", "double_val", b"double_val", "dtype", b"dtype", "float8_val", b"float8_val", "float_val", b"float_val", "half_val", b"half_val", "int64_val", b"int64_val", "int_val", b"int_val", "resource_handle_val", b"resource_handle_val", "scomplex_val", b"scomplex_val", "string_val", b"string_val", "tensor_content", b"tensor_content", "tensor_shape", b"tensor_shape", "uint32_val", b"uint32_val", "uint64_val", b"uint64_val", "variant_val", b"variant_val", "version_number", b"version_number"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bool_val", b"bool_val", "dcomplex_val", b"dcomplex_val", "double_val", b"double_val", "dtype", b"dtype", "float8_val", b"float8_val", "float_val", b"float_val", "half_val", b"half_val", "int64_val", b"int64_val", "int_val", b"int_val", "resource_handle_val", b"resource_handle_val", "scomplex_val", b"scomplex_val", "string_val", b"string_val", "tensor_content", b"tensor_content", "tensor_shape", b"tensor_shape", "uint32_val", b"uint32_val", "uint64_val", b"uint64_val", "variant_val", b"variant_val", "version_number", b"version_number"]) -> None: ...
 
 global___TensorProto = TensorProto
 
-@typing_extensions.final
+@typing.final
 class VariantTensorDataProto(google.protobuf.message.Message):
     """Protocol buffer representing the serialization format of DT_VARIANT tensors."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_NAME_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
@@ -154,17 +169,18 @@
     type_name: builtins.str
     """Name of the type of objects being serialized."""
     metadata: builtins.bytes
     """Portions of the object that are not Tensors."""
     @property
     def tensors(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorProto]:
         """Tensors contained within objects being serialized."""
+
     def __init__(
         self,
         *,
         type_name: builtins.str | None = ...,
         metadata: builtins.bytes | None = ...,
         tensors: collections.abc.Iterable[global___TensorProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["metadata", b"metadata", "tensors", b"tensors", "type_name", b"type_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["metadata", b"metadata", "tensors", b"tensors", "type_name", b"type_name"]) -> None: ...
 
 global___VariantTensorDataProto = VariantTensorDataProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol buffer representing the shape of tensors."""
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TensorShapeProto(google.protobuf.message.Message):
     """Dimensions of a tensor."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Dim(google.protobuf.message.Message):
         """One dimension of the tensor."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         SIZE_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
@@ -37,18 +38,23 @@
         """Optional name of the tensor dimension."""
         def __init__(
             self,
             *,
             size: builtins.int | None = ...,
             name: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "size", b"size"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["name", b"name", "size", b"size"]) -> None: ...
 
     DIM_FIELD_NUMBER: builtins.int
     UNKNOWN_RANK_FIELD_NUMBER: builtins.int
+    unknown_rank: builtins.bool
+    """If true, the number of dimensions in the shape is unknown.
+
+    If true, "dim.size()" must be 0.
+    """
     @property
     def dim(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorShapeProto.Dim]:
         """Dimensions of the tensor, such as {"input", 30}, {"output", 40}
         for a 30 x 40 2D tensor.  If an entry has size -1, this
         corresponds to a dimension of unknown size. The names are
         optional.
 
@@ -57,21 +63,17 @@
 
         The first entry in "dim" is the outermost dimension used to layout the
         values, the last entry is the innermost dimension.  This matches the
         in-memory layout of RowMajor Eigen tensors.
 
         If "dim.size()" > 0, "unknown_rank" must be false.
         """
-    unknown_rank: builtins.bool
-    """If true, the number of dimensions in the shape is unknown.
 
-    If true, "dim.size()" must be 0.
-    """
     def __init__(
         self,
         *,
         dim: collections.abc.Iterable[global___TensorShapeProto.Dim] | None = ...,
         unknown_rank: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dim", b"dim", "unknown_rank", b"unknown_rank"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["dim", b"dim", "unknown_rank", b"unknown_rank"]) -> None: ...
 
 global___TensorShapeProto = TensorShapeProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol buffer representing slices of a tensor"""
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TensorSliceProto(google.protobuf.message.Message):
     """Can only be interpreted if you know the corresponding TensorShape."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Extent(google.protobuf.message.Message):
         """Extent of the slice in one dimension.
         Either both or no attributes must be set.  When no attribute is set
         means: All data in that dimension.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -34,28 +35,29 @@
         length: builtins.int
         def __init__(
             self,
             *,
             start: builtins.int | None = ...,
             length: builtins.int | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["has_length", b"has_length", "length", b"length"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["has_length", b"has_length", "length", b"length", "start", b"start"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["has_length", b"has_length"]) -> typing_extensions.Literal["length"] | None: ...
+        def HasField(self, field_name: typing.Literal["has_length", b"has_length", "length", b"length"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["has_length", b"has_length", "length", b"length", "start", b"start"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing.Literal["has_length", b"has_length"]) -> typing.Literal["length"] | None: ...
 
     EXTENT_FIELD_NUMBER: builtins.int
     @property
     def extent(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorSliceProto.Extent]:
         """Extent of the slice in all tensor dimensions.
 
         Must have one entry for each of the dimension of the tensor that this
         slice belongs to.  The order of sizes is the same as the order of
         dimensions in the TensorShape.
         """
+
     def __init__(
         self,
         *,
         extent: collections.abc.Iterable[global___TensorSliceProto.Extent] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extent", b"extent"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["extent", b"extent"]) -> None: ...
 
 global___TensorSliceProto = TensorSliceProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -173,23 +174,23 @@
 DT_VARIANT_REF: DataType.ValueType  # 121
 DT_UINT32_REF: DataType.ValueType  # 122
 DT_UINT64_REF: DataType.ValueType  # 123
 DT_FLOAT8_E5M2_REF: DataType.ValueType  # 124
 DT_FLOAT8_E4M3FN_REF: DataType.ValueType  # 125
 global___DataType = DataType
 
-@typing_extensions.final
+@typing.final
 class SerializedDType(google.protobuf.message.Message):
     """Represents a serialized tf.dtypes.Dtype"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATATYPE_FIELD_NUMBER: builtins.int
     datatype: global___DataType.ValueType
     def __init__(
         self,
         *,
         datatype: global___DataType.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["datatype", b"datatype"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["datatype", b"datatype"]) -> None: ...
 
 global___SerializedDType = SerializedDType
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -105,15 +106,15 @@
 VARIABLE_AGGREGATION_ONLY_FIRST_REPLICA: VariableAggregation.ValueType  # 3
 """`ONLY_FIRST_REPLICA`: This is for when every replica is performing the same
 update, but we only want to perform the update once. Used, e.g., for the
 global step counter.
 """
 global___VariableAggregation = VariableAggregation
 
-@typing_extensions.final
+@typing.final
 class VariableDef(google.protobuf.message.Message):
     """Protocol buffer representing a Variable."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VARIABLE_NAME_FIELD_NUMBER: builtins.int
     INITIAL_VALUE_NAME_FIELD_NUMBER: builtins.int
@@ -128,66 +129,70 @@
     """Name of the variable tensor."""
     initial_value_name: builtins.str
     """Name of the tensor holding the variable's initial value."""
     initializer_name: builtins.str
     """Name of the initializer op."""
     snapshot_name: builtins.str
     """Name of the snapshot tensor."""
-    @property
-    def save_slice_info_def(self) -> global___SaveSliceInfoDef:
-        """Support for saving variables as slices of a larger variable."""
     is_resource: builtins.bool
     """Whether to represent this as a ResourceVariable."""
     trainable: builtins.bool
     """Whether this variable should be trained."""
     synchronization: global___VariableSynchronization.ValueType
     """Indicates when a distributed variable will be synced."""
     aggregation: global___VariableAggregation.ValueType
     """Indicates how a distributed variable will be aggregated."""
+    @property
+    def save_slice_info_def(self) -> global___SaveSliceInfoDef:
+        """Support for saving variables as slices of a larger variable."""
+
     def __init__(
         self,
         *,
         variable_name: builtins.str | None = ...,
         initial_value_name: builtins.str | None = ...,
         initializer_name: builtins.str | None = ...,
         snapshot_name: builtins.str | None = ...,
         save_slice_info_def: global___SaveSliceInfoDef | None = ...,
         is_resource: builtins.bool | None = ...,
         trainable: builtins.bool | None = ...,
         synchronization: global___VariableSynchronization.ValueType | None = ...,
         aggregation: global___VariableAggregation.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["save_slice_info_def", b"save_slice_info_def"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aggregation", b"aggregation", "initial_value_name", b"initial_value_name", "initializer_name", b"initializer_name", "is_resource", b"is_resource", "save_slice_info_def", b"save_slice_info_def", "snapshot_name", b"snapshot_name", "synchronization", b"synchronization", "trainable", b"trainable", "variable_name", b"variable_name"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["save_slice_info_def", b"save_slice_info_def"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["aggregation", b"aggregation", "initial_value_name", b"initial_value_name", "initializer_name", b"initializer_name", "is_resource", b"is_resource", "save_slice_info_def", b"save_slice_info_def", "snapshot_name", b"snapshot_name", "synchronization", b"synchronization", "trainable", b"trainable", "variable_name", b"variable_name"]) -> None: ...
 
 global___VariableDef = VariableDef
 
-@typing_extensions.final
+@typing.final
 class SaveSliceInfoDef(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FULL_NAME_FIELD_NUMBER: builtins.int
     FULL_SHAPE_FIELD_NUMBER: builtins.int
     VAR_OFFSET_FIELD_NUMBER: builtins.int
     VAR_SHAPE_FIELD_NUMBER: builtins.int
     full_name: builtins.str
     """Name of the full variable of which this is a slice."""
     @property
     def full_shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Shape of the full variable."""
+
     @property
     def var_offset(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Offset of this variable into the full variable."""
+
     @property
     def var_shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Shape of this variable."""
+
     def __init__(
         self,
         *,
         full_name: builtins.str | None = ...,
         full_shape: collections.abc.Iterable[builtins.int] | None = ...,
         var_offset: collections.abc.Iterable[builtins.int] | None = ...,
         var_shape: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["full_name", b"full_name", "full_shape", b"full_shape", "var_offset", b"var_offset", "var_shape", b"var_shape"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["full_name", b"full_name", "full_shape", b"full_shape", "var_offset", b"var_offset", "var_shape", b"var_shape"]) -> None: ...
 
 global___SaveSliceInfoDef = SaveSliceInfoDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class VersionDef(google.protobuf.message.Message):
     """Version information for a piece of serialized data
 
     There are different types of versions for each type of data
     (GraphDef, etc.), but they all have the same common shape
     described here.
 
@@ -36,17 +37,18 @@
     producer: builtins.int
     """The version of the code that produced this data."""
     min_consumer: builtins.int
     """Any consumer below this version is not allowed to consume this data."""
     @property
     def bad_consumers(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Specific consumer versions which are disallowed (e.g. due to bugs)."""
+
     def __init__(
         self,
         *,
         producer: builtins.int | None = ...,
         min_consumer: builtins.int | None = ...,
         bad_consumers: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bad_consumers", b"bad_consumers", "min_consumer", b"min_consumer", "producer", b"producer"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bad_consumers", b"bad_consumers", "min_consumer", b"min_consumer", "producer", b"producer"]) -> None: ...
 
 global___VersionDef = VersionDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class JobDef(google.protobuf.message.Message):
     """This file contains protos to be used when defining a TensorFlow
     cluster.
 
     EXAMPLES
     --------
 
@@ -70,63 +71,65 @@
          cluster { $CLUSTER } job_name: 'ps'     task_index: 1
 
     Defines a single job in a TensorFlow cluster.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class TasksEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     TASKS_FIELD_NUMBER: builtins.int
     name: builtins.str
     """The name of this job."""
     @property
     def tasks(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.str]:
         """Mapping from task ID to "hostname:port" string.
 
         If the `name` field contains "worker", and the `tasks` map contains a
         mapping from 7 to "example.org:2222", then the device prefix
         "/job:worker/task:7" will be assigned to "example.org:2222".
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         tasks: collections.abc.Mapping[builtins.int, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "tasks", b"tasks"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "tasks", b"tasks"]) -> None: ...
 
 global___JobDef = JobDef
 
-@typing_extensions.final
+@typing.final
 class ClusterDef(google.protobuf.message.Message):
     """Defines a TensorFlow cluster as a set of jobs."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_FIELD_NUMBER: builtins.int
     @property
     def job(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___JobDef]:
         """The jobs that comprise the cluster."""
+
     def __init__(
         self,
         *,
         job: collections.abc.Iterable[global___JobDef] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job", b"job"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["job", b"job"]) -> None: ...
 
 global___ClusterDef = ClusterDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.protobuf.struct_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CompositeTensorVariantMetadata(google.protobuf.message.Message):
     """Metadata for CompositeTensorVariant, used when serializing as Variant.
 
     We define a new message here (rather than directly using TypeSpecProto for
     the metadata string) to retain flexibility to change the metadata encoding
     to support additional features.
     """
@@ -26,11 +27,11 @@
     @property
     def type_spec_proto(self) -> tensorflow.core.protobuf.struct_pb2.TypeSpecProto: ...
     def __init__(
         self,
         *,
         type_spec_proto: tensorflow.core.protobuf.struct_pb2.TypeSpecProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["type_spec_proto", b"type_spec_proto"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["type_spec_proto", b"type_spec_proto"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["type_spec_proto", b"type_spec_proto"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["type_spec_proto", b"type_spec_proto"]) -> None: ...
 
 global___CompositeTensorVariantMetadata = CompositeTensorVariantMetadata
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -23,23 +24,23 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GPUOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Experimental(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class VirtualDevices(google.protobuf.message.Message):
             """Configuration for breaking down a visible GPU into multiple "virtual"
             devices.
             """
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -53,97 +54,59 @@
                 corresponding visible GPU (see "virtual_devices" below).
                 If empty, it will create single virtual device taking all available
                 memory from the device.
 
                 For the concept of "visible" and "virtual" GPU, see the comments for
                 "visible_device_list" above for more information.
                 """
+
             @property
             def priority(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
                 """Priority values to use with the virtual devices. Use the cuda function
                 cudaDeviceGetStreamPriorityRange to query for valid range of values for
                 priority.
 
                 On a P4000 GPU with cuda 10.1, the priority range reported was 0 for
                 least priority and -1 for greatest priority.
 
                 If this field is not specified, then the virtual devices will be
                 created with the default. If this field has values set, then the size
                 of this must match with the above memory_limit_mb.
                 """
+
             @property
             def device_ordinal(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
                 """Virtual Device ordinal number determines the device ID of the device.
                 A Virtual device with a lower ordinal number always receives the a
                 smaller device id. The phyiscal device id and location in the
                 virtual device list is used to break ties.
                 """
+
             def __init__(
                 self,
                 *,
                 memory_limit_mb: collections.abc.Iterable[builtins.float] | None = ...,
                 priority: collections.abc.Iterable[builtins.int] | None = ...,
                 device_ordinal: collections.abc.Iterable[builtins.int] | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["device_ordinal", b"device_ordinal", "memory_limit_mb", b"memory_limit_mb", "priority", b"priority"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["device_ordinal", b"device_ordinal", "memory_limit_mb", b"memory_limit_mb", "priority", b"priority"]) -> None: ...
 
         VIRTUAL_DEVICES_FIELD_NUMBER: builtins.int
         USE_UNIFIED_MEMORY_FIELD_NUMBER: builtins.int
         NUM_DEV_TO_DEV_COPY_STREAMS_FIELD_NUMBER: builtins.int
         COLLECTIVE_RING_ORDER_FIELD_NUMBER: builtins.int
         TIMESTAMPED_ALLOCATOR_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_INTERVAL_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_BYTES_FIELD_NUMBER: builtins.int
         KERNEL_TRACKER_MAX_PENDING_FIELD_NUMBER: builtins.int
         INTERNAL_FRAGMENTATION_FRACTION_FIELD_NUMBER: builtins.int
         USE_CUDA_MALLOC_ASYNC_FIELD_NUMBER: builtins.int
         DISALLOW_RETRY_ON_ALLOCATION_FAILURE_FIELD_NUMBER: builtins.int
         GPU_HOST_MEM_LIMIT_IN_MB_FIELD_NUMBER: builtins.int
         GPU_HOST_MEM_DISALLOW_GROWTH_FIELD_NUMBER: builtins.int
-        @property
-        def virtual_devices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GPUOptions.Experimental.VirtualDevices]:
-            """The multi virtual device settings. If empty (not set), it will create
-            single virtual device on each visible GPU, according to the settings
-            in "visible_device_list" above. Otherwise, the number of elements in the
-            list must be the same as the number of visible GPUs (after
-            "visible_device_list" filtering if it is set), and the string represented
-            device names (e.g. /device:GPU:<id>) will refer to the virtual
-            devices and have the <id> field assigned sequentially starting from 0,
-            according to the order of the virtual devices determined by
-            device_ordinal and the location in the virtual device list.
-
-            For example,
-              visible_device_list = "1,0"
-              virtual_devices { memory_limit: 1GB memory_limit: 2GB }
-              virtual_devices { memory_limit: 3GB memory_limit: 4GB }
-            will create 4 virtual devices as:
-              /device:GPU:0 -> visible GPU 1 with 1GB memory
-              /device:GPU:1 -> visible GPU 1 with 2GB memory
-              /device:GPU:2 -> visible GPU 0 with 3GB memory
-              /device:GPU:3 -> visible GPU 0 with 4GB memory
-
-            but
-              visible_device_list = "1,0"
-              virtual_devices { memory_limit: 1GB memory_limit: 2GB
-                                device_ordinal: 10 device_ordinal: 20}
-              virtual_devices { memory_limit: 3GB memory_limit: 4GB
-                                device_ordinal: 10 device_ordinal: 20}
-            will create 4 virtual devices as:
-              /device:GPU:0 -> visible GPU 1 with 1GB memory  (ordinal 10)
-              /device:GPU:1 -> visible GPU 0 with 3GB memory  (ordinal 10)
-              /device:GPU:2 -> visible GPU 1 with 2GB memory  (ordinal 20)
-              /device:GPU:3 -> visible GPU 0 with 4GB memory  (ordinal 20)
-
-            NOTE:
-            1. It's invalid to set both this and "per_process_gpu_memory_fraction"
-               at the same time.
-            2. Currently this setting is per-process, not per-session. Using
-               different settings in different sessions within same process will
-               result in undefined behavior.
-            """
         use_unified_memory: builtins.bool
         """If true, uses CUDA unified memory for memory allocations. If
         per_process_gpu_memory_fraction option is greater than 1.0, then unified
         memory is used regardless of the value for this field. See comments for
         per_process_gpu_memory_fraction field for more details and requirements
         of the unified memory. This option is useful to oversubscribe memory if
         multiple processes are sharing a single GPU while individually using less
@@ -218,14 +181,56 @@
         never grows.  This can be useful for latency-sensitive systems, because
         growing the GPU host memory pool can be expensive.
 
         You probably only want to use this in combination with
         gpu_host_mem_limit_in_mb, because the default GPU host memory limit is
         quite high.
         """
+        @property
+        def virtual_devices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GPUOptions.Experimental.VirtualDevices]:
+            """The multi virtual device settings. If empty (not set), it will create
+            single virtual device on each visible GPU, according to the settings
+            in "visible_device_list" above. Otherwise, the number of elements in the
+            list must be the same as the number of visible GPUs (after
+            "visible_device_list" filtering if it is set), and the string represented
+            device names (e.g. /device:GPU:<id>) will refer to the virtual
+            devices and have the <id> field assigned sequentially starting from 0,
+            according to the order of the virtual devices determined by
+            device_ordinal and the location in the virtual device list.
+
+            For example,
+              visible_device_list = "1,0"
+              virtual_devices { memory_limit: 1GB memory_limit: 2GB }
+              virtual_devices { memory_limit: 3GB memory_limit: 4GB }
+            will create 4 virtual devices as:
+              /device:GPU:0 -> visible GPU 1 with 1GB memory
+              /device:GPU:1 -> visible GPU 1 with 2GB memory
+              /device:GPU:2 -> visible GPU 0 with 3GB memory
+              /device:GPU:3 -> visible GPU 0 with 4GB memory
+
+            but
+              visible_device_list = "1,0"
+              virtual_devices { memory_limit: 1GB memory_limit: 2GB
+                                device_ordinal: 10 device_ordinal: 20}
+              virtual_devices { memory_limit: 3GB memory_limit: 4GB
+                                device_ordinal: 10 device_ordinal: 20}
+            will create 4 virtual devices as:
+              /device:GPU:0 -> visible GPU 1 with 1GB memory  (ordinal 10)
+              /device:GPU:1 -> visible GPU 0 with 3GB memory  (ordinal 10)
+              /device:GPU:2 -> visible GPU 1 with 2GB memory  (ordinal 20)
+              /device:GPU:3 -> visible GPU 0 with 4GB memory  (ordinal 20)
+
+            NOTE:
+            1. It's invalid to set both this and "per_process_gpu_memory_fraction"
+               at the same time.
+            2. Currently this setting is per-process, not per-session. Using
+               different settings in different sessions within same process will
+               result in undefined behavior.
+            """
+
         def __init__(
             self,
             *,
             virtual_devices: collections.abc.Iterable[global___GPUOptions.Experimental.VirtualDevices] | None = ...,
             use_unified_memory: builtins.bool | None = ...,
             num_dev_to_dev_copy_streams: builtins.int | None = ...,
             collective_ring_order: builtins.str | None = ...,
@@ -235,15 +240,15 @@
             kernel_tracker_max_pending: builtins.int | None = ...,
             internal_fragmentation_fraction: builtins.float | None = ...,
             use_cuda_malloc_async: builtins.bool | None = ...,
             disallow_retry_on_allocation_failure: builtins.bool | None = ...,
             gpu_host_mem_limit_in_mb: builtins.float | None = ...,
             gpu_host_mem_disallow_growth: builtins.bool | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["collective_ring_order", b"collective_ring_order", "disallow_retry_on_allocation_failure", b"disallow_retry_on_allocation_failure", "gpu_host_mem_disallow_growth", b"gpu_host_mem_disallow_growth", "gpu_host_mem_limit_in_mb", b"gpu_host_mem_limit_in_mb", "internal_fragmentation_fraction", b"internal_fragmentation_fraction", "kernel_tracker_max_bytes", b"kernel_tracker_max_bytes", "kernel_tracker_max_interval", b"kernel_tracker_max_interval", "kernel_tracker_max_pending", b"kernel_tracker_max_pending", "num_dev_to_dev_copy_streams", b"num_dev_to_dev_copy_streams", "timestamped_allocator", b"timestamped_allocator", "use_cuda_malloc_async", b"use_cuda_malloc_async", "use_unified_memory", b"use_unified_memory", "virtual_devices", b"virtual_devices"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["collective_ring_order", b"collective_ring_order", "disallow_retry_on_allocation_failure", b"disallow_retry_on_allocation_failure", "gpu_host_mem_disallow_growth", b"gpu_host_mem_disallow_growth", "gpu_host_mem_limit_in_mb", b"gpu_host_mem_limit_in_mb", "internal_fragmentation_fraction", b"internal_fragmentation_fraction", "kernel_tracker_max_bytes", b"kernel_tracker_max_bytes", "kernel_tracker_max_interval", b"kernel_tracker_max_interval", "kernel_tracker_max_pending", b"kernel_tracker_max_pending", "num_dev_to_dev_copy_streams", b"num_dev_to_dev_copy_streams", "timestamped_allocator", b"timestamped_allocator", "use_cuda_malloc_async", b"use_cuda_malloc_async", "use_unified_memory", b"use_unified_memory", "virtual_devices", b"virtual_devices"]) -> None: ...
 
     PER_PROCESS_GPU_MEMORY_FRACTION_FIELD_NUMBER: builtins.int
     ALLOW_GROWTH_FIELD_NUMBER: builtins.int
     ALLOCATOR_TYPE_FIELD_NUMBER: builtins.int
     DEFERRED_DELETION_BYTES_FIELD_NUMBER: builtins.int
     VISIBLE_DEVICE_LIST_FIELD_NUMBER: builtins.int
     POLLING_ACTIVE_DELAY_USECS_FIELD_NUMBER: builtins.int
@@ -332,33 +337,34 @@
     """
     @property
     def experimental(self) -> global___GPUOptions.Experimental:
         """Everything inside experimental is subject to change and is not subject
         to API stability guarantees in
         https://www.tensorflow.org/guide/version_compat.
         """
+
     def __init__(
         self,
         *,
         per_process_gpu_memory_fraction: builtins.float | None = ...,
         allow_growth: builtins.bool | None = ...,
         allocator_type: builtins.str | None = ...,
         deferred_deletion_bytes: builtins.int | None = ...,
         visible_device_list: builtins.str | None = ...,
         polling_active_delay_usecs: builtins.int | None = ...,
         polling_inactive_delay_msecs: builtins.int | None = ...,
         force_gpu_compatible: builtins.bool | None = ...,
         experimental: global___GPUOptions.Experimental | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["experimental", b"experimental"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocator_type", b"allocator_type", "allow_growth", b"allow_growth", "deferred_deletion_bytes", b"deferred_deletion_bytes", "experimental", b"experimental", "force_gpu_compatible", b"force_gpu_compatible", "per_process_gpu_memory_fraction", b"per_process_gpu_memory_fraction", "polling_active_delay_usecs", b"polling_active_delay_usecs", "polling_inactive_delay_msecs", b"polling_inactive_delay_msecs", "visible_device_list", b"visible_device_list"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["experimental", b"experimental"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allocator_type", b"allocator_type", "allow_growth", b"allow_growth", "deferred_deletion_bytes", b"deferred_deletion_bytes", "experimental", b"experimental", "force_gpu_compatible", b"force_gpu_compatible", "per_process_gpu_memory_fraction", b"per_process_gpu_memory_fraction", "polling_active_delay_usecs", b"polling_active_delay_usecs", "polling_inactive_delay_msecs", b"polling_inactive_delay_msecs", "visible_device_list", b"visible_device_list"]) -> None: ...
 
 global___GPUOptions = GPUOptions
 
-@typing_extensions.final
+@typing.final
 class OptimizerOptions(google.protobuf.message.Message):
     """Options passed to the graph optimizer"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Level:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -462,19 +468,19 @@
         do_constant_folding: builtins.bool | None = ...,
         max_folded_constant_in_bytes: builtins.int | None = ...,
         do_function_inlining: builtins.bool | None = ...,
         opt_level: global___OptimizerOptions.Level.ValueType | None = ...,
         global_jit_level: global___OptimizerOptions.GlobalJitLevel.ValueType | None = ...,
         cpu_global_jit: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu_global_jit", b"cpu_global_jit", "do_common_subexpression_elimination", b"do_common_subexpression_elimination", "do_constant_folding", b"do_constant_folding", "do_function_inlining", b"do_function_inlining", "global_jit_level", b"global_jit_level", "max_folded_constant_in_bytes", b"max_folded_constant_in_bytes", "opt_level", b"opt_level"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cpu_global_jit", b"cpu_global_jit", "do_common_subexpression_elimination", b"do_common_subexpression_elimination", "do_constant_folding", b"do_constant_folding", "do_function_inlining", b"do_function_inlining", "global_jit_level", b"global_jit_level", "max_folded_constant_in_bytes", b"max_folded_constant_in_bytes", "opt_level", b"opt_level"]) -> None: ...
 
 global___OptimizerOptions = OptimizerOptions
 
-@typing_extensions.final
+@typing.final
 class GraphOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENABLE_RECV_SCHEDULING_FIELD_NUMBER: builtins.int
     OPTIMIZER_OPTIONS_FIELD_NUMBER: builtins.int
     BUILD_COST_MODEL_FIELD_NUMBER: builtins.int
     BUILD_COST_MODEL_AFTER_FIELD_NUMBER: builtins.int
@@ -483,17 +489,14 @@
     ENABLE_BFLOAT16_SENDRECV_FIELD_NUMBER: builtins.int
     TIMELINE_STEP_FIELD_NUMBER: builtins.int
     REWRITE_OPTIONS_FIELD_NUMBER: builtins.int
     enable_recv_scheduling: builtins.bool
     """If true, use control flow to schedule the activation of Recv nodes.
     (Currently ignored.)
     """
-    @property
-    def optimizer_options(self) -> global___OptimizerOptions:
-        """Options controlling how graph is optimized."""
     build_cost_model: builtins.int
     """The number of steps to run before returning a cost model detailing
     the memory usage and performance of each node of the graph. 0 means
     no cost model.
     """
     build_cost_model_after: builtins.int
     """The number of steps to skip before collecting statistics for the
@@ -515,38 +518,43 @@
     enable_bfloat16_sendrecv: builtins.bool
     """If true, transfer float values between processes as bfloat16."""
     timeline_step: builtins.int
     """If > 0, record a timeline every this many steps.
     EXPERIMENTAL: This currently has no effect in MasterSession.
     """
     @property
+    def optimizer_options(self) -> global___OptimizerOptions:
+        """Options controlling how graph is optimized."""
+
+    @property
     def rewrite_options(self) -> tensorflow.core.protobuf.rewriter_config_pb2.RewriterConfig:
         """Options that control the type and amount of graph rewriting.
         Not currently configurable via the public Python API (i.e. there is no API
         stability guarantee if you import RewriterConfig explicitly).
         """
+
     def __init__(
         self,
         *,
         enable_recv_scheduling: builtins.bool | None = ...,
         optimizer_options: global___OptimizerOptions | None = ...,
         build_cost_model: builtins.int | None = ...,
         build_cost_model_after: builtins.int | None = ...,
         infer_shapes: builtins.bool | None = ...,
         place_pruned_graph: builtins.bool | None = ...,
         enable_bfloat16_sendrecv: builtins.bool | None = ...,
         timeline_step: builtins.int | None = ...,
         rewrite_options: tensorflow.core.protobuf.rewriter_config_pb2.RewriterConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["optimizer_options", b"optimizer_options", "rewrite_options", b"rewrite_options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["build_cost_model", b"build_cost_model", "build_cost_model_after", b"build_cost_model_after", "enable_bfloat16_sendrecv", b"enable_bfloat16_sendrecv", "enable_recv_scheduling", b"enable_recv_scheduling", "infer_shapes", b"infer_shapes", "optimizer_options", b"optimizer_options", "place_pruned_graph", b"place_pruned_graph", "rewrite_options", b"rewrite_options", "timeline_step", b"timeline_step"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["optimizer_options", b"optimizer_options", "rewrite_options", b"rewrite_options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["build_cost_model", b"build_cost_model", "build_cost_model_after", b"build_cost_model_after", "enable_bfloat16_sendrecv", b"enable_bfloat16_sendrecv", "enable_recv_scheduling", b"enable_recv_scheduling", "infer_shapes", b"infer_shapes", "optimizer_options", b"optimizer_options", "place_pruned_graph", b"place_pruned_graph", "rewrite_options", b"rewrite_options", "timeline_step", b"timeline_step"]) -> None: ...
 
 global___GraphOptions = GraphOptions
 
-@typing_extensions.final
+@typing.final
 class ThreadPoolOptionProto(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NUM_THREADS_FIELD_NUMBER: builtins.int
     GLOBAL_NAME_FIELD_NUMBER: builtins.int
     num_threads: builtins.int
     """The number of threads in the pool.
@@ -573,19 +581,19 @@
     """
     def __init__(
         self,
         *,
         num_threads: builtins.int | None = ...,
         global_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["global_name", b"global_name", "num_threads", b"num_threads"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["global_name", b"global_name", "num_threads", b"num_threads"]) -> None: ...
 
 global___ThreadPoolOptionProto = ThreadPoolOptionProto
 
-@typing_extensions.final
+@typing.final
 class SessionMetadata(google.protobuf.message.Message):
     """Metadata about the session.
 
     This can be used by the runtime and the Ops for debugging, monitoring, etc.
 
     The (name, version) tuple is expected to be a unique identifier for
     sessions within the same process.
@@ -602,43 +610,43 @@
     """The version is optional. If set, needs to be >= 0."""
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         version: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "version", b"version"]) -> None: ...
 
 global___SessionMetadata = SessionMetadata
 
-@typing_extensions.final
+@typing.final
 class ConfigProto(google.protobuf.message.Message):
     """Session configuration parameters.
     The system picks appropriate values for fields that are not set.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class DeviceCountEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.int
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Experimental(google.protobuf.message.Message):
         """Everything inside Experimental is subject to change and is not subject
         to API stability guarantees in
         https://www.tensorflow.org/guide/version_compat.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -743,24 +751,14 @@
         but in the case where there is a lot of spinning may result in lower
         CPU usage.
         """
         share_cluster_devices_in_session: builtins.bool
         """This was promoted to a non-experimental API. Please use
         ConfigProto.share_cluster_devices_in_session instead.
         """
-        @property
-        def session_metadata(self) -> global___SessionMetadata:
-            """Metadata about the session.
-
-            If set, this can be used by the runtime and the Ops for debugging,
-            monitoring, etc.
-
-            NOTE: This is currently used and propagated only by the direct session
-            and EagerContext.
-            """
         optimize_for_static_graph: builtins.bool
         """If true, the session may treat the graph as being static for optimization
         purposes.
 
         If this option is set to true when a session is created, the full
         GraphDef must be passed in a single call to Session::Create(), and
         Session::Extend() may not be supported.
@@ -808,28 +806,40 @@
         useful when executing within a portable runtime where control flow op
         kernels may not be loaded due to selective registration.
         """
         xla_prefer_single_graph_cluster: builtins.bool
         """Provides a hint to XLA auto clustering to prefer forming a single large
         cluster that encompases most of the graph.
         """
-        @property
-        def coordination_config(self) -> tensorflow.tsl.protobuf.coordination_config_pb2.CoordinationServiceConfig:
-            """Distributed coordination service configurations."""
         disable_optimize_for_static_graph: builtins.bool
         """If true, the session will treat the graph as being non-static for
         optimization purposes.
 
         If this option is set to true when a session is created, the full
         GraphDef will be retained to enable calls to Session::Extend().
         Calling Extend() without setting this flag will result in errors.
 
         This option is meant to replace `optimize_for_static_graph` and it
         aims to negate its value.
         """
+        @property
+        def session_metadata(self) -> global___SessionMetadata:
+            """Metadata about the session.
+
+            If set, this can be used by the runtime and the Ops for debugging,
+            monitoring, etc.
+
+            NOTE: This is currently used and propagated only by the direct session
+            and EagerContext.
+            """
+
+        @property
+        def coordination_config(self) -> tensorflow.tsl.protobuf.coordination_config_pb2.CoordinationServiceConfig:
+            """Distributed coordination service configurations."""
+
         def __init__(
             self,
             *,
             collective_group_leader: builtins.str | None = ...,
             executor_type: builtins.str | None = ...,
             recv_buf_max_chunk: builtins.int | None = ...,
             use_numa_affinity: builtins.bool | None = ...,
@@ -847,16 +857,16 @@
             xla_fusion_autotuner_thresh: builtins.int | None = ...,
             use_tfrt: builtins.bool | None = ...,
             disable_functional_ops_lowering: builtins.bool | None = ...,
             xla_prefer_single_graph_cluster: builtins.bool | None = ...,
             coordination_config: tensorflow.tsl.protobuf.coordination_config_pb2.CoordinationServiceConfig | None = ...,
             disable_optimize_for_static_graph: builtins.bool | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["coordination_config", b"coordination_config", "session_metadata", b"session_metadata"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["collective_deterministic_sequential_execution", b"collective_deterministic_sequential_execution", "collective_group_leader", b"collective_group_leader", "collective_nccl", b"collective_nccl", "coordination_config", b"coordination_config", "disable_functional_ops_lowering", b"disable_functional_ops_lowering", "disable_optimize_for_static_graph", b"disable_optimize_for_static_graph", "disable_output_partition_graphs", b"disable_output_partition_graphs", "disable_thread_spinning", b"disable_thread_spinning", "enable_mlir_bridge", b"enable_mlir_bridge", "enable_mlir_graph_optimization", b"enable_mlir_graph_optimization", "executor_type", b"executor_type", "mlir_bridge_rollout", b"mlir_bridge_rollout", "optimize_for_static_graph", b"optimize_for_static_graph", "recv_buf_max_chunk", b"recv_buf_max_chunk", "session_metadata", b"session_metadata", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "share_session_state_in_clusterspec_propagation", b"share_session_state_in_clusterspec_propagation", "use_numa_affinity", b"use_numa_affinity", "use_tfrt", b"use_tfrt", "xla_fusion_autotuner_thresh", b"xla_fusion_autotuner_thresh", "xla_prefer_single_graph_cluster", b"xla_prefer_single_graph_cluster"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["coordination_config", b"coordination_config", "session_metadata", b"session_metadata"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["collective_deterministic_sequential_execution", b"collective_deterministic_sequential_execution", "collective_group_leader", b"collective_group_leader", "collective_nccl", b"collective_nccl", "coordination_config", b"coordination_config", "disable_functional_ops_lowering", b"disable_functional_ops_lowering", "disable_optimize_for_static_graph", b"disable_optimize_for_static_graph", "disable_output_partition_graphs", b"disable_output_partition_graphs", "disable_thread_spinning", b"disable_thread_spinning", "enable_mlir_bridge", b"enable_mlir_bridge", "enable_mlir_graph_optimization", b"enable_mlir_graph_optimization", "executor_type", b"executor_type", "mlir_bridge_rollout", b"mlir_bridge_rollout", "optimize_for_static_graph", b"optimize_for_static_graph", "recv_buf_max_chunk", b"recv_buf_max_chunk", "session_metadata", b"session_metadata", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "share_session_state_in_clusterspec_propagation", b"share_session_state_in_clusterspec_propagation", "use_numa_affinity", b"use_numa_affinity", "use_tfrt", b"use_tfrt", "xla_fusion_autotuner_thresh", b"xla_fusion_autotuner_thresh", "xla_prefer_single_graph_cluster", b"xla_prefer_single_graph_cluster"]) -> None: ...
 
     DEVICE_COUNT_FIELD_NUMBER: builtins.int
     INTRA_OP_PARALLELISM_THREADS_FIELD_NUMBER: builtins.int
     INTER_OP_PARALLELISM_THREADS_FIELD_NUMBER: builtins.int
     USE_PER_SESSION_THREADS_FIELD_NUMBER: builtins.int
     SESSION_INTER_OP_THREAD_POOL_FIELD_NUMBER: builtins.int
     PLACEMENT_PERIOD_FIELD_NUMBER: builtins.int
@@ -867,21 +877,14 @@
     GRAPH_OPTIONS_FIELD_NUMBER: builtins.int
     OPERATION_TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
     RPC_OPTIONS_FIELD_NUMBER: builtins.int
     CLUSTER_DEF_FIELD_NUMBER: builtins.int
     ISOLATE_SESSION_STATE_FIELD_NUMBER: builtins.int
     SHARE_CLUSTER_DEVICES_IN_SESSION_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_FIELD_NUMBER: builtins.int
-    @property
-    def device_count(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.int]:
-        """Map from device type name (e.g., "CPU" or "GPU" ) to maximum
-        number of devices of that type to use.  If a particular device
-        type is not found in the map, the system picks an appropriate
-        number.
-        """
     intra_op_parallelism_threads: builtins.int
     """The execution of an individual op (for some op types) can be
     parallelized on a pool of intra_op_parallelism_threads.
     0 means the system picks an appropriate number.
 
     If you create an ordinary session, e.g., from Python or C++,
     then there is exactly one intra op thread pool per process.
@@ -912,14 +915,54 @@
     If false, use the global threads created by the first session, or the
     per-session thread pools configured by session_inter_op_thread_pool.
 
     This option is deprecated. The same effect can be achieved by setting
     session_inter_op_thread_pool to have one element, whose num_threads equals
     inter_op_parallelism_threads.
     """
+    placement_period: builtins.int
+    """Assignment of Nodes to Devices is recomputed every placement_period
+    steps until the system warms up (at which point the recomputation
+    typically slows down automatically).
+    """
+    allow_soft_placement: builtins.bool
+    """Whether soft placement is allowed. If allow_soft_placement is true,
+    an op will be placed on CPU if
+      1. there's no GPU implementation for the OP
+    or
+      2. no GPU devices are known or registered
+    or
+      3. need to co-locate with reftype input(s) which are from CPU.
+    """
+    log_device_placement: builtins.bool
+    """Whether device placements should be logged."""
+    operation_timeout_in_ms: builtins.int
+    """Global timeout for all blocking operations in this session.  If non-zero,
+    and not overridden on a per-operation basis, this value will be used as the
+    deadline for all blocking operations.
+    """
+    isolate_session_state: builtins.bool
+    """If true, any resources such as Variables used in the session will not be
+    shared with other sessions. However, when clusterspec propagation is
+    enabled, this field is ignored and sessions are always isolated.
+    """
+    share_cluster_devices_in_session: builtins.bool
+    """When true, WorkerSessions are created with device attributes from the
+    full cluster.
+    This is helpful when a worker wants to partition a graph
+    (for example during a PartitionedCallOp).
+    """
+    @property
+    def device_count(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.int]:
+        """Map from device type name (e.g., "CPU" or "GPU" ) to maximum
+        number of devices of that type to use.  If a particular device
+        type is not found in the map, the system picks an appropriate
+        number.
+        """
+
     @property
     def session_inter_op_thread_pool(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ThreadPoolOptionProto]:
         """This option is experimental - it may be replaced with a different mechanism
         in the future.
 
         Configures session thread pools. If this is configured, then RunOptions for
         a Run call can select the thread pool to use.
@@ -934,64 +977,38 @@
         - Using this setting is normally not needed in training, but may help some
         serving use cases.
         - It is also generally recommended to set the global_name field of this
         proto, to avoid creating multiple large pools. It is typically better to
         run the non-low-priority work, even across sessions, in a single large
         pool.
         """
-    placement_period: builtins.int
-    """Assignment of Nodes to Devices is recomputed every placement_period
-    steps until the system warms up (at which point the recomputation
-    typically slows down automatically).
-    """
+
     @property
     def device_filters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """When any filters are present sessions will ignore all devices which do not
         match the filters. Each filter can be partially specified, e.g. "/job:ps"
         "/job:worker/replica:3", etc.
         """
+
     @property
     def gpu_options(self) -> global___GPUOptions:
         """Options that apply to all GPUs."""
-    allow_soft_placement: builtins.bool
-    """Whether soft placement is allowed. If allow_soft_placement is true,
-    an op will be placed on CPU if
-      1. there's no GPU implementation for the OP
-    or
-      2. no GPU devices are known or registered
-    or
-      3. need to co-locate with reftype input(s) which are from CPU.
-    """
-    log_device_placement: builtins.bool
-    """Whether device placements should be logged."""
+
     @property
     def graph_options(self) -> global___GraphOptions:
         """Options that apply to all graphs."""
-    operation_timeout_in_ms: builtins.int
-    """Global timeout for all blocking operations in this session.  If non-zero,
-    and not overridden on a per-operation basis, this value will be used as the
-    deadline for all blocking operations.
-    """
+
     @property
     def rpc_options(self) -> tensorflow.tsl.protobuf.rpc_options_pb2.RPCOptions:
         """Options that apply when this session uses the distributed runtime."""
+
     @property
     def cluster_def(self) -> tensorflow.core.protobuf.cluster_pb2.ClusterDef:
         """Optional list of all workers to use in this session."""
-    isolate_session_state: builtins.bool
-    """If true, any resources such as Variables used in the session will not be
-    shared with other sessions. However, when clusterspec propagation is
-    enabled, this field is ignored and sessions are always isolated.
-    """
-    share_cluster_devices_in_session: builtins.bool
-    """When true, WorkerSessions are created with device attributes from the
-    full cluster.
-    This is helpful when a worker wants to partition a graph
-    (for example during a PartitionedCallOp).
-    """
+
     @property
     def experimental(self) -> global___ConfigProto.Experimental: ...
     def __init__(
         self,
         *,
         device_count: collections.abc.Mapping[builtins.str, builtins.int] | None = ...,
         intra_op_parallelism_threads: builtins.int | None = ...,
@@ -1007,20 +1024,20 @@
         operation_timeout_in_ms: builtins.int | None = ...,
         rpc_options: tensorflow.tsl.protobuf.rpc_options_pb2.RPCOptions | None = ...,
         cluster_def: tensorflow.core.protobuf.cluster_pb2.ClusterDef | None = ...,
         isolate_session_state: builtins.bool | None = ...,
         share_cluster_devices_in_session: builtins.bool | None = ...,
         experimental: global___ConfigProto.Experimental | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cluster_def", b"cluster_def", "experimental", b"experimental", "gpu_options", b"gpu_options", "graph_options", b"graph_options", "rpc_options", b"rpc_options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_soft_placement", b"allow_soft_placement", "cluster_def", b"cluster_def", "device_count", b"device_count", "device_filters", b"device_filters", "experimental", b"experimental", "gpu_options", b"gpu_options", "graph_options", b"graph_options", "inter_op_parallelism_threads", b"inter_op_parallelism_threads", "intra_op_parallelism_threads", b"intra_op_parallelism_threads", "isolate_session_state", b"isolate_session_state", "log_device_placement", b"log_device_placement", "operation_timeout_in_ms", b"operation_timeout_in_ms", "placement_period", b"placement_period", "rpc_options", b"rpc_options", "session_inter_op_thread_pool", b"session_inter_op_thread_pool", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "use_per_session_threads", b"use_per_session_threads"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cluster_def", b"cluster_def", "experimental", b"experimental", "gpu_options", b"gpu_options", "graph_options", b"graph_options", "rpc_options", b"rpc_options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allow_soft_placement", b"allow_soft_placement", "cluster_def", b"cluster_def", "device_count", b"device_count", "device_filters", b"device_filters", "experimental", b"experimental", "gpu_options", b"gpu_options", "graph_options", b"graph_options", "inter_op_parallelism_threads", b"inter_op_parallelism_threads", "intra_op_parallelism_threads", b"intra_op_parallelism_threads", "isolate_session_state", b"isolate_session_state", "log_device_placement", b"log_device_placement", "operation_timeout_in_ms", b"operation_timeout_in_ms", "placement_period", b"placement_period", "rpc_options", b"rpc_options", "session_inter_op_thread_pool", b"session_inter_op_thread_pool", "share_cluster_devices_in_session", b"share_cluster_devices_in_session", "use_per_session_threads", b"use_per_session_threads"]) -> None: ...
 
 global___ConfigProto = ConfigProto
 
-@typing_extensions.final
+@typing.final
 class RunOptions(google.protobuf.message.Message):
     """Options for a single Run() call."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _TraceLevel:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -1039,24 +1056,24 @@
         """
 
     NO_TRACE: RunOptions.TraceLevel.ValueType  # 0
     SOFTWARE_TRACE: RunOptions.TraceLevel.ValueType  # 1
     HARDWARE_TRACE: RunOptions.TraceLevel.ValueType  # 2
     FULL_TRACE: RunOptions.TraceLevel.ValueType  # 3
 
-    @typing_extensions.final
+    @typing.final
     class Experimental(google.protobuf.message.Message):
         """Everything inside Experimental is subject to change and is not subject
         to API stability guarantees in
         https://www.tensorflow.org/guide/version_compat.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class RunHandlerPoolOptions(google.protobuf.message.Message):
             """Options for run handler thread pool."""
 
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             PRIORITY_FIELD_NUMBER: builtins.int
             priority: builtins.int
@@ -1064,15 +1081,15 @@
             based on the priority number. The larger number means higher priority.
             """
             def __init__(
                 self,
                 *,
                 priority: builtins.int | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["priority", b"priority"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["priority", b"priority"]) -> None: ...
 
         COLLECTIVE_GRAPH_KEY_FIELD_NUMBER: builtins.int
         USE_RUN_HANDLER_POOL_FIELD_NUMBER: builtins.int
         RUN_HANDLER_POOL_OPTIONS_FIELD_NUMBER: builtins.int
         collective_graph_key: builtins.int
         """If non-zero, declares that this graph is going to use collective
         ops and must synchronize step_ids with any other graph with this
@@ -1090,16 +1107,16 @@
         def __init__(
             self,
             *,
             collective_graph_key: builtins.int | None = ...,
             use_run_handler_pool: builtins.bool | None = ...,
             run_handler_pool_options: global___RunOptions.Experimental.RunHandlerPoolOptions | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["run_handler_pool_options", b"run_handler_pool_options"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["collective_graph_key", b"collective_graph_key", "run_handler_pool_options", b"run_handler_pool_options", "use_run_handler_pool", b"use_run_handler_pool"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["run_handler_pool_options", b"run_handler_pool_options"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["collective_graph_key", b"collective_graph_key", "run_handler_pool_options", b"run_handler_pool_options", "use_run_handler_pool", b"use_run_handler_pool"]) -> None: ...
 
     TRACE_LEVEL_FIELD_NUMBER: builtins.int
     TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
     INTER_OP_THREAD_POOL_FIELD_NUMBER: builtins.int
     OUTPUT_PARTITION_GRAPHS_FIELD_NUMBER: builtins.int
     DEBUG_OPTIONS_FIELD_NUMBER: builtins.int
     REPORT_TENSOR_ALLOCATIONS_UPON_OOM_FIELD_NUMBER: builtins.int
@@ -1115,120 +1132,127 @@
     graphs, where the overhead of an additional context switch is
     comparable with the overhead of Session::Run().
     """
     output_partition_graphs: builtins.bool
     """Whether the partition graph(s) executed by the executor(s) should be
     outputted via RunMetadata.
     """
-    @property
-    def debug_options(self) -> tensorflow.core.protobuf.debug_pb2.DebugOptions:
-        """EXPERIMENTAL.  Options used to initialize DebuggerState, if enabled."""
     report_tensor_allocations_upon_oom: builtins.bool
     """When enabled, causes tensor allocation information to be included in
     the error message when the Run() call fails because the allocator ran
     out of memory (OOM).
 
     Enabling this option can slow down the Run() call.
     """
     @property
+    def debug_options(self) -> tensorflow.core.protobuf.debug_pb2.DebugOptions:
+        """EXPERIMENTAL.  Options used to initialize DebuggerState, if enabled."""
+
+    @property
     def experimental(self) -> global___RunOptions.Experimental: ...
     def __init__(
         self,
         *,
         trace_level: global___RunOptions.TraceLevel.ValueType | None = ...,
         timeout_in_ms: builtins.int | None = ...,
         inter_op_thread_pool: builtins.int | None = ...,
         output_partition_graphs: builtins.bool | None = ...,
         debug_options: tensorflow.core.protobuf.debug_pb2.DebugOptions | None = ...,
         report_tensor_allocations_upon_oom: builtins.bool | None = ...,
         experimental: global___RunOptions.Experimental | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["debug_options", b"debug_options", "experimental", b"experimental"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["debug_options", b"debug_options", "experimental", b"experimental", "inter_op_thread_pool", b"inter_op_thread_pool", "output_partition_graphs", b"output_partition_graphs", "report_tensor_allocations_upon_oom", b"report_tensor_allocations_upon_oom", "timeout_in_ms", b"timeout_in_ms", "trace_level", b"trace_level"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["debug_options", b"debug_options", "experimental", b"experimental"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["debug_options", b"debug_options", "experimental", b"experimental", "inter_op_thread_pool", b"inter_op_thread_pool", "output_partition_graphs", b"output_partition_graphs", "report_tensor_allocations_upon_oom", b"report_tensor_allocations_upon_oom", "timeout_in_ms", b"timeout_in_ms", "trace_level", b"trace_level"]) -> None: ...
 
 global___RunOptions = RunOptions
 
-@typing_extensions.final
+@typing.final
 class RunMetadata(google.protobuf.message.Message):
     """Metadata output (i.e., non-Tensor) for a single Run() call."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FunctionGraphs(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PARTITION_GRAPHS_FIELD_NUMBER: builtins.int
         PRE_OPTIMIZATION_GRAPH_FIELD_NUMBER: builtins.int
         POST_OPTIMIZATION_GRAPH_FIELD_NUMBER: builtins.int
         @property
         def partition_graphs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.graph_pb2.GraphDef]:
             """TODO(nareshmodi): Include some sort of function/cache-key identifier?"""
+
         @property
         def pre_optimization_graph(self) -> tensorflow.core.framework.graph_pb2.GraphDef: ...
         @property
         def post_optimization_graph(self) -> tensorflow.core.framework.graph_pb2.GraphDef: ...
         def __init__(
             self,
             *,
             partition_graphs: collections.abc.Iterable[tensorflow.core.framework.graph_pb2.GraphDef] | None = ...,
             pre_optimization_graph: tensorflow.core.framework.graph_pb2.GraphDef | None = ...,
             post_optimization_graph: tensorflow.core.framework.graph_pb2.GraphDef | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["post_optimization_graph", b"post_optimization_graph", "pre_optimization_graph", b"pre_optimization_graph"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["partition_graphs", b"partition_graphs", "post_optimization_graph", b"post_optimization_graph", "pre_optimization_graph", b"pre_optimization_graph"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["post_optimization_graph", b"post_optimization_graph", "pre_optimization_graph", b"pre_optimization_graph"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["partition_graphs", b"partition_graphs", "post_optimization_graph", b"post_optimization_graph", "pre_optimization_graph", b"pre_optimization_graph"]) -> None: ...
 
     STEP_STATS_FIELD_NUMBER: builtins.int
     COST_GRAPH_FIELD_NUMBER: builtins.int
     PARTITION_GRAPHS_FIELD_NUMBER: builtins.int
     FUNCTION_GRAPHS_FIELD_NUMBER: builtins.int
     SESSION_METADATA_FIELD_NUMBER: builtins.int
     @property
     def step_stats(self) -> tensorflow.core.framework.step_stats_pb2.StepStats:
         """Statistics traced for this step. Populated if tracing is turned on via the
         "RunOptions" proto.
         EXPERIMENTAL: The format and set of events may change in future versions.
         """
+
     @property
     def cost_graph(self) -> tensorflow.core.framework.cost_graph_pb2.CostGraphDef:
         """The cost graph for the computation defined by the run call."""
+
     @property
     def partition_graphs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.graph_pb2.GraphDef]:
         """Graphs of the partitions executed by executors."""
+
     @property
     def function_graphs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RunMetadata.FunctionGraphs]:
         """This is only populated for graphs that are run as functions in TensorFlow
         V2. There will be an entry below for each function that is traced.
         The main use cases of the post_optimization_graph and the partition_graphs
         is to give the caller insight into the graphs that were actually run by the
         runtime. Additional information (such as those in step_stats) will match
         these graphs.
         We also include the pre_optimization_graph since it is usually easier to
         read, and is helpful in situations where the caller wants to get a high
         level idea of what the built graph looks like (since the various graph
         optimization passes might change the structure of the graph significantly).
         """
+
     @property
     def session_metadata(self) -> global___SessionMetadata:
         """Metadata about the session."""
+
     def __init__(
         self,
         *,
         step_stats: tensorflow.core.framework.step_stats_pb2.StepStats | None = ...,
         cost_graph: tensorflow.core.framework.cost_graph_pb2.CostGraphDef | None = ...,
         partition_graphs: collections.abc.Iterable[tensorflow.core.framework.graph_pb2.GraphDef] | None = ...,
         function_graphs: collections.abc.Iterable[global___RunMetadata.FunctionGraphs] | None = ...,
         session_metadata: global___SessionMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cost_graph", b"cost_graph", "session_metadata", b"session_metadata", "step_stats", b"step_stats"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cost_graph", b"cost_graph", "function_graphs", b"function_graphs", "partition_graphs", b"partition_graphs", "session_metadata", b"session_metadata", "step_stats", b"step_stats"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cost_graph", b"cost_graph", "session_metadata", b"session_metadata", "step_stats", b"step_stats"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["cost_graph", b"cost_graph", "function_graphs", b"function_graphs", "partition_graphs", b"partition_graphs", "session_metadata", b"session_metadata", "step_stats", b"step_stats"]) -> None: ...
 
 global___RunMetadata = RunMetadata
 
-@typing_extensions.final
+@typing.final
 class TensorConnection(google.protobuf.message.Message):
     """Defines a connection between two tensors in a `GraphDef`."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FROM_TENSOR_FIELD_NUMBER: builtins.int
     TO_TENSOR_FIELD_NUMBER: builtins.int
@@ -1242,91 +1266,108 @@
     """
     def __init__(
         self,
         *,
         from_tensor: builtins.str | None = ...,
         to_tensor: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["from_tensor", b"from_tensor", "to_tensor", b"to_tensor"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["from_tensor", b"from_tensor", "to_tensor", b"to_tensor"]) -> None: ...
 
 global___TensorConnection = TensorConnection
 
-@typing_extensions.final
+@typing.final
 class CallableOptions(google.protobuf.message.Message):
     """Defines a subgraph in another `GraphDef` as a set of feed points and nodes
     to be fetched or executed.
 
     Compare with the arguments to `Session::Run()`.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FeedDevicesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class FetchDevicesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FEED_FIELD_NUMBER: builtins.int
     FETCH_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
     RUN_OPTIONS_FIELD_NUMBER: builtins.int
     TENSOR_CONNECTION_FIELD_NUMBER: builtins.int
     FEED_DEVICES_FIELD_NUMBER: builtins.int
     FETCH_DEVICES_FIELD_NUMBER: builtins.int
     FETCH_SKIP_SYNC_FIELD_NUMBER: builtins.int
+    fetch_skip_sync: builtins.bool
+    """By default, RunCallable() will synchronize the GPU stream before returning
+    fetched tensors on a GPU device, to ensure that the values in those tensors
+    have been produced. This simplifies interacting with the tensors, but
+    potentially incurs a performance hit.
+
+    If this options is set to true, the caller is responsible for ensuring
+    that the values in the fetched tensors have been produced before they are
+    used. The caller can do this by invoking `Device::Sync()` on the underlying
+    device(s), or by feeding the tensors back to the same Session using
+    `feed_devices` with the same corresponding device name.
+    """
     @property
     def feed(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Tensors to be fed in the callable. Each feed is the name of a tensor."""
+
     @property
     def fetch(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Fetches. A list of tensor names. The caller of the callable expects a
         tensor to be returned for each fetch[i] (see RunStepResponse.tensor). The
         order of specified fetches does not change the execution order.
         """
+
     @property
     def target(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Target Nodes. A list of node names. The named nodes will be run by the
         callable but their outputs will not be returned.
         """
+
     @property
     def run_options(self) -> global___RunOptions:
         """Options that will be applied to each run."""
+
     @property
     def tensor_connection(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorConnection]:
         """Tensors to be connected in the callable. Each TensorConnection denotes
         a pair of tensors in the graph, between which an edge will be created
         in the callable.
         """
+
     @property
     def feed_devices(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """The Tensor objects fed in the callable and fetched from the callable
         are expected to be backed by host (CPU) memory by default.
 
         The options below allow changing that - feeding tensors backed by
         device memory, or returning tensors that are backed by device memory.
@@ -1369,37 +1410,26 @@
         (Device::GetAllocator()) to create the Tensor to be fed.
 
         Alternatively, for CUDA-enabled GPU devices, this typically means that the
         operation that produced the contents of the tensor has completed, i.e., the
         CUDA stream has been synchronized (e.g., via cuCtxSynchronize() or
         cuStreamSynchronize()).
         """
+
     @property
     def fetch_devices(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    fetch_skip_sync: builtins.bool
-    """By default, RunCallable() will synchronize the GPU stream before returning
-    fetched tensors on a GPU device, to ensure that the values in those tensors
-    have been produced. This simplifies interacting with the tensors, but
-    potentially incurs a performance hit.
-
-    If this options is set to true, the caller is responsible for ensuring
-    that the values in the fetched tensors have been produced before they are
-    used. The caller can do this by invoking `Device::Sync()` on the underlying
-    device(s), or by feeding the tensors back to the same Session using
-    `feed_devices` with the same corresponding device name.
-    """
     def __init__(
         self,
         *,
         feed: collections.abc.Iterable[builtins.str] | None = ...,
         fetch: collections.abc.Iterable[builtins.str] | None = ...,
         target: collections.abc.Iterable[builtins.str] | None = ...,
         run_options: global___RunOptions | None = ...,
         tensor_connection: collections.abc.Iterable[global___TensorConnection] | None = ...,
         feed_devices: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         fetch_devices: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         fetch_skip_sync: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["run_options", b"run_options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["feed", b"feed", "feed_devices", b"feed_devices", "fetch", b"fetch", "fetch_devices", b"fetch_devices", "fetch_skip_sync", b"fetch_skip_sync", "run_options", b"run_options", "target", b"target", "tensor_connection", b"tensor_connection"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["run_options", b"run_options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["feed", b"feed", "feed_devices", b"feed_devices", "fetch", b"fetch", "fetch_devices", b"fetch_devices", "fetch_skip_sync", b"fetch_skip_sync", "run_options", b"run_options", "target", b"target", "tensor_connection", b"tensor_connection"]) -> None: ...
 
 global___CallableOptions = CallableOptions
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ValuesDef(google.protobuf.message.Message):
     """Control flow context related protocol buffers.
 
     Protocol buffer representing the values in ControlFlowContext.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ExternalValuesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     VALUES_FIELD_NUMBER: builtins.int
     EXTERNAL_VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Value names that have been seen in this context."""
+
     @property
     def external_values(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Value names referenced by but external to this context."""
+
     def __init__(
         self,
         *,
         values: collections.abc.Iterable[builtins.str] | None = ...,
         external_values: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["external_values", b"external_values", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["external_values", b"external_values", "values", b"values"]) -> None: ...
 
 global___ValuesDef = ValuesDef
 
-@typing_extensions.final
+@typing.final
 class ControlFlowContextDef(google.protobuf.message.Message):
     """Container for any kind of control flow context. Any other control flow
     contexts that are added below should also be added here.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -71,21 +74,21 @@
     def while_ctxt(self) -> global___WhileContextDef: ...
     def __init__(
         self,
         *,
         cond_ctxt: global___CondContextDef | None = ...,
         while_ctxt: global___WhileContextDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cond_ctxt", b"cond_ctxt", "ctxt", b"ctxt", "while_ctxt", b"while_ctxt"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cond_ctxt", b"cond_ctxt", "ctxt", b"ctxt", "while_ctxt", b"while_ctxt"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["ctxt", b"ctxt"]) -> typing_extensions.Literal["cond_ctxt", "while_ctxt"] | None: ...
+    def HasField(self, field_name: typing.Literal["cond_ctxt", b"cond_ctxt", "ctxt", b"ctxt", "while_ctxt", b"while_ctxt"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["cond_ctxt", b"cond_ctxt", "ctxt", b"ctxt", "while_ctxt", b"while_ctxt"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["ctxt", b"ctxt"]) -> typing.Literal["cond_ctxt", "while_ctxt"] | None: ...
 
 global___ControlFlowContextDef = ControlFlowContextDef
 
-@typing_extensions.final
+@typing.final
 class CondContextDef(google.protobuf.message.Message):
     """Protocol buffer representing a CondContext object."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTEXT_NAME_FIELD_NUMBER: builtins.int
     PRED_NAME_FIELD_NUMBER: builtins.int
@@ -100,33 +103,35 @@
     pivot_name: builtins.str
     """Name of the pivot tensor."""
     branch: builtins.int
     """Branch prediction. 0 or 1."""
     @property
     def values_def(self) -> global___ValuesDef:
         """Values and external values in control flow context."""
+
     @property
     def nested_contexts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ControlFlowContextDef]:
         """Contexts contained inside this context (e.g. nested conds)."""
+
     def __init__(
         self,
         *,
         context_name: builtins.str | None = ...,
         pred_name: builtins.str | None = ...,
         pivot_name: builtins.str | None = ...,
         branch: builtins.int | None = ...,
         values_def: global___ValuesDef | None = ...,
         nested_contexts: collections.abc.Iterable[global___ControlFlowContextDef] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["values_def", b"values_def"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["branch", b"branch", "context_name", b"context_name", "nested_contexts", b"nested_contexts", "pivot_name", b"pivot_name", "pred_name", b"pred_name", "values_def", b"values_def"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["values_def", b"values_def"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["branch", b"branch", "context_name", b"context_name", "nested_contexts", b"nested_contexts", "pivot_name", b"pivot_name", "pred_name", b"pred_name", "values_def", b"values_def"]) -> None: ...
 
 global___CondContextDef = CondContextDef
 
-@typing_extensions.final
+@typing.final
 class WhileContextDef(google.protobuf.message.Message):
     """Protocol buffer representing a WhileContext object."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONTEXT_NAME_FIELD_NUMBER: builtins.int
     PARALLEL_ITERATIONS_FIELD_NUMBER: builtins.int
@@ -150,28 +155,32 @@
     """Whether GPU-CPU memory swap is enabled for this loop."""
     pivot_name: builtins.str
     """Name of the pivot tensor."""
     pivot_for_pred_name: builtins.str
     """Name of the pivot_for_pred tensor."""
     pivot_for_body_name: builtins.str
     """Name of the pivot_for_body tensor."""
+    maximum_iterations_name: builtins.str
+    """Optional name of the maximum_iterations tensor."""
     @property
     def loop_exit_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of names for exit tensors."""
+
     @property
     def loop_enter_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """List of names for enter tensors."""
+
     @property
     def values_def(self) -> global___ValuesDef:
         """Values and external values in control flow context."""
-    maximum_iterations_name: builtins.str
-    """Optional name of the maximum_iterations tensor."""
+
     @property
     def nested_contexts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ControlFlowContextDef]:
         """Contexts contained inside this context (e.g. nested whiles)."""
+
     def __init__(
         self,
         *,
         context_name: builtins.str | None = ...,
         parallel_iterations: builtins.int | None = ...,
         back_prop: builtins.bool | None = ...,
         swap_memory: builtins.bool | None = ...,
@@ -180,11 +189,11 @@
         pivot_for_body_name: builtins.str | None = ...,
         loop_exit_names: collections.abc.Iterable[builtins.str] | None = ...,
         loop_enter_names: collections.abc.Iterable[builtins.str] | None = ...,
         values_def: global___ValuesDef | None = ...,
         maximum_iterations_name: builtins.str | None = ...,
         nested_contexts: collections.abc.Iterable[global___ControlFlowContextDef] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["values_def", b"values_def"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["back_prop", b"back_prop", "context_name", b"context_name", "loop_enter_names", b"loop_enter_names", "loop_exit_names", b"loop_exit_names", "maximum_iterations_name", b"maximum_iterations_name", "nested_contexts", b"nested_contexts", "parallel_iterations", b"parallel_iterations", "pivot_for_body_name", b"pivot_for_body_name", "pivot_for_pred_name", b"pivot_for_pred_name", "pivot_name", b"pivot_name", "swap_memory", b"swap_memory", "values_def", b"values_def"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["values_def", b"values_def"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["back_prop", b"back_prop", "context_name", b"context_name", "loop_enter_names", b"loop_enter_names", "loop_exit_names", b"loop_exit_names", "maximum_iterations_name", b"maximum_iterations_name", "nested_contexts", b"nested_contexts", "parallel_iterations", b"parallel_iterations", "pivot_for_body_name", b"pivot_for_body_name", "pivot_for_pred_name", b"pivot_for_pred_name", "pivot_name", b"pivot_name", "swap_memory", b"swap_memory", "values_def", b"values_def"]) -> None: ...
 
 global___WhileContextDef = WhileContextDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CoordinatedJob(google.protobuf.message.Message):
     """Represents a job type and the number of tasks under this job.
     For example, ("worker", 20) implies that there will be 20 worker tasks.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -26,19 +27,19 @@
     num_tasks: builtins.int
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         num_tasks: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "num_tasks", b"num_tasks"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "num_tasks", b"num_tasks"]) -> None: ...
 
 global___CoordinatedJob = CoordinatedJob
 
-@typing_extensions.final
+@typing.final
 class CoordinationServiceConfig(google.protobuf.message.Message):
     """Coordination service configuration parameters.
     The system picks appropriate values for fields that are not set.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -66,43 +67,44 @@
     heartbeat_timeout_in_ms: builtins.int
     """Heartbeat timeout, if a task does not record heartbeat in this time
     window, it will be considered disconnected.
     Note: This is also used as a grace period to accept any heartbeats after
     the agent has disconnected, to account for the lag time between the service
     recording the state change and the agent stopping heartbeats.
     """
-    @property
-    def coordinated_job_list(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedJob]: ...
     shutdown_barrier_timeout_in_ms: builtins.int
     """Denotes how long to wait for all coordination agents to reach the barriers
     (after the first shutdown request) before disconnecting together. If
     set to 0, no barrier is imposed upon shutdown and each worker can
     disconnect individually.
     """
     agent_destruction_without_shutdown: builtins.bool
     """If set, agents do not make an explicit Shutdown() call. Service will only
     find out about the disconnecte agent via stale heartbeats. Used for
     testing.
     """
     @property
+    def coordinated_job_list(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedJob]: ...
+    @property
     def recoverable_jobs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The list of jobs which are recoverable. If a task in this list fails,
         it will not propagate error to other tasks.
         If empty, no jobs will be recoverable and every task failure will cause
         error propagation to other tasks.
         """
+
     def __init__(
         self,
         *,
         service_type: builtins.str | None = ...,
         service_leader: builtins.str | None = ...,
         enable_health_check: builtins.bool | None = ...,
         cluster_register_timeout_in_ms: builtins.int | None = ...,
         heartbeat_timeout_in_ms: builtins.int | None = ...,
         coordinated_job_list: collections.abc.Iterable[global___CoordinatedJob] | None = ...,
         shutdown_barrier_timeout_in_ms: builtins.int | None = ...,
         agent_destruction_without_shutdown: builtins.bool | None = ...,
         recoverable_jobs: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["agent_destruction_without_shutdown", b"agent_destruction_without_shutdown", "cluster_register_timeout_in_ms", b"cluster_register_timeout_in_ms", "coordinated_job_list", b"coordinated_job_list", "enable_health_check", b"enable_health_check", "heartbeat_timeout_in_ms", b"heartbeat_timeout_in_ms", "recoverable_jobs", b"recoverable_jobs", "service_leader", b"service_leader", "service_type", b"service_type", "shutdown_barrier_timeout_in_ms", b"shutdown_barrier_timeout_in_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["agent_destruction_without_shutdown", b"agent_destruction_without_shutdown", "cluster_register_timeout_in_ms", b"cluster_register_timeout_in_ms", "coordinated_job_list", b"coordinated_job_list", "enable_health_check", b"enable_health_check", "heartbeat_timeout_in_ms", b"heartbeat_timeout_in_ms", "recoverable_jobs", b"recoverable_jobs", "service_leader", b"service_leader", "service_type", b"service_type", "shutdown_barrier_timeout_in_ms", b"shutdown_barrier_timeout_in_ms"]) -> None: ...
 
 global___CoordinationServiceConfig = CoordinationServiceConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -13,15 +14,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ErrorSourceProto(google.protobuf.message.Message):
     """If included as a payload, this message contains the error source information
     where the error was raised.
     URI: "type.googleapis.com/tensorflow.core.platform.ErrorSourceProto"
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -58,10 +59,10 @@
     ERROR_SOURCE_FIELD_NUMBER: builtins.int
     error_source: global___ErrorSourceProto.ErrorSource.ValueType
     def __init__(
         self,
         *,
         error_source: global___ErrorSourceProto.ErrorSource.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_source", b"error_source"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["error_source", b"error_source"]) -> None: ...
 
 global___ErrorSourceProto = ErrorSourceProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -43,15 +44,15 @@
 """tf.data service workers run in dedicated tf.data hosts."""
 DEPLOYMENT_MODE_HYBRID: DeploymentMode.ValueType  # 3
 """tf.data service workers run in colocated TF hosts and dedicated tf.data
 hosts.
 """
 global___DeploymentMode = DeploymentMode
 
-@typing_extensions.final
+@typing.final
 class ProcessingModeDef(google.protobuf.message.Message):
     """Next tag: 2"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _ShardingPolicy:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -141,19 +142,19 @@
     SHARDING_POLICY_FIELD_NUMBER: builtins.int
     sharding_policy: global___ProcessingModeDef.ShardingPolicy.ValueType
     def __init__(
         self,
         *,
         sharding_policy: global___ProcessingModeDef.ShardingPolicy.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["sharding_policy", b"sharding_policy"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["sharding_policy", b"sharding_policy"]) -> None: ...
 
 global___ProcessingModeDef = ProcessingModeDef
 
-@typing_extensions.final
+@typing.final
 class DataServiceMetadata(google.protobuf.message.Message):
     """Metadata related to tf.data service datasets.
     Next tag: 4
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -187,46 +188,46 @@
     def __init__(
         self,
         *,
         element_spec: builtins.bytes | None = ...,
         compression: global___DataServiceMetadata.Compression.ValueType | None = ...,
         cardinality: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["element_spec", b"element_spec", "optional_element_spec", b"optional_element_spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cardinality", b"cardinality", "compression", b"compression", "element_spec", b"element_spec", "optional_element_spec", b"optional_element_spec"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_element_spec", b"optional_element_spec"]) -> typing_extensions.Literal["element_spec"] | None: ...
+    def HasField(self, field_name: typing.Literal["element_spec", b"element_spec", "optional_element_spec", b"optional_element_spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["cardinality", b"cardinality", "compression", b"compression", "element_spec", b"element_spec", "optional_element_spec", b"optional_element_spec"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_element_spec", b"optional_element_spec"]) -> typing.Literal["element_spec"] | None: ...
 
 global___DataServiceMetadata = DataServiceMetadata
 
-@typing_extensions.final
+@typing.final
 class CrossTrainerCacheOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TRAINER_ID_FIELD_NUMBER: builtins.int
     trainer_id: builtins.str
     def __init__(
         self,
         *,
         trainer_id: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["trainer_id", b"trainer_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["trainer_id", b"trainer_id"]) -> None: ...
 
 global___CrossTrainerCacheOptions = CrossTrainerCacheOptions
 
-@typing_extensions.final
+@typing.final
 class DataServiceConfig(google.protobuf.message.Message):
     """Data service config available to the client through GetDataServiceConfig RPC.
     Next tag: 2
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEPLOYMENT_MODE_FIELD_NUMBER: builtins.int
     deployment_mode: global___DeploymentMode.ValueType
     def __init__(
         self,
         *,
         deployment_mode: global___DeploymentMode.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deployment_mode", b"deployment_mode"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["deployment_mode", b"deployment_mode"]) -> None: ...
 
 global___DataServiceConfig = DataServiceConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -126,15 +127,15 @@
 - the 2nd element is +inf if any element of the tensor is +inf,
   or zero otherwise.
 - the 3rd element is nan if any element of the tensor is nan, or zero
   otherwise.
 """
 global___TensorDebugMode = TensorDebugMode
 
-@typing_extensions.final
+@typing.final
 class DebugEvent(google.protobuf.message.Message):
     """An Event related to the debugging of a TensorFlow program."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WALL_TIME_FIELD_NUMBER: builtins.int
     STEP_FIELD_NUMBER: builtins.int
@@ -147,48 +148,56 @@
     GRAPH_EXECUTION_TRACE_FIELD_NUMBER: builtins.int
     GRAPH_ID_FIELD_NUMBER: builtins.int
     DEBUGGED_DEVICE_FIELD_NUMBER: builtins.int
     wall_time: builtins.float
     """Timestamp in seconds (with microsecond precision)."""
     step: builtins.int
     """Step of training (if available)."""
+    graph_id: builtins.str
+    """The ID of the graph (i.e., FuncGraph) executed here: applicable only
+    to the execution of a FuncGraph.
+    """
     @property
     def debug_metadata(self) -> global___DebugMetadata:
         """Metadata related to this debugging data."""
+
     @property
     def source_file(self) -> global___SourceFile:
         """The content of a source file."""
+
     @property
     def stack_frame_with_id(self) -> global___StackFrameWithId:
         """A stack frame (filename, line number and column number, function name and
         code string) with ID.
         """
+
     @property
     def graph_op_creation(self) -> global___GraphOpCreation:
         """The creation of an op within a graph (e.g., a FuncGraph compiled from
         a Python function).
         """
+
     @property
     def debugged_graph(self) -> global___DebuggedGraph:
         """Information about a debugged graph."""
+
     @property
     def execution(self) -> global___Execution:
         """Execution of an op or a Graph (e.g., a tf.function)."""
+
     @property
     def graph_execution_trace(self) -> global___GraphExecutionTrace:
         """A graph execution trace: Contains information about the intermediate
         tensors computed during the graph execution.
         """
-    graph_id: builtins.str
-    """The ID of the graph (i.e., FuncGraph) executed here: applicable only
-    to the execution of a FuncGraph.
-    """
+
     @property
     def debugged_device(self) -> global___DebuggedDevice:
         """A device on which debugger-instrumented ops and/or tensors reside."""
+
     def __init__(
         self,
         *,
         wall_time: builtins.float | None = ...,
         step: builtins.int | None = ...,
         debug_metadata: global___DebugMetadata | None = ...,
         source_file: global___SourceFile | None = ...,
@@ -196,21 +205,21 @@
         graph_op_creation: global___GraphOpCreation | None = ...,
         debugged_graph: global___DebuggedGraph | None = ...,
         execution: global___Execution | None = ...,
         graph_execution_trace: global___GraphExecutionTrace | None = ...,
         graph_id: builtins.str | None = ...,
         debugged_device: global___DebuggedDevice | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["debug_metadata", b"debug_metadata", "debugged_device", b"debugged_device", "debugged_graph", b"debugged_graph", "execution", b"execution", "graph_execution_trace", b"graph_execution_trace", "graph_id", b"graph_id", "graph_op_creation", b"graph_op_creation", "source_file", b"source_file", "stack_frame_with_id", b"stack_frame_with_id", "what", b"what"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["debug_metadata", b"debug_metadata", "debugged_device", b"debugged_device", "debugged_graph", b"debugged_graph", "execution", b"execution", "graph_execution_trace", b"graph_execution_trace", "graph_id", b"graph_id", "graph_op_creation", b"graph_op_creation", "source_file", b"source_file", "stack_frame_with_id", b"stack_frame_with_id", "step", b"step", "wall_time", b"wall_time", "what", b"what"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["what", b"what"]) -> typing_extensions.Literal["debug_metadata", "source_file", "stack_frame_with_id", "graph_op_creation", "debugged_graph", "execution", "graph_execution_trace", "graph_id", "debugged_device"] | None: ...
+    def HasField(self, field_name: typing.Literal["debug_metadata", b"debug_metadata", "debugged_device", b"debugged_device", "debugged_graph", b"debugged_graph", "execution", b"execution", "graph_execution_trace", b"graph_execution_trace", "graph_id", b"graph_id", "graph_op_creation", b"graph_op_creation", "source_file", b"source_file", "stack_frame_with_id", b"stack_frame_with_id", "what", b"what"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["debug_metadata", b"debug_metadata", "debugged_device", b"debugged_device", "debugged_graph", b"debugged_graph", "execution", b"execution", "graph_execution_trace", b"graph_execution_trace", "graph_id", b"graph_id", "graph_op_creation", b"graph_op_creation", "source_file", b"source_file", "stack_frame_with_id", b"stack_frame_with_id", "step", b"step", "wall_time", b"wall_time", "what", b"what"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["what", b"what"]) -> typing.Literal["debug_metadata", "source_file", "stack_frame_with_id", "graph_op_creation", "debugged_graph", "execution", "graph_execution_trace", "graph_id", "debugged_device"] | None: ...
 
 global___DebugEvent = DebugEvent
 
-@typing_extensions.final
+@typing.final
 class DebugMetadata(google.protobuf.message.Message):
     """Metadata about the debugger and the debugged TensorFlow program."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSORFLOW_VERSION_FIELD_NUMBER: builtins.int
     FILE_VERSION_FIELD_NUMBER: builtins.int
@@ -230,19 +239,19 @@
     def __init__(
         self,
         *,
         tensorflow_version: builtins.str | None = ...,
         file_version: builtins.str | None = ...,
         tfdbg_run_id: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_version", b"file_version", "tensorflow_version", b"tensorflow_version", "tfdbg_run_id", b"tfdbg_run_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_version", b"file_version", "tensorflow_version", b"tensorflow_version", "tfdbg_run_id", b"tfdbg_run_id"]) -> None: ...
 
 global___DebugMetadata = DebugMetadata
 
-@typing_extensions.final
+@typing.final
 class SourceFile(google.protobuf.message.Message):
     """Content of a source file involved in the execution of the debugged TensorFlow
     program.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -252,26 +261,27 @@
     file_path: builtins.str
     """Path to the file."""
     host_name: builtins.str
     """Name of the host on which the file is located."""
     @property
     def lines(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Line-by-line content of the file."""
+
     def __init__(
         self,
         *,
         file_path: builtins.str | None = ...,
         host_name: builtins.str | None = ...,
         lines: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_path", b"file_path", "host_name", b"host_name", "lines", b"lines"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_path", b"file_path", "host_name", b"host_name", "lines", b"lines"]) -> None: ...
 
 global___SourceFile = SourceFile
 
-@typing_extensions.final
+@typing.final
 class StackFrameWithId(google.protobuf.message.Message):
     """A stack frame with ID."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     FILE_LINE_COL_FIELD_NUMBER: builtins.int
@@ -279,26 +289,27 @@
     """A unique ID for the stack frame: A UUID-like string."""
     @property
     def file_line_col(self) -> tensorflow.core.protobuf.graph_debug_info_pb2.GraphDebugInfo.FileLineCol:
         """Stack frame, i.e., a frame of a stack trace, containing information
         regarding the file name, line number, function name, code content
         of the line, and column number (if available).
         """
+
     def __init__(
         self,
         *,
         id: builtins.str | None = ...,
         file_line_col: tensorflow.core.protobuf.graph_debug_info_pb2.GraphDebugInfo.FileLineCol | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["file_line_col", b"file_line_col"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_line_col", b"file_line_col", "id", b"id"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["file_line_col", b"file_line_col"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["file_line_col", b"file_line_col", "id", b"id"]) -> None: ...
 
 global___StackFrameWithId = StackFrameWithId
 
-@typing_extensions.final
+@typing.final
 class CodeLocation(google.protobuf.message.Message):
     """Code location information: A stack trace with host-name information.
     Instead of encoding the detailed stack trace, this proto refers to IDs of
     stack frames stored as `StackFrameWithId` protos.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -309,25 +320,26 @@
     """Host name on which the source files are located."""
     @property
     def stack_frame_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """ID to a stack frame, each of which is pointed to
         by a unique ID. The ordering of the frames is consistent with Python's
         `traceback.extract_tb()`.
         """
+
     def __init__(
         self,
         *,
         host_name: builtins.str | None = ...,
         stack_frame_ids: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["host_name", b"host_name", "stack_frame_ids", b"stack_frame_ids"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["host_name", b"host_name", "stack_frame_ids", b"stack_frame_ids"]) -> None: ...
 
 global___CodeLocation = CodeLocation
 
-@typing_extensions.final
+@typing.final
 class GraphOpCreation(google.protobuf.message.Message):
     """The creation of an op in a TensorFlow Graph (e.g., FuncGraph in TF2)."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OP_TYPE_FIELD_NUMBER: builtins.int
     OP_NAME_FIELD_NUMBER: builtins.int
@@ -346,44 +358,47 @@
     """Name of the graph that the op is a part of (if available)."""
     graph_id: builtins.str
     """Unique ID of the graph (generated by debugger).
     This is the ID of the immediately-enclosing graph.
     """
     device_name: builtins.str
     """Name of the device that the op is assigned to (if available)."""
+    num_outputs: builtins.int
+    """Number of output tensors emitted by the op."""
     @property
     def input_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Names of the input tensors to the op."""
-    num_outputs: builtins.int
-    """Number of output tensors emitted by the op."""
+
     @property
     def code_location(self) -> global___CodeLocation:
         """The unique ID for code location (stack trace) of the op's creation."""
+
     @property
     def output_tensor_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Unique IDs for the output tensors of this op."""
+
     def __init__(
         self,
         *,
         op_type: builtins.str | None = ...,
         op_name: builtins.str | None = ...,
         graph_name: builtins.str | None = ...,
         graph_id: builtins.str | None = ...,
         device_name: builtins.str | None = ...,
         input_names: collections.abc.Iterable[builtins.str] | None = ...,
         num_outputs: builtins.int | None = ...,
         code_location: global___CodeLocation | None = ...,
         output_tensor_ids: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["code_location", b"code_location"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code_location", b"code_location", "device_name", b"device_name", "graph_id", b"graph_id", "graph_name", b"graph_name", "input_names", b"input_names", "num_outputs", b"num_outputs", "op_name", b"op_name", "op_type", b"op_type", "output_tensor_ids", b"output_tensor_ids"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["code_location", b"code_location"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["code_location", b"code_location", "device_name", b"device_name", "graph_id", b"graph_id", "graph_name", b"graph_name", "input_names", b"input_names", "num_outputs", b"num_outputs", "op_name", b"op_name", "op_type", b"op_type", "output_tensor_ids", b"output_tensor_ids"]) -> None: ...
 
 global___GraphOpCreation = GraphOpCreation
 
-@typing_extensions.final
+@typing.final
 class DebuggedGraph(google.protobuf.message.Message):
     """A debugger-instrumented graph."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRAPH_ID_FIELD_NUMBER: builtins.int
     GRAPH_NAME_FIELD_NUMBER: builtins.int
@@ -393,42 +408,43 @@
     OUTER_CONTEXT_ID_FIELD_NUMBER: builtins.int
     graph_id: builtins.str
     """An ID for the graph.
     This can be used up to look up graph names. Generated by the debugger.
     """
     graph_name: builtins.str
     """Name of the graph (if available)."""
-    @property
-    def instrumented_ops(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Names of the instrumented ops. This can be used to look up op name
-        based on the numeric-summary tensors (2nd column).
-        """
     original_graph_def: builtins.bytes
     """Original (uninstrumented) GraphDef (if available)."""
     instrumented_graph_def: builtins.bytes
     """An encoded version of a GraphDef.
     This graph may include the debugger-inserted ops.
     """
     outer_context_id: builtins.str
     """IDs of the immediate enclosing context (graph), if any."""
+    @property
+    def instrumented_ops(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Names of the instrumented ops. This can be used to look up op name
+        based on the numeric-summary tensors (2nd column).
+        """
+
     def __init__(
         self,
         *,
         graph_id: builtins.str | None = ...,
         graph_name: builtins.str | None = ...,
         instrumented_ops: collections.abc.Iterable[builtins.str] | None = ...,
         original_graph_def: builtins.bytes | None = ...,
         instrumented_graph_def: builtins.bytes | None = ...,
         outer_context_id: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["graph_id", b"graph_id", "graph_name", b"graph_name", "instrumented_graph_def", b"instrumented_graph_def", "instrumented_ops", b"instrumented_ops", "original_graph_def", b"original_graph_def", "outer_context_id", b"outer_context_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["graph_id", b"graph_id", "graph_name", b"graph_name", "instrumented_graph_def", b"instrumented_graph_def", "instrumented_ops", b"instrumented_ops", "original_graph_def", b"original_graph_def", "outer_context_id", b"outer_context_id"]) -> None: ...
 
 global___DebuggedGraph = DebuggedGraph
 
-@typing_extensions.final
+@typing.final
 class DebuggedDevice(google.protobuf.message.Message):
     """A device on which ops and/or tensors are instrumented by the debugger."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEVICE_NAME_FIELD_NUMBER: builtins.int
     DEVICE_ID_FIELD_NUMBER: builtins.int
@@ -442,19 +458,19 @@
     """
     def __init__(
         self,
         *,
         device_name: builtins.str | None = ...,
         device_id: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_id", b"device_id", "device_name", b"device_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device_id", b"device_id", "device_name", b"device_name"]) -> None: ...
 
 global___DebuggedDevice = DebuggedDevice
 
-@typing_extensions.final
+@typing.final
 class Execution(google.protobuf.message.Message):
     """Data relating to the eager execution of an op or a Graph.
     For a op that generates N output tensors (N >= 0), only one
     Execution proto will be used to describe the execution event.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -474,57 +490,62 @@
     """
     num_outputs: builtins.int
     """Number of output tensors."""
     graph_id: builtins.str
     """The graph that's executed: applicable only to the eager
     execution of a FuncGraph.
     """
+    tensor_debug_mode: global___TensorDebugMode.ValueType
+    """Type of the tensor value encapsulated in this proto."""
     @property
     def input_tensor_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """IDs of the input tensors (if available)."""
+
     @property
     def output_tensor_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """IDs of the output tensors (if availbable).
         If specified, must have the same length as tensor_protos.
         """
-    tensor_debug_mode: global___TensorDebugMode.ValueType
-    """Type of the tensor value encapsulated in this proto."""
+
     @property
     def tensor_protos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_pb2.TensorProto]:
         """Output Tensor values in the type described by `tensor_value_type`.
         The length of this should match `num_outputs`.
         """
+
     @property
     def code_location(self) -> global___CodeLocation:
         """Stack trace of the eager execution."""
+
     @property
     def output_tensor_device_ids(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Debugged-generated IDs of the devices on which the output tensors reside.
         To look up details about the device (e.g., name), cross-reference this
         field with the DebuggedDevice messages.
         """
+
     def __init__(
         self,
         *,
         op_type: builtins.str | None = ...,
         num_outputs: builtins.int | None = ...,
         graph_id: builtins.str | None = ...,
         input_tensor_ids: collections.abc.Iterable[builtins.int] | None = ...,
         output_tensor_ids: collections.abc.Iterable[builtins.int] | None = ...,
         tensor_debug_mode: global___TensorDebugMode.ValueType | None = ...,
         tensor_protos: collections.abc.Iterable[tensorflow.core.framework.tensor_pb2.TensorProto] | None = ...,
         code_location: global___CodeLocation | None = ...,
         output_tensor_device_ids: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["code_location", b"code_location"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["code_location", b"code_location", "graph_id", b"graph_id", "input_tensor_ids", b"input_tensor_ids", "num_outputs", b"num_outputs", "op_type", b"op_type", "output_tensor_device_ids", b"output_tensor_device_ids", "output_tensor_ids", b"output_tensor_ids", "tensor_debug_mode", b"tensor_debug_mode", "tensor_protos", b"tensor_protos"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["code_location", b"code_location"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["code_location", b"code_location", "graph_id", b"graph_id", "input_tensor_ids", b"input_tensor_ids", "num_outputs", b"num_outputs", "op_type", b"op_type", "output_tensor_device_ids", b"output_tensor_device_ids", "output_tensor_ids", b"output_tensor_ids", "tensor_debug_mode", b"tensor_debug_mode", "tensor_protos", b"tensor_protos"]) -> None: ...
 
 global___Execution = Execution
 
-@typing_extensions.final
+@typing.final
 class GraphExecutionTrace(google.protobuf.message.Message):
     """Data relating to an execution of a Graph (e.g., an eager execution of a
     FuncGraph).
     The values of the intermediate tensors computed in the graph are recorded
     in this proto. A graph execution may correspond to one or more pieces of
     `GraphExecutionTrace`, depending on whether the instrumented tensor values
     are summarized in an aggregated or separate fashion.
@@ -548,29 +569,30 @@
     """
     output_slot: builtins.int
     """Output slot of the tensor (applicable only in the case of the `FULL_TENSOR`
     trace level).
     """
     tensor_debug_mode: global___TensorDebugMode.ValueType
     """Type of the tensor value encapsulated in this proto."""
+    device_name: builtins.str
+    """Name of the device that the op belongs to."""
     @property
     def tensor_proto(self) -> tensorflow.core.framework.tensor_pb2.TensorProto:
         """Tensor value in the type described by `tensor_value_type`.
         This tensor may summarize the value of a single intermediate op of the
         graph, or those of multiple intermediate tensors.
         """
-    device_name: builtins.str
-    """Name of the device that the op belongs to."""
+
     def __init__(
         self,
         *,
         tfdbg_context_id: builtins.str | None = ...,
         op_name: builtins.str | None = ...,
         output_slot: builtins.int | None = ...,
         tensor_debug_mode: global___TensorDebugMode.ValueType | None = ...,
         tensor_proto: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
         device_name: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_proto", b"tensor_proto"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_name", b"device_name", "op_name", b"op_name", "output_slot", b"output_slot", "tensor_debug_mode", b"tensor_debug_mode", "tensor_proto", b"tensor_proto", "tfdbg_context_id", b"tfdbg_context_id"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_proto", b"tensor_proto"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["device_name", b"device_name", "op_name", b"op_name", "output_slot", b"output_slot", "tensor_debug_mode", b"tensor_debug_mode", "tensor_proto", b"tensor_proto", "tfdbg_context_id", b"tfdbg_context_id"]) -> None: ...
 
 global___GraphExecutionTrace = GraphExecutionTrace
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DebugTensorWatch(google.protobuf.message.Message):
     """Option for watching a node in TensorFlow Debugger (tfdbg)."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_NAME_FIELD_NUMBER: builtins.int
     OUTPUT_SLOT_FIELD_NUMBER: builtins.int
@@ -31,20 +32,25 @@
     output_slot: builtins.int
     """Output slot to watch.
     The semantics of output_slot == -1 is that all outputs of the node
     will be watched (i.e., a wildcard).
     Other negative values of output_slot are invalid and will lead to
     errors currently.
     """
+    tolerate_debug_op_creation_failures: builtins.bool
+    """Do not error out if debug op creation fails (e.g., due to dtype
+    incompatibility). Instead, just log the failure.
+    """
     @property
     def debug_ops(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Name(s) of the debugging op(s).
         One or more than one probes on a tensor.
         e.g., {"DebugIdentity", "DebugNanCount"}
         """
+
     @property
     def debug_urls(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """URL(s) for debug targets(s).
 
         Supported URL formats are:
           - file:///foo/tfdbg_dump: Writes out Event content to file
             /foo/tfdbg_dump.  Assumes all directories can be created if they don't
@@ -60,66 +66,64 @@
         N.B. Session::Run() supports concurrent invocations of the same inputs
         (feed keys), outputs and target nodes. If such concurrent invocations
         are to be debugged, the callers of Session::Run() must use distinct
         debug_urls to make sure that the streamed or dumped events do not overlap
         among the invocations.
         TODO(cais): More visible documentation of this in g3docs.
         """
-    tolerate_debug_op_creation_failures: builtins.bool
-    """Do not error out if debug op creation fails (e.g., due to dtype
-    incompatibility). Instead, just log the failure.
-    """
+
     def __init__(
         self,
         *,
         node_name: builtins.str | None = ...,
         output_slot: builtins.int | None = ...,
         debug_ops: collections.abc.Iterable[builtins.str] | None = ...,
         debug_urls: collections.abc.Iterable[builtins.str] | None = ...,
         tolerate_debug_op_creation_failures: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["debug_ops", b"debug_ops", "debug_urls", b"debug_urls", "node_name", b"node_name", "output_slot", b"output_slot", "tolerate_debug_op_creation_failures", b"tolerate_debug_op_creation_failures"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["debug_ops", b"debug_ops", "debug_urls", b"debug_urls", "node_name", b"node_name", "output_slot", b"output_slot", "tolerate_debug_op_creation_failures", b"tolerate_debug_op_creation_failures"]) -> None: ...
 
 global___DebugTensorWatch = DebugTensorWatch
 
-@typing_extensions.final
+@typing.final
 class DebugOptions(google.protobuf.message.Message):
     """Options for initializing DebuggerState in TensorFlow Debugger (tfdbg)."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEBUG_TENSOR_WATCH_OPTS_FIELD_NUMBER: builtins.int
     GLOBAL_STEP_FIELD_NUMBER: builtins.int
     RESET_DISK_BYTE_USAGE_FIELD_NUMBER: builtins.int
-    @property
-    def debug_tensor_watch_opts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DebugTensorWatch]:
-        """Debugging options"""
     global_step: builtins.int
     """Caller-specified global step count.
     Note that this is distinct from the session run count and the executor
     step count.
     """
     reset_disk_byte_usage: builtins.bool
     """Whether the total disk usage of tfdbg is to be reset to zero
     in this Session.run call. This is used by wrappers and hooks
     such as the local CLI ones to indicate that the dumped tensors
     are cleaned up from the disk after each Session.run.
     """
+    @property
+    def debug_tensor_watch_opts(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DebugTensorWatch]:
+        """Debugging options"""
+
     def __init__(
         self,
         *,
         debug_tensor_watch_opts: collections.abc.Iterable[global___DebugTensorWatch] | None = ...,
         global_step: builtins.int | None = ...,
         reset_disk_byte_usage: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["debug_tensor_watch_opts", b"debug_tensor_watch_opts", "global_step", b"global_step", "reset_disk_byte_usage", b"reset_disk_byte_usage"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["debug_tensor_watch_opts", b"debug_tensor_watch_opts", "global_step", b"global_step", "reset_disk_byte_usage", b"reset_disk_byte_usage"]) -> None: ...
 
 global___DebugOptions = DebugOptions
 
-@typing_extensions.final
+@typing.final
 class DebuggedSourceFile(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HOST_FIELD_NUMBER: builtins.int
     FILE_PATH_FIELD_NUMBER: builtins.int
     LAST_MODIFIED_FIELD_NUMBER: builtins.int
     BYTES_FIELD_NUMBER: builtins.int
@@ -131,36 +135,38 @@
     last_modified: builtins.int
     """The timestamp at which the source code file is last modified."""
     bytes: builtins.int
     """Byte size of the file."""
     @property
     def lines(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Line-by-line content of the source code file."""
+
     def __init__(
         self,
         *,
         host: builtins.str | None = ...,
         file_path: builtins.str | None = ...,
         last_modified: builtins.int | None = ...,
         bytes: builtins.int | None = ...,
         lines: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bytes", b"bytes", "file_path", b"file_path", "host", b"host", "last_modified", b"last_modified", "lines", b"lines"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bytes", b"bytes", "file_path", b"file_path", "host", b"host", "last_modified", b"last_modified", "lines", b"lines"]) -> None: ...
 
 global___DebuggedSourceFile = DebuggedSourceFile
 
-@typing_extensions.final
+@typing.final
 class DebuggedSourceFiles(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_FILES_FIELD_NUMBER: builtins.int
     @property
     def source_files(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DebuggedSourceFile]:
         """A collection of source code files."""
+
     def __init__(
         self,
         *,
         source_files: collections.abc.Iterable[global___DebuggedSourceFile] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["source_files", b"source_files"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["source_files", b"source_files"]) -> None: ...
 
 global___DebuggedSourceFiles = DebuggedSourceFiles
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TaskDeviceFilters(google.protobuf.message.Message):
     """This file contains protos to be used when defining a TensorFlow
     cluster.
 
     Configure device filters for remote tasks in the cluster. When associated
     with a ClusterDef in setting up the cluster, a remote task will ignore all
     devices which do not match any of its filters. Device filters must be
@@ -67,69 +68,70 @@
     @property
     def device_filters(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
         device_filters: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_filters", b"device_filters"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device_filters", b"device_filters"]) -> None: ...
 
 global___TaskDeviceFilters = TaskDeviceFilters
 
-@typing_extensions.final
+@typing.final
 class JobDeviceFilters(google.protobuf.message.Message):
     """Defines the device filters for tasks in a job."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class TasksEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         @property
         def value(self) -> global___TaskDeviceFilters: ...
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: global___TaskDeviceFilters | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     TASKS_FIELD_NUMBER: builtins.int
     name: builtins.str
     """The name of this job."""
     @property
     def tasks(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___TaskDeviceFilters]:
         """Mapping from task ID to task device filters."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         tasks: collections.abc.Mapping[builtins.int, global___TaskDeviceFilters] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "tasks", b"tasks"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "tasks", b"tasks"]) -> None: ...
 
 global___JobDeviceFilters = JobDeviceFilters
 
-@typing_extensions.final
+@typing.final
 class ClusterDeviceFilters(google.protobuf.message.Message):
     """Defines the device filters for jobs in a cluster."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOBS_FIELD_NUMBER: builtins.int
     @property
     def jobs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___JobDeviceFilters]: ...
     def __init__(
         self,
         *,
         jobs: collections.abc.Iterable[global___JobDeviceFilters] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["jobs", b"jobs"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["jobs", b"jobs"]) -> None: ...
 
 global___ClusterDeviceFilters = ClusterDeviceFilters
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,43 +12,44 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DeviceProperties(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class EnvironmentEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     TYPE_FIELD_NUMBER: builtins.int
     VENDOR_FIELD_NUMBER: builtins.int
     MODEL_FIELD_NUMBER: builtins.int
     FREQUENCY_FIELD_NUMBER: builtins.int
     NUM_CORES_FIELD_NUMBER: builtins.int
     ENVIRONMENT_FIELD_NUMBER: builtins.int
@@ -65,19 +66,14 @@
     """Vendor (Intel, nvidia, ...)"""
     model: builtins.str
     """Model (Haswell, K40, ...)"""
     frequency: builtins.int
     """Core Frequency in Mhz"""
     num_cores: builtins.int
     """Number of cores"""
-    @property
-    def environment(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
-        """Version of the tools and libraries used with this device (e.g. gcc 4.9,
-        cudnn 5.1)
-        """
     num_registers: builtins.int
     """Number of registers per core."""
     l1_cache_size: builtins.int
     """L1 cache size in bytes"""
     l2_cache_size: builtins.int
     """L2 cache size in bytes"""
     l3_cache_size: builtins.int
@@ -86,14 +82,20 @@
     """Shared memory size per multiprocessor in bytes. This field is
     applicable to GPUs only.
     """
     memory_size: builtins.int
     """Memory size in bytes"""
     bandwidth: builtins.int
     """Memory bandwidth in KB/s"""
+    @property
+    def environment(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
+        """Version of the tools and libraries used with this device (e.g. gcc 4.9,
+        cudnn 5.1)
+        """
+
     def __init__(
         self,
         *,
         type: builtins.str | None = ...,
         vendor: builtins.str | None = ...,
         model: builtins.str | None = ...,
         frequency: builtins.int | None = ...,
@@ -103,30 +105,30 @@
         l1_cache_size: builtins.int | None = ...,
         l2_cache_size: builtins.int | None = ...,
         l3_cache_size: builtins.int | None = ...,
         shared_memory_size_per_multiprocessor: builtins.int | None = ...,
         memory_size: builtins.int | None = ...,
         bandwidth: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bandwidth", b"bandwidth", "environment", b"environment", "frequency", b"frequency", "l1_cache_size", b"l1_cache_size", "l2_cache_size", b"l2_cache_size", "l3_cache_size", b"l3_cache_size", "memory_size", b"memory_size", "model", b"model", "num_cores", b"num_cores", "num_registers", b"num_registers", "shared_memory_size_per_multiprocessor", b"shared_memory_size_per_multiprocessor", "type", b"type", "vendor", b"vendor"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bandwidth", b"bandwidth", "environment", b"environment", "frequency", b"frequency", "l1_cache_size", b"l1_cache_size", "l2_cache_size", b"l2_cache_size", "l3_cache_size", b"l3_cache_size", "memory_size", b"memory_size", "model", b"model", "num_cores", b"num_cores", "num_registers", b"num_registers", "shared_memory_size_per_multiprocessor", b"shared_memory_size_per_multiprocessor", "type", b"type", "vendor", b"vendor"]) -> None: ...
 
 global___DeviceProperties = DeviceProperties
 
-@typing_extensions.final
+@typing.final
 class NamedDevice(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def properties(self) -> global___DeviceProperties: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         properties: global___DeviceProperties | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["properties", b"properties"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "properties", b"properties"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["properties", b"properties"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "properties", b"properties"]) -> None: ...
 
 global___NamedDevice = NamedDevice
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GrpcPayloadContainer(google.protobuf.message.Message):
     """Used to serialize and transmit tensorflow::Status payloads through
     grpc::Status `error_details` since grpc::Status lacks payload API.
     TODO(b/204231601): Use GRPC API once supported.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class PayloadsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.bytes
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.bytes | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     PAYLOADS_FIELD_NUMBER: builtins.int
     @property
     def payloads(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.bytes]: ...
     def __init__(
         self,
         *,
         payloads: collections.abc.Mapping[builtins.str, builtins.bytes] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["payloads", b"payloads"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["payloads", b"payloads"]) -> None: ...
 
 global___GrpcPayloadContainer = GrpcPayloadContainer
 
-@typing_extensions.final
+@typing.final
 class GrpcPayloadsLost(google.protobuf.message.Message):
     """If included as a payload, this message flags the Status to have lost payloads
     during the GRPC transmission.
     URI: "type.googleapis.com/tensorflow.distributed_runtime.GrpcPayloadsLost"
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GrpcPayloadsLost = GrpcPayloadsLost
 
-@typing_extensions.final
+@typing.final
 class WorkerPossiblyRestarted(google.protobuf.message.Message):
     """If included as a payload, this message flags the Status to be a possible
     outcome of a worker restart.
     URI:
     "type.googleapis.com/tensorflow.distributed_runtime.WorkerPossiblyRestarted"
     """
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Add a dummy package name. Having no package, like
 core/lib/core/error_codes.proto, or having tensorflow.error, like
 tsl/protobuf/error_codes.proto, results in name collision errors in generated
 code for some users that use JS through J2CL.
 """
+
 import google.protobuf.descriptor
 from tensorflow.tsl.protobuf.error_codes_pb2 import (
     ABORTED as ABORTED,
     ALREADY_EXISTS as ALREADY_EXISTS,
     CANCELLED as CANCELLED,
     DATA_LOSS as DATA_LOSS,
     DEADLINE_EXCEEDED as DEADLINE_EXCEEDED,
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.framework.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class FingerprintDef(google.protobuf.message.Message):
     """Protocol buffer representing a SavedModel Fingerprint.
 
     If there are multiple MetaGraphDefs in the SavedModel, the FingerprintDef
     corresponds to the first one.
     """
 
@@ -36,21 +37,22 @@
     saved_object_graph_hash: builtins.int
     """Hash of the regularized SavedObjectGraph."""
     checkpoint_hash: builtins.int
     """Hash of the checkpoint."""
     @property
     def version(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
         """Version specification of the fingerprint."""
+
     def __init__(
         self,
         *,
         saved_model_checksum: builtins.int | None = ...,
         graph_def_program_hash: builtins.int | None = ...,
         signature_def_hash: builtins.int | None = ...,
         saved_object_graph_hash: builtins.int | None = ...,
         checkpoint_hash: builtins.int | None = ...,
         version: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["version", b"version"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_hash", b"checkpoint_hash", "graph_def_program_hash", b"graph_def_program_hash", "saved_model_checksum", b"saved_model_checksum", "saved_object_graph_hash", b"saved_object_graph_hash", "signature_def_hash", b"signature_def_hash", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["version", b"version"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["checkpoint_hash", b"checkpoint_hash", "graph_def_program_hash", b"graph_def_program_hash", "saved_model_checksum", b"saved_model_checksum", "saved_object_graph_hash", b"saved_object_graph_hash", "signature_def_hash", b"signature_def_hash", "version", b"version"]) -> None: ...
 
 global___FingerprintDef = FingerprintDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class GraphDebugInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FileLineCol(google.protobuf.message.Message):
         """This represents a file/line location in the source code."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         FILE_INDEX_FIELD_NUMBER: builtins.int
         LINE_FIELD_NUMBER: builtins.int
@@ -44,73 +45,76 @@
             *,
             file_index: builtins.int | None = ...,
             line: builtins.int | None = ...,
             col: builtins.int | None = ...,
             func: builtins.str | None = ...,
             code: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["code", b"code", "col", b"col", "file_index", b"file_index", "func", b"func", "line", b"line"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["code", b"code", "col", b"col", "file_index", b"file_index", "func", b"func", "line", b"line"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class StackTrace(google.protobuf.message.Message):
         """This represents a stack trace which is a ordered list of `FileLineCol`."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         FILE_LINE_COLS_FIELD_NUMBER: builtins.int
         @property
         def file_line_cols(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GraphDebugInfo.FileLineCol]:
             """Each line in the stack trace."""
+
         def __init__(
             self,
             *,
             file_line_cols: collections.abc.Iterable[global___GraphDebugInfo.FileLineCol] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["file_line_cols", b"file_line_cols"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["file_line_cols", b"file_line_cols"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class TracesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___GraphDebugInfo.StackTrace: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___GraphDebugInfo.StackTrace | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FILES_FIELD_NUMBER: builtins.int
     TRACES_FIELD_NUMBER: builtins.int
     @property
     def files(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """This stores all the source code file names and can be indexed by the
         `file_index`.
         """
+
     @property
     def traces(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___GraphDebugInfo.StackTrace]:
         """This maps a node name to a stack trace in the source code.
         The map key is a mangling of the containing function and op name with
         syntax:
           op.name '@' func_name
         For ops in the top-level graph, the func_name is the empty string.
         Note that op names are restricted to a small number of characters which
         exclude '@', making it impossible to collide keys of this form. Function
         names accept a much wider set of characters.
         It would be preferable to avoid mangling and use a tuple key of (op.name,
         func_name), but this is not supported with protocol buffers.
         """
+
     def __init__(
         self,
         *,
         files: collections.abc.Iterable[builtins.str] | None = ...,
         traces: collections.abc.Mapping[builtins.str, global___GraphDebugInfo.StackTrace] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["files", b"files", "traces", b"traces"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["files", b"files", "traces", b"traces"]) -> None: ...
 
 global___GraphDebugInfo = GraphDebugInfo
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.graph_pb2
 import tensorflow.core.framework.op_def_pb2
@@ -16,15 +17,15 @@
 import tensorflow.core.framework.types_pb2
 import tensorflow.core.protobuf.saved_object_graph_pb2
 import tensorflow.core.protobuf.saver_pb2
 import tensorflow.core.protobuf.struct_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class MetaGraphDef(google.protobuf.message.Message):
     """Protocol buffer containing the following which are necessary to restart
     training, run inference. It can be used to serialize/de-serialize memory
     objects necessary for running computation in a graph when crossing the
     process boundary. It can be used for long term storage of graphs,
     cross-language execution of graphs, etc.
       MetaInfoDef
@@ -33,185 +34,195 @@
       CollectionDef
       TensorInfo
       SignatureDef
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class MetaInfoDef(google.protobuf.message.Message):
         """Meta information regarding the graph to be exported.  To be used by users
         of this protocol buffer to encode information regarding their meta graph.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class FunctionAliasesEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: builtins.str
             value: builtins.str
             def __init__(
                 self,
                 *,
                 key: builtins.str | None = ...,
                 value: builtins.str | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         META_GRAPH_VERSION_FIELD_NUMBER: builtins.int
         STRIPPED_OP_LIST_FIELD_NUMBER: builtins.int
         ANY_INFO_FIELD_NUMBER: builtins.int
         TAGS_FIELD_NUMBER: builtins.int
         TENSORFLOW_VERSION_FIELD_NUMBER: builtins.int
         TENSORFLOW_GIT_VERSION_FIELD_NUMBER: builtins.int
         STRIPPED_DEFAULT_ATTRS_FIELD_NUMBER: builtins.int
         FUNCTION_ALIASES_FIELD_NUMBER: builtins.int
         meta_graph_version: builtins.str
         """User specified Version string. Can be the name of the model and revision,
         steps this model has been trained to, etc.
         """
+        tensorflow_version: builtins.str
+        """The __version__ string of the tensorflow build used to write this graph.
+        This will be populated by the framework, which will overwrite any user
+        supplied value.
+        """
+        tensorflow_git_version: builtins.str
+        """The __git_version__ string of the tensorflow build used to write this
+        graph. This will be populated by the framework, which will overwrite any
+        user supplied value.
+        """
+        stripped_default_attrs: builtins.bool
+        """A flag to denote whether default-valued attrs have been stripped from
+        the nodes in this graph_def.
+        """
         @property
         def stripped_op_list(self) -> tensorflow.core.framework.op_def_pb2.OpList:
             """A copy of the OpDefs used by the producer of this graph_def.
             Descriptions and Ops not used in graph_def are stripped out.
             """
+
         @property
         def any_info(self) -> google.protobuf.any_pb2.Any:
             """A serialized protobuf. Can be the time this meta graph is created, or
             modified, or name of the model.
             """
+
         @property
         def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
             """User supplied tag(s) on the meta_graph and included graph_def.
 
             MetaGraphDefs should be tagged with their capabilities or use-cases.
             Examples: "train", "serve", "gpu", "tpu", etc.
             These tags enable loaders to access the MetaGraph(s) appropriate for a
             specific use-case or runtime environment.
             """
-        tensorflow_version: builtins.str
-        """The __version__ string of the tensorflow build used to write this graph.
-        This will be populated by the framework, which will overwrite any user
-        supplied value.
-        """
-        tensorflow_git_version: builtins.str
-        """The __git_version__ string of the tensorflow build used to write this
-        graph. This will be populated by the framework, which will overwrite any
-        user supplied value.
-        """
-        stripped_default_attrs: builtins.bool
-        """A flag to denote whether default-valued attrs have been stripped from
-        the nodes in this graph_def.
-        """
+
         @property
         def function_aliases(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
             """FunctionDef name to aliases mapping."""
+
         def __init__(
             self,
             *,
             meta_graph_version: builtins.str | None = ...,
             stripped_op_list: tensorflow.core.framework.op_def_pb2.OpList | None = ...,
             any_info: google.protobuf.any_pb2.Any | None = ...,
             tags: collections.abc.Iterable[builtins.str] | None = ...,
             tensorflow_version: builtins.str | None = ...,
             tensorflow_git_version: builtins.str | None = ...,
             stripped_default_attrs: builtins.bool | None = ...,
             function_aliases: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["any_info", b"any_info", "stripped_op_list", b"stripped_op_list"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["any_info", b"any_info", "function_aliases", b"function_aliases", "meta_graph_version", b"meta_graph_version", "stripped_default_attrs", b"stripped_default_attrs", "stripped_op_list", b"stripped_op_list", "tags", b"tags", "tensorflow_git_version", b"tensorflow_git_version", "tensorflow_version", b"tensorflow_version"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["any_info", b"any_info", "stripped_op_list", b"stripped_op_list"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["any_info", b"any_info", "function_aliases", b"function_aliases", "meta_graph_version", b"meta_graph_version", "stripped_default_attrs", b"stripped_default_attrs", "stripped_op_list", b"stripped_op_list", "tags", b"tags", "tensorflow_git_version", b"tensorflow_git_version", "tensorflow_version", b"tensorflow_version"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class CollectionDefEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___CollectionDef: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___CollectionDef | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class SignatureDefEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___SignatureDef: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___SignatureDef | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     META_INFO_DEF_FIELD_NUMBER: builtins.int
     GRAPH_DEF_FIELD_NUMBER: builtins.int
     SAVER_DEF_FIELD_NUMBER: builtins.int
     COLLECTION_DEF_FIELD_NUMBER: builtins.int
     SIGNATURE_DEF_FIELD_NUMBER: builtins.int
     ASSET_FILE_DEF_FIELD_NUMBER: builtins.int
     OBJECT_GRAPH_DEF_FIELD_NUMBER: builtins.int
     @property
     def meta_info_def(self) -> global___MetaGraphDef.MetaInfoDef: ...
     @property
     def graph_def(self) -> tensorflow.core.framework.graph_pb2.GraphDef:
         """GraphDef."""
+
     @property
     def saver_def(self) -> tensorflow.core.protobuf.saver_pb2.SaverDef:
         """SaverDef."""
+
     @property
     def collection_def(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___CollectionDef]:
         """collection_def: Map from collection name to collections.
         See CollectionDef section for details.
         """
+
     @property
     def signature_def(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___SignatureDef]:
         """signature_def: Map from user supplied key for a signature to a single
         SignatureDef.
         """
+
     @property
     def asset_file_def(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AssetFileDef]:
         """Asset file def to be used with the defined graph."""
+
     @property
     def object_graph_def(self) -> tensorflow.core.protobuf.saved_object_graph_pb2.SavedObjectGraph:
         """Extra information about the structure of functions and stateful objects."""
+
     def __init__(
         self,
         *,
         meta_info_def: global___MetaGraphDef.MetaInfoDef | None = ...,
         graph_def: tensorflow.core.framework.graph_pb2.GraphDef | None = ...,
         saver_def: tensorflow.core.protobuf.saver_pb2.SaverDef | None = ...,
         collection_def: collections.abc.Mapping[builtins.str, global___CollectionDef] | None = ...,
         signature_def: collections.abc.Mapping[builtins.str, global___SignatureDef] | None = ...,
         asset_file_def: collections.abc.Iterable[global___AssetFileDef] | None = ...,
         object_graph_def: tensorflow.core.protobuf.saved_object_graph_pb2.SavedObjectGraph | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["graph_def", b"graph_def", "meta_info_def", b"meta_info_def", "object_graph_def", b"object_graph_def", "saver_def", b"saver_def"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["asset_file_def", b"asset_file_def", "collection_def", b"collection_def", "graph_def", b"graph_def", "meta_info_def", b"meta_info_def", "object_graph_def", b"object_graph_def", "saver_def", b"saver_def", "signature_def", b"signature_def"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["graph_def", b"graph_def", "meta_info_def", b"meta_info_def", "object_graph_def", b"object_graph_def", "saver_def", b"saver_def"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["asset_file_def", b"asset_file_def", "collection_def", b"collection_def", "graph_def", b"graph_def", "meta_info_def", b"meta_info_def", "object_graph_def", b"object_graph_def", "saver_def", b"saver_def", "signature_def", b"signature_def"]) -> None: ...
 
 global___MetaGraphDef = MetaGraphDef
 
-@typing_extensions.final
+@typing.final
 class CollectionDef(google.protobuf.message.Message):
     """CollectionDef should cover most collections.
     To add a user-defined collection, do one of the following:
     1. For simple data types, such as string, int, float:
          tf.add_to_collection("your_collection_name", your_simple_value)
        strings will be stored as bytes_list.
 
@@ -271,15 +282,15 @@
                                    proto_type=variable_pb2.VariableDef,
                                    to_proto=Variable.to_proto,
                                    from_proto=Variable.from_proto)
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class NodeList(google.protobuf.message.Message):
         """NodeList is used for collecting nodes in graph. For example
         collection_def {
           key: "summaries"
           value {
             node_list {
               value: "input_producer/ScalarSummary:0"
@@ -295,17 +306,17 @@
         @property
         def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
         def __init__(
             self,
             *,
             value: collections.abc.Iterable[builtins.str] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class BytesList(google.protobuf.message.Message):
         """BytesList is used for collecting strings and serialized protobufs. For
         example:
         collection_def {
           key: "trainable_variables"
           value {
             bytes_list {
@@ -324,63 +335,63 @@
         @property
         def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]: ...
         def __init__(
             self,
             *,
             value: collections.abc.Iterable[builtins.bytes] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class Int64List(google.protobuf.message.Message):
         """Int64List is used for collecting int, int64 and long values."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         VALUE_FIELD_NUMBER: builtins.int
         @property
         def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
         def __init__(
             self,
             *,
             value: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class FloatList(google.protobuf.message.Message):
         """FloatList is used for collecting float values."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         VALUE_FIELD_NUMBER: builtins.int
         @property
         def value(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
         def __init__(
             self,
             *,
             value: collections.abc.Iterable[builtins.float] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class AnyList(google.protobuf.message.Message):
         """AnyList is used for collecting Any protos."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         VALUE_FIELD_NUMBER: builtins.int
         @property
         def value(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]: ...
         def __init__(
             self,
             *,
             value: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["value", b"value"]) -> None: ...
 
     NODE_LIST_FIELD_NUMBER: builtins.int
     BYTES_LIST_FIELD_NUMBER: builtins.int
     INT64_LIST_FIELD_NUMBER: builtins.int
     FLOAT_LIST_FIELD_NUMBER: builtins.int
     ANY_LIST_FIELD_NUMBER: builtins.int
     @property
@@ -398,27 +409,27 @@
         *,
         node_list: global___CollectionDef.NodeList | None = ...,
         bytes_list: global___CollectionDef.BytesList | None = ...,
         int64_list: global___CollectionDef.Int64List | None = ...,
         float_list: global___CollectionDef.FloatList | None = ...,
         any_list: global___CollectionDef.AnyList | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["any_list", b"any_list", "bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind", "node_list", b"node_list"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["any_list", b"any_list", "bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind", "node_list", b"node_list"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["node_list", "bytes_list", "int64_list", "float_list", "any_list"] | None: ...
+    def HasField(self, field_name: typing.Literal["any_list", b"any_list", "bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind", "node_list", b"node_list"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["any_list", b"any_list", "bytes_list", b"bytes_list", "float_list", b"float_list", "int64_list", b"int64_list", "kind", b"kind", "node_list", b"node_list"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["node_list", "bytes_list", "int64_list", "float_list", "any_list"] | None: ...
 
 global___CollectionDef = CollectionDef
 
-@typing_extensions.final
+@typing.final
 class TensorInfo(google.protobuf.message.Message):
     """Information about a Tensor necessary for feeding or retrieval."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class CooSparse(google.protobuf.message.Message):
         """For sparse tensors, The COO encoding stores a triple of values, indices,
         and shape.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -438,79 +449,84 @@
         def __init__(
             self,
             *,
             values_tensor_name: builtins.str | None = ...,
             indices_tensor_name: builtins.str | None = ...,
             dense_shape_tensor_name: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["dense_shape_tensor_name", b"dense_shape_tensor_name", "indices_tensor_name", b"indices_tensor_name", "values_tensor_name", b"values_tensor_name"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["dense_shape_tensor_name", b"dense_shape_tensor_name", "indices_tensor_name", b"indices_tensor_name", "values_tensor_name", b"values_tensor_name"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class CompositeTensor(google.protobuf.message.Message):
         """Generic encoding for composite tensors."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         TYPE_SPEC_FIELD_NUMBER: builtins.int
         COMPONENTS_FIELD_NUMBER: builtins.int
         @property
         def type_spec(self) -> tensorflow.core.protobuf.struct_pb2.TypeSpecProto:
             """The serialized TypeSpec for the composite tensor."""
+
         @property
         def components(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorInfo]:
             """A TensorInfo for each flattened component tensor."""
+
         def __init__(
             self,
             *,
             type_spec: tensorflow.core.protobuf.struct_pb2.TypeSpecProto | None = ...,
             components: collections.abc.Iterable[global___TensorInfo] | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["type_spec", b"type_spec"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["components", b"components", "type_spec", b"type_spec"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["type_spec", b"type_spec"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["components", b"components", "type_spec", b"type_spec"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     COO_SPARSE_FIELD_NUMBER: builtins.int
     COMPOSITE_TENSOR_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     TENSOR_SHAPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     """For dense `Tensor`s, the name of the tensor in the graph."""
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def coo_sparse(self) -> global___TensorInfo.CooSparse:
         """There are many possible encodings of sparse matrices
         (https://en.wikipedia.org/wiki/Sparse_matrix).  Currently, TensorFlow
         uses only the COO encoding.  This is supported and documented in the
         SparseTensor Python class.
         """
+
     @property
     def composite_tensor(self) -> global___TensorInfo.CompositeTensor:
         """Generic encoding for CompositeTensors."""
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
+
     @property
     def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """The static shape should be recorded here, to the extent that it can
         be known in advance.  In the case of a SparseTensor, this field describes
         the logical shape of the represented tensor (aka dense_shape).
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         coo_sparse: global___TensorInfo.CooSparse | None = ...,
         composite_tensor: global___TensorInfo.CompositeTensor | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         tensor_shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["composite_tensor", b"composite_tensor", "coo_sparse", b"coo_sparse", "encoding", b"encoding", "name", b"name", "tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["composite_tensor", b"composite_tensor", "coo_sparse", b"coo_sparse", "dtype", b"dtype", "encoding", b"encoding", "name", b"name", "tensor_shape", b"tensor_shape"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["encoding", b"encoding"]) -> typing_extensions.Literal["name", "coo_sparse", "composite_tensor"] | None: ...
+    def HasField(self, field_name: typing.Literal["composite_tensor", b"composite_tensor", "coo_sparse", b"coo_sparse", "encoding", b"encoding", "name", b"name", "tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["composite_tensor", b"composite_tensor", "coo_sparse", b"coo_sparse", "dtype", b"dtype", "encoding", b"encoding", "name", b"name", "tensor_shape", b"tensor_shape"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["encoding", b"encoding"]) -> typing.Literal["name", "coo_sparse", "composite_tensor"] | None: ...
 
 global___TensorInfo = TensorInfo
 
-@typing_extensions.final
+@typing.final
 class SignatureDef(google.protobuf.message.Message):
     """SignatureDef defines the signature of a computation supported by a TensorFlow
     graph.
 
     For example, a model with two loss computations, sharing a single input,
     might have the following signature_def map, in a MetaGraphDef message.
 
@@ -565,101 +581,104 @@
       }
       ...
     }
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class InputsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___TensorInfo: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___TensorInfo | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class OutputsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___TensorInfo: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___TensorInfo | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     INPUTS_FIELD_NUMBER: builtins.int
     OUTPUTS_FIELD_NUMBER: builtins.int
     METHOD_NAME_FIELD_NUMBER: builtins.int
-    @property
-    def inputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
-        """Named input parameters."""
-    @property
-    def outputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
-        """Named output parameters."""
     method_name: builtins.str
     """Extensible method_name information enabling third-party users to mark a
     SignatureDef as supporting a particular method. This enables producers and
     consumers of SignatureDefs, e.g. a model definition library and a serving
     library to have a clear hand-off regarding the semantics of a computation.
 
     Note that multiple SignatureDefs in a single MetaGraphDef may have the same
     method_name. This is commonly used to support multi-headed computation,
     where a single graph computation may return multiple results.
     """
+    @property
+    def inputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
+        """Named input parameters."""
+
+    @property
+    def outputs(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___TensorInfo]:
+        """Named output parameters."""
+
     def __init__(
         self,
         *,
         inputs: collections.abc.Mapping[builtins.str, global___TensorInfo] | None = ...,
         outputs: collections.abc.Mapping[builtins.str, global___TensorInfo] | None = ...,
         method_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["inputs", b"inputs", "method_name", b"method_name", "outputs", b"outputs"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["inputs", b"inputs", "method_name", b"method_name", "outputs", b"outputs"]) -> None: ...
 
 global___SignatureDef = SignatureDef
 
-@typing_extensions.final
+@typing.final
 class AssetFileDef(google.protobuf.message.Message):
     """An asset file def for a single file or a set of sharded files with the same
     name.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_INFO_FIELD_NUMBER: builtins.int
     FILENAME_FIELD_NUMBER: builtins.int
-    @property
-    def tensor_info(self) -> global___TensorInfo:
-        """The tensor to bind the asset filename to."""
     filename: builtins.str
     """The filename within an assets directory. Note: does not include the path
     prefix, i.e. directories. For an asset at /tmp/path/vocab.txt, the filename
     would be "vocab.txt".
     """
+    @property
+    def tensor_info(self) -> global___TensorInfo:
+        """The tensor to bind the asset filename to."""
+
     def __init__(
         self,
         *,
         tensor_info: global___TensorInfo | None = ...,
         filename: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_info", b"tensor_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["filename", b"filename", "tensor_info", b"tensor_info"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_info", b"tensor_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["filename", b"filename", "tensor_info", b"tensor_info"]) -> None: ...
 
 global___AssetFileDef = AssetFileDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class NamedTensorProto(google.protobuf.message.Message):
     """A pair of tensor name and tensor values."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TENSOR_FIELD_NUMBER: builtins.int
@@ -26,17 +27,18 @@
         """The client can populate a TensorProto using a tensorflow::Tensor`, or
         directly using the protobuf field accessors.
 
         The client specifies whether the returned tensor values should be
         filled tensor fields (float_val, int_val, etc.) or encoded in a
         compact form in tensor.tensor_content.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         tensor: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor", b"tensor"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "tensor", b"tensor"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor", b"tensor"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "tensor", b"tensor"]) -> None: ...
 
 global___NamedTensorProto = NamedTensorProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.tsl.protobuf.error_codes_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class QueueRunnerDef(google.protobuf.message.Message):
     """Protocol buffer representing a QueueRunner."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     QUEUE_NAME_FIELD_NUMBER: builtins.int
     ENQUEUE_OP_NAME_FIELD_NUMBER: builtins.int
     CLOSE_OP_NAME_FIELD_NUMBER: builtins.int
     CANCEL_OP_NAME_FIELD_NUMBER: builtins.int
     QUEUE_CLOSED_EXCEPTION_TYPES_FIELD_NUMBER: builtins.int
     queue_name: builtins.str
     """Queue name."""
-    @property
-    def enqueue_op_name(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """A list of enqueue operations."""
     close_op_name: builtins.str
     """The operation to run to close the queue."""
     cancel_op_name: builtins.str
     """The operation to run to cancel the queue."""
     @property
+    def enqueue_op_name(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """A list of enqueue operations."""
+
+    @property
     def queue_closed_exception_types(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[tensorflow.tsl.protobuf.error_codes_pb2.Code.ValueType]:
         """A list of exception types considered to signal a safely closed queue
         if raised during enqueue operations.
         """
+
     def __init__(
         self,
         *,
         queue_name: builtins.str | None = ...,
         enqueue_op_name: collections.abc.Iterable[builtins.str] | None = ...,
         close_op_name: builtins.str | None = ...,
         cancel_op_name: builtins.str | None = ...,
         queue_closed_exception_types: collections.abc.Iterable[tensorflow.tsl.protobuf.error_codes_pb2.Code.ValueType] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cancel_op_name", b"cancel_op_name", "close_op_name", b"close_op_name", "enqueue_op_name", b"enqueue_op_name", "queue_closed_exception_types", b"queue_closed_exception_types", "queue_name", b"queue_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cancel_op_name", b"cancel_op_name", "close_op_name", b"close_op_name", "enqueue_op_name", b"enqueue_op_name", "queue_closed_exception_types", b"queue_closed_exception_types", "queue_name", b"queue_name"]) -> None: ...
 
 global___QueueRunnerDef = QueueRunnerDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ResourceDtypeAndShape(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "shape", b"shape"]) -> None: ...
 
 global___ResourceDtypeAndShape = ResourceDtypeAndShape
 
-@typing_extensions.final
+@typing.final
 class RemoteTensorHandle(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OP_ID_FIELD_NUMBER: builtins.int
     OUTPUT_NUM_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     OP_DEVICE_FIELD_NUMBER: builtins.int
@@ -57,20 +58,21 @@
     operation producing this tensor is a multi-device function.
     """
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     """Tensor type."""
     @property
     def resource_dtypes_and_shapes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ResourceDtypeAndShape]:
         """Optional data types and shapes of a remote resource variable."""
+
     def __init__(
         self,
         *,
         op_id: builtins.int | None = ...,
         output_num: builtins.int | None = ...,
         device: builtins.str | None = ...,
         op_device: builtins.str | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         resource_dtypes_and_shapes: collections.abc.Iterable[global___ResourceDtypeAndShape] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device", "dtype", b"dtype", "op_device", b"op_device", "op_id", b"op_id", "output_num", b"output_num", "resource_dtypes_and_shapes", b"resource_dtypes_and_shapes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device", b"device", "dtype", b"dtype", "op_device", b"op_device", "op_id", b"op_id", "output_num", b"output_num", "resource_dtypes_and_shapes", b"resource_dtypes_and_shapes"]) -> None: ...
 
 global___RemoteTensorHandle = RemoteTensorHandle
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -17,50 +18,51 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class AutoParallelOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENABLE_FIELD_NUMBER: builtins.int
     NUM_REPLICAS_FIELD_NUMBER: builtins.int
     enable: builtins.bool
     num_replicas: builtins.int
     def __init__(
         self,
         *,
         enable: builtins.bool | None = ...,
         num_replicas: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enable", b"enable", "num_replicas", b"num_replicas"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["enable", b"enable", "num_replicas", b"num_replicas"]) -> None: ...
 
 global___AutoParallelOptions = AutoParallelOptions
 
-@typing_extensions.final
+@typing.final
 class ScopedAllocatorOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENABLE_OP_FIELD_NUMBER: builtins.int
     @property
     def enable_op(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """If present, only perform optimization for these ops."""
+
     def __init__(
         self,
         *,
         enable_op: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enable_op", b"enable_op"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["enable_op", b"enable_op"]) -> None: ...
 
 global___ScopedAllocatorOptions = ScopedAllocatorOptions
 
-@typing_extensions.final
+@typing.final
 class RewriterConfig(google.protobuf.message.Message):
     """Graph rewriting is experimental and subject to change, not covered by any
     API stability guarantees.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -203,50 +205,50 @@
     SCHEDULING_HEURISTICS: RewriterConfig.MemOptType.ValueType  # 6
     """Scheduling will split big ops such as AddN and try to enforce a schedule
     of the new computations that decreases peak memory usage.
     """
     HEURISTICS: RewriterConfig.MemOptType.ValueType  # 3
     """Use any combination of swapping and recomputation heuristics."""
 
-    @typing_extensions.final
+    @typing.final
     class CustomGraphOptimizer(google.protobuf.message.Message):
         """Message to describe custom graph optimizer and its parameters"""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class ParameterMapEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: builtins.str
             @property
             def value(self) -> tensorflow.core.framework.attr_value_pb2.AttrValue: ...
             def __init__(
                 self,
                 *,
                 key: builtins.str | None = ...,
                 value: tensorflow.core.framework.attr_value_pb2.AttrValue | None = ...,
             ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+            def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         NAME_FIELD_NUMBER: builtins.int
         PARAMETER_MAP_FIELD_NUMBER: builtins.int
         name: builtins.str
         @property
         def parameter_map(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue]: ...
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             parameter_map: collections.abc.Mapping[builtins.str, tensorflow.core.framework.attr_value_pb2.AttrValue] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "parameter_map", b"parameter_map"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["name", b"name", "parameter_map", b"parameter_map"]) -> None: ...
 
     CPU_LAYOUT_CONVERSION_FIELD_NUMBER: builtins.int
     LAYOUT_OPTIMIZER_FIELD_NUMBER: builtins.int
     CONSTANT_FOLDING_FIELD_NUMBER: builtins.int
     SHAPE_OPTIMIZATION_FIELD_NUMBER: builtins.int
     REMAPPING_FIELD_NUMBER: builtins.int
     COMMON_SUBGRAPH_ELIMINATION_FIELD_NUMBER: builtins.int
@@ -399,25 +401,26 @@
     "foo/gradients/bar", but not "foo_gradients/"
     """
     meta_optimizer_timeout_ms: builtins.int
     """Maximum number of milliseconds to spend optimizing a single graph before
     timing out. If less than or equal to 0 (default value) the optimizer will
     never time out.
     """
-    @property
-    def auto_parallel(self) -> global___AutoParallelOptions:
-        """Configures AutoParallel optimization passes either through the
-        meta-optimizer or when manually specified through the optimizers field.
-        """
     fail_on_optimizer_errors: builtins.bool
     """If true, any optimization pass failing will cause the MetaOptimizer to
     stop with an error. By default - or when set to false, failing passes are
     skipped silently.
     """
     @property
+    def auto_parallel(self) -> global___AutoParallelOptions:
+        """Configures AutoParallel optimization passes either through the
+        meta-optimizer or when manually specified through the optimizers field.
+        """
+
+    @property
     def scoped_allocator_opts(self) -> global___ScopedAllocatorOptions: ...
     @property
     def optimizers(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """If non-empty, will use this as an alternative way to specify a list of
         optimizations to turn on and the order of the optimizations (replacing the
         meta-optimizer).
 
@@ -426,25 +429,29 @@
         ("autoparallel"). Memory optimization passes ("memory") invoked here are
         not configurable (in contrast to memory optimization passes through the
         meta-optimizer) and act only on manual op annotations.
 
         Custom optimizers (see custom_optimizers) that are not part of this
         schedule will be run after - in the order that they were specified.
         """
+
     @property
     def custom_optimizers(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RewriterConfig.CustomGraphOptimizer]:
         """list of CustomGraphOptimizers to apply."""
+
     @property
     def inter_optimizer_verifier_config(self) -> tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig:
         """VerifierConfig specifying the verifiers to be run after every optimizer."""
+
     @property
     def post_optimization_verifier_config(self) -> tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig:
         """VerifierConfig specifying the verifiers to be run at the end, after all
         optimizers have run.
         """
+
     def __init__(
         self,
         *,
         cpu_layout_conversion: global___RewriterConfig.CpuLayout.ValueType | None = ...,
         layout_optimizer: global___RewriterConfig.Toggle.ValueType | None = ...,
         constant_folding: global___RewriterConfig.Toggle.ValueType | None = ...,
         shape_optimization: global___RewriterConfig.Toggle.ValueType | None = ...,
@@ -477,11 +484,11 @@
         fail_on_optimizer_errors: builtins.bool | None = ...,
         scoped_allocator_opts: global___ScopedAllocatorOptions | None = ...,
         optimizers: collections.abc.Iterable[builtins.str] | None = ...,
         custom_optimizers: collections.abc.Iterable[global___RewriterConfig.CustomGraphOptimizer] | None = ...,
         inter_optimizer_verifier_config: tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig | None = ...,
         post_optimization_verifier_config: tensorflow.core.protobuf.verifier_config_pb2.VerifierConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auto_parallel", b"auto_parallel", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "post_optimization_verifier_config", b"post_optimization_verifier_config", "scoped_allocator_opts", b"scoped_allocator_opts"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arithmetic_optimization", b"arithmetic_optimization", "auto_mixed_precision", b"auto_mixed_precision", "auto_mixed_precision_cpu", b"auto_mixed_precision_cpu", "auto_mixed_precision_mkl", b"auto_mixed_precision_mkl", "auto_mixed_precision_onednn_bfloat16", b"auto_mixed_precision_onednn_bfloat16", "auto_parallel", b"auto_parallel", "common_subgraph_elimination", b"common_subgraph_elimination", "constant_folding", b"constant_folding", "cpu_layout_conversion", b"cpu_layout_conversion", "custom_optimizers", b"custom_optimizers", "debug_stripper", b"debug_stripper", "dependency_optimization", b"dependency_optimization", "disable_meta_optimizer", b"disable_meta_optimizer", "disable_model_pruning", b"disable_model_pruning", "experimental_conditional_code_motion", b"experimental_conditional_code_motion", "experimental_disable_compressed_tensor_optimization", b"experimental_disable_compressed_tensor_optimization", "experimental_disable_folding_quantization_emulation", b"experimental_disable_folding_quantization_emulation", "fail_on_optimizer_errors", b"fail_on_optimizer_errors", "function_optimization", b"function_optimization", "implementation_selector", b"implementation_selector", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "layout_optimizer", b"layout_optimizer", "loop_optimization", b"loop_optimization", "memory_optimization", b"memory_optimization", "memory_optimizer_target_node_name_scope", b"memory_optimizer_target_node_name_scope", "meta_optimizer_iterations", b"meta_optimizer_iterations", "meta_optimizer_timeout_ms", b"meta_optimizer_timeout_ms", "min_graph_nodes", b"min_graph_nodes", "optimizers", b"optimizers", "pin_to_host_optimization", b"pin_to_host_optimization", "post_optimization_verifier_config", b"post_optimization_verifier_config", "remapping", b"remapping", "scoped_allocator_optimization", b"scoped_allocator_optimization", "scoped_allocator_opts", b"scoped_allocator_opts", "shape_optimization", b"shape_optimization", "use_plugin_optimizers", b"use_plugin_optimizers"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["auto_parallel", b"auto_parallel", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "post_optimization_verifier_config", b"post_optimization_verifier_config", "scoped_allocator_opts", b"scoped_allocator_opts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["arithmetic_optimization", b"arithmetic_optimization", "auto_mixed_precision", b"auto_mixed_precision", "auto_mixed_precision_cpu", b"auto_mixed_precision_cpu", "auto_mixed_precision_mkl", b"auto_mixed_precision_mkl", "auto_mixed_precision_onednn_bfloat16", b"auto_mixed_precision_onednn_bfloat16", "auto_parallel", b"auto_parallel", "common_subgraph_elimination", b"common_subgraph_elimination", "constant_folding", b"constant_folding", "cpu_layout_conversion", b"cpu_layout_conversion", "custom_optimizers", b"custom_optimizers", "debug_stripper", b"debug_stripper", "dependency_optimization", b"dependency_optimization", "disable_meta_optimizer", b"disable_meta_optimizer", "disable_model_pruning", b"disable_model_pruning", "experimental_conditional_code_motion", b"experimental_conditional_code_motion", "experimental_disable_compressed_tensor_optimization", b"experimental_disable_compressed_tensor_optimization", "experimental_disable_folding_quantization_emulation", b"experimental_disable_folding_quantization_emulation", "fail_on_optimizer_errors", b"fail_on_optimizer_errors", "function_optimization", b"function_optimization", "implementation_selector", b"implementation_selector", "inter_optimizer_verifier_config", b"inter_optimizer_verifier_config", "layout_optimizer", b"layout_optimizer", "loop_optimization", b"loop_optimization", "memory_optimization", b"memory_optimization", "memory_optimizer_target_node_name_scope", b"memory_optimizer_target_node_name_scope", "meta_optimizer_iterations", b"meta_optimizer_iterations", "meta_optimizer_timeout_ms", b"meta_optimizer_timeout_ms", "min_graph_nodes", b"min_graph_nodes", "optimizers", b"optimizers", "pin_to_host_optimization", b"pin_to_host_optimization", "post_optimization_verifier_config", b"post_optimization_verifier_config", "remapping", b"remapping", "scoped_allocator_optimization", b"scoped_allocator_optimization", "scoped_allocator_opts", b"scoped_allocator_opts", "shape_optimization", b"shape_optimization", "use_plugin_optimizers", b"use_plugin_optimizers"]) -> None: ...
 
 global___RewriterConfig = RewriterConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.protobuf.meta_graph_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SavedModel(google.protobuf.message.Message):
     """SavedModel is the high level serialization format for TensorFlow Models.
     See [todo: doc links, similar to session_bundle] for more information.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -27,16 +28,17 @@
     """The schema version of the SavedModel instance. Used for versioning when
     making future changes to the specification/implementation. Initial value
     at release will be 1.
     """
     @property
     def meta_graphs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.protobuf.meta_graph_pb2.MetaGraphDef]:
         """One or more MetaGraphs."""
+
     def __init__(
         self,
         *,
         saved_model_schema_version: builtins.int | None = ...,
         meta_graphs: collections.abc.Iterable[tensorflow.core.protobuf.meta_graph_pb2.MetaGraphDef] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["meta_graphs", b"meta_graphs", "saved_model_schema_version", b"saved_model_schema_version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["meta_graphs", b"meta_graphs", "saved_model_schema_version", b"saved_model_schema_version"]) -> None: ...
 
 global___SavedModel = SavedModel
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
@@ -22,87 +23,89 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SavedObjectGraph(google.protobuf.message.Message):
     """SavedObjectGraph shares some structure with TrackableObjectGraph, but
     SavedObjectGraph belongs to the MetaGraph and contains pointers to functions
     and type information, while TrackableObjectGraph lives in the checkpoint
     and contains pointers only to variable values.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ConcreteFunctionsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___SavedConcreteFunction: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___SavedConcreteFunction | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NODES_FIELD_NUMBER: builtins.int
     CONCRETE_FUNCTIONS_FIELD_NUMBER: builtins.int
     @property
     def nodes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SavedObject]:
         """Flattened list of objects in the object graph.
 
         The position of the object in this list indicates its id.
         Nodes[0] is considered the root node.
         """
+
     @property
     def concrete_functions(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___SavedConcreteFunction]:
         """Information about captures and output structures in concrete functions.
         Referenced from SavedBareConcreteFunction and SavedFunction.
         """
+
     def __init__(
         self,
         *,
         nodes: collections.abc.Iterable[global___SavedObject] | None = ...,
         concrete_functions: collections.abc.Mapping[builtins.str, global___SavedConcreteFunction] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["concrete_functions", b"concrete_functions", "nodes", b"nodes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["concrete_functions", b"concrete_functions", "nodes", b"nodes"]) -> None: ...
 
 global___SavedObjectGraph = SavedObjectGraph
 
-@typing_extensions.final
+@typing.final
 class SavedObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class SaveableObjectsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___SaveableObject: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___SaveableObject | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     CHILDREN_FIELD_NUMBER: builtins.int
     DEPENDENCIES_FIELD_NUMBER: builtins.int
     SLOT_VARIABLES_FIELD_NUMBER: builtins.int
     USER_OBJECT_FIELD_NUMBER: builtins.int
     ASSET_FIELD_NUMBER: builtins.int
     FUNCTION_FIELD_NUMBER: builtins.int
@@ -111,36 +114,61 @@
     CONSTANT_FIELD_NUMBER: builtins.int
     RESOURCE_FIELD_NUMBER: builtins.int
     CAPTURED_TENSOR_FIELD_NUMBER: builtins.int
     SAVEABLE_OBJECTS_FIELD_NUMBER: builtins.int
     REGISTERED_NAME_FIELD_NUMBER: builtins.int
     SERIALIZED_USER_PROTO_FIELD_NUMBER: builtins.int
     REGISTERED_SAVER_FIELD_NUMBER: builtins.int
+    registered_name: builtins.str
+    """The fields below are filled when the user serializes a registered Trackable
+    class or an object with a registered saver function.
+
+    Registered classes may save additional metadata and supersede the
+    default loading process where nodes are recreated from the proto.
+    If the registered class cannot be found, then the object will load as one
+    one of the default trackable objects: Autotrackable (a class similar to
+    tf.Module), tf.function, or tf.Variable.
+
+    Unlike SaveableObjects, which store the functions for saving and restoring
+    from tensors, registered savers allow Trackables to write checkpoint shards
+    directly (e.g. for performance or coordination reasons).
+    *All registered savers must be available when loading the SavedModel.*
+
+    The name of the registered class of the form "{package}.{class_name}".
+    This field is used to search for the registered class at loading time.
+    """
+    registered_saver: builtins.str
+    """String name of the registered saver. At most one of `saveable_objects` or
+    `registered_saver` is defined for each SavedObject.
+    """
     @property
     def children(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.ObjectReference]:
         """Objects which this object depends on: named edges in the dependency
         graph.
 
         Note: All kinds of SavedObject may have children, except
         "constant" and "captured_tensor".
         """
+
     @property
     def dependencies(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.ObjectReference]:
         """Ordered list of dependencies that must be loaded before this object.
         SavedModel loads with the bottom-up approach, by first creating all objects
         (in the order defined by the dependencies), then connecting the edges.
         """
+
     @property
     def slot_variables(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.SlotVariableReference]:
         """Slot variables owned by this object. This describes the three-way
         (optimizer, variable, slot variable) relationship; none of the three
         depend on the others directly.
 
         Note: currently only valid if kind == "user_object".
         """
+
     @property
     def user_object(self) -> global___SavedUserObject: ...
     @property
     def asset(self) -> global___SavedAsset: ...
     @property
     def function(self) -> global___SavedFunction: ...
     @property
@@ -156,42 +184,22 @@
     @property
     def saveable_objects(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___SaveableObject]:
         """Stores the functions used to save and restore this object. At most one of
         `saveable_objects` or `registered_saver` is defined for each SavedObject.
         See the comment below for the difference between SaveableObject and
         registered savers.
         """
-    registered_name: builtins.str
-    """The fields below are filled when the user serializes a registered Trackable
-    class or an object with a registered saver function.
-
-    Registered classes may save additional metadata and supersede the
-    default loading process where nodes are recreated from the proto.
-    If the registered class cannot be found, then the object will load as one
-    one of the default trackable objects: Autotrackable (a class similar to
-    tf.Module), tf.function, or tf.Variable.
-
-    Unlike SaveableObjects, which store the functions for saving and restoring
-    from tensors, registered savers allow Trackables to write checkpoint shards
-    directly (e.g. for performance or coordination reasons).
-    *All registered savers must be available when loading the SavedModel.*
 
-    The name of the registered class of the form "{package}.{class_name}".
-    This field is used to search for the registered class at loading time.
-    """
     @property
     def serialized_user_proto(self) -> google.protobuf.any_pb2.Any:
         """The user-generated proto storing metadata for this object, to be passed to
         the registered classes's _deserialize_from_proto method when this object is
         loaded from the SavedModel.
         """
-    registered_saver: builtins.str
-    """String name of the registered saver. At most one of `saveable_objects` or
-    `registered_saver` is defined for each SavedObject.
-    """
+
     def __init__(
         self,
         *,
         children: collections.abc.Iterable[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.ObjectReference] | None = ...,
         dependencies: collections.abc.Iterable[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.ObjectReference] | None = ...,
         slot_variables: collections.abc.Iterable[tensorflow.core.protobuf.trackable_object_graph_pb2.TrackableObjectGraph.TrackableObject.SlotVariableReference] | None = ...,
         user_object: global___SavedUserObject | None = ...,
@@ -203,21 +211,21 @@
         resource: global___SavedResource | None = ...,
         captured_tensor: global___CapturedTensor | None = ...,
         saveable_objects: collections.abc.Mapping[builtins.str, global___SaveableObject] | None = ...,
         registered_name: builtins.str | None = ...,
         serialized_user_proto: google.protobuf.any_pb2.Any | None = ...,
         registered_saver: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["asset", b"asset", "bare_concrete_function", b"bare_concrete_function", "captured_tensor", b"captured_tensor", "constant", b"constant", "function", b"function", "kind", b"kind", "resource", b"resource", "serialized_user_proto", b"serialized_user_proto", "user_object", b"user_object", "variable", b"variable"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["asset", b"asset", "bare_concrete_function", b"bare_concrete_function", "captured_tensor", b"captured_tensor", "children", b"children", "constant", b"constant", "dependencies", b"dependencies", "function", b"function", "kind", b"kind", "registered_name", b"registered_name", "registered_saver", b"registered_saver", "resource", b"resource", "saveable_objects", b"saveable_objects", "serialized_user_proto", b"serialized_user_proto", "slot_variables", b"slot_variables", "user_object", b"user_object", "variable", b"variable"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["user_object", "asset", "function", "variable", "bare_concrete_function", "constant", "resource", "captured_tensor"] | None: ...
+    def HasField(self, field_name: typing.Literal["asset", b"asset", "bare_concrete_function", b"bare_concrete_function", "captured_tensor", b"captured_tensor", "constant", b"constant", "function", b"function", "kind", b"kind", "resource", b"resource", "serialized_user_proto", b"serialized_user_proto", "user_object", b"user_object", "variable", b"variable"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["asset", b"asset", "bare_concrete_function", b"bare_concrete_function", "captured_tensor", b"captured_tensor", "children", b"children", "constant", b"constant", "dependencies", b"dependencies", "function", b"function", "kind", b"kind", "registered_name", b"registered_name", "registered_saver", b"registered_saver", "resource", b"resource", "saveable_objects", b"saveable_objects", "serialized_user_proto", b"serialized_user_proto", "slot_variables", b"slot_variables", "user_object", b"user_object", "variable", b"variable"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["user_object", "asset", "function", "variable", "bare_concrete_function", "constant", "resource", "captured_tensor"] | None: ...
 
 global___SavedObject = SavedObject
 
-@typing_extensions.final
+@typing.final
 class SavedUserObject(google.protobuf.message.Message):
     """A SavedUserObject is an object (in the object-oriented language of the
     TensorFlow program) of some user- or framework-defined class other than
     those handled specifically by the other kinds of SavedObjects.
 
     This object cannot be evaluated as a tensor, and therefore cannot be bound
     to an input of a function.
@@ -226,37 +234,38 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IDENTIFIER_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     identifier: builtins.str
     """Corresponds to a registration of the type to use in the loading program."""
-    @property
-    def version(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
-        """Version information from the producer of this SavedUserObject."""
     metadata: builtins.str
     """Metadata for deserializing this object.
 
     Deprecated! At the time of deprecation, Keras was the only user of this
     field, and its saving and loading code will be updated shortly.
     Please save your application-specific metadata to a separate file.
     """
+    @property
+    def version(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
+        """Version information from the producer of this SavedUserObject."""
+
     def __init__(
         self,
         *,
         identifier: builtins.str | None = ...,
         version: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
         metadata: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["version", b"version"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["identifier", b"identifier", "metadata", b"metadata", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["version", b"version"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["identifier", b"identifier", "metadata", b"metadata", "version", b"version"]) -> None: ...
 
 global___SavedUserObject = SavedUserObject
 
-@typing_extensions.final
+@typing.final
 class SavedAsset(google.protobuf.message.Message):
     """A SavedAsset points to an asset in the MetaGraph.
 
     When bound to a function this object evaluates to a tensor with the absolute
     filename. Users should not depend on a particular part of the filename to
     remain stable (e.g. basename could be changed).
     """
@@ -271,19 +280,19 @@
     `AssetFileDef.tensor_info`, MUST be ignored.
     """
     def __init__(
         self,
         *,
         asset_file_def_index: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["asset_file_def_index", b"asset_file_def_index"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["asset_file_def_index", b"asset_file_def_index"]) -> None: ...
 
 global___SavedAsset = SavedAsset
 
-@typing_extensions.final
+@typing.final
 class SavedFunction(google.protobuf.message.Message):
     """A function with multiple signatures, possibly with non-Tensor arguments."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONCRETE_FUNCTIONS_FIELD_NUMBER: builtins.int
     FUNCTION_SPEC_FIELD_NUMBER: builtins.int
@@ -293,20 +302,20 @@
     def function_spec(self) -> global___FunctionSpec: ...
     def __init__(
         self,
         *,
         concrete_functions: collections.abc.Iterable[builtins.str] | None = ...,
         function_spec: global___FunctionSpec | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["function_spec", b"function_spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["concrete_functions", b"concrete_functions", "function_spec", b"function_spec"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["function_spec", b"function_spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["concrete_functions", b"concrete_functions", "function_spec", b"function_spec"]) -> None: ...
 
 global___SavedFunction = SavedFunction
 
-@typing_extensions.final
+@typing.final
 class CapturedTensor(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     CONCRETE_FUNCTION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Name of captured tensor"""
@@ -314,19 +323,19 @@
     """Name of concrete function which contains the computed graph tensor."""
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         concrete_function: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["concrete_function", b"concrete_function", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["concrete_function", b"concrete_function", "name", b"name"]) -> None: ...
 
 global___CapturedTensor = CapturedTensor
 
-@typing_extensions.final
+@typing.final
 class SavedConcreteFunction(google.protobuf.message.Message):
     """Stores low-level information about a concrete function. Referenced in either
     a SavedFunction or a SavedBareConcreteFunction.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -336,86 +345,90 @@
     @property
     def bound_inputs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     @property
     def canonicalized_input_signature(self) -> tensorflow.core.protobuf.struct_pb2.StructuredValue:
         """Input in canonicalized form that was received to create this concrete
         function.
         """
+
     @property
     def output_signature(self) -> tensorflow.core.protobuf.struct_pb2.StructuredValue:
         """Output that was the return value of this function after replacing all
         Tensors with TensorSpecs. This can be an arbitrary nested function and will
         be used to reconstruct the full structure from pure tensors.
         """
+
     def __init__(
         self,
         *,
         bound_inputs: collections.abc.Iterable[builtins.int] | None = ...,
         canonicalized_input_signature: tensorflow.core.protobuf.struct_pb2.StructuredValue | None = ...,
         output_signature: tensorflow.core.protobuf.struct_pb2.StructuredValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["canonicalized_input_signature", b"canonicalized_input_signature", "output_signature", b"output_signature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bound_inputs", b"bound_inputs", "canonicalized_input_signature", b"canonicalized_input_signature", "output_signature", b"output_signature"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["canonicalized_input_signature", b"canonicalized_input_signature", "output_signature", b"output_signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bound_inputs", b"bound_inputs", "canonicalized_input_signature", b"canonicalized_input_signature", "output_signature", b"output_signature"]) -> None: ...
 
 global___SavedConcreteFunction = SavedConcreteFunction
 
-@typing_extensions.final
+@typing.final
 class SavedBareConcreteFunction(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONCRETE_FUNCTION_NAME_FIELD_NUMBER: builtins.int
     ARGUMENT_KEYWORDS_FIELD_NUMBER: builtins.int
     ALLOWED_POSITIONAL_ARGUMENTS_FIELD_NUMBER: builtins.int
     FUNCTION_SPEC_FIELD_NUMBER: builtins.int
     concrete_function_name: builtins.str
     """Identifies a SavedConcreteFunction."""
+    allowed_positional_arguments: builtins.int
+    """The prefix of `argument_keywords` which may be identified by position."""
     @property
     def argument_keywords(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """A sequence of unique strings, one per Tensor argument."""
-    allowed_positional_arguments: builtins.int
-    """The prefix of `argument_keywords` which may be identified by position."""
+
     @property
     def function_spec(self) -> global___FunctionSpec:
         """The spec of the function that this ConcreteFunction is traced from. This
         allows the ConcreteFunction to be called with nest structure inputs. This
         field may not be populated. If this field is absent, the concrete function
         can only be called with flat inputs.
         TODO(b/169361281): support calling saved ConcreteFunction with structured
         inputs in C++ SavedModel API.
         """
+
     def __init__(
         self,
         *,
         concrete_function_name: builtins.str | None = ...,
         argument_keywords: collections.abc.Iterable[builtins.str] | None = ...,
         allowed_positional_arguments: builtins.int | None = ...,
         function_spec: global___FunctionSpec | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["function_spec", b"function_spec"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allowed_positional_arguments", b"allowed_positional_arguments", "argument_keywords", b"argument_keywords", "concrete_function_name", b"concrete_function_name", "function_spec", b"function_spec"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["function_spec", b"function_spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allowed_positional_arguments", b"allowed_positional_arguments", "argument_keywords", b"argument_keywords", "concrete_function_name", b"concrete_function_name", "function_spec", b"function_spec"]) -> None: ...
 
 global___SavedBareConcreteFunction = SavedBareConcreteFunction
 
-@typing_extensions.final
+@typing.final
 class SavedConstant(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OPERATION_FIELD_NUMBER: builtins.int
     operation: builtins.str
     """An Operation name for a ConstantOp in this SavedObjectGraph's MetaGraph."""
     def __init__(
         self,
         *,
         operation: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["operation", b"operation"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["operation", b"operation"]) -> None: ...
 
 global___SavedConstant = SavedConstant
 
-@typing_extensions.final
+@typing.final
 class SavedVariable(google.protobuf.message.Message):
     """Represents a Variable that is initialized by loading the contents from the
     checkpoint.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -424,48 +437,49 @@
     TRAINABLE_FIELD_NUMBER: builtins.int
     SYNCHRONIZATION_FIELD_NUMBER: builtins.int
     AGGREGATION_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     DEVICE_FIELD_NUMBER: builtins.int
     EXPERIMENTAL_DISTRIBUTED_VARIABLE_COMPONENTS_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
-    @property
-    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     trainable: builtins.bool
     synchronization: tensorflow.core.framework.variable_pb2.VariableSynchronization.ValueType
     aggregation: tensorflow.core.framework.variable_pb2.VariableAggregation.ValueType
     name: builtins.str
     device: builtins.str
     @property
+    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
+    @property
     def experimental_distributed_variable_components(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SavedVariable]:
         """List of component variables for a distributed variable.
 
         When this field is non-empty, the SavedVariable will be assumed
         to be a distributed variable defined by the components listed here.
 
         This is only supported by experimental loaders at the moment.
         """
+
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         trainable: builtins.bool | None = ...,
         synchronization: tensorflow.core.framework.variable_pb2.VariableSynchronization.ValueType | None = ...,
         aggregation: tensorflow.core.framework.variable_pb2.VariableAggregation.ValueType | None = ...,
         name: builtins.str | None = ...,
         device: builtins.str | None = ...,
         experimental_distributed_variable_components: collections.abc.Iterable[global___SavedVariable] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aggregation", b"aggregation", "device", b"device", "dtype", b"dtype", "experimental_distributed_variable_components", b"experimental_distributed_variable_components", "name", b"name", "shape", b"shape", "synchronization", b"synchronization", "trainable", b"trainable"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["aggregation", b"aggregation", "device", b"device", "dtype", b"dtype", "experimental_distributed_variable_components", b"experimental_distributed_variable_components", "name", b"name", "shape", b"shape", "synchronization", b"synchronization", "trainable", b"trainable"]) -> None: ...
 
 global___SavedVariable = SavedVariable
 
-@typing_extensions.final
+@typing.final
 class FunctionSpec(google.protobuf.message.Message):
     """Represents `FunctionSpec` used in `Function`. This represents a
     function that has been wrapped as a TensorFlow `Function`.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -494,37 +508,39 @@
     ON: FunctionSpec.JitCompile.ValueType  # 1
     OFF: FunctionSpec.JitCompile.ValueType  # 2
 
     FULLARGSPEC_FIELD_NUMBER: builtins.int
     IS_METHOD_FIELD_NUMBER: builtins.int
     INPUT_SIGNATURE_FIELD_NUMBER: builtins.int
     JIT_COMPILE_FIELD_NUMBER: builtins.int
+    is_method: builtins.bool
+    """Whether this represents a class method."""
+    jit_compile: global___FunctionSpec.JitCompile.ValueType
     @property
     def fullargspec(self) -> tensorflow.core.protobuf.struct_pb2.StructuredValue:
         """Full arg spec from inspect.getfullargspec()."""
-    is_method: builtins.bool
-    """Whether this represents a class method."""
+
     @property
     def input_signature(self) -> tensorflow.core.protobuf.struct_pb2.StructuredValue:
         """The input signature, if specified."""
-    jit_compile: global___FunctionSpec.JitCompile.ValueType
+
     def __init__(
         self,
         *,
         fullargspec: tensorflow.core.protobuf.struct_pb2.StructuredValue | None = ...,
         is_method: builtins.bool | None = ...,
         input_signature: tensorflow.core.protobuf.struct_pb2.StructuredValue | None = ...,
         jit_compile: global___FunctionSpec.JitCompile.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["fullargspec", b"fullargspec", "input_signature", b"input_signature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fullargspec", b"fullargspec", "input_signature", b"input_signature", "is_method", b"is_method", "jit_compile", b"jit_compile"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["fullargspec", b"fullargspec", "input_signature", b"input_signature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["fullargspec", b"fullargspec", "input_signature", b"input_signature", "is_method", b"is_method", "jit_compile", b"jit_compile"]) -> None: ...
 
 global___FunctionSpec = FunctionSpec
 
-@typing_extensions.final
+@typing.final
 class SavedResource(google.protobuf.message.Message):
     """A SavedResource represents a TF object that holds state during its lifetime.
     An object of this type can have a reference to a:
     create_resource() and an initialize() function.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -536,19 +552,19 @@
     device.
     """
     def __init__(
         self,
         *,
         device: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device", b"device"]) -> None: ...
 
 global___SavedResource = SavedResource
 
-@typing_extensions.final
+@typing.final
 class SaveableObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SAVE_FUNCTION_FIELD_NUMBER: builtins.int
     RESTORE_FUNCTION_FIELD_NUMBER: builtins.int
     save_function: builtins.int
     """Node ids of concrete functions for saving and loading from a checkpoint.
@@ -557,10 +573,10 @@
     restore_function: builtins.int
     def __init__(
         self,
         *,
         save_function: builtins.int | None = ...,
         restore_function: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["restore_function", b"restore_function", "save_function", b"save_function"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["restore_function", b"restore_function", "save_function", b"save_function"]) -> None: ...
 
 global___SaveableObject = SaveableObject
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -13,15 +14,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SaverDef(google.protobuf.message.Message):
     """Protocol buffer representing the configuration of a Saver."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CheckpointFormatVersion:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -83,10 +84,10 @@
         save_tensor_name: builtins.str | None = ...,
         restore_op_name: builtins.str | None = ...,
         max_to_keep: builtins.int | None = ...,
         sharded: builtins.bool | None = ...,
         keep_checkpoint_every_n_hours: builtins.float | None = ...,
         version: global___SaverDef.CheckpointFormatVersion.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["filename_tensor_name", b"filename_tensor_name", "keep_checkpoint_every_n_hours", b"keep_checkpoint_every_n_hours", "max_to_keep", b"max_to_keep", "restore_op_name", b"restore_op_name", "save_tensor_name", b"save_tensor_name", "sharded", b"sharded", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["filename_tensor_name", b"filename_tensor_name", "keep_checkpoint_every_n_hours", b"keep_checkpoint_every_n_hours", "max_to_keep", b"max_to_keep", "restore_op_name", b"restore_op_name", "save_tensor_name", b"save_tensor_name", "sharded", b"sharded", "version", b"version"]) -> None: ...
 
 global___SaverDef = SaverDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.protobuf.data_service_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class DispatcherConfig(google.protobuf.message.Message):
     """Configuration for a tf.data service DispatchServer.
     Next id: 11
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -41,21 +42,14 @@
     """A work directory to use for storing dispatcher state, and for recovering
     during restarts. The empty string indicates not to use any work directory.
     """
     fault_tolerant_mode: builtins.bool
     """Whether to run in fault tolerant mode, where dispatcher state is saved
     across restarts. Requires that `work_dir` is nonempty.
     """
-    @property
-    def worker_addresses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """(Optional.) If the job uses auto-sharding, it needs to specify a fixed list
-        of worker addresses that will register with the dispatcher. The worker
-        addresses should be in the format "host" or "host:port", where "port" is an
-        integer, named port, or %port% to match any port.
-        """
     deployment_mode: tensorflow.core.protobuf.data_service_pb2.DeploymentMode.ValueType
     """(Optional.) tf.data service deployment mode. Supported values are "REMOTE",
     "COLOCATED", and "HYBRID". If unspecified, it is assumed to be "REMOTE".
     """
     job_gc_check_interval_ms: builtins.int
     """How often the dispatcher should scan through to delete old and unused
     jobs. A value of 0 indicates that the decision should be left up to the
@@ -72,33 +66,41 @@
     heartbeated to the dispatcher. A value of 0 indicates that the timeout
     should be left to the runtime.
     """
     worker_timeout_ms: builtins.int
     """How long to wait for a worker to heartbeat before considering it missing.
     A value of 0 indicates that the timeout should be left to the runtime.
     """
+    @property
+    def worker_addresses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """(Optional.) If the job uses auto-sharding, it needs to specify a fixed list
+        of worker addresses that will register with the dispatcher. The worker
+        addresses should be in the format "host" or "host:port", where "port" is an
+        integer, named port, or %port% to match any port.
+        """
+
     def __init__(
         self,
         *,
         port: builtins.int | None = ...,
         protocol: builtins.str | None = ...,
         work_dir: builtins.str | None = ...,
         fault_tolerant_mode: builtins.bool | None = ...,
         worker_addresses: collections.abc.Iterable[builtins.str] | None = ...,
         deployment_mode: tensorflow.core.protobuf.data_service_pb2.DeploymentMode.ValueType | None = ...,
         job_gc_check_interval_ms: builtins.int | None = ...,
         job_gc_timeout_ms: builtins.int | None = ...,
         client_timeout_ms: builtins.int | None = ...,
         worker_timeout_ms: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_timeout_ms", b"client_timeout_ms", "deployment_mode", b"deployment_mode", "fault_tolerant_mode", b"fault_tolerant_mode", "job_gc_check_interval_ms", b"job_gc_check_interval_ms", "job_gc_timeout_ms", b"job_gc_timeout_ms", "port", b"port", "protocol", b"protocol", "work_dir", b"work_dir", "worker_addresses", b"worker_addresses", "worker_timeout_ms", b"worker_timeout_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["client_timeout_ms", b"client_timeout_ms", "deployment_mode", b"deployment_mode", "fault_tolerant_mode", b"fault_tolerant_mode", "job_gc_check_interval_ms", b"job_gc_check_interval_ms", "job_gc_timeout_ms", b"job_gc_timeout_ms", "port", b"port", "protocol", b"protocol", "work_dir", b"work_dir", "worker_addresses", b"worker_addresses", "worker_timeout_ms", b"worker_timeout_ms"]) -> None: ...
 
 global___DispatcherConfig = DispatcherConfig
 
-@typing_extensions.final
+@typing.final
 class WorkerConfig(google.protobuf.message.Message):
     """Configuration for a tf.data service WorkerServer.
     Next id: 12
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -122,21 +124,14 @@
     dispatcher_address: builtins.str
     """The address of the dispatcher to register with."""
     worker_address: builtins.str
     """The address of the worker server. The substring "%port%", if specified,
     will be replaced with the worker's bound port. This is useful when the port
     is set to `0`.
     """
-    @property
-    def worker_tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
-        """Tags attached to the worker. This allows reading from selected workers.
-        For example, by applying a "COLOCATED" tag, tf.data service is able to read
-        from the local tf.data worker if one exists, then from off-TF-host workers,
-        to avoid cross-TF-host reads.
-        """
     heartbeat_interval_ms: builtins.int
     """How often the worker should heartbeat to the master. A value of 0 indicates
     that the decision should be left up to the runtime.
     """
     dispatcher_timeout_ms: builtins.int
     """How long to retry requests to the dispatcher before giving up and reporting
     an error. A value of 0 indicates that the decision should be left up to the
@@ -154,14 +149,22 @@
     your training job provides sufficient memory resources.
     """
     shutdown_quiet_period_ms: builtins.int
     """When shutting down a worker, how long to wait for the gRPC server to
     process the final requests. This is used to achieve clean shutdown in unit
     tests.
     """
+    @property
+    def worker_tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
+        """Tags attached to the worker. This allows reading from selected workers.
+        For example, by applying a "COLOCATED" tag, tf.data service is able to read
+        from the local tf.data worker if one exists, then from off-TF-host workers,
+        to avoid cross-TF-host reads.
+        """
+
     def __init__(
         self,
         *,
         port: builtins.int | None = ...,
         protocol: builtins.str | None = ...,
         dispatcher_address: builtins.str | None = ...,
         worker_address: builtins.str | None = ...,
@@ -169,10 +172,10 @@
         heartbeat_interval_ms: builtins.int | None = ...,
         dispatcher_timeout_ms: builtins.int | None = ...,
         data_transfer_protocol: builtins.str | None = ...,
         data_transfer_address: builtins.str | None = ...,
         cross_trainer_cache_size_bytes: builtins.int | None = ...,
         shutdown_quiet_period_ms: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cross_trainer_cache_size_bytes", b"cross_trainer_cache_size_bytes", "data_transfer_address", b"data_transfer_address", "data_transfer_protocol", b"data_transfer_protocol", "dispatcher_address", b"dispatcher_address", "dispatcher_timeout_ms", b"dispatcher_timeout_ms", "heartbeat_interval_ms", b"heartbeat_interval_ms", "port", b"port", "protocol", b"protocol", "shutdown_quiet_period_ms", b"shutdown_quiet_period_ms", "worker_address", b"worker_address", "worker_tags", b"worker_tags"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cross_trainer_cache_size_bytes", b"cross_trainer_cache_size_bytes", "data_transfer_address", b"data_transfer_address", "data_transfer_protocol", b"data_transfer_protocol", "dispatcher_address", b"dispatcher_address", "dispatcher_timeout_ms", b"dispatcher_timeout_ms", "heartbeat_interval_ms", b"heartbeat_interval_ms", "port", b"port", "protocol", b"protocol", "shutdown_quiet_period_ms", b"shutdown_quiet_period_ms", "worker_address", b"worker_address", "worker_tags", b"worker_tags"]) -> None: ...
 
 global___WorkerConfig = WorkerConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.types_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SnapshotRecord(google.protobuf.message.Message):
     """Each SnapshotRecord represents one batch of pre-processed input data. A batch
     consists of a list of tensors that we encode as TensorProtos. This message
     doesn't store the structure of the batch.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -28,19 +29,19 @@
     @property
     def tensor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_pb2.TensorProto]: ...
     def __init__(
         self,
         *,
         tensor: collections.abc.Iterable[tensorflow.core.framework.tensor_pb2.TensorProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tensor", b"tensor"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["tensor", b"tensor"]) -> None: ...
 
 global___SnapshotRecord = SnapshotRecord
 
-@typing_extensions.final
+@typing.final
 class SnapshotMetadataRecord(google.protobuf.message.Message):
     """This stores the metadata information present in each snapshot record."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     GRAPH_HASH_FIELD_NUMBER: builtins.int
     RUN_ID_FIELD_NUMBER: builtins.int
@@ -55,77 +56,78 @@
     """
     run_id: builtins.str
     """Run ID that this snapshot corresponds to."""
     creation_timestamp: builtins.int
     """Time when we started creating this snapshot."""
     version: builtins.int
     """Version of the snapshot data file format."""
-    @property
-    def dtype(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[tensorflow.core.framework.types_pb2.DataType.ValueType]:
-        """A list of tensor dtype corresponding to each element of the snapshot."""
     num_elements: builtins.int
     """The number of elements in the snapshot."""
     finalized: builtins.bool
+    @property
+    def dtype(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[tensorflow.core.framework.types_pb2.DataType.ValueType]:
+        """A list of tensor dtype corresponding to each element of the snapshot."""
+
     def __init__(
         self,
         *,
         graph_hash: builtins.str | None = ...,
         run_id: builtins.str | None = ...,
         creation_timestamp: builtins.int | None = ...,
         version: builtins.int | None = ...,
         dtype: collections.abc.Iterable[tensorflow.core.framework.types_pb2.DataType.ValueType] | None = ...,
         num_elements: builtins.int | None = ...,
         finalized: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "dtype", b"dtype", "finalized", b"finalized", "graph_hash", b"graph_hash", "num_elements", b"num_elements", "run_id", b"run_id", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["creation_timestamp", b"creation_timestamp", "dtype", b"dtype", "finalized", b"finalized", "graph_hash", b"graph_hash", "num_elements", b"num_elements", "run_id", b"run_id", "version", b"version"]) -> None: ...
 
 global___SnapshotMetadataRecord = SnapshotMetadataRecord
 
-@typing_extensions.final
+@typing.final
 class TensorMetadata(google.protobuf.message.Message):
     """Metadata for a single tensor in the Snapshot Record."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_SHAPE_FIELD_NUMBER: builtins.int
     TENSOR_SIZE_BYTES_FIELD_NUMBER: builtins.int
-    @property
-    def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     tensor_size_bytes: builtins.int
     """Number of uncompressed bytes used to store the tensor representation."""
+    @property
+    def tensor_shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     def __init__(
         self,
         *,
         tensor_shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         tensor_size_bytes: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tensor_shape", b"tensor_shape", "tensor_size_bytes", b"tensor_size_bytes"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tensor_shape", b"tensor_shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["tensor_shape", b"tensor_shape", "tensor_size_bytes", b"tensor_size_bytes"]) -> None: ...
 
 global___TensorMetadata = TensorMetadata
 
-@typing_extensions.final
+@typing.final
 class SnapshotTensorMetadata(google.protobuf.message.Message):
     """Metadata for all the tensors in a Snapshot Record."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_METADATA_FIELD_NUMBER: builtins.int
     @property
     def tensor_metadata(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TensorMetadata]: ...
     def __init__(
         self,
         *,
         tensor_metadata: collections.abc.Iterable[global___TensorMetadata] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tensor_metadata", b"tensor_metadata"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["tensor_metadata", b"tensor_metadata"]) -> None: ...
 
 global___SnapshotTensorMetadata = SnapshotTensorMetadata
 
-@typing_extensions.final
+@typing.final
 class DistributedSnapshotMetadata(google.protobuf.message.Message):
     """Metadata for a `tf.data.Dataset` distributed snapshot."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ELEMENT_SPEC_FIELD_NUMBER: builtins.int
     COMPRESSION_FIELD_NUMBER: builtins.int
@@ -138,10 +140,10 @@
     """
     def __init__(
         self,
         *,
         element_spec: builtins.bytes | None = ...,
         compression: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compression", b"compression", "element_spec", b"element_spec"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["compression", b"compression", "element_spec", b"element_spec"]) -> None: ...
 
 global___DistributedSnapshotMetadata = DistributedSnapshotMetadata
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -18,15 +19,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class StructuredValue(google.protobuf.message.Message):
     """`StructuredValue` represents a dynamically typed value representing various
     data structures that are inspired by Python data structures typically used in
     TensorFlow functions as inputs and outputs.
 
     For example when saving a Layer there may be a `training` argument. If the
     user passes a boolean True/False, that switches between two concrete
@@ -62,17 +63,14 @@
     TENSOR_SPEC_VALUE_FIELD_NUMBER: builtins.int
     TYPE_SPEC_VALUE_FIELD_NUMBER: builtins.int
     BOUNDED_TENSOR_SPEC_VALUE_FIELD_NUMBER: builtins.int
     LIST_VALUE_FIELD_NUMBER: builtins.int
     TUPLE_VALUE_FIELD_NUMBER: builtins.int
     DICT_VALUE_FIELD_NUMBER: builtins.int
     NAMED_TUPLE_VALUE_FIELD_NUMBER: builtins.int
-    @property
-    def none_value(self) -> global___NoneValue:
-        """Represents None."""
     float64_value: builtins.float
     """Represents a double-precision floating-point value (a Python `float`)."""
     int64_value: builtins.int
     """Represents a signed integer value, limited to 64 bits.
     Larger values from Python's arbitrary-precision integers are unsupported.
     """
     string_value: builtins.str
@@ -81,40 +79,52 @@
     In Python 2, this is the UTF-8 encoding of the characters.
     For strings with ASCII characters only (as often used in TensorFlow code)
     there is effectively no difference between the language versions.
     The obsolescent `unicode` type of Python 2 is not supported here.
     """
     bool_value: builtins.bool
     """Represents a boolean value."""
+    tensor_dtype_value: tensorflow.core.framework.types_pb2.DataType.ValueType
+    """Represents an enum value for dtype."""
+    @property
+    def none_value(self) -> global___NoneValue:
+        """Represents None."""
+
     @property
     def tensor_shape_value(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """Represents a TensorShape."""
-    tensor_dtype_value: tensorflow.core.framework.types_pb2.DataType.ValueType
-    """Represents an enum value for dtype."""
+
     @property
     def tensor_spec_value(self) -> global___TensorSpecProto:
         """Represents a value for tf.TensorSpec."""
+
     @property
     def type_spec_value(self) -> global___TypeSpecProto:
         """Represents a value for tf.TypeSpec."""
+
     @property
     def bounded_tensor_spec_value(self) -> global___BoundedTensorSpecProto:
         """Represents a value for tf.BoundedTensorSpec."""
+
     @property
     def list_value(self) -> global___ListValue:
         """Represents a list of `Value`."""
+
     @property
     def tuple_value(self) -> global___TupleValue:
         """Represents a tuple of `Value`."""
+
     @property
     def dict_value(self) -> global___DictValue:
         """Represents a dict `Value`."""
+
     @property
     def named_tuple_value(self) -> global___NamedTupleValue:
         """Represents Python's namedtuple."""
+
     def __init__(
         self,
         *,
         none_value: global___NoneValue | None = ...,
         float64_value: builtins.float | None = ...,
         int64_value: builtins.int | None = ...,
         string_value: builtins.str | None = ...,
@@ -125,107 +135,107 @@
         type_spec_value: global___TypeSpecProto | None = ...,
         bounded_tensor_spec_value: global___BoundedTensorSpecProto | None = ...,
         list_value: global___ListValue | None = ...,
         tuple_value: global___TupleValue | None = ...,
         dict_value: global___DictValue | None = ...,
         named_tuple_value: global___NamedTupleValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["none_value", "float64_value", "int64_value", "string_value", "bool_value", "tensor_shape_value", "tensor_dtype_value", "tensor_spec_value", "type_spec_value", "bounded_tensor_spec_value", "list_value", "tuple_value", "dict_value", "named_tuple_value"] | None: ...
+    def HasField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bool_value", b"bool_value", "bounded_tensor_spec_value", b"bounded_tensor_spec_value", "dict_value", b"dict_value", "float64_value", b"float64_value", "int64_value", b"int64_value", "kind", b"kind", "list_value", b"list_value", "named_tuple_value", b"named_tuple_value", "none_value", b"none_value", "string_value", b"string_value", "tensor_dtype_value", b"tensor_dtype_value", "tensor_shape_value", b"tensor_shape_value", "tensor_spec_value", b"tensor_spec_value", "tuple_value", b"tuple_value", "type_spec_value", b"type_spec_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["none_value", "float64_value", "int64_value", "string_value", "bool_value", "tensor_shape_value", "tensor_dtype_value", "tensor_spec_value", "type_spec_value", "bounded_tensor_spec_value", "list_value", "tuple_value", "dict_value", "named_tuple_value"] | None: ...
 
 global___StructuredValue = StructuredValue
 
-@typing_extensions.final
+@typing.final
 class NoneValue(google.protobuf.message.Message):
     """Represents None."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___NoneValue = NoneValue
 
-@typing_extensions.final
+@typing.final
 class ListValue(google.protobuf.message.Message):
     """Represents a Python list."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StructuredValue]: ...
     def __init__(
         self,
         *,
         values: collections.abc.Iterable[global___StructuredValue] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["values", b"values"]) -> None: ...
 
 global___ListValue = ListValue
 
-@typing_extensions.final
+@typing.final
 class TupleValue(google.protobuf.message.Message):
     """Represents a Python tuple."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StructuredValue]: ...
     def __init__(
         self,
         *,
         values: collections.abc.Iterable[global___StructuredValue] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["values", b"values"]) -> None: ...
 
 global___TupleValue = TupleValue
 
-@typing_extensions.final
+@typing.final
 class DictValue(google.protobuf.message.Message):
     """Represents a Python dict keyed by `str`.
     The comment on Unicode from Value.string_value applies analogously.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FieldsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___StructuredValue: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___StructuredValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELDS_FIELD_NUMBER: builtins.int
     @property
     def fields(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___StructuredValue]: ...
     def __init__(
         self,
         *,
         fields: collections.abc.Mapping[builtins.str, global___StructuredValue] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields", b"fields"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["fields", b"fields"]) -> None: ...
 
 global___DictValue = DictValue
 
-@typing_extensions.final
+@typing.final
 class PairValue(google.protobuf.message.Message):
     """Represents a (key, value) pair."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
@@ -234,20 +244,20 @@
     def value(self) -> global___StructuredValue: ...
     def __init__(
         self,
         *,
         key: builtins.str | None = ...,
         value: global___StructuredValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
 global___PairValue = PairValue
 
-@typing_extensions.final
+@typing.final
 class NamedTupleValue(google.protobuf.message.Message):
     """Represents Python's namedtuple."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VALUES_FIELD_NUMBER: builtins.int
@@ -256,77 +266,77 @@
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___PairValue]: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         values: collections.abc.Iterable[global___PairValue] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "values", b"values"]) -> None: ...
 
 global___NamedTupleValue = NamedTupleValue
 
-@typing_extensions.final
+@typing.final
 class TensorSpecProto(google.protobuf.message.Message):
     """A protobuf to represent tf.TensorSpec."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "name", b"name", "shape", b"shape"]) -> None: ...
 
 global___TensorSpecProto = TensorSpecProto
 
-@typing_extensions.final
+@typing.final
 class BoundedTensorSpecProto(google.protobuf.message.Message):
     """A protobuf to represent tf.BoundedTensorSpec."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     DTYPE_FIELD_NUMBER: builtins.int
     MINIMUM_FIELD_NUMBER: builtins.int
     MAXIMUM_FIELD_NUMBER: builtins.int
     name: builtins.str
+    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
-    dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     @property
     def minimum(self) -> tensorflow.core.framework.tensor_pb2.TensorProto: ...
     @property
     def maximum(self) -> tensorflow.core.framework.tensor_pb2.TensorProto: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         minimum: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
         maximum: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["maximum", b"maximum", "minimum", b"minimum", "shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dtype", b"dtype", "maximum", b"maximum", "minimum", b"minimum", "name", b"name", "shape", b"shape"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["maximum", b"maximum", "minimum", b"minimum", "shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dtype", b"dtype", "maximum", b"maximum", "minimum", b"minimum", "name", b"name", "shape", b"shape"]) -> None: ...
 
 global___BoundedTensorSpecProto = BoundedTensorSpecProto
 
-@typing_extensions.final
+@typing.final
 class TypeSpecProto(google.protobuf.message.Message):
     """Represents a tf.TypeSpec"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _TypeSpecClass:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -388,34 +398,35 @@
     """Subclasses of tf.ExtensionType"""
 
     TYPE_SPEC_CLASS_FIELD_NUMBER: builtins.int
     TYPE_STATE_FIELD_NUMBER: builtins.int
     TYPE_SPEC_CLASS_NAME_FIELD_NUMBER: builtins.int
     NUM_FLAT_COMPONENTS_FIELD_NUMBER: builtins.int
     type_spec_class: global___TypeSpecProto.TypeSpecClass.ValueType
-    @property
-    def type_state(self) -> global___StructuredValue:
-        """The value returned by TypeSpec._serialize()."""
     type_spec_class_name: builtins.str
     """The name of the TypeSpec class.
      * If type_spec_class == REGISTERED_TYPE_SPEC, the TypeSpec class is
        the one registered under this name. For types registered outside
        core TensorFlow by an add-on library, that library must be loaded
        before this value can be deserialized by nested_structure_coder.
      * If type_spec_class specifies a particular TypeSpec class, this field is
        redundant with the type_spec_class enum, and is only used for error
        reporting in older binaries that do not know the tupe_spec_class enum.
     """
     num_flat_components: builtins.int
     """The number of flat tensor components required by this TypeSpec."""
+    @property
+    def type_state(self) -> global___StructuredValue:
+        """The value returned by TypeSpec._serialize()."""
+
     def __init__(
         self,
         *,
         type_spec_class: global___TypeSpecProto.TypeSpecClass.ValueType | None = ...,
         type_state: global___StructuredValue | None = ...,
         type_spec_class_name: builtins.str | None = ...,
         num_flat_components: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["type_state", b"type_state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["num_flat_components", b"num_flat_components", "type_spec_class", b"type_spec_class", "type_spec_class_name", b"type_spec_class_name", "type_state", b"type_state"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["type_state", b"type_state"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["num_flat_components", b"num_flat_components", "type_spec_class", b"type_spec_class", "type_spec_class_name", b"type_spec_class_name", "type_state", b"type_state"]) -> None: ...
 
 global___TypeSpecProto = TypeSpecProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -19,15 +20,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class BundleHeaderProto(google.protobuf.message.Message):
     """Protos used in the tensor bundle module (tf/core/util/tensor_bundle/).
 
     Special header that is associated with a bundle.
 
     TODO(zongheng,zhifengc): maybe in the future, we can add information about
     which binary produced this checkpoint, timestamp, etc. Sometime, these can be
@@ -63,69 +64,71 @@
     VERSION_FIELD_NUMBER: builtins.int
     num_shards: builtins.int
     """Number of data files in the bundle."""
     endianness: global___BundleHeaderProto.Endianness.ValueType
     @property
     def version(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
         """Versioning of the tensor bundle format."""
+
     def __init__(
         self,
         *,
         num_shards: builtins.int | None = ...,
         endianness: global___BundleHeaderProto.Endianness.ValueType | None = ...,
         version: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["version", b"version"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["endianness", b"endianness", "num_shards", b"num_shards", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["version", b"version"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["endianness", b"endianness", "num_shards", b"num_shards", "version", b"version"]) -> None: ...
 
 global___BundleHeaderProto = BundleHeaderProto
 
-@typing_extensions.final
+@typing.final
 class BundleEntryProto(google.protobuf.message.Message):
     """Describes the metadata related to a checkpointed tensor."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DTYPE_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     SHARD_ID_FIELD_NUMBER: builtins.int
     OFFSET_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     CRC32C_FIELD_NUMBER: builtins.int
     SLICES_FIELD_NUMBER: builtins.int
     dtype: tensorflow.core.framework.types_pb2.DataType.ValueType
     """The tensor dtype and shape."""
-    @property
-    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
     shard_id: builtins.int
     """The binary content of the tensor lies in:
       File "shard_id": bytes [offset, offset + size).
     """
     offset: builtins.int
     size: builtins.int
     crc32c: builtins.int
     """The CRC32C checksum of the tensor bytes."""
     @property
+    def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto: ...
+    @property
     def slices(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto]:
         """Iff present, this entry represents a partitioned tensor.  The previous
         fields are interpreted as follows:
 
           "dtype", "shape": describe the full tensor.
           "shard_id", "offset", "size", "crc32c": all IGNORED.
              These information for each slice can be looked up in their own
              BundleEntryProto, keyed by each "slice_name".
         """
+
     def __init__(
         self,
         *,
         dtype: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         shard_id: builtins.int | None = ...,
         offset: builtins.int | None = ...,
         size: builtins.int | None = ...,
         crc32c: builtins.int | None = ...,
         slices: collections.abc.Iterable[tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["crc32c", b"crc32c", "dtype", b"dtype", "offset", b"offset", "shape", b"shape", "shard_id", b"shard_id", "size", b"size", "slices", b"slices"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["crc32c", b"crc32c", "dtype", b"dtype", "offset", b"offset", "shape", b"shape", "shard_id", b"shard_id", "size", b"size", "slices", b"slices"]) -> None: ...
 
 global___BundleEntryProto = BundleEntryProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,76 +12,80 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 import tensorflow.core.protobuf.cluster_pb2
 import tensorflow.core.protobuf.config_pb2
 import tensorflow.core.protobuf.device_filters_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ServerDef(google.protobuf.message.Message):
     """Defines the configuration of a single TensorFlow server."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CLUSTER_FIELD_NUMBER: builtins.int
     JOB_NAME_FIELD_NUMBER: builtins.int
     TASK_INDEX_FIELD_NUMBER: builtins.int
     DEFAULT_SESSION_CONFIG_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     PORT_FIELD_NUMBER: builtins.int
     CLUSTER_DEVICE_FILTERS_FIELD_NUMBER: builtins.int
-    @property
-    def cluster(self) -> tensorflow.core.protobuf.cluster_pb2.ClusterDef:
-        """The cluster of which this server is a member."""
     job_name: builtins.str
     """The name of the job of which this server is a member.
 
     NOTE(mrry): The `cluster` field must contain a `JobDef` with a `name` field
     that matches this name.
     """
     task_index: builtins.int
     """The task index of this server in its job.
 
     NOTE: The `cluster` field must contain a `JobDef` with a matching `name`
     and a mapping in its `tasks` field for this index.
     """
-    @property
-    def default_session_config(self) -> tensorflow.core.protobuf.config_pb2.ConfigProto:
-        """The default configuration for sessions that run on this server."""
     protocol: builtins.str
     """The protocol to be used by this server.
 
     Acceptable values include: "grpc", "grpc+verbs".
     """
     port: builtins.int
     """The server port. If not set, then we identify the port from the job_name."""
     @property
+    def cluster(self) -> tensorflow.core.protobuf.cluster_pb2.ClusterDef:
+        """The cluster of which this server is a member."""
+
+    @property
+    def default_session_config(self) -> tensorflow.core.protobuf.config_pb2.ConfigProto:
+        """The default configuration for sessions that run on this server."""
+
+    @property
     def cluster_device_filters(self) -> tensorflow.core.protobuf.device_filters_pb2.ClusterDeviceFilters:
         """Device filters for remote tasks in the cluster.
         NOTE: This is an experimental feature and only effective in TensorFlow 2.x.
         """
+
     def __init__(
         self,
         *,
         cluster: tensorflow.core.protobuf.cluster_pb2.ClusterDef | None = ...,
         job_name: builtins.str | None = ...,
         task_index: builtins.int | None = ...,
         default_session_config: tensorflow.core.protobuf.config_pb2.ConfigProto | None = ...,
         protocol: builtins.str | None = ...,
         port: builtins.int | None = ...,
         cluster_device_filters: tensorflow.core.protobuf.device_filters_pb2.ClusterDeviceFilters | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config", "job_name", b"job_name", "port", b"port", "protocol", b"protocol", "task_index", b"task_index"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["cluster", b"cluster", "cluster_device_filters", b"cluster_device_filters", "default_session_config", b"default_session_config", "job_name", b"job_name", "port", b"port", "protocol", b"protocol", "task_index", b"task_index"]) -> None: ...
 
 global___ServerDef = ServerDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -17,15 +18,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CompilationResultProto(google.protobuf.message.Message):
     """Describes the result of a TPU compilation. This is also used as TPU
     compilation result status payload.
     URI: "type.googleapis.com/tensorflow.tpu.CompilationResultProto"
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -46,22 +47,23 @@
     STATUS_CODE_FIELD_NUMBER: builtins.int
     STATUS_ERROR_MESSAGE_FIELD_NUMBER: builtins.int
     HLO_PROTOS_FIELD_NUMBER: builtins.int
     ERROR_CODE_FIELD_NUMBER: builtins.int
     status_code: tensorflow.tsl.protobuf.error_codes_pb2.Code.ValueType
     """The error message, if any, returned during compilation."""
     status_error_message: builtins.str
+    error_code: global___CompilationResultProto.ErrorCode.ValueType
     @property
     def hlo_protos(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.compiler.xla.service.hlo_pb2.HloProto]:
         """HLO proto."""
-    error_code: global___CompilationResultProto.ErrorCode.ValueType
+
     def __init__(
         self,
         *,
         status_code: tensorflow.tsl.protobuf.error_codes_pb2.Code.ValueType | None = ...,
         status_error_message: builtins.str | None = ...,
         hlo_protos: collections.abc.Iterable[tensorflow.compiler.xla.service.hlo_pb2.HloProto] | None = ...,
         error_code: global___CompilationResultProto.ErrorCode.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "hlo_protos", b"hlo_protos", "status_code", b"status_code", "status_error_message", b"status_error_message"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "hlo_protos", b"hlo_protos", "status_code", b"status_code", "status_error_message", b"status_error_message"]) -> None: ...
 
 global___CompilationResultProto = CompilationResultProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class PaddingMap(google.protobuf.message.Message):
     """A mapping between the dynamic shape dimension of an input and the arg that
     represents the real shape.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -32,10 +33,10 @@
     def __init__(
         self,
         *,
         arg_index: builtins.int | None = ...,
         shape_index: builtins.int | None = ...,
         padding_arg_index: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["arg_index", b"arg_index", "padding_arg_index", b"padding_arg_index", "shape_index", b"shape_index"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["arg_index", b"arg_index", "padding_arg_index", b"padding_arg_index", "shape_index", b"shape_index"]) -> None: ...
 
 global___PaddingMap = PaddingMap
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -15,38 +16,40 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class ClippingLimits(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LOWER_FIELD_NUMBER: builtins.int
     UPPER_FIELD_NUMBER: builtins.int
     @property
     def lower(self) -> google.protobuf.wrappers_pb2.FloatValue:
         """-inf if not set"""
+
     @property
     def upper(self) -> google.protobuf.wrappers_pb2.FloatValue:
         """+inf if not set"""
+
     def __init__(
         self,
         *,
         lower: google.protobuf.wrappers_pb2.FloatValue | None = ...,
         upper: google.protobuf.wrappers_pb2.FloatValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["lower", b"lower", "upper", b"upper"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lower", b"lower", "upper", b"upper"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["lower", b"lower", "upper", b"upper"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["lower", b"lower", "upper", b"upper"]) -> None: ...
 
 global___ClippingLimits = ClippingLimits
 
-@typing_extensions.final
+@typing.final
 class SimulatedQuantization(google.protobuf.message.Message):
     """Configuration for simulated quantization; simulated quantization is used to
     reduce training/serving skew when the serving variables are quantized. The
     same quantization operations are executed during training to minimize
     differences with serving.
 
     Simulated quantization inserts the following operations on the forward pass
@@ -62,32 +65,33 @@
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENABLED_FIELD_NUMBER: builtins.int
     CLIPPING_LIMITS_FIELD_NUMBER: builtins.int
     NUM_BUCKETS_FIELD_NUMBER: builtins.int
     enabled: builtins.bool
     """Whether simulated quantization is enabled."""
+    num_buckets: builtins.int
+    """Number of possible quantized values."""
     @property
     def clipping_limits(self) -> global___ClippingLimits:
         """Minimum and maximum values of the range used for quantization."""
-    num_buckets: builtins.int
-    """Number of possible quantized values."""
+
     def __init__(
         self,
         *,
         enabled: builtins.bool | None = ...,
         clipping_limits: global___ClippingLimits | None = ...,
         num_buckets: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["clipping_limits", b"clipping_limits"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["clipping_limits", b"clipping_limits", "enabled", b"enabled", "num_buckets", b"num_buckets"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["clipping_limits", b"clipping_limits"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["clipping_limits", b"clipping_limits", "enabled", b"enabled", "num_buckets", b"num_buckets"]) -> None: ...
 
 global___SimulatedQuantization = SimulatedQuantization
 
-@typing_extensions.final
+@typing.final
 class DynamicLearningRate(google.protobuf.message.Message):
     """Dynamic learning rate specification in the TPUEmbeddingConfiguration. The
     actual learning rates are provided as a scalar input list to the
     SendTPUEmbeddingGradients Op indexed by their tag specified through the
     following proto.
     """
 
@@ -123,19 +127,19 @@
     list of learning_rate scalars.
     """
     def __init__(
         self,
         *,
         tag: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tag", b"tag"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["tag", b"tag"]) -> None: ...
 
 global___DynamicLearningRate = DynamicLearningRate
 
-@typing_extensions.final
+@typing.final
 class LearningRate(google.protobuf.message.Message):
     """Source of learning rate to use."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONSTANT_FIELD_NUMBER: builtins.int
     DYNAMIC_FIELD_NUMBER: builtins.int
@@ -144,21 +148,21 @@
     def dynamic(self) -> global___DynamicLearningRate: ...
     def __init__(
         self,
         *,
         constant: builtins.float | None = ...,
         dynamic: global___DynamicLearningRate | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["constant", b"constant", "dynamic", b"dynamic", "learning_rate", b"learning_rate"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["constant", b"constant", "dynamic", b"dynamic", "learning_rate", b"learning_rate"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["learning_rate", b"learning_rate"]) -> typing_extensions.Literal["constant", "dynamic"] | None: ...
+    def HasField(self, field_name: typing.Literal["constant", b"constant", "dynamic", b"dynamic", "learning_rate", b"learning_rate"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["constant", b"constant", "dynamic", b"dynamic", "learning_rate", b"learning_rate"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["learning_rate", b"learning_rate"]) -> typing.Literal["constant", "dynamic"] | None: ...
 
 global___LearningRate = LearningRate
 
-@typing_extensions.final
+@typing.final
 class AdagradParameters(google.protobuf.message.Message):
     """Each optimizer's parameter proto has a link to its documentation and CPU
     implementation (if available) for user reference.
 
     https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adagrad
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L1634
     """
@@ -167,15 +171,15 @@
 
     def __init__(
         self,
     ) -> None: ...
 
 global___AdagradParameters = AdagradParameters
 
-@typing_extensions.final
+@typing.final
 class AdagradMomentumParameters(google.protobuf.message.Message):
     """This optimizer combines the Adagrad and Momentum update rules.
     accum(new) = beta2 == 1.0 ?
                  accum(old) + grad^2 :
                  beta2 * accum(old) + (1 - beta2) * grad^2
     accum_with_exponent = (accum(new) + epsilon)^(-1.0 / exponent)
     mom_accum(new) = momentum * mom_accum(old) + accum_with_exponent
@@ -208,19 +212,19 @@
         *,
         momentum: builtins.float | None = ...,
         use_nesterov: builtins.bool | None = ...,
         exponent: builtins.float | None = ...,
         beta2: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["beta2", b"beta2", "epsilon", b"epsilon", "exponent", b"exponent", "momentum", b"momentum", "use_nesterov", b"use_nesterov"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["beta2", b"beta2", "epsilon", b"epsilon", "exponent", b"exponent", "momentum", b"momentum", "use_nesterov", b"use_nesterov"]) -> None: ...
 
 global___AdagradMomentumParameters = AdagradMomentumParameters
 
-@typing_extensions.final
+@typing.final
 class BoundedAdagradParameters(google.protobuf.message.Message):
     """Algorithm in http://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     UPDATE_ACCUMULATOR_FIRST_FIELD_NUMBER: builtins.int
     MAX_VAR_UPDATE_FIELD_NUMBER: builtins.int
@@ -241,33 +245,33 @@
     def __init__(
         self,
         *,
         update_accumulator_first: builtins.bool | None = ...,
         max_var_update: builtins.float | None = ...,
         max_accumulator: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_accumulator", b"max_accumulator", "max_var_update", b"max_var_update", "update_accumulator_first", b"update_accumulator_first"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_accumulator", b"max_accumulator", "max_var_update", b"max_var_update", "update_accumulator_first", b"update_accumulator_first"]) -> None: ...
 
 global___BoundedAdagradParameters = BoundedAdagradParameters
 
-@typing_extensions.final
+@typing.final
 class StochasticGradientDescentParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/SGD
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L629
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___StochasticGradientDescentParameters = StochasticGradientDescentParameters
 
-@typing_extensions.final
+@typing.final
 class FtrlParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Ftrl
     https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41159.pdf
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L2646
 
     The hyperparameters for FTRL are the same as for the Keras implementation,
     with some additions. The "beta" parameter matches the behavior described in
@@ -309,19 +313,19 @@
         l1: builtins.float | None = ...,
         l2: builtins.float | None = ...,
         lr_power: builtins.float | None = ...,
         beta: builtins.float | None = ...,
         multiply_linear_by_lr: builtins.bool | None = ...,
         allow_zero_accumulator: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_zero_accumulator", b"allow_zero_accumulator", "beta", b"beta", "l1", b"l1", "l2", b"l2", "lr_power", b"lr_power", "multiply_linear_by_lr", b"multiply_linear_by_lr"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["allow_zero_accumulator", b"allow_zero_accumulator", "beta", b"beta", "l1", b"l1", "l2", b"l2", "lr_power", b"lr_power", "multiply_linear_by_lr", b"multiply_linear_by_lr"]) -> None: ...
 
 global___FtrlParameters = FtrlParameters
 
-@typing_extensions.final
+@typing.final
 class AdamParameters(google.protobuf.message.Message):
     """The Adam optimizer does not implement hyper-parameter update due to hardware
     limitations; use the dynamic learning rate feature instead, setting the
     learning rate to: user learning_rate * sqrt(1 - beta2^t) / (1 - beta1^t)
     Here, t is the current timestep.
 
     https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adam
@@ -358,19 +362,19 @@
         *,
         beta1: builtins.float | None = ...,
         beta2: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
         use_non_lazy_adam: builtins.bool | None = ...,
         use_sum_inside_sqrt: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["beta1", b"beta1", "beta2", b"beta2", "epsilon", b"epsilon", "use_non_lazy_adam", b"use_non_lazy_adam", "use_sum_inside_sqrt", b"use_sum_inside_sqrt"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["beta1", b"beta1", "beta2", b"beta2", "epsilon", b"epsilon", "use_non_lazy_adam", b"use_non_lazy_adam", "use_sum_inside_sqrt", b"use_sum_inside_sqrt"]) -> None: ...
 
 global___AdamParameters = AdamParameters
 
-@typing_extensions.final
+@typing.final
 class MomentumParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/SGD
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L3068
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -380,19 +384,19 @@
     use_nesterov: builtins.bool
     def __init__(
         self,
         *,
         momentum: builtins.float | None = ...,
         use_nesterov: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["momentum", b"momentum", "use_nesterov", b"use_nesterov"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["momentum", b"momentum", "use_nesterov", b"use_nesterov"]) -> None: ...
 
 global___MomentumParameters = MomentumParameters
 
-@typing_extensions.final
+@typing.final
 class RmsPropParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/RMSprop
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L4229
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -405,19 +409,19 @@
     def __init__(
         self,
         *,
         rho: builtins.float | None = ...,
         momentum: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["epsilon", b"epsilon", "momentum", b"momentum", "rho", b"rho"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["epsilon", b"epsilon", "momentum", b"momentum", "rho", b"rho"]) -> None: ...
 
 global___RmsPropParameters = RmsPropParameters
 
-@typing_extensions.final
+@typing.final
 class CenteredRmsPropParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/RMSprop
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L4358
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -430,19 +434,19 @@
     def __init__(
         self,
         *,
         rho: builtins.float | None = ...,
         momentum: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["epsilon", b"epsilon", "momentum", b"momentum", "rho", b"rho"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["epsilon", b"epsilon", "momentum", b"momentum", "rho", b"rho"]) -> None: ...
 
 global___CenteredRmsPropParameters = CenteredRmsPropParameters
 
-@typing_extensions.final
+@typing.final
 class MdlAdagradLightParameters(google.protobuf.message.Message):
     """Variant of algorithm in http://proceedings.mlr.press/v44/shamir15.pdf"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     L2_FIELD_NUMBER: builtins.int
     LR_POWER_FIELD_NUMBER: builtins.int
@@ -480,19 +484,19 @@
         benefit_revisit_scale: builtins.float | None = ...,
         max_event_benefit: builtins.float | None = ...,
         max_total_benefit: builtins.float | None = ...,
         mdl_hard_limit: builtins.float | None = ...,
         hard_limit_min_benefit: builtins.bool | None = ...,
         mdl_regularize: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["benefit_revisit_scale", b"benefit_revisit_scale", "hard_limit_min_benefit", b"hard_limit_min_benefit", "l2", b"l2", "lr_power", b"lr_power", "max_event_benefit", b"max_event_benefit", "max_total_benefit", b"max_total_benefit", "mdl_benefit_rampup_coeff", b"mdl_benefit_rampup_coeff", "mdl_hard_limit", b"mdl_hard_limit", "mdl_min_weight", b"mdl_min_weight", "mdl_mix_in_margin", b"mdl_mix_in_margin", "mdl_regularize", b"mdl_regularize", "min_servable_mdl_benefit", b"min_servable_mdl_benefit"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["benefit_revisit_scale", b"benefit_revisit_scale", "hard_limit_min_benefit", b"hard_limit_min_benefit", "l2", b"l2", "lr_power", b"lr_power", "max_event_benefit", b"max_event_benefit", "max_total_benefit", b"max_total_benefit", "mdl_benefit_rampup_coeff", b"mdl_benefit_rampup_coeff", "mdl_hard_limit", b"mdl_hard_limit", "mdl_min_weight", b"mdl_min_weight", "mdl_mix_in_margin", b"mdl_mix_in_margin", "mdl_regularize", b"mdl_regularize", "min_servable_mdl_benefit", b"min_servable_mdl_benefit"]) -> None: ...
 
 global___MdlAdagradLightParameters = MdlAdagradLightParameters
 
-@typing_extensions.final
+@typing.final
 class AdadeltaParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/keras/optimizers/Adadelta
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L933
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -502,19 +506,19 @@
     epsilon: builtins.float
     def __init__(
         self,
         *,
         rho: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["epsilon", b"epsilon", "rho", b"rho"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["epsilon", b"epsilon", "rho", b"rho"]) -> None: ...
 
 global___AdadeltaParameters = AdadeltaParameters
 
-@typing_extensions.final
+@typing.final
 class ProximalAdagradParameters(google.protobuf.message.Message):
     """https://www.tensorflow.org/api_docs/python/tf/compat/v1/train/ProximalAdagradOptimizer
     https://github.com/tensorflow/tensorflow/blob/6b6471f3ffb7f1fefe42d814aa5fb9ab7a535b58/tensorflow/core/kernels/training_ops.cc#L1961
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -524,19 +528,19 @@
     l2: builtins.float
     def __init__(
         self,
         *,
         l1: builtins.float | None = ...,
         l2: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["l1", b"l1", "l2", b"l2"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["l1", b"l1", "l2", b"l2"]) -> None: ...
 
 global___ProximalAdagradParameters = ProximalAdagradParameters
 
-@typing_extensions.final
+@typing.final
 class OnlineYogiParameters(google.protobuf.message.Message):
     """The online Yogi optimizer does not implement hyper-parameter update; use the
     dynamic learning rate feature instead, setting the learning rate to:
     user learning_rate * sqrt(1 - beta2^t) / (1 - beta1^t)
     Here, t is the current timestep.
 
     https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization.pdf
@@ -559,19 +563,19 @@
     def __init__(
         self,
         *,
         l1: builtins.float | None = ...,
         l2: builtins.float | None = ...,
         beta2: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["beta2", b"beta2", "l1", b"l1", "l2", b"l2"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["beta2", b"beta2", "l1", b"l1", "l2", b"l2"]) -> None: ...
 
 global___OnlineYogiParameters = OnlineYogiParameters
 
-@typing_extensions.final
+@typing.final
 class ProximalYogiParameters(google.protobuf.message.Message):
     """The online Yogi optimizer does not implement hyper-parameter update; use the
     dynamic learning rate feature instead, setting the learning rate to:
     user learning_rate * sqrt(1 - beta2^t) / (1 - beta1^t)
     Here, t is the current timestep.
 
     https://papers.nips.cc/paper/8186-adaptive-methods-for-nonconvex-optimization.pdf
@@ -602,19 +606,19 @@
         *,
         l1: builtins.float | None = ...,
         l2: builtins.float | None = ...,
         beta1: builtins.float | None = ...,
         beta2: builtins.float | None = ...,
         epsilon: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["beta1", b"beta1", "beta2", b"beta2", "epsilon", b"epsilon", "l1", b"l1", "l2", b"l2"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["beta1", b"beta1", "beta2", b"beta2", "epsilon", b"epsilon", "l1", b"l1", "l2", b"l2"]) -> None: ...
 
 global___ProximalYogiParameters = ProximalYogiParameters
 
-@typing_extensions.final
+@typing.final
 class FrequencyEstimatorParameters(google.protobuf.message.Message):
     """Estimator for the frequency of updates to a lookup table. It maintains an
     array (tf.Variable) D, where each element records the average number of
     global steps between two consecutive batches that hit the corresponding
     bucket. Once an item with bucket id i is sampled, D[i] is updated by:
       D[i] <- D[i] * (1 - tau) + delta[i] * tau,
 
@@ -660,19 +664,19 @@
         self,
         *,
         tau: builtins.float | None = ...,
         max_delta: builtins.float | None = ...,
         outlier_threshold: builtins.float | None = ...,
         weight_exponent: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_delta", b"max_delta", "outlier_threshold", b"outlier_threshold", "tau", b"tau", "weight_exponent", b"weight_exponent"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["max_delta", b"max_delta", "outlier_threshold", b"outlier_threshold", "tau", b"tau", "weight_exponent", b"weight_exponent"]) -> None: ...
 
 global___FrequencyEstimatorParameters = FrequencyEstimatorParameters
 
-@typing_extensions.final
+@typing.final
 class UserDefinedProgramParameters(google.protobuf.message.Message):
     """A user-defined optimizer.
     The contained HLO program must take the following arguments in the following
     order:
     1.  gradients
     2.  table weights
     3.  slot variables
@@ -697,20 +701,20 @@
     @property
     def program(self) -> tensorflow.compiler.xla.service.hlo_pb2.HloModuleProto: ...
     def __init__(
         self,
         *,
         program: tensorflow.compiler.xla.service.hlo_pb2.HloModuleProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["program", b"program"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["program", b"program"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["program", b"program"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["program", b"program"]) -> None: ...
 
 global___UserDefinedProgramParameters = UserDefinedProgramParameters
 
-@typing_extensions.final
+@typing.final
 class AssignParameters(google.protobuf.message.Message):
     """Optimizer that just sets the variable to the value of the gradient. To be
     correct, this requires either gradient accumulation (to sum the values of a
     computed expression across the samples) or to deduplicate IDs within a single
     host (to assign the value from an arbitrary sample).
     """
 
@@ -718,15 +722,15 @@
 
     def __init__(
         self,
     ) -> None: ...
 
 global___AssignParameters = AssignParameters
 
-@typing_extensions.final
+@typing.final
 class GradientAccumulationStatus(google.protobuf.message.Message):
     """Status of using gradient accumulation (doing two passes over the input
     gradients: one to accumulate them into a temporary array and another to apply
     them using the actual optimization algorithm). The extra message is to wrap
     the enum for scoping.
     """
 
@@ -751,15 +755,15 @@
 
     def __init__(
         self,
     ) -> None: ...
 
 global___GradientAccumulationStatus = GradientAccumulationStatus
 
-@typing_extensions.final
+@typing.final
 class LowDimensionalPackingStatus(google.protobuf.message.Message):
     """Whether to optimize the packing of low-dimensional embedding tables in HBM
     (high bandwidth memory). TPUs access HBM at 32-byte (8-float) granularity.
     For functional correctness, the TPU software internally pads the embedding
     dimension to a multiple of 8. This can sometimes lead to significant memory
     wastage due to padding. For 1-dimensional, 2-dimensional, and 4-dimensional,
     the TPU software can remove this padding by packing multiple rows into the
@@ -828,15 +832,15 @@
 
     def __init__(
         self,
     ) -> None: ...
 
 global___LowDimensionalPackingStatus = LowDimensionalPackingStatus
 
-@typing_extensions.final
+@typing.final
 class HotIdReplicationConfiguration(google.protobuf.message.Message):
     """Configuration proto for hot ID optimization. This is an experimental feature
     that is currently disabled (by default).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -866,19 +870,19 @@
     STATUS_FIELD_NUMBER: builtins.int
     status: global___HotIdReplicationConfiguration.Status.ValueType
     def __init__(
         self,
         *,
         status: global___HotIdReplicationConfiguration.Status.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["status", b"status"]) -> None: ...
 
 global___HotIdReplicationConfiguration = HotIdReplicationConfiguration
 
-@typing_extensions.final
+@typing.final
 class OptimizationParameters(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LEARNING_RATE_FIELD_NUMBER: builtins.int
     CLIPPING_LIMITS_FIELD_NUMBER: builtins.int
     GRADIENT_CLIPPING_LIMITS_FIELD_NUMBER: builtins.int
     WEIGHT_DECAY_FACTOR_FIELD_NUMBER: builtins.int
@@ -900,61 +904,66 @@
     ADADELTA_FIELD_NUMBER: builtins.int
     PROXIMAL_ADAGRAD_FIELD_NUMBER: builtins.int
     ONLINE_YOGI_FIELD_NUMBER: builtins.int
     PROXIMAL_YOGI_FIELD_NUMBER: builtins.int
     FREQUENCY_ESTIMATOR_FIELD_NUMBER: builtins.int
     USER_DEFINED_PROGRAM_FIELD_NUMBER: builtins.int
     ASSIGN_FIELD_NUMBER: builtins.int
-    @property
-    def learning_rate(self) -> global___LearningRate:
-        """Learning rate used for updating the embedding layer parameters."""
-    @property
-    def clipping_limits(self) -> global___ClippingLimits:
-        """Limits to which to clip the weight values after the backward pass; not
-        present means no limits are applied.
-        """
-    @property
-    def gradient_clipping_limits(self) -> global___ClippingLimits:
-        """Limits to which to clip the backward pass gradient before using it for
-        updates; not present means no limits are applied.
-        """
     weight_decay_factor: builtins.float
     """Amount of weight decay to apply; see weight_decay_optimizers.py for
     details. All optimizers except MDL Adagrad Light are supported with this
     option. Although there is no check, users who want weight decay will also
     want to ensure that gradient accumulation is enabled so that the decay will
     happen once per global batch.
     """
     multiply_weight_decay_factor_by_learning_rate: builtins.bool
     """If true, the weight decay factor is multiplied by the current learning rate
     before use; this is to match the note in DecoupledWeightDecayExtension in
     weight_decay_optimizers.py.
     """
-    @property
-    def simulated_quantization(self) -> global___SimulatedQuantization:
-        """Configuration for simulated quantization which is used to reduce
-        training/serving skew when the serving variables are quantized. The same
-        quantization operations are executed during training to minimize
-        differences with serving.
-        """
     gradient_accumulation_status: global___GradientAccumulationStatus.Status.ValueType
     """Status of using gradient accumulation (doing two passes over the input
     gradients: one to accumulate them into a temporary array and another to
     apply them using the actual optimization algorithm).
     """
     low_dimensional_packing_status: global___LowDimensionalPackingStatus.Status.ValueType
     """Status of the low-dimensional embedding packing optimization. This controls
     whether to optimize the packing of 1-dimensional, 2-dimensional, and
     4-dimensional embedding tables in memory.
     """
     @property
+    def learning_rate(self) -> global___LearningRate:
+        """Learning rate used for updating the embedding layer parameters."""
+
+    @property
+    def clipping_limits(self) -> global___ClippingLimits:
+        """Limits to which to clip the weight values after the backward pass; not
+        present means no limits are applied.
+        """
+
+    @property
+    def gradient_clipping_limits(self) -> global___ClippingLimits:
+        """Limits to which to clip the backward pass gradient before using it for
+        updates; not present means no limits are applied.
+        """
+
+    @property
+    def simulated_quantization(self) -> global___SimulatedQuantization:
+        """Configuration for simulated quantization which is used to reduce
+        training/serving skew when the serving variables are quantized. The same
+        quantization operations are executed during training to minimize
+        differences with serving.
+        """
+
+    @property
     def hot_id_replication_configuration(self) -> global___HotIdReplicationConfiguration:
         """Configuration proto for hot ID replication. This is an experimental
         feature that is currently disabled (by default).
         """
+
     @property
     def adagrad(self) -> global___AdagradParameters: ...
     @property
     def adagrad_momentum(self) -> global___AdagradMomentumParameters: ...
     @property
     def bounded_adagrad(self) -> global___BoundedAdagradParameters: ...
     @property
@@ -1011,42 +1020,42 @@
         proximal_adagrad: global___ProximalAdagradParameters | None = ...,
         online_yogi: global___OnlineYogiParameters | None = ...,
         proximal_yogi: global___ProximalYogiParameters | None = ...,
         frequency_estimator: global___FrequencyEstimatorParameters | None = ...,
         user_defined_program: global___UserDefinedProgramParameters | None = ...,
         assign: global___AssignParameters | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_accumulation_status", b"gradient_accumulation_status", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "low_dimensional_packing_status", b"low_dimensional_packing_status", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "multiply_weight_decay_factor_by_learning_rate", b"multiply_weight_decay_factor_by_learning_rate", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program", "weight_decay_factor", b"weight_decay_factor"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["parameters", b"parameters"]) -> typing_extensions.Literal["adagrad", "adagrad_momentum", "bounded_adagrad", "stochastic_gradient_descent", "ftrl", "adam", "momentum", "rms_prop", "centered_rms_prop", "mdl_adagrad_light", "adadelta", "proximal_adagrad", "online_yogi", "proximal_yogi", "frequency_estimator", "user_defined_program", "assign"] | None: ...
+    def HasField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["adadelta", b"adadelta", "adagrad", b"adagrad", "adagrad_momentum", b"adagrad_momentum", "adam", b"adam", "assign", b"assign", "bounded_adagrad", b"bounded_adagrad", "centered_rms_prop", b"centered_rms_prop", "clipping_limits", b"clipping_limits", "frequency_estimator", b"frequency_estimator", "ftrl", b"ftrl", "gradient_accumulation_status", b"gradient_accumulation_status", "gradient_clipping_limits", b"gradient_clipping_limits", "hot_id_replication_configuration", b"hot_id_replication_configuration", "learning_rate", b"learning_rate", "low_dimensional_packing_status", b"low_dimensional_packing_status", "mdl_adagrad_light", b"mdl_adagrad_light", "momentum", b"momentum", "multiply_weight_decay_factor_by_learning_rate", b"multiply_weight_decay_factor_by_learning_rate", "online_yogi", b"online_yogi", "parameters", b"parameters", "proximal_adagrad", b"proximal_adagrad", "proximal_yogi", b"proximal_yogi", "rms_prop", b"rms_prop", "simulated_quantization", b"simulated_quantization", "stochastic_gradient_descent", b"stochastic_gradient_descent", "user_defined_program", b"user_defined_program", "weight_decay_factor", b"weight_decay_factor"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["parameters", b"parameters"]) -> typing.Literal["adagrad", "adagrad_momentum", "bounded_adagrad", "stochastic_gradient_descent", "ftrl", "adam", "momentum", "rms_prop", "centered_rms_prop", "mdl_adagrad_light", "adadelta", "proximal_adagrad", "online_yogi", "proximal_yogi", "frequency_estimator", "user_defined_program", "assign"] | None: ...
 
 global___OptimizationParameters = OptimizationParameters
 
-@typing_extensions.final
+@typing.final
 class StateVariableSpecification(google.protobuf.message.Message):
     """Specification of an optimization algorithm's state variables (both the main
     value vector and any extra accumulators, etc.). This proto is only used
     internally by the TPU software and is not exposed directly to the TF model.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class UserDefined(google.protobuf.message.Message):
         """A normal state variable that should be saved and restored in checkpoints
         and used as an input or output to non-debug TensorFlow ops.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         def __init__(
             self,
         ) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class FillWithConstant(google.protobuf.message.Message):
         """A state variable that should be filled with a constant and normally hidden
         from users (used for intermediate gradients being accumulated, for
         example).
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -1054,15 +1063,15 @@
         INITIAL_VALUE_FIELD_NUMBER: builtins.int
         initial_value: builtins.float
         def __init__(
             self,
             *,
             initial_value: builtins.float | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["initial_value", b"initial_value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["initial_value", b"initial_value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     USER_DEFINED_FIELD_NUMBER: builtins.int
     FILL_WITH_CONSTANT_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Parameter name for the state variable."""
     @property
@@ -1072,12 +1081,12 @@
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         user_defined: global___StateVariableSpecification.UserDefined | None = ...,
         fill_with_constant: global___StateVariableSpecification.FillWithConstant | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["fill_with_constant", b"fill_with_constant", "usage", b"usage", "user_defined", b"user_defined"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fill_with_constant", b"fill_with_constant", "name", b"name", "usage", b"usage", "user_defined", b"user_defined"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["usage", b"usage"]) -> typing_extensions.Literal["user_defined", "fill_with_constant"] | None: ...
+    def HasField(self, field_name: typing.Literal["fill_with_constant", b"fill_with_constant", "usage", b"usage", "user_defined", b"user_defined"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["fill_with_constant", b"fill_with_constant", "name", b"name", "usage", b"usage", "user_defined", b"user_defined"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["usage", b"usage"]) -> typing.Literal["user_defined", "fill_with_constant"] | None: ...
 
 global___StateVariableSpecification = StateVariableSpecification
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -15,15 +16,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TPUHardwareFeature(google.protobuf.message.Message):
     """Describes features of a tpu."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _EmbeddingFeature:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -63,58 +64,61 @@
     EMBEDDING_FEATURE_FIELD_NUMBER: builtins.int
     embedding_feature: global___TPUHardwareFeature.EmbeddingFeature.ValueType
     def __init__(
         self,
         *,
         embedding_feature: global___TPUHardwareFeature.EmbeddingFeature.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["embedding_feature", b"embedding_feature"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["embedding_feature", b"embedding_feature"]) -> None: ...
 
 global___TPUHardwareFeature = TPUHardwareFeature
 
-@typing_extensions.final
+@typing.final
 class TopologyProto(google.protobuf.message.Message):
     """Describes the geometry of a TPU mesh."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MESH_SHAPE_FIELD_NUMBER: builtins.int
     NUM_TASKS_FIELD_NUMBER: builtins.int
     NUM_TPU_DEVICES_PER_TASK_FIELD_NUMBER: builtins.int
     DEVICE_COORDINATES_FIELD_NUMBER: builtins.int
     TPU_HARDWARE_FEATURE_FIELD_NUMBER: builtins.int
+    num_tasks: builtins.int
+    """Number of TensorFlow tasks in the cluster."""
+    num_tpu_devices_per_task: builtins.int
+    """Number of TPU devices per task."""
     @property
     def mesh_shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """The dimensions of the TPU topology, in cores. Typically, this is a 4D
         topology [x, y, z, core], where the major dimensions correspond to TPU
         chips, and the minor dimension describes the number of cores on a multicore
         chip.
         """
-    num_tasks: builtins.int
-    """Number of TensorFlow tasks in the cluster."""
-    num_tpu_devices_per_task: builtins.int
-    """Number of TPU devices per task."""
+
     @property
     def device_coordinates(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """A flattened rank 3 int32 array with shape
         [num_tasks, num_tpu_devices_per_task, len(mesh_shape)].
         `tasks` is the number of tasks in the TPU cluster, `devices` is the number
         of TPU devices per task, and the minor dimension corresponds to a position
         in the TPU mesh topology. Each entry [task, device, axis] gives the
         `axis`-th coordinate in the topology of a task/device pair.
         """
+
     @property
     def tpu_hardware_feature(self) -> global___TPUHardwareFeature:
         """TPU supported features."""
+
     def __init__(
         self,
         *,
         mesh_shape: collections.abc.Iterable[builtins.int] | None = ...,
         num_tasks: builtins.int | None = ...,
         num_tpu_devices_per_task: builtins.int | None = ...,
         device_coordinates: collections.abc.Iterable[builtins.int] | None = ...,
         tpu_hardware_feature: global___TPUHardwareFeature | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["tpu_hardware_feature", b"tpu_hardware_feature"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_coordinates", b"device_coordinates", "mesh_shape", b"mesh_shape", "num_tasks", b"num_tasks", "num_tpu_devices_per_task", b"num_tpu_devices_per_task", "tpu_hardware_feature", b"tpu_hardware_feature"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["tpu_hardware_feature", b"tpu_hardware_feature"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["device_coordinates", b"device_coordinates", "mesh_shape", b"mesh_shape", "num_tasks", b"num_tasks", "num_tpu_devices_per_task", b"num_tpu_devices_per_task", "tpu_hardware_feature", b"tpu_hardware_feature"]) -> None: ...
 
 global___TopologyProto = TopologyProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -16,15 +17,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TPUEmbeddingConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Mode:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -68,15 +69,15 @@
         This partitioning strategy exactly follows that in the embedding_lookup
         TensorFlow function at tensorflow/python/ops/embedding_ops.py.
         """
 
     DIV_DEFAULT: TPUEmbeddingConfiguration.ShardingStrategy.ValueType  # 0
     MOD: TPUEmbeddingConfiguration.ShardingStrategy.ValueType  # 1
 
-    @typing_extensions.final
+    @typing.final
     class TableDescriptor(google.protobuf.message.Message):
         """Description of the various embedding tables."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         VOCABULARY_SIZE_FIELD_NUMBER: builtins.int
@@ -92,27 +93,28 @@
         num_features: builtins.int
         """Number of features mapped to this table."""
         @property
         def optimization_parameters(self) -> tensorflow.core.protobuf.tpu.optimization_parameters_pb2.OptimizationParameters:
             """Details of the learning algorithm used to update the embedding
             parameters.
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             vocabulary_size: builtins.int | None = ...,
             dimension: builtins.int | None = ...,
             num_features: builtins.int | None = ...,
             optimization_parameters: tensorflow.core.protobuf.tpu.optimization_parameters_pb2.OptimizationParameters | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["optimization_parameters", b"optimization_parameters"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["dimension", b"dimension", "name", b"name", "num_features", b"num_features", "optimization_parameters", b"optimization_parameters", "vocabulary_size", b"vocabulary_size"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["optimization_parameters", b"optimization_parameters"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["dimension", b"dimension", "name", b"name", "num_features", b"num_features", "optimization_parameters", b"optimization_parameters", "vocabulary_size", b"vocabulary_size"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class FeatureDescriptor(google.protobuf.message.Message):
         """Description of different input features."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         TABLE_ID_FIELD_NUMBER: builtins.int
@@ -127,24 +129,25 @@
             the shape of the actual inputs provided using the infeed op must be
             strictly smaller than input_shape. The outputs received at the TensorCore
             will have rank = input_shape.size() + 1. The innermost axis corresponds
             to the embedding dimension. If the input has shape [m, n, k] (excluding
             the reduction axis) and the embedding dimension is d, the output received
             at the TensorCore will have shape [m, n, k, d].
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             table_id: builtins.int | None = ...,
             input_shape: collections.abc.Iterable[builtins.int] | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["input_shape", b"input_shape", "name", b"name", "table_id", b"table_id"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["input_shape", b"input_shape", "name", b"name", "table_id", b"table_id"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class SpmdSharding(google.protobuf.message.Message):
         """SPMD (Single Program Multiple Data) sharding configuration for
         TPUEmbedding. When model parallelism is used on the TensorCore, the number
         of cores per replica must be passed to TPUEmbedding so that the right
         shapes can be computed in the TF/XLA bridge.
         """
 
@@ -158,28 +161,26 @@
         """Number of cores per replica."""
         def __init__(
             self,
             *,
             enabled: builtins.bool | None = ...,
             num_cores_per_replica: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["enabled", b"enabled", "num_cores_per_replica", b"num_cores_per_replica"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["enabled", b"enabled", "num_cores_per_replica", b"num_cores_per_replica"]) -> None: ...
 
     TABLE_DESCRIPTOR_FIELD_NUMBER: builtins.int
     MODE_FIELD_NUMBER: builtins.int
     BATCH_SIZE_PER_TENSOR_CORE_FIELD_NUMBER: builtins.int
     NUM_HOSTS_FIELD_NUMBER: builtins.int
     NUM_TENSOR_CORES_FIELD_NUMBER: builtins.int
     SHARDING_STRATEGY_FIELD_NUMBER: builtins.int
     PIPELINE_EXECUTION_WITH_TENSOR_CORE_FIELD_NUMBER: builtins.int
     PROFILE_DATA_DIRECTORY_FIELD_NUMBER: builtins.int
     FEATURE_DESCRIPTOR_FIELD_NUMBER: builtins.int
     SPMD_SHARDING_FIELD_NUMBER: builtins.int
-    @property
-    def table_descriptor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TPUEmbeddingConfiguration.TableDescriptor]: ...
     mode: global___TPUEmbeddingConfiguration.Mode.ValueType
     batch_size_per_tensor_core: builtins.int
     """Number of samples in each batch of embedding layer activations sent to
     the TensorCore.
     """
     num_hosts: builtins.int
     """Number of TPU hosts used for inference/training."""
@@ -227,19 +228,22 @@
     filename corresponding to each table is obtained by hashing table specific
     parameters (e.g., table name and number of features) and global
     configuration parameters (e.g., sharding strategy and TPU worker task
     count). The same profile data directory can be shared amongst several
     models to reuse embedding lookup statistics.
     """
     @property
+    def table_descriptor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TPUEmbeddingConfiguration.TableDescriptor]: ...
+    @property
     def feature_descriptor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TPUEmbeddingConfiguration.FeatureDescriptor]:
         """If the feature_descriptor field is populated, the model should NOT populate
         TableDescriptor.num_features and batch_size_per_tensor_core. These two
         fields will be auto-populated by the TPUEmbedding rewrite passes.
         """
+
     @property
     def spmd_sharding(self) -> global___TPUEmbeddingConfiguration.SpmdSharding: ...
     def __init__(
         self,
         *,
         table_descriptor: collections.abc.Iterable[global___TPUEmbeddingConfiguration.TableDescriptor] | None = ...,
         mode: global___TPUEmbeddingConfiguration.Mode.ValueType | None = ...,
@@ -248,20 +252,20 @@
         num_tensor_cores: builtins.int | None = ...,
         sharding_strategy: global___TPUEmbeddingConfiguration.ShardingStrategy.ValueType | None = ...,
         pipeline_execution_with_tensor_core: builtins.bool | None = ...,
         profile_data_directory: builtins.str | None = ...,
         feature_descriptor: collections.abc.Iterable[global___TPUEmbeddingConfiguration.FeatureDescriptor] | None = ...,
         spmd_sharding: global___TPUEmbeddingConfiguration.SpmdSharding | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["spmd_sharding", b"spmd_sharding"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["batch_size_per_tensor_core", b"batch_size_per_tensor_core", "feature_descriptor", b"feature_descriptor", "mode", b"mode", "num_hosts", b"num_hosts", "num_tensor_cores", b"num_tensor_cores", "pipeline_execution_with_tensor_core", b"pipeline_execution_with_tensor_core", "profile_data_directory", b"profile_data_directory", "sharding_strategy", b"sharding_strategy", "spmd_sharding", b"spmd_sharding", "table_descriptor", b"table_descriptor"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["spmd_sharding", b"spmd_sharding"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["batch_size_per_tensor_core", b"batch_size_per_tensor_core", "feature_descriptor", b"feature_descriptor", "mode", b"mode", "num_hosts", b"num_hosts", "num_tensor_cores", b"num_tensor_cores", "pipeline_execution_with_tensor_core", b"pipeline_execution_with_tensor_core", "profile_data_directory", b"profile_data_directory", "sharding_strategy", b"sharding_strategy", "spmd_sharding", b"spmd_sharding", "table_descriptor", b"table_descriptor"]) -> None: ...
 
 global___TPUEmbeddingConfiguration = TPUEmbeddingConfiguration
 
-@typing_extensions.final
+@typing.final
 class TPUEmbeddingError(google.protobuf.message.Message):
     """A placeholder message that is used to define a unique Status payload
     URL for TPU embedding errors.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.wrappers_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class TrackableObjectGraph(google.protobuf.message.Message):
     """A TensorBundle addition which saves extra information about the objects which
     own variables, allowing for more robust checkpoint loading into modified
     programs.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class TrackableObject(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-        @typing_extensions.final
+        @typing.final
         class ObjectReference(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             NODE_ID_FIELD_NUMBER: builtins.int
             LOCAL_NAME_FIELD_NUMBER: builtins.int
             node_id: builtins.int
             """An index into `TrackableObjectGraph.nodes`, indicating the object
@@ -40,17 +41,17 @@
             """A user-provided name for the edge."""
             def __init__(
                 self,
                 *,
                 node_id: builtins.int | None = ...,
                 local_name: builtins.str | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["local_name", b"local_name", "node_id", b"node_id"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["local_name", b"local_name", "node_id", b"node_id"]) -> None: ...
 
-        @typing_extensions.final
+        @typing.final
         class SerializedTensor(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             NAME_FIELD_NUMBER: builtins.int
             FULL_NAME_FIELD_NUMBER: builtins.int
             CHECKPOINT_KEY_FIELD_NUMBER: builtins.int
             name: builtins.str
@@ -69,17 +70,17 @@
             def __init__(
                 self,
                 *,
                 name: builtins.str | None = ...,
                 full_name: builtins.str | None = ...,
                 checkpoint_key: builtins.str | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["checkpoint_key", b"checkpoint_key", "full_name", b"full_name", "name", b"name"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["checkpoint_key", b"checkpoint_key", "full_name", b"full_name", "name", b"name"]) -> None: ...
 
-        @typing_extensions.final
+        @typing.final
         class SlotVariableReference(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
             ORIGINAL_VARIABLE_NODE_ID_FIELD_NUMBER: builtins.int
             SLOT_NAME_FIELD_NUMBER: builtins.int
             SLOT_VARIABLE_NODE_ID_FIELD_NUMBER: builtins.int
             original_variable_node_id: builtins.int
@@ -95,67 +96,72 @@
             def __init__(
                 self,
                 *,
                 original_variable_node_id: builtins.int | None = ...,
                 slot_name: builtins.str | None = ...,
                 slot_variable_node_id: builtins.int | None = ...,
             ) -> None: ...
-            def ClearField(self, field_name: typing_extensions.Literal["original_variable_node_id", b"original_variable_node_id", "slot_name", b"slot_name", "slot_variable_node_id", b"slot_variable_node_id"]) -> None: ...
+            def ClearField(self, field_name: typing.Literal["original_variable_node_id", b"original_variable_node_id", "slot_name", b"slot_name", "slot_variable_node_id", b"slot_variable_node_id"]) -> None: ...
 
         CHILDREN_FIELD_NUMBER: builtins.int
         ATTRIBUTES_FIELD_NUMBER: builtins.int
         SLOT_VARIABLES_FIELD_NUMBER: builtins.int
         REGISTERED_SAVER_FIELD_NUMBER: builtins.int
         HAS_CHECKPOINT_VALUES_FIELD_NUMBER: builtins.int
         @property
         def children(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrackableObjectGraph.TrackableObject.ObjectReference]:
             """Objects which this object depends on."""
+
         @property
         def attributes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrackableObjectGraph.TrackableObject.SerializedTensor]:
             """Serialized data specific to this object."""
+
         @property
         def slot_variables(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrackableObjectGraph.TrackableObject.SlotVariableReference]:
             """Slot variables owned by this object."""
+
         @property
         def registered_saver(self) -> global___RegisteredSaver:
             """The registered saver used to save this object. If this saver is not
             present when loading the checkpoint, then loading will fail.
             """
+
         @property
         def has_checkpoint_values(self) -> google.protobuf.wrappers_pb2.BoolValue:
             """Whether this object has checkpoint values or descendants with checkpoint
             values. This is computed at save time to avoid traversing the entire
             object graph proto when restoring (which also has to traverse the live
             object graph).
             """
+
         def __init__(
             self,
             *,
             children: collections.abc.Iterable[global___TrackableObjectGraph.TrackableObject.ObjectReference] | None = ...,
             attributes: collections.abc.Iterable[global___TrackableObjectGraph.TrackableObject.SerializedTensor] | None = ...,
             slot_variables: collections.abc.Iterable[global___TrackableObjectGraph.TrackableObject.SlotVariableReference] | None = ...,
             registered_saver: global___RegisteredSaver | None = ...,
             has_checkpoint_values: google.protobuf.wrappers_pb2.BoolValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["has_checkpoint_values", b"has_checkpoint_values", "registered_saver", b"registered_saver"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["attributes", b"attributes", "children", b"children", "has_checkpoint_values", b"has_checkpoint_values", "registered_saver", b"registered_saver", "slot_variables", b"slot_variables"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["has_checkpoint_values", b"has_checkpoint_values", "registered_saver", b"registered_saver"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["attributes", b"attributes", "children", b"children", "has_checkpoint_values", b"has_checkpoint_values", "registered_saver", b"registered_saver", "slot_variables", b"slot_variables"]) -> None: ...
 
     NODES_FIELD_NUMBER: builtins.int
     @property
     def nodes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TrackableObjectGraph.TrackableObject]: ...
     def __init__(
         self,
         *,
         nodes: collections.abc.Iterable[global___TrackableObjectGraph.TrackableObject] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["nodes", b"nodes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["nodes", b"nodes"]) -> None: ...
 
 global___TrackableObjectGraph = TrackableObjectGraph
 
-@typing_extensions.final
+@typing.final
 class RegisteredSaver(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     OBJECT_NAME_FIELD_NUMBER: builtins.int
     name: builtins.str
     """The name of the registered saver/restore function."""
@@ -163,10 +169,10 @@
     """Unique auto-generated name of the object."""
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         object_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "object_name", b"object_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "object_name", b"object_name"]) -> None: ...
 
 global___RegisteredSaver = RegisteredSaver
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class RecvBufRespExtra(google.protobuf.message.Message):
     """Extra data needed on a non-RDMA RecvBufResponse."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_CONTENT_FIELD_NUMBER: builtins.int
     @property
     def tensor_content(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.bytes]: ...
     def __init__(
         self,
         *,
         tensor_content: collections.abc.Iterable[builtins.bytes] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tensor_content", b"tensor_content"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["tensor_content", b"tensor_content"]) -> None: ...
 
 global___RecvBufRespExtra = RecvBufRespExtra
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
@@ -13,15 +14,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class VerifierConfig(google.protobuf.message.Message):
     """The config for graph verifiers."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Toggle:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -48,10 +49,10 @@
     """Perform structural validation on a tensorflow graph. Default is OFF."""
     def __init__(
         self,
         *,
         verification_timeout_in_ms: builtins.int | None = ...,
         structure_verifier: global___VerifierConfig.Toggle.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["structure_verifier", b"structure_verifier", "verification_timeout_in_ms", b"verification_timeout_in_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["structure_verifier", b"structure_verifier", "verification_timeout_in_ms", b"verification_timeout_in_ms"]) -> None: ...
 
 global___VerifierConfig = VerifierConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -66,15 +67,15 @@
 
 DEFAULT: WorkerShutdownMode.ValueType  # 0
 NOT_CONFIGURED: WorkerShutdownMode.ValueType  # 1
 WAIT_FOR_COORDINATOR: WorkerShutdownMode.ValueType  # 2
 SHUTDOWN_AFTER_TIMEOUT: WorkerShutdownMode.ValueType  # 3
 global___WorkerShutdownMode = WorkerShutdownMode
 
-@typing_extensions.final
+@typing.final
 class Event(google.protobuf.message.Message):
     """Protocol buffer representing an event that happened during
     the execution of a Brain model.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -96,57 +97,62 @@
     """An event file was started, with the specified version.
     This is use to identify the contents of the record IO files
     easily.  Current version is "brain.Event:2".  All versions
     start with "brain.Event:".
     """
     graph_def: builtins.bytes
     """An encoded version of a GraphDef."""
+    meta_graph_def: builtins.bytes
+    """An encoded version of a MetaGraphDef."""
     @property
     def summary(self) -> tensorflow.core.framework.summary_pb2.Summary:
         """A summary was generated."""
+
     @property
     def log_message(self) -> global___LogMessage:
         """The user output a log message. This was theoretically used by the defunct
         tensorboard_logging module, which has since been removed; this field is
         now deprecated and should not be used.
         """
+
     @property
     def session_log(self) -> global___SessionLog:
         """The state of the session which can be used for restarting after crashes."""
+
     @property
     def tagged_run_metadata(self) -> global___TaggedRunMetadata:
         """The metadata returned by running a session.run() call."""
-    meta_graph_def: builtins.bytes
-    """An encoded version of a MetaGraphDef."""
+
     @property
     def source_metadata(self) -> global___SourceMetadata:
         """Information of the source that writes the events, this is only logged in
         the very first event along with the `file_version` field.
         """
+
     def __init__(
         self,
         *,
         wall_time: builtins.float | None = ...,
         step: builtins.int | None = ...,
         file_version: builtins.str | None = ...,
         graph_def: builtins.bytes | None = ...,
         summary: tensorflow.core.framework.summary_pb2.Summary | None = ...,
         log_message: global___LogMessage | None = ...,
         session_log: global___SessionLog | None = ...,
         tagged_run_metadata: global___TaggedRunMetadata | None = ...,
         meta_graph_def: builtins.bytes | None = ...,
         source_metadata: global___SourceMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["file_version", b"file_version", "graph_def", b"graph_def", "log_message", b"log_message", "meta_graph_def", b"meta_graph_def", "session_log", b"session_log", "source_metadata", b"source_metadata", "summary", b"summary", "tagged_run_metadata", b"tagged_run_metadata", "what", b"what"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_version", b"file_version", "graph_def", b"graph_def", "log_message", b"log_message", "meta_graph_def", b"meta_graph_def", "session_log", b"session_log", "source_metadata", b"source_metadata", "step", b"step", "summary", b"summary", "tagged_run_metadata", b"tagged_run_metadata", "wall_time", b"wall_time", "what", b"what"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["what", b"what"]) -> typing_extensions.Literal["file_version", "graph_def", "summary", "log_message", "session_log", "tagged_run_metadata", "meta_graph_def"] | None: ...
+    def HasField(self, field_name: typing.Literal["file_version", b"file_version", "graph_def", b"graph_def", "log_message", b"log_message", "meta_graph_def", b"meta_graph_def", "session_log", b"session_log", "source_metadata", b"source_metadata", "summary", b"summary", "tagged_run_metadata", b"tagged_run_metadata", "what", b"what"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["file_version", b"file_version", "graph_def", b"graph_def", "log_message", b"log_message", "meta_graph_def", b"meta_graph_def", "session_log", b"session_log", "source_metadata", b"source_metadata", "step", b"step", "summary", b"summary", "tagged_run_metadata", b"tagged_run_metadata", "wall_time", b"wall_time", "what", b"what"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["what", b"what"]) -> typing.Literal["file_version", "graph_def", "summary", "log_message", "session_log", "tagged_run_metadata", "meta_graph_def"] | None: ...
 
 global___Event = Event
 
-@typing_extensions.final
+@typing.final
 class SourceMetadata(google.protobuf.message.Message):
     """Holds the information of the source that writes the events."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WRITER_FIELD_NUMBER: builtins.int
     writer: builtins.str
@@ -154,19 +160,19 @@
     `tensorflow.core.util.events_writer`.
     """
     def __init__(
         self,
         *,
         writer: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["writer", b"writer"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["writer", b"writer"]) -> None: ...
 
 global___SourceMetadata = SourceMetadata
 
-@typing_extensions.final
+@typing.final
 class LogMessage(google.protobuf.message.Message):
     """Protocol buffer used for logging messages to the events file.
 
     This was theoretically used by the defunct tensorboard_logging module, which
     has been removed; this message is now deprecated and should not be used.
     """
 
@@ -209,19 +215,19 @@
     message: builtins.str
     def __init__(
         self,
         *,
         level: global___LogMessage.Level.ValueType | None = ...,
         message: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["level", b"level", "message", b"message"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["level", b"level", "message", b"message"]) -> None: ...
 
 global___LogMessage = LogMessage
 
-@typing_extensions.final
+@typing.final
 class SessionLog(google.protobuf.message.Message):
     """Protocol buffer used for logging session state."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _SessionStatus:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -250,19 +256,19 @@
     def __init__(
         self,
         *,
         status: global___SessionLog.SessionStatus.ValueType | None = ...,
         checkpoint_path: builtins.str | None = ...,
         msg: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["checkpoint_path", b"checkpoint_path", "msg", b"msg", "status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["checkpoint_path", b"checkpoint_path", "msg", b"msg", "status", b"status"]) -> None: ...
 
 global___SessionLog = SessionLog
 
-@typing_extensions.final
+@typing.final
 class TaggedRunMetadata(google.protobuf.message.Message):
     """For logging the metadata output for a single session.run() call."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TAG_FIELD_NUMBER: builtins.int
     RUN_METADATA_FIELD_NUMBER: builtins.int
@@ -274,49 +280,49 @@
     """
     def __init__(
         self,
         *,
         tag: builtins.str | None = ...,
         run_metadata: builtins.bytes | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["run_metadata", b"run_metadata", "tag", b"tag"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["run_metadata", b"run_metadata", "tag", b"tag"]) -> None: ...
 
 global___TaggedRunMetadata = TaggedRunMetadata
 
-@typing_extensions.final
+@typing.final
 class WatchdogConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TIMEOUT_MS_FIELD_NUMBER: builtins.int
     timeout_ms: builtins.int
     def __init__(
         self,
         *,
         timeout_ms: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["timeout_ms", b"timeout_ms"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["timeout_ms", b"timeout_ms"]) -> None: ...
 
 global___WatchdogConfig = WatchdogConfig
 
-@typing_extensions.final
+@typing.final
 class RequestedExitCode(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     EXIT_CODE_FIELD_NUMBER: builtins.int
     exit_code: builtins.int
     def __init__(
         self,
         *,
         exit_code: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exit_code", b"exit_code"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["exit_code", b"exit_code"]) -> None: ...
 
 global___RequestedExitCode = RequestedExitCode
 
-@typing_extensions.final
+@typing.final
 class WorkerHeartbeatRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SHUTDOWN_MODE_FIELD_NUMBER: builtins.int
     WATCHDOG_CONFIG_FIELD_NUMBER: builtins.int
     EXIT_CODE_FIELD_NUMBER: builtins.int
     shutdown_mode: global___WorkerShutdownMode.ValueType
@@ -327,33 +333,33 @@
     def __init__(
         self,
         *,
         shutdown_mode: global___WorkerShutdownMode.ValueType | None = ...,
         watchdog_config: global___WatchdogConfig | None = ...,
         exit_code: global___RequestedExitCode | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["exit_code", b"exit_code", "watchdog_config", b"watchdog_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exit_code", b"exit_code", "shutdown_mode", b"shutdown_mode", "watchdog_config", b"watchdog_config"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["exit_code", b"exit_code", "watchdog_config", b"watchdog_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["exit_code", b"exit_code", "shutdown_mode", b"shutdown_mode", "watchdog_config", b"watchdog_config"]) -> None: ...
 
 global___WorkerHeartbeatRequest = WorkerHeartbeatRequest
 
-@typing_extensions.final
+@typing.final
 class WorkerHeartbeatResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HEALTH_STATUS_FIELD_NUMBER: builtins.int
     WORKER_LOG_FIELD_NUMBER: builtins.int
     HOSTNAME_FIELD_NUMBER: builtins.int
     health_status: global___WorkerHealth.ValueType
+    hostname: builtins.str
     @property
     def worker_log(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Event]: ...
-    hostname: builtins.str
     def __init__(
         self,
         *,
         health_status: global___WorkerHealth.ValueType | None = ...,
         worker_log: collections.abc.Iterable[global___Event] | None = ...,
         hostname: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["health_status", b"health_status", "hostname", b"hostname", "worker_log", b"worker_log"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["health_status", b"health_status", "hostname", b"hostname", "worker_log", b"worker_log"]) -> None: ...
 
 global___WorkerHeartbeatResponse = WorkerHeartbeatResponse
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ==============================================================================
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class MemmappedFileSystemDirectoryElement(google.protobuf.message.Message):
     """A message that describes one region of memmapped file."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     OFFSET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
@@ -41,28 +42,28 @@
     def __init__(
         self,
         *,
         offset: builtins.int | None = ...,
         name: builtins.str | None = ...,
         length: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["length", b"length", "name", b"name", "offset", b"offset"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["length", b"length", "name", b"name", "offset", b"offset"]) -> None: ...
 
 global___MemmappedFileSystemDirectoryElement = MemmappedFileSystemDirectoryElement
 
-@typing_extensions.final
+@typing.final
 class MemmappedFileSystemDirectory(google.protobuf.message.Message):
     """A directory of regions in a memmapped file."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ELEMENT_FIELD_NUMBER: builtins.int
     @property
     def element(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MemmappedFileSystemDirectoryElement]: ...
     def __init__(
         self,
         *,
         element: collections.abc.Iterable[global___MemmappedFileSystemDirectoryElement] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["element", b"element"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["element", b"element"]) -> None: ...
 
 global___MemmappedFileSystemDirectory = MemmappedFileSystemDirectory
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -11,94 +11,99 @@
 
 Each of the rest of the records in a checkpoint stores the raw data of a
 particular tensor slice, in SavedSlice format. The corresponding key is an
 ordered code that encodes the name of the tensor and the slice
 information. The name is also stored in the SaveSlice message for ease of
 debugging and manual examination.
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.core.framework.tensor_pb2
 import tensorflow.core.framework.tensor_shape_pb2
 import tensorflow.core.framework.tensor_slice_pb2
 import tensorflow.core.framework.types_pb2
 import tensorflow.core.framework.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SavedSliceMeta(google.protobuf.message.Message):
     """Metadata describing the set of slices of the same tensor saved in a
     checkpoint file.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     SHAPE_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     SLICE_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Name of the tensor."""
+    type: tensorflow.core.framework.types_pb2.DataType.ValueType
+    """Type of the tensor"""
     @property
     def shape(self) -> tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto:
         """Shape of the tensor"""
-    type: tensorflow.core.framework.types_pb2.DataType.ValueType
-    """Type of the tensor"""
+
     @property
     def slice(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto]:
         """Explicit list of slices saved in the checkpoint file."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         shape: tensorflow.core.framework.tensor_shape_pb2.TensorShapeProto | None = ...,
         type: tensorflow.core.framework.types_pb2.DataType.ValueType | None = ...,
         slice: collections.abc.Iterable[tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["shape", b"shape"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "shape", b"shape", "slice", b"slice", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["shape", b"shape"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "shape", b"shape", "slice", b"slice", "type", b"type"]) -> None: ...
 
 global___SavedSliceMeta = SavedSliceMeta
 
-@typing_extensions.final
+@typing.final
 class SavedTensorSliceMeta(google.protobuf.message.Message):
     """Metadata describing the set of tensor slices saved in a checkpoint file.
     It is always stored at the beginning of each checkpoint file.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_FIELD_NUMBER: builtins.int
     VERSIONS_FIELD_NUMBER: builtins.int
     @property
     def tensor(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SavedSliceMeta]:
         """Each SavedSliceMeta describes the slices for one tensor."""
+
     @property
     def versions(self) -> tensorflow.core.framework.versions_pb2.VersionDef:
         """Compatibility version of this checkpoint.  See core/public/version.h
         for version history.
         """
+
     def __init__(
         self,
         *,
         tensor: collections.abc.Iterable[global___SavedSliceMeta] | None = ...,
         versions: tensorflow.core.framework.versions_pb2.VersionDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["versions", b"versions"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["tensor", b"tensor", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["versions", b"versions"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["tensor", b"tensor", "versions", b"versions"]) -> None: ...
 
 global___SavedTensorSliceMeta = SavedTensorSliceMeta
 
-@typing_extensions.final
+@typing.final
 class SavedSlice(google.protobuf.message.Message):
     """Saved tensor slice: it stores the name of the tensors, the slice, and the
     raw data.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -110,52 +115,56 @@
     the name used to encode the key for this record.
     """
     @property
     def slice(self) -> tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto:
         """Extent of the slice.  Must have one entry for each of the dimension of the
         tensor that this slice belongs to.
         """
+
     @property
     def data(self) -> tensorflow.core.framework.tensor_pb2.TensorProto:
         """The raw data of the slice is stored as a TensorProto. Only raw data are
         stored (we don't fill in fields such as dtype or tensor_shape).
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         slice: tensorflow.core.framework.tensor_slice_pb2.TensorSliceProto | None = ...,
         data: tensorflow.core.framework.tensor_pb2.TensorProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "slice", b"slice"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "name", b"name", "slice", b"slice"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "slice", b"slice"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data", "name", b"name", "slice", b"slice"]) -> None: ...
 
 global___SavedSlice = SavedSlice
 
-@typing_extensions.final
+@typing.final
 class SavedTensorSlices(google.protobuf.message.Message):
     """Each record in a v3 checkpoint file is a serialized SavedTensorSlices
     message.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     DATA_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___SavedTensorSliceMeta:
         """This is only present at the first item of each checkpoint file and serves
         as a table of contents, listing all the tensor slices saved in this file.
         """
+
     @property
     def data(self) -> global___SavedSlice:
         """This exists in all but the first item of each checkpoint file."""
+
     def __init__(
         self,
         *,
         meta: global___SavedTensorSliceMeta | None = ...,
         data: global___SavedSlice | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data", b"data", "meta", b"meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "meta", b"meta"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["data", b"data", "meta", b"meta"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data", b"data", "meta", b"meta"]) -> None: ...
 
 global___SavedTensorSlices = SavedTensorSlices
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol messages for describing the results of benchmarks and unit tests."""
+
 import google.protobuf.descriptor
 from tensorflow.tsl.protobuf.test_log_pb2 import (
     AvailableDeviceInfo as AvailableDeviceInfo,
     BenchmarkEntries as BenchmarkEntries,
     BenchmarkEntry as BenchmarkEntry,
     BuildConfiguration as BuildConfiguration,
     CommitId as CommitId,
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/experimental/dtensor.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/experimental/dtensor.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/activations.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/activations.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/callbacks.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/callbacks.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/losses.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/losses.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/metrics.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/metrics.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/models.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/models.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/linalg.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/linalg.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/math.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/nn.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/nn.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,101 +1,104 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 This file is a copy of the TensorBoard ProjectorConfig proto.
 Keep this file in sync with the source proto definition at
 https://github.com/tensorflow/tensorboard/blob/master/tensorboard/plugins/projector/projector_config.proto
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SpriteMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     IMAGE_PATH_FIELD_NUMBER: builtins.int
     SINGLE_IMAGE_DIM_FIELD_NUMBER: builtins.int
     image_path: builtins.str
     @property
     def single_image_dim(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """[width, height] of a single image in the sprite."""
+
     def __init__(
         self,
         *,
         image_path: builtins.str | None = ...,
         single_image_dim: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["image_path", b"image_path", "single_image_dim", b"single_image_dim"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["image_path", b"image_path", "single_image_dim", b"single_image_dim"]) -> None: ...
 
 global___SpriteMetadata = SpriteMetadata
 
-@typing_extensions.final
+@typing.final
 class EmbeddingInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TENSOR_NAME_FIELD_NUMBER: builtins.int
     METADATA_PATH_FIELD_NUMBER: builtins.int
     BOOKMARKS_PATH_FIELD_NUMBER: builtins.int
     TENSOR_SHAPE_FIELD_NUMBER: builtins.int
     SPRITE_FIELD_NUMBER: builtins.int
     TENSOR_PATH_FIELD_NUMBER: builtins.int
     tensor_name: builtins.str
     metadata_path: builtins.str
     bookmarks_path: builtins.str
+    tensor_path: builtins.str
+    """Path to the TSV file holding the tensor values. If missing, the tensor
+    is assumed to be stored in the model checkpoint.
+    """
     @property
     def tensor_shape(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Shape of the 2D tensor [N x D]. If missing, it will be inferred from the
         model checkpoint.
         """
+
     @property
     def sprite(self) -> global___SpriteMetadata: ...
-    tensor_path: builtins.str
-    """Path to the TSV file holding the tensor values. If missing, the tensor
-    is assumed to be stored in the model checkpoint.
-    """
     def __init__(
         self,
         *,
         tensor_name: builtins.str | None = ...,
         metadata_path: builtins.str | None = ...,
         bookmarks_path: builtins.str | None = ...,
         tensor_shape: collections.abc.Iterable[builtins.int] | None = ...,
         sprite: global___SpriteMetadata | None = ...,
         tensor_path: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["sprite", b"sprite"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bookmarks_path", b"bookmarks_path", "metadata_path", b"metadata_path", "sprite", b"sprite", "tensor_name", b"tensor_name", "tensor_path", b"tensor_path", "tensor_shape", b"tensor_shape"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["sprite", b"sprite"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bookmarks_path", b"bookmarks_path", "metadata_path", b"metadata_path", "sprite", b"sprite", "tensor_name", b"tensor_name", "tensor_path", b"tensor_path", "tensor_shape", b"tensor_shape"]) -> None: ...
 
 global___EmbeddingInfo = EmbeddingInfo
 
-@typing_extensions.final
+@typing.final
 class ProjectorConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODEL_CHECKPOINT_PATH_FIELD_NUMBER: builtins.int
     EMBEDDINGS_FIELD_NUMBER: builtins.int
     MODEL_CHECKPOINT_DIR_FIELD_NUMBER: builtins.int
     model_checkpoint_path: builtins.str
     """Path to the checkpoint file. Use either this or model_checkpoint_dir."""
-    @property
-    def embeddings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EmbeddingInfo]: ...
     model_checkpoint_dir: builtins.str
     """Path to the checkpoint directory. The directory will be scanned for the
     latest checkpoint file.
     """
+    @property
+    def embeddings(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EmbeddingInfo]: ...
     def __init__(
         self,
         *,
         model_checkpoint_path: builtins.str | None = ...,
         embeddings: collections.abc.Iterable[global___EmbeddingInfo] | None = ...,
         model_checkpoint_dir: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["embeddings", b"embeddings", "model_checkpoint_dir", b"model_checkpoint_dir", "model_checkpoint_path", b"model_checkpoint_path"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["embeddings", b"embeddings", "model_checkpoint_dir", b"model_checkpoint_dir", "model_checkpoint_path", b"model_checkpoint_path"]) -> None: ...
 
 global___ProjectorConfig = ProjectorConfig
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protobuf containing the metadata for each Keras object saved in a SavedModel."""
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import tensorflow.python.keras.protobuf.versions_pb2
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SavedMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODES_FIELD_NUMBER: builtins.int
     @property
     def nodes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SavedObject]:
         """Nodes represent trackable objects in the SavedModel. The data for every
         Keras object is stored.
         """
+
     def __init__(
         self,
         *,
         nodes: collections.abc.Iterable[global___SavedObject] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["nodes", b"nodes"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["nodes", b"nodes"]) -> None: ...
 
 global___SavedMetadata = SavedMetadata
 
-@typing_extensions.final
+@typing.final
 class SavedObject(google.protobuf.message.Message):
     """Metadata of an individual Keras object."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NODE_ID_FIELD_NUMBER: builtins.int
     NODE_PATH_FIELD_NUMBER: builtins.int
@@ -57,20 +59,21 @@
     metadata: builtins.str
     """Metadata containing a JSON-serialized object with the non-TensorFlow
     attributes for this Keras object.
     """
     @property
     def version(self) -> tensorflow.python.keras.protobuf.versions_pb2.VersionDef:
         """Version defined by the code serializing this Keras object."""
+
     def __init__(
         self,
         *,
         node_id: builtins.int | None = ...,
         node_path: builtins.str | None = ...,
         identifier: builtins.str | None = ...,
         metadata: builtins.str | None = ...,
         version: tensorflow.python.keras.protobuf.versions_pb2.VersionDef | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["version", b"version"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["identifier", b"identifier", "metadata", b"metadata", "node_id", b"node_id", "node_path", b"node_path", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["version", b"version"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["identifier", b"identifier", "metadata", b"metadata", "node_id", b"node_id", "node_path", b"node_path", "version", b"version"]) -> None: ...
 
 global___SavedObject = SavedObject
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class VersionDef(google.protobuf.message.Message):
     """This file is a copy of the TensorFlow Versions proto.
     Keep this file in sync with the source proto definition at
     https://github.com/tensorflow/tensorflow/blob/master/tensorflow/core/framework/versions.proto
 
     Version information for a piece of serialized data
 
@@ -42,17 +43,18 @@
     producer: builtins.int
     """The version of the code that produced this data."""
     min_consumer: builtins.int
     """Any consumer below this version is not allowed to consume this data."""
     @property
     def bad_consumers(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Specific consumer versions which are disallowed (e.g. due to bugs)."""
+
     def __init__(
         self,
         *,
         producer: builtins.int | None = ...,
         min_consumer: builtins.int | None = ...,
         bad_consumers: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bad_consumers", b"bad_consumers", "min_consumer", b"min_consumer", "producer", b"producer"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bad_consumers", b"bad_consumers", "min_consumer", b"min_consumer", "producer", b"producer"]) -> None: ...
 
 global___VersionDef = VersionDef
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/random.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/raw_ops.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/raw_ops.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/saved_model/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/saved_model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/saved_model/experimental.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/saved_model/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/strings.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/summary.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/summary.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/train/__init__.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/train/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 isort:skip_file
 This file defines protos that store the results of autotuning various
 operations.
 
 They are in proto format because we want to log them structured. They offer
 tremendous statistical, testing, and debugging value.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
@@ -23,15 +24,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class CudnnVersion(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAJOR_FIELD_NUMBER: builtins.int
     MINOR_FIELD_NUMBER: builtins.int
     PATCH_FIELD_NUMBER: builtins.int
     major: builtins.int
@@ -40,37 +41,37 @@
     def __init__(
         self,
         *,
         major: builtins.int | None = ...,
         minor: builtins.int | None = ...,
         patch: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["major", b"major", "minor", b"minor", "patch", b"patch"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["major", b"major", "minor", b"minor", "patch", b"patch"]) -> None: ...
 
 global___CudnnVersion = CudnnVersion
 
-@typing_extensions.final
+@typing.final
 class ComputeCapability(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAJOR_FIELD_NUMBER: builtins.int
     MINOR_FIELD_NUMBER: builtins.int
     major: builtins.int
     minor: builtins.int
     def __init__(
         self,
         *,
         major: builtins.int | None = ...,
         minor: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["major", b"major", "minor", b"minor"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["major", b"major", "minor", b"minor"]) -> None: ...
 
 global___ComputeCapability = ComputeCapability
 
-@typing_extensions.final
+@typing.final
 class AutotuneResult(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _FailureKind:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -89,52 +90,52 @@
     REDZONE_MODIFIED: AutotuneResult.FailureKind.ValueType  # 1
     """Algorithm wrote memory outside its output buffers."""
     WRONG_RESULT: AutotuneResult.FailureKind.ValueType  # 2
     """Algorithm gave a different result from a reference algorithm."""
     DISQUALIFIED: AutotuneResult.FailureKind.ValueType  # 3
     """Algorithm was rejected for failing to run or for known bugs."""
 
-    @typing_extensions.final
+    @typing.final
     class FailureResult(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KIND_FIELD_NUMBER: builtins.int
         MSG_FIELD_NUMBER: builtins.int
         REFERENCE_CONV_FIELD_NUMBER: builtins.int
         REFERENCE_GEMM_FIELD_NUMBER: builtins.int
         REFERENCE_CUDA_CONV_PLAN_FIELD_NUMBER: builtins.int
         REFERENCE_ALGORITHM_FIELD_NUMBER: builtins.int
         BUFFER_ADDRESS_FIELD_NUMBER: builtins.int
         kind: global___AutotuneResult.FailureKind.ValueType
         msg: builtins.str
+        buffer_address: builtins.int
         @property
         def reference_conv(self) -> global___AutotuneResult.ConvKey: ...
         @property
         def reference_gemm(self) -> global___AutotuneResult.GemmKey: ...
         @property
         def reference_cuda_conv_plan(self) -> global___AutotuneResult.CudaConvPlanKey: ...
         @property
         def reference_algorithm(self) -> tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto: ...
-        buffer_address: builtins.int
         def __init__(
             self,
             *,
             kind: global___AutotuneResult.FailureKind.ValueType | None = ...,
             msg: builtins.str | None = ...,
             reference_conv: global___AutotuneResult.ConvKey | None = ...,
             reference_gemm: global___AutotuneResult.GemmKey | None = ...,
             reference_cuda_conv_plan: global___AutotuneResult.CudaConvPlanKey | None = ...,
             reference_algorithm: tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto | None = ...,
             buffer_address: builtins.int | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["key", b"key", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["buffer_address", b"buffer_address", "key", b"key", "kind", b"kind", "msg", b"msg", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["key", b"key"]) -> typing_extensions.Literal["reference_conv", "reference_gemm", "reference_cuda_conv_plan", "reference_algorithm"] | None: ...
+        def HasField(self, field_name: typing.Literal["key", b"key", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["buffer_address", b"buffer_address", "key", b"key", "kind", b"kind", "msg", b"msg", "reference_algorithm", b"reference_algorithm", "reference_conv", b"reference_conv", "reference_cuda_conv_plan", b"reference_cuda_conv_plan", "reference_gemm", b"reference_gemm"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing.Literal["key", b"key"]) -> typing.Literal["reference_conv", "reference_gemm", "reference_cuda_conv_plan", "reference_algorithm"] | None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ConvKey(google.protobuf.message.Message):
         """Legacy and unused in new data; superseded by AlgorithmProto."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ALGORITHM_FIELD_NUMBER: builtins.int
         TENSOR_OPS_ENABLED_FIELD_NUMBER: builtins.int
@@ -142,43 +143,43 @@
         tensor_ops_enabled: builtins.bool
         def __init__(
             self,
             *,
             algorithm: builtins.int | None = ...,
             tensor_ops_enabled: builtins.bool | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "tensor_ops_enabled", b"tensor_ops_enabled"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "tensor_ops_enabled", b"tensor_ops_enabled"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class GemmKey(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         ALGORITHM_FIELD_NUMBER: builtins.int
         algorithm: builtins.int
         def __init__(
             self,
             *,
             algorithm: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class CudaConvPlanKey(google.protobuf.message.Message):
         """Legacy and unused in new data; superseded by AlgorithmProto."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         EXEC_PLAN_ID_FIELD_NUMBER: builtins.int
         exec_plan_id: builtins.str
         def __init__(
             self,
             *,
             exec_plan_id: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["exec_plan_id", b"exec_plan_id"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["exec_plan_id", b"exec_plan_id"]) -> None: ...
 
     SCRATCH_BYTES_FIELD_NUMBER: builtins.int
     RUN_TIME_FIELD_NUMBER: builtins.int
     FAILURE_FIELD_NUMBER: builtins.int
     CONV_FIELD_NUMBER: builtins.int
     GEMM_FIELD_NUMBER: builtins.int
     CUDA_CONV_PLAN_FIELD_NUMBER: builtins.int
@@ -203,49 +204,50 @@
         run_time: google.protobuf.duration_pb2.Duration | None = ...,
         failure: global___AutotuneResult.FailureResult | None = ...,
         conv: global___AutotuneResult.ConvKey | None = ...,
         gemm: global___AutotuneResult.GemmKey | None = ...,
         cuda_conv_plan: global___AutotuneResult.CudaConvPlanKey | None = ...,
         algorithm: tensorflow.tsl.protobuf.dnn_pb2.AlgorithmProto | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time", "scratch_bytes", b"scratch_bytes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["key", b"key"]) -> typing_extensions.Literal["conv", "gemm", "cuda_conv_plan", "algorithm"] | None: ...
+    def HasField(self, field_name: typing.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "conv", b"conv", "cuda_conv_plan", b"cuda_conv_plan", "failure", b"failure", "gemm", b"gemm", "key", b"key", "run_time", b"run_time", "scratch_bytes", b"scratch_bytes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["key", b"key"]) -> typing.Literal["conv", "gemm", "cuda_conv_plan", "algorithm"] | None: ...
 
 global___AutotuneResult = AutotuneResult
 
-@typing_extensions.final
+@typing.final
 class AutotuningLog(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INSTR_FIELD_NUMBER: builtins.int
     RESULTS_FIELD_NUMBER: builtins.int
     CUDNN_VERSION_FIELD_NUMBER: builtins.int
     COMPUTE_CAPABILITY_FIELD_NUMBER: builtins.int
     DEVICE_PCI_BUS_ID_FIELD_NUMBER: builtins.int
     BLAS_VERSION_FIELD_NUMBER: builtins.int
+    device_pci_bus_id: builtins.str
+    """stream_executor::DeviceDescription::pci_bus_id."""
+    blas_version: builtins.str
     @property
     def instr(self) -> google.protobuf.any_pb2.Any: ...
     @property
     def results(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AutotuneResult]:
         """Records all auto-tuning results per algorithm."""
+
     @property
     def cudnn_version(self) -> global___CudnnVersion: ...
     @property
     def compute_capability(self) -> global___ComputeCapability: ...
-    device_pci_bus_id: builtins.str
-    """stream_executor::DeviceDescription::pci_bus_id."""
-    blas_version: builtins.str
     def __init__(
         self,
         *,
         instr: google.protobuf.any_pb2.Any | None = ...,
         results: collections.abc.Iterable[global___AutotuneResult] | None = ...,
         cudnn_version: global___CudnnVersion | None = ...,
         compute_capability: global___ComputeCapability | None = ...,
         device_pci_bus_id: builtins.str | None = ...,
         blas_version: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "instr", b"instr"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["blas_version", b"blas_version", "compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "device_pci_bus_id", b"device_pci_bus_id", "instr", b"instr", "results", b"results"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "instr", b"instr"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["blas_version", b"blas_version", "compute_capability", b"compute_capability", "cudnn_version", b"cudnn_version", "device_pci_bus_id", b"device_pci_bus_id", "instr", b"instr", "results", b"results"]) -> None: ...
 
 global___AutotuningLog = AutotuningLog
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class MemAllocatorStats(google.protobuf.message.Message):
     """Some of the data from AllocatorStats"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NUM_ALLOCS_FIELD_NUMBER: builtins.int
     BYTES_IN_USE_FIELD_NUMBER: builtins.int
@@ -33,19 +34,19 @@
         *,
         num_allocs: builtins.int | None = ...,
         bytes_in_use: builtins.int | None = ...,
         peak_bytes_in_use: builtins.int | None = ...,
         largest_alloc_size: builtins.int | None = ...,
         fragmentation_metric: builtins.float | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bytes_in_use", b"bytes_in_use", "fragmentation_metric", b"fragmentation_metric", "largest_alloc_size", b"largest_alloc_size", "num_allocs", b"num_allocs", "peak_bytes_in_use", b"peak_bytes_in_use"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bytes_in_use", b"bytes_in_use", "fragmentation_metric", b"fragmentation_metric", "largest_alloc_size", b"largest_alloc_size", "num_allocs", b"num_allocs", "peak_bytes_in_use", b"peak_bytes_in_use"]) -> None: ...
 
 global___MemAllocatorStats = MemAllocatorStats
 
-@typing_extensions.final
+@typing.final
 class MemChunk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ADDRESS_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     REQUESTED_SIZE_FIELD_NUMBER: builtins.int
     BIN_FIELD_NUMBER: builtins.int
@@ -72,19 +73,19 @@
         bin: builtins.int | None = ...,
         op_name: builtins.str | None = ...,
         freed_at_count: builtins.int | None = ...,
         action_count: builtins.int | None = ...,
         in_use: builtins.bool | None = ...,
         step_id: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_count", b"action_count", "address", b"address", "bin", b"bin", "freed_at_count", b"freed_at_count", "in_use", b"in_use", "op_name", b"op_name", "requested_size", b"requested_size", "size", b"size", "step_id", b"step_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["action_count", b"action_count", "address", b"address", "bin", b"bin", "freed_at_count", b"freed_at_count", "in_use", b"in_use", "op_name", b"op_name", "requested_size", b"requested_size", "size", b"size", "step_id", b"step_id"]) -> None: ...
 
 global___MemChunk = MemChunk
 
-@typing_extensions.final
+@typing.final
 class BinSummary(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BIN_FIELD_NUMBER: builtins.int
     TOTAL_BYTES_IN_USE_FIELD_NUMBER: builtins.int
     TOTAL_BYTES_IN_BIN_FIELD_NUMBER: builtins.int
     TOTAL_CHUNKS_IN_USE_FIELD_NUMBER: builtins.int
@@ -99,37 +100,37 @@
         *,
         bin: builtins.int | None = ...,
         total_bytes_in_use: builtins.int | None = ...,
         total_bytes_in_bin: builtins.int | None = ...,
         total_chunks_in_use: builtins.int | None = ...,
         total_chunks_in_bin: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bin", b"bin", "total_bytes_in_bin", b"total_bytes_in_bin", "total_bytes_in_use", b"total_bytes_in_use", "total_chunks_in_bin", b"total_chunks_in_bin", "total_chunks_in_use", b"total_chunks_in_use"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bin", b"bin", "total_bytes_in_bin", b"total_bytes_in_bin", "total_bytes_in_use", b"total_bytes_in_use", "total_chunks_in_bin", b"total_chunks_in_bin", "total_chunks_in_use", b"total_chunks_in_use"]) -> None: ...
 
 global___BinSummary = BinSummary
 
-@typing_extensions.final
+@typing.final
 class SnapShot(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ACTION_COUNT_FIELD_NUMBER: builtins.int
     SIZE_FIELD_NUMBER: builtins.int
     action_count: builtins.int
     size: builtins.int
     def __init__(
         self,
         *,
         action_count: builtins.int | None = ...,
         size: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_count", b"action_count", "size", b"size"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["action_count", b"action_count", "size", b"size"]) -> None: ...
 
 global___SnapShot = SnapShot
 
-@typing_extensions.final
+@typing.final
 class MemoryDump(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOCATOR_NAME_FIELD_NUMBER: builtins.int
     BIN_SUMMARY_FIELD_NUMBER: builtins.int
     CHUNK_FIELD_NUMBER: builtins.int
     SNAP_SHOT_FIELD_NUMBER: builtins.int
@@ -148,11 +149,11 @@
         *,
         allocator_name: builtins.str | None = ...,
         bin_summary: collections.abc.Iterable[global___BinSummary] | None = ...,
         chunk: collections.abc.Iterable[global___MemChunk] | None = ...,
         snap_shot: collections.abc.Iterable[global___SnapShot] | None = ...,
         stats: global___MemAllocatorStats | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["stats", b"stats"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allocator_name", b"allocator_name", "bin_summary", b"bin_summary", "chunk", b"chunk", "snap_shot", b"snap_shot", "stats", b"stats"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["stats", b"stats"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allocator_name", b"allocator_name", "bin_summary", b"bin_summary", "chunk", b"chunk", "snap_shot", b"snap_shot", "stats", b"stats"]) -> None: ...
 
 global___MemoryDump = MemoryDump
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
@@ -48,15 +49,15 @@
 initialized/uninitialized.
 """
 TASKSTATE_DISCONNECTED: CoordinatedTaskState.ValueType  # 2
 TASKSTATE_CONNECTED: CoordinatedTaskState.ValueType  # 3
 TASKSTATE_ERROR: CoordinatedTaskState.ValueType  # 4
 global___CoordinatedTaskState = CoordinatedTaskState
 
-@typing_extensions.final
+@typing.final
 class CoordinatedTask(google.protobuf.message.Message):
     """Represents a remote worker task, specified by job name and task id."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_NAME_FIELD_NUMBER: builtins.int
     TASK_ID_FIELD_NUMBER: builtins.int
@@ -64,19 +65,19 @@
     task_id: builtins.int
     def __init__(
         self,
         *,
         job_name: builtins.str | None = ...,
         task_id: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["job_name", b"job_name", "task_id", b"task_id"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["job_name", b"job_name", "task_id", b"task_id"]) -> None: ...
 
 global___CoordinatedTask = CoordinatedTask
 
-@typing_extensions.final
+@typing.final
 class CoordinationServiceError(google.protobuf.message.Message):
     """Status payload for all coordination service errors.
     Note: an empty proto may be set if the error is triggered by the task's own
     agent calls (i.e. not propagated by the service from another remote task).
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -88,74 +89,75 @@
     internal service error).
     """
     @property
     def source_task(self) -> global___CoordinatedTask:
         """Denotes which task hit the error. If unset, the error originated from the
         same task that is processing this error.
         """
+
     def __init__(
         self,
         *,
         is_reported_error: builtins.bool | None = ...,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_reported_error", b"is_reported_error", "source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["is_reported_error", b"is_reported_error", "source_task", b"source_task"]) -> None: ...
 
 global___CoordinationServiceError = CoordinationServiceError
 
-@typing_extensions.final
+@typing.final
 class CoordinatedTaskStateInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TASK_FIELD_NUMBER: builtins.int
     STATE_FIELD_NUMBER: builtins.int
     ERROR_CODE_FIELD_NUMBER: builtins.int
     ERROR_MESSAGE_FIELD_NUMBER: builtins.int
     ERROR_PAYLOAD_FIELD_NUMBER: builtins.int
-    @property
-    def task(self) -> global___CoordinatedTask: ...
     state: global___CoordinatedTaskState.ValueType
     error_code: builtins.int
     error_message: builtins.str
     @property
+    def task(self) -> global___CoordinatedTask: ...
+    @property
     def error_payload(self) -> global___CoordinationServiceError: ...
     def __init__(
         self,
         *,
         task: global___CoordinatedTask | None = ...,
         state: global___CoordinatedTaskState.ValueType | None = ...,
         error_code: builtins.int | None = ...,
         error_message: builtins.str | None = ...,
         error_payload: global___CoordinationServiceError | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["error_payload", b"error_payload", "task", b"task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "error_message", b"error_message", "error_payload", b"error_payload", "state", b"state", "task", b"task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["error_payload", b"error_payload", "task", b"task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "error_message", b"error_message", "error_payload", b"error_payload", "state", b"state", "task", b"task"]) -> None: ...
 
 global___CoordinatedTaskStateInfo = CoordinatedTaskStateInfo
 
-@typing_extensions.final
+@typing.final
 class DeviceInfo(google.protobuf.message.Message):
     """Placeholder message to be extended by other runtimes' device representations."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEVICE_FIELD_NUMBER: builtins.int
     @property
     def device(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]: ...
     def __init__(
         self,
         *,
         device: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device", b"device"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["device", b"device"]) -> None: ...
 
 global___DeviceInfo = DeviceInfo
 
-@typing_extensions.final
+@typing.final
 class RegisterTaskRequest(google.protobuf.message.Message):
     """Request and response messages for registering a task to the cluster leader.
     A task is uniquely represented by its `job_name`, `task_id` and
     `incarnation`. Leader responds with its `incarnation` to identify a leader
     process.
     """
 
@@ -168,35 +170,35 @@
     def source_task(self) -> global___CoordinatedTask: ...
     def __init__(
         self,
         *,
         incarnation: builtins.int | None = ...,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["incarnation", b"incarnation", "source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["incarnation", b"incarnation", "source_task", b"source_task"]) -> None: ...
 
 global___RegisterTaskRequest = RegisterTaskRequest
 
-@typing_extensions.final
+@typing.final
 class RegisterTaskResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LEADER_INCARNATION_FIELD_NUMBER: builtins.int
     leader_incarnation: builtins.int
     def __init__(
         self,
         *,
         leader_incarnation: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["leader_incarnation", b"leader_incarnation"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["leader_incarnation", b"leader_incarnation"]) -> None: ...
 
 global___RegisterTaskResponse = RegisterTaskResponse
 
-@typing_extensions.final
+@typing.final
 class HeartbeatRequest(google.protobuf.message.Message):
     """Request and response messages for sending heartbeats."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     INCARNATION_FIELD_NUMBER: builtins.int
     SOURCE_TASK_FIELD_NUMBER: builtins.int
@@ -205,141 +207,143 @@
     def source_task(self) -> global___CoordinatedTask: ...
     def __init__(
         self,
         *,
         incarnation: builtins.int | None = ...,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["incarnation", b"incarnation", "source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["incarnation", b"incarnation", "source_task", b"source_task"]) -> None: ...
 
 global___HeartbeatRequest = HeartbeatRequest
 
-@typing_extensions.final
+@typing.final
 class HeartbeatResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LEADER_INCARNATION_FIELD_NUMBER: builtins.int
     leader_incarnation: builtins.int
     """If there are failures in cluster, use additional metadata in response to
     broadcast error code and message to other tasks.
     """
     def __init__(
         self,
         *,
         leader_incarnation: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["leader_incarnation", b"leader_incarnation"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["leader_incarnation", b"leader_incarnation"]) -> None: ...
 
 global___HeartbeatResponse = HeartbeatResponse
 
-@typing_extensions.final
+@typing.final
 class WaitForAllTasksRequest(google.protobuf.message.Message):
     """Request and response messages for waiting for all tasks."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_TASK_FIELD_NUMBER: builtins.int
     DEVICE_INFO_FIELD_NUMBER: builtins.int
     @property
     def source_task(self) -> global___CoordinatedTask: ...
     @property
     def device_info(self) -> global___DeviceInfo:
         """All local device attributes on the request sender;"""
+
     def __init__(
         self,
         *,
         source_task: global___CoordinatedTask | None = ...,
         device_info: global___DeviceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["device_info", b"device_info", "source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_info", b"device_info", "source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["device_info", b"device_info", "source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["device_info", b"device_info", "source_task", b"source_task"]) -> None: ...
 
 global___WaitForAllTasksRequest = WaitForAllTasksRequest
 
-@typing_extensions.final
+@typing.final
 class WaitForAllTasksResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     LEADER_INCARNATION_FIELD_NUMBER: builtins.int
     DEVICE_INFO_FIELD_NUMBER: builtins.int
     leader_incarnation: builtins.int
     @property
     def device_info(self) -> global___DeviceInfo:
         """All devices in the cluster."""
+
     def __init__(
         self,
         *,
         leader_incarnation: builtins.int | None = ...,
         device_info: global___DeviceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["device_info", b"device_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["device_info", b"device_info", "leader_incarnation", b"leader_incarnation"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["device_info", b"device_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["device_info", b"device_info", "leader_incarnation", b"leader_incarnation"]) -> None: ...
 
 global___WaitForAllTasksResponse = WaitForAllTasksResponse
 
-@typing_extensions.final
+@typing.final
 class ShutdownTaskRequest(google.protobuf.message.Message):
     """Request and response messages for disconnecting a task from the service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_TASK_FIELD_NUMBER: builtins.int
     @property
     def source_task(self) -> global___CoordinatedTask: ...
     def __init__(
         self,
         *,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["source_task", b"source_task"]) -> None: ...
 
 global___ShutdownTaskRequest = ShutdownTaskRequest
 
-@typing_extensions.final
+@typing.final
 class ShutdownTaskResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ShutdownTaskResponse = ShutdownTaskResponse
 
-@typing_extensions.final
+@typing.final
 class ResetTaskRequest(google.protobuf.message.Message):
     """Request and response messages for resetting a task state in the service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_TASK_FIELD_NUMBER: builtins.int
     @property
     def source_task(self) -> global___CoordinatedTask: ...
     def __init__(
         self,
         *,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["source_task", b"source_task"]) -> None: ...
 
 global___ResetTaskRequest = ResetTaskRequest
 
-@typing_extensions.final
+@typing.final
 class ResetTaskResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ResetTaskResponse = ResetTaskResponse
 
-@typing_extensions.final
+@typing.final
 class ReportErrorToTaskRequest(google.protobuf.message.Message):
     """Request and response messages for reporting errors to task."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_CODE_FIELD_NUMBER: builtins.int
     ERROR_MESSAGE_FIELD_NUMBER: builtins.int
@@ -351,30 +355,30 @@
     def __init__(
         self,
         *,
         error_code: builtins.int | None = ...,
         error_message: builtins.str | None = ...,
         error_payload: global___CoordinationServiceError | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["error_payload", b"error_payload"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "error_message", b"error_message", "error_payload", b"error_payload"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["error_payload", b"error_payload"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "error_message", b"error_message", "error_payload", b"error_payload"]) -> None: ...
 
 global___ReportErrorToTaskRequest = ReportErrorToTaskRequest
 
-@typing_extensions.final
+@typing.final
 class ReportErrorToTaskResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ReportErrorToTaskResponse = ReportErrorToTaskResponse
 
-@typing_extensions.final
+@typing.final
 class ReportErrorToServiceRequest(google.protobuf.message.Message):
     """Request and response messages for reporting errors to service instance."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ERROR_CODE_FIELD_NUMBER: builtins.int
     ERROR_MESSAGE_FIELD_NUMBER: builtins.int
@@ -386,64 +390,64 @@
     def __init__(
         self,
         *,
         error_code: builtins.int | None = ...,
         error_message: builtins.str | None = ...,
         error_origin: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["error_origin", b"error_origin"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error_code", b"error_code", "error_message", b"error_message", "error_origin", b"error_origin"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["error_origin", b"error_origin"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["error_code", b"error_code", "error_message", b"error_message", "error_origin", b"error_origin"]) -> None: ...
 
 global___ReportErrorToServiceRequest = ReportErrorToServiceRequest
 
-@typing_extensions.final
+@typing.final
 class ReportErrorToServiceResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___ReportErrorToServiceResponse = ReportErrorToServiceResponse
 
-@typing_extensions.final
+@typing.final
 class GetTaskStateRequest(google.protobuf.message.Message):
     """Request and response messages for getting state of a remote task."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SOURCE_TASK_FIELD_NUMBER: builtins.int
     @property
     def source_task(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedTask]: ...
     def __init__(
         self,
         *,
         source_task: collections.abc.Iterable[global___CoordinatedTask] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["source_task", b"source_task"]) -> None: ...
 
 global___GetTaskStateRequest = GetTaskStateRequest
 
-@typing_extensions.final
+@typing.final
 class GetTaskStateResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TASK_STATE_FIELD_NUMBER: builtins.int
     @property
     def task_state(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedTaskStateInfo]: ...
     def __init__(
         self,
         *,
         task_state: collections.abc.Iterable[global___CoordinatedTaskStateInfo] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["task_state", b"task_state"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["task_state", b"task_state"]) -> None: ...
 
 global___GetTaskStateResponse = GetTaskStateResponse
 
-@typing_extensions.final
+@typing.final
 class KeyValueEntry(google.protobuf.message.Message):
     """Message for configuration key value.
     Key is structured like Unix file system, with multiple levels of directory
     names separated by the slash ('/') characters.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -454,148 +458,148 @@
     value: builtins.bytes
     def __init__(
         self,
         *,
         key: builtins.str | None = ...,
         value: builtins.bytes | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
 global___KeyValueEntry = KeyValueEntry
 
-@typing_extensions.final
+@typing.final
 class InsertKeyValueRequest(google.protobuf.message.Message):
     """Request and response messages for inserting configuration key-value data."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KV_FIELD_NUMBER: builtins.int
     @property
     def kv(self) -> global___KeyValueEntry: ...
     def __init__(
         self,
         *,
         kv: global___KeyValueEntry | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["kv", b"kv"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["kv", b"kv"]) -> None: ...
 
 global___InsertKeyValueRequest = InsertKeyValueRequest
 
-@typing_extensions.final
+@typing.final
 class InsertKeyValueResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___InsertKeyValueResponse = InsertKeyValueResponse
 
-@typing_extensions.final
+@typing.final
 class GetKeyValueRequest(google.protobuf.message.Message):
     """Request and response messages for getting configuration key-value data."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     key: builtins.str
     def __init__(
         self,
         *,
         key: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key", b"key"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["key", b"key"]) -> None: ...
 
 global___GetKeyValueRequest = GetKeyValueRequest
 
-@typing_extensions.final
+@typing.final
 class GetKeyValueResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KV_FIELD_NUMBER: builtins.int
     @property
     def kv(self) -> global___KeyValueEntry: ...
     def __init__(
         self,
         *,
         kv: global___KeyValueEntry | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["kv", b"kv"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["kv", b"kv"]) -> None: ...
 
 global___GetKeyValueResponse = GetKeyValueResponse
 
-@typing_extensions.final
+@typing.final
 class TryGetKeyValueRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KEY_FIELD_NUMBER: builtins.int
     key: builtins.str
     def __init__(
         self,
         *,
         key: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key", b"key"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["key", b"key"]) -> None: ...
 
 global___TryGetKeyValueRequest = TryGetKeyValueRequest
 
-@typing_extensions.final
+@typing.final
 class TryGetKeyValueResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     KV_FIELD_NUMBER: builtins.int
     @property
     def kv(self) -> global___KeyValueEntry: ...
     def __init__(
         self,
         *,
         kv: global___KeyValueEntry | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kv", b"kv"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["kv", b"kv"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["kv", b"kv"]) -> None: ...
 
 global___TryGetKeyValueResponse = TryGetKeyValueResponse
 
-@typing_extensions.final
+@typing.final
 class GetKeyValueDirRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DIRECTORY_KEY_FIELD_NUMBER: builtins.int
     directory_key: builtins.str
     def __init__(
         self,
         *,
         directory_key: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["directory_key", b"directory_key"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["directory_key", b"directory_key"]) -> None: ...
 
 global___GetKeyValueDirRequest = GetKeyValueDirRequest
 
-@typing_extensions.final
+@typing.final
 class GetKeyValueDirResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DIRECTORY_KEY_FIELD_NUMBER: builtins.int
     KV_FIELD_NUMBER: builtins.int
     directory_key: builtins.str
     @property
     def kv(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___KeyValueEntry]: ...
     def __init__(
         self,
         *,
         directory_key: builtins.str | None = ...,
         kv: collections.abc.Iterable[global___KeyValueEntry] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["directory_key", b"directory_key", "kv", b"kv"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["directory_key", b"directory_key", "kv", b"kv"]) -> None: ...
 
 global___GetKeyValueDirResponse = GetKeyValueDirResponse
 
-@typing_extensions.final
+@typing.final
 class DeleteKeyValueRequest(google.protobuf.message.Message):
     """Request and response messages for deleting configuration key-value data.
     When is_directory is true, delete key-values recursively under `key`.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -605,29 +609,29 @@
     is_directory: builtins.bool
     def __init__(
         self,
         *,
         key: builtins.str | None = ...,
         is_directory: builtins.bool | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["is_directory", b"is_directory", "key", b"key"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["is_directory", b"is_directory", "key", b"key"]) -> None: ...
 
 global___DeleteKeyValueRequest = DeleteKeyValueRequest
 
-@typing_extensions.final
+@typing.final
 class DeleteKeyValueResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___DeleteKeyValueResponse = DeleteKeyValueResponse
 
-@typing_extensions.final
+@typing.final
 class BarrierRequest(google.protobuf.message.Message):
     """Request and response messages for generic sync barriers."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BARRIER_ID_FIELD_NUMBER: builtins.int
     BARRIER_TIMEOUT_IN_MS_FIELD_NUMBER: builtins.int
@@ -636,64 +640,67 @@
     barrier_id: builtins.str
     barrier_timeout_in_ms: builtins.int
     @property
     def tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CoordinatedTask]:
         """Denotes list of tasks that will wait for the barrier. If unspecified, it
         implies that the entire cluster is participating in the barrier.
         """
+
     @property
     def source_task(self) -> global___CoordinatedTask:
         """Task that is making the request."""
+
     def __init__(
         self,
         *,
         barrier_id: builtins.str | None = ...,
         barrier_timeout_in_ms: builtins.int | None = ...,
         tasks: collections.abc.Iterable[global___CoordinatedTask] | None = ...,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["barrier_id", b"barrier_id", "barrier_timeout_in_ms", b"barrier_timeout_in_ms", "source_task", b"source_task", "tasks", b"tasks"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["barrier_id", b"barrier_id", "barrier_timeout_in_ms", b"barrier_timeout_in_ms", "source_task", b"source_task", "tasks", b"tasks"]) -> None: ...
 
 global___BarrierRequest = BarrierRequest
 
-@typing_extensions.final
+@typing.final
 class BarrierResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
 global___BarrierResponse = BarrierResponse
 
-@typing_extensions.final
+@typing.final
 class CancelBarrierRequest(google.protobuf.message.Message):
     """Request and response messages for  cancelling generic sync barriers."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BARRIER_ID_FIELD_NUMBER: builtins.int
     SOURCE_TASK_FIELD_NUMBER: builtins.int
     barrier_id: builtins.str
     @property
     def source_task(self) -> global___CoordinatedTask:
         """Task that is making the request."""
+
     def __init__(
         self,
         *,
         barrier_id: builtins.str | None = ...,
         source_task: global___CoordinatedTask | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_task", b"source_task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["barrier_id", b"barrier_id", "source_task", b"source_task"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_task", b"source_task"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["barrier_id", b"barrier_id", "source_task", b"source_task"]) -> None: ...
 
 global___CancelBarrierRequest = CancelBarrierRequest
 
-@typing_extensions.final
+@typing.final
 class CancelBarrierResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 LINT: LEGACY_NAMES"""
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -246,44 +247,44 @@
 INVALID: ConvolutionKind.ValueType  # 0
 FORWARD: ConvolutionKind.ValueType  # 1
 BACKWARD_FILTER: ConvolutionKind.ValueType  # 2
 BACKWARD_DATA: ConvolutionKind.ValueType  # 3
 FORWARD_BIAS_ACTIVATION: ConvolutionKind.ValueType  # 4
 global___ConvolutionKind = ConvolutionKind
 
-@typing_extensions.final
+@typing.final
 class TensorDescriptorProto(google.protobuf.message.Message):
     """Generic tensor representation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DIMENSIONS_FIELD_NUMBER: builtins.int
     DATA_TYPE_FIELD_NUMBER: builtins.int
     DATA_LAYOUT_FIELD_NUMBER: builtins.int
     FILTER_LAYOUT_FIELD_NUMBER: builtins.int
-    @property
-    def dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     data_type: global___DataType.ValueType
     data_layout: global___DataLayout.ValueType
     filter_layout: global___FilterLayout.ValueType
+    @property
+    def dimensions(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         dimensions: collections.abc.Iterable[builtins.int] | None = ...,
         data_type: global___DataType.ValueType | None = ...,
         data_layout: global___DataLayout.ValueType | None = ...,
         filter_layout: global___FilterLayout.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["data_layout", b"data_layout", "filter_layout", b"filter_layout", "layout_oneof", b"layout_oneof"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data_layout", b"data_layout", "data_type", b"data_type", "dimensions", b"dimensions", "filter_layout", b"filter_layout", "layout_oneof", b"layout_oneof"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["layout_oneof", b"layout_oneof"]) -> typing_extensions.Literal["data_layout", "filter_layout"] | None: ...
+    def HasField(self, field_name: typing.Literal["data_layout", b"data_layout", "filter_layout", b"filter_layout", "layout_oneof", b"layout_oneof"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["data_layout", b"data_layout", "data_type", b"data_type", "dimensions", b"dimensions", "filter_layout", b"filter_layout", "layout_oneof", b"layout_oneof"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["layout_oneof", b"layout_oneof"]) -> typing.Literal["data_layout", "filter_layout"] | None: ...
 
 global___TensorDescriptorProto = TensorDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class AlgorithmProto(google.protobuf.message.Message):
     """Generic algorithm representation."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _MathType:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -300,142 +301,143 @@
     class MathType(_MathType, metaclass=_MathTypeEnumTypeWrapper): ...
     DEFAULT_MATH: AlgorithmProto.MathType.ValueType  # 0
     TENSOR_OP_MATH: AlgorithmProto.MathType.ValueType  # 1
     """The GPU may operate 4x4 matrix FMA.
     See cuDNN's documentation for CUDNN_TENSOR_OP_MATH.
     """
 
-    @typing_extensions.final
+    @typing.final
     class TuningKnobsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.int
         value: builtins.int
         def __init__(
             self,
             *,
             key: builtins.int | None = ...,
             value: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     ALGO_ID_FIELD_NUMBER: builtins.int
     MATH_TYPE_FIELD_NUMBER: builtins.int
     TUNING_KNOBS_FIELD_NUMBER: builtins.int
     IS_CUDNN_FRONTEND_FIELD_NUMBER: builtins.int
     WORKSPACE_SIZE_FIELD_NUMBER: builtins.int
     algo_id: builtins.int
     math_type: global___AlgorithmProto.MathType.ValueType
-    @property
-    def tuning_knobs(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.int]: ...
     is_cudnn_frontend: builtins.bool
     """Legacy algorithm enums and cuDNN Frontend engine numbers need to coexist in
     the same proto medium-term, until we can be confident of no longer needing
     the legacy cuDNN convolution API.  Once the migration is complete, we can
     stop producing legacy algorithm enums and remove this field.
     """
     @property
+    def tuning_knobs(self) -> google.protobuf.internal.containers.ScalarMap[builtins.int, builtins.int]: ...
+    @property
     def workspace_size(self) -> google.protobuf.wrappers_pb2.UInt64Value:
         """For ROCm only, it's impossible to re-query the required workspace size
         after running the algorithm search, so we must store the workspace size
         along with the choice of algorithm.  For consistency and convenience,
         cuDNN uses this field in the same way, even though it would be possible to
         re-query the workspace size from cuDNN at each use.
 
         Since this message is persisted in files, we need to be able to distinguish
         0 workspace size from unknown workspace size in an old message, so this is
         a message field.
         """
+
     def __init__(
         self,
         *,
         algo_id: builtins.int | None = ...,
         math_type: global___AlgorithmProto.MathType.ValueType | None = ...,
         tuning_knobs: collections.abc.Mapping[builtins.int, builtins.int] | None = ...,
         is_cudnn_frontend: builtins.bool | None = ...,
         workspace_size: google.protobuf.wrappers_pb2.UInt64Value | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["workspace_size", b"workspace_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["algo_id", b"algo_id", "is_cudnn_frontend", b"is_cudnn_frontend", "math_type", b"math_type", "tuning_knobs", b"tuning_knobs", "workspace_size", b"workspace_size"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["workspace_size", b"workspace_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["algo_id", b"algo_id", "is_cudnn_frontend", b"is_cudnn_frontend", "math_type", b"math_type", "tuning_knobs", b"tuning_knobs", "workspace_size", b"workspace_size"]) -> None: ...
 
 global___AlgorithmProto = AlgorithmProto
 
-@typing_extensions.final
+@typing.final
 class AlgorithmConfigProto(google.protobuf.message.Message):
     """Proto definition of AlgorithmConfig in "dnn.h".
     TODO(ruochengw): After cl/380702564 is submitted, add support for algorithm
     configs with cuDNN Frontend APIs.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALGORITHM_FIELD_NUMBER: builtins.int
     ALGORITHM_NO_SCRATCH_FIELD_NUMBER: builtins.int
     SCRATCH_SIZE_FIELD_NUMBER: builtins.int
+    scratch_size: builtins.int
     @property
     def algorithm(self) -> global___AlgorithmProto: ...
     @property
     def algorithm_no_scratch(self) -> global___AlgorithmProto: ...
-    scratch_size: builtins.int
     def __init__(
         self,
         *,
         algorithm: global___AlgorithmProto | None = ...,
         algorithm_no_scratch: global___AlgorithmProto | None = ...,
         scratch_size: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "algorithm_no_scratch", b"algorithm_no_scratch", "optional_algorithm", b"optional_algorithm", "optional_algorithm_no_scratch", b"optional_algorithm_no_scratch", "optional_scratch_size", b"optional_scratch_size", "scratch_size", b"scratch_size"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["algorithm", b"algorithm", "algorithm_no_scratch", b"algorithm_no_scratch", "optional_algorithm", b"optional_algorithm", "optional_algorithm_no_scratch", b"optional_algorithm_no_scratch", "optional_scratch_size", b"optional_scratch_size", "scratch_size", b"scratch_size"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["algorithm", b"algorithm", "algorithm_no_scratch", b"algorithm_no_scratch", "optional_algorithm", b"optional_algorithm", "optional_algorithm_no_scratch", b"optional_algorithm_no_scratch", "optional_scratch_size", b"optional_scratch_size", "scratch_size", b"scratch_size"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["algorithm", b"algorithm", "algorithm_no_scratch", b"algorithm_no_scratch", "optional_algorithm", b"optional_algorithm", "optional_algorithm_no_scratch", b"optional_algorithm_no_scratch", "optional_scratch_size", b"optional_scratch_size", "scratch_size", b"scratch_size"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_algorithm", b"optional_algorithm"]) -> typing_extensions.Literal["algorithm"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_algorithm", b"optional_algorithm"]) -> typing.Literal["algorithm"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_algorithm_no_scratch", b"optional_algorithm_no_scratch"]) -> typing_extensions.Literal["algorithm_no_scratch"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_algorithm_no_scratch", b"optional_algorithm_no_scratch"]) -> typing.Literal["algorithm_no_scratch"] | None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["optional_scratch_size", b"optional_scratch_size"]) -> typing_extensions.Literal["scratch_size"] | None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["optional_scratch_size", b"optional_scratch_size"]) -> typing.Literal["scratch_size"] | None: ...
 
 global___AlgorithmConfigProto = AlgorithmConfigProto
 
-@typing_extensions.final
+@typing.final
 class ConvolutionDescriptorProto(google.protobuf.message.Message):
     """Convolution-specific parameters."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PADDINGS_FIELD_NUMBER: builtins.int
     STRIDES_FIELD_NUMBER: builtins.int
     DILATIONS_FIELD_NUMBER: builtins.int
     COMPUTE_MODE_FIELD_NUMBER: builtins.int
     GROUP_COUNT_FIELD_NUMBER: builtins.int
     CONVOLUTION_MODE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    @property
-    def paddings(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def strides(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    @property
-    def dilations(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     compute_mode: global___DataType.ValueType
     """The "accumulator" type. For example, use F32 as an accumulator for F16
     convolutions.
     See cuDNN's cudnnConvolutionMode_t.
     """
     group_count: builtins.int
     """See cuDNN's group count."""
     convolution_mode: global___ConvolutionMode.ValueType
     name: builtins.str
     """Tensorflow node name, same as in NodeDef, for debugging purposes."""
+    @property
+    def paddings(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def strides(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
+    @property
+    def dilations(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
     def __init__(
         self,
         *,
         paddings: collections.abc.Iterable[builtins.int] | None = ...,
         strides: collections.abc.Iterable[builtins.int] | None = ...,
         dilations: collections.abc.Iterable[builtins.int] | None = ...,
         compute_mode: global___DataType.ValueType | None = ...,
         group_count: builtins.int | None = ...,
         convolution_mode: global___ConvolutionMode.ValueType | None = ...,
         name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compute_mode", b"compute_mode", "convolution_mode", b"convolution_mode", "dilations", b"dilations", "group_count", b"group_count", "name", b"name", "paddings", b"paddings", "strides", b"strides"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["compute_mode", b"compute_mode", "convolution_mode", b"convolution_mode", "dilations", b"dilations", "group_count", b"group_count", "name", b"name", "paddings", b"paddings", "strides", b"strides"]) -> None: ...
 
 global___ConvolutionDescriptorProto = ConvolutionDescriptorProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 TODO(b/247876220): Change package and java_package once we figure out how to
 migrate.
 """
+
 import builtins
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.enum_type_wrapper
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
 import collections.abc
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class HistogramProto(google.protobuf.message.Message):
     """Serialization format for histogram module in
     tsl/lib/histogram/histogram.h
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -36,23 +37,24 @@
     def bucket_limit(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]:
         """Parallel arrays encoding the bucket boundaries and the bucket values.
         bucket(i) is the count for the bucket i.  The range for
         a bucket is:
           i == 0:  -DBL_MAX .. bucket_limit(0)
           i != 0:  bucket_limit(i-1) .. bucket_limit(i)
         """
+
     @property
     def bucket(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.float]: ...
     def __init__(
         self,
         *,
         min: builtins.float | None = ...,
         max: builtins.float | None = ...,
         num: builtins.float | None = ...,
         sum: builtins.float | None = ...,
         sum_squares: builtins.float | None = ...,
         bucket_limit: collections.abc.Iterable[builtins.float] | None = ...,
         bucket: collections.abc.Iterable[builtins.float] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "bucket_limit", b"bucket_limit", "max", b"max", "min", b"min", "num", b"num", "sum", b"sum", "sum_squares", b"sum_squares"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bucket", b"bucket", "bucket_limit", b"bucket_limit", "max", b"max", "min", b"min", "num", b"num", "sum", b"sum", "sum_squares", b"sum_squares"]) -> None: ...
 
 global___HistogramProto = HistogramProto
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
+
 import builtins
-import typing as typing_extensions
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class RPCOptions(google.protobuf.message.Message):
     """RPC options for distributed runtime."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     USE_RPC_FOR_INPROCESS_MASTER_FIELD_NUMBER: builtins.int
     COMPRESSION_ALGORITHM_FIELD_NUMBER: builtins.int
@@ -59,10 +60,10 @@
         use_rpc_for_inprocess_master: builtins.bool | None = ...,
         compression_algorithm: builtins.str | None = ...,
         compression_level: builtins.int | None = ...,
         cache_rpc_response: builtins.bool | None = ...,
         disable_session_connection_sharing: builtins.bool | None = ...,
         num_channels_per_target: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cache_rpc_response", b"cache_rpc_response", "compression_algorithm", b"compression_algorithm", "compression_level", b"compression_level", "disable_session_connection_sharing", b"disable_session_connection_sharing", "num_channels_per_target", b"num_channels_per_target", "use_rpc_for_inprocess_master", b"use_rpc_for_inprocess_master"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cache_rpc_response", b"cache_rpc_response", "compression_algorithm", b"compression_algorithm", "compression_level", b"compression_level", "disable_session_connection_sharing", b"disable_session_connection_sharing", "num_channels_per_target", b"num_channels_per_target", "use_rpc_for_inprocess_master", b"use_rpc_for_inprocess_master"]) -> None: ...
 
 global___RPCOptions = RPCOptions
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Protocol messages for describing the results of benchmarks and unit tests."""
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
@@ -17,95 +18,97 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class EntryValue(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DOUBLE_VALUE_FIELD_NUMBER: builtins.int
     STRING_VALUE_FIELD_NUMBER: builtins.int
     double_value: builtins.float
     string_value: builtins.str
     def __init__(
         self,
         *,
         double_value: builtins.float | None = ...,
         string_value: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["double_value", b"double_value", "kind", b"kind", "string_value", b"string_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["double_value", b"double_value", "kind", b"kind", "string_value", b"string_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["double_value", "string_value"] | None: ...
+    def HasField(self, field_name: typing.Literal["double_value", b"double_value", "kind", b"kind", "string_value", b"string_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["double_value", b"double_value", "kind", b"kind", "string_value", b"string_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["double_value", "string_value"] | None: ...
 
 global___EntryValue = EntryValue
 
-@typing_extensions.final
+@typing.final
 class MetricEntry(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     MIN_VALUE_FIELD_NUMBER: builtins.int
     MAX_VALUE_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Metric name"""
     value: builtins.float
     """Metric value"""
     @property
     def min_value(self) -> google.protobuf.wrappers_pb2.DoubleValue:
         """The minimum acceptable value for the metric if specified"""
+
     @property
     def max_value(self) -> google.protobuf.wrappers_pb2.DoubleValue:
         """The maximum acceptable value for the metric if specified"""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         value: builtins.float | None = ...,
         min_value: google.protobuf.wrappers_pb2.DoubleValue | None = ...,
         max_value: google.protobuf.wrappers_pb2.DoubleValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["max_value", b"max_value", "min_value", b"min_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_value", b"max_value", "min_value", b"min_value", "name", b"name", "value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["max_value", b"max_value", "min_value", b"min_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["max_value", b"max_value", "min_value", b"min_value", "name", b"name", "value", b"value"]) -> None: ...
 
 global___MetricEntry = MetricEntry
 
-@typing_extensions.final
+@typing.final
 class BenchmarkEntry(google.protobuf.message.Message):
     """Each unit test or benchmark in a test or benchmark run provides
     some set of information.  Here we provide some reasonable keys
     one would expect to see, with optional key/value pairs for things
     we haven't considered.
 
     This BenchmarkEntry should be emitted by each unit test or benchmark
     reporter.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ExtrasEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___EntryValue: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___EntryValue | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     ITERS_FIELD_NUMBER: builtins.int
     CPU_TIME_FIELD_NUMBER: builtins.int
     WALL_TIME_FIELD_NUMBER: builtins.int
     THROUGHPUT_FIELD_NUMBER: builtins.int
     EXTRAS_FIELD_NUMBER: builtins.int
@@ -121,77 +124,81 @@
     wall_time: builtins.float
     """Total wall time used for all iterations (in seconds)"""
     throughput: builtins.float
     """Throughput (in MB/s)"""
     @property
     def extras(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___EntryValue]:
         """Generic map from result key to value."""
+
     @property
     def metrics(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MetricEntry]:
         """Metric name, value and expected range. This can include accuracy metrics
         typically used to determine whether the accuracy test has passed
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         iters: builtins.int | None = ...,
         cpu_time: builtins.float | None = ...,
         wall_time: builtins.float | None = ...,
         throughput: builtins.float | None = ...,
         extras: collections.abc.Mapping[builtins.str, global___EntryValue] | None = ...,
         metrics: collections.abc.Iterable[global___MetricEntry] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cpu_time", b"cpu_time", "extras", b"extras", "iters", b"iters", "metrics", b"metrics", "name", b"name", "throughput", b"throughput", "wall_time", b"wall_time"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cpu_time", b"cpu_time", "extras", b"extras", "iters", b"iters", "metrics", b"metrics", "name", b"name", "throughput", b"throughput", "wall_time", b"wall_time"]) -> None: ...
 
 global___BenchmarkEntry = BenchmarkEntry
 
-@typing_extensions.final
+@typing.final
 class BenchmarkEntries(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ENTRY_FIELD_NUMBER: builtins.int
     @property
     def entry(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BenchmarkEntry]: ...
     def __init__(
         self,
         *,
         entry: collections.abc.Iterable[global___BenchmarkEntry] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["entry", b"entry"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["entry", b"entry"]) -> None: ...
 
 global___BenchmarkEntries = BenchmarkEntries
 
-@typing_extensions.final
+@typing.final
 class BuildConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODE_FIELD_NUMBER: builtins.int
     CC_FLAGS_FIELD_NUMBER: builtins.int
     OPTS_FIELD_NUMBER: builtins.int
     mode: builtins.str
     """opt, dbg, etc"""
     @property
     def cc_flags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """CC compiler flags, if known"""
+
     @property
     def opts(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Bazel compilation options, if known"""
+
     def __init__(
         self,
         *,
         mode: builtins.str | None = ...,
         cc_flags: collections.abc.Iterable[builtins.str] | None = ...,
         opts: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cc_flags", b"cc_flags", "mode", b"mode", "opts", b"opts"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cc_flags", b"cc_flags", "mode", b"mode", "opts", b"opts"]) -> None: ...
 
 global___BuildConfiguration = BuildConfiguration
 
-@typing_extensions.final
+@typing.final
 class CommitId(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CHANGELIST_FIELD_NUMBER: builtins.int
     HASH_FIELD_NUMBER: builtins.int
     SNAPSHOT_FIELD_NUMBER: builtins.int
     PENDING_CHANGELIST_FIELD_NUMBER: builtins.int
@@ -208,39 +215,39 @@
         self,
         *,
         changelist: builtins.int | None = ...,
         hash: builtins.str | None = ...,
         snapshot: builtins.str | None = ...,
         pending_changelist: builtins.int | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["changelist", b"changelist", "hash", b"hash", "kind", b"kind"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["changelist", b"changelist", "hash", b"hash", "kind", b"kind", "pending_changelist", b"pending_changelist", "snapshot", b"snapshot"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["changelist", "hash"] | None: ...
+    def HasField(self, field_name: typing.Literal["changelist", b"changelist", "hash", b"hash", "kind", b"kind"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["changelist", b"changelist", "hash", b"hash", "kind", b"kind", "pending_changelist", b"pending_changelist", "snapshot", b"snapshot"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["changelist", "hash"] | None: ...
 
 global___CommitId = CommitId
 
-@typing_extensions.final
+@typing.final
 class CPUInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class CacheSizeEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.int
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.int | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     NUM_CORES_FIELD_NUMBER: builtins.int
     NUM_CORES_ALLOWED_FIELD_NUMBER: builtins.int
     MHZ_PER_CPU_FIELD_NUMBER: builtins.int
     CPU_INFO_FIELD_NUMBER: builtins.int
     CPU_GOVERNOR_FIELD_NUMBER: builtins.int
     CACHE_SIZE_FIELD_NUMBER: builtins.int
@@ -255,29 +262,30 @@
     cpu_governor: builtins.str
     """What kind of cpu scaling is enabled on the host.
     Examples include "performance", "ondemand", "conservative", "mixed".
     """
     @property
     def cache_size(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.int]:
         """Cache sizes (in bytes), e.g. "L2": 262144 (for 256KB)"""
+
     def __init__(
         self,
         *,
         num_cores: builtins.int | None = ...,
         num_cores_allowed: builtins.int | None = ...,
         mhz_per_cpu: builtins.float | None = ...,
         cpu_info: builtins.str | None = ...,
         cpu_governor: builtins.str | None = ...,
         cache_size: collections.abc.Mapping[builtins.str, builtins.int] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cache_size", b"cache_size", "cpu_governor", b"cpu_governor", "cpu_info", b"cpu_info", "mhz_per_cpu", b"mhz_per_cpu", "num_cores", b"num_cores", "num_cores_allowed", b"num_cores_allowed"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cache_size", b"cache_size", "cpu_governor", b"cpu_governor", "cpu_info", b"cpu_info", "mhz_per_cpu", b"mhz_per_cpu", "num_cores", b"num_cores", "num_cores_allowed", b"num_cores_allowed"]) -> None: ...
 
 global___CPUInfo = CPUInfo
 
-@typing_extensions.final
+@typing.final
 class MemoryInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TOTAL_FIELD_NUMBER: builtins.int
     AVAILABLE_FIELD_NUMBER: builtins.int
     total: builtins.int
     """Total virtual memory in bytes"""
@@ -285,19 +293,19 @@
     """Immediately available memory in bytes"""
     def __init__(
         self,
         *,
         total: builtins.int | None = ...,
         available: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["available", b"available", "total", b"total"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["available", b"available", "total", b"total"]) -> None: ...
 
 global___MemoryInfo = MemoryInfo
 
-@typing_extensions.final
+@typing.final
 class GPUInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MODEL_FIELD_NUMBER: builtins.int
     UUID_FIELD_NUMBER: builtins.int
     BUS_ID_FIELD_NUMBER: builtins.int
     model: builtins.str
@@ -309,19 +317,19 @@
     def __init__(
         self,
         *,
         model: builtins.str | None = ...,
         uuid: builtins.str | None = ...,
         bus_id: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bus_id", b"bus_id", "model", b"model", "uuid", b"uuid"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bus_id", b"bus_id", "model", b"model", "uuid", b"uuid"]) -> None: ...
 
 global___GPUInfo = GPUInfo
 
-@typing_extensions.final
+@typing.final
 class PlatformInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BITS_FIELD_NUMBER: builtins.int
     LINKAGE_FIELD_NUMBER: builtins.int
     MACHINE_FIELD_NUMBER: builtins.int
     RELEASE_FIELD_NUMBER: builtins.int
@@ -345,19 +353,19 @@
         bits: builtins.str | None = ...,
         linkage: builtins.str | None = ...,
         machine: builtins.str | None = ...,
         release: builtins.str | None = ...,
         system: builtins.str | None = ...,
         version: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bits", b"bits", "linkage", b"linkage", "machine", b"machine", "release", b"release", "system", b"system", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["bits", b"bits", "linkage", b"linkage", "machine", b"machine", "release", b"release", "system", b"system", "version", b"version"]) -> None: ...
 
 global___PlatformInfo = PlatformInfo
 
-@typing_extensions.final
+@typing.final
 class AvailableDeviceInfo(google.protobuf.message.Message):
     """Matches DeviceAttributes"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
@@ -375,19 +383,19 @@
         self,
         *,
         name: builtins.str | None = ...,
         type: builtins.str | None = ...,
         memory_limit: builtins.int | None = ...,
         physical_description: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["memory_limit", b"memory_limit", "name", b"name", "physical_description", b"physical_description", "type", b"type"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["memory_limit", b"memory_limit", "name", b"name", "physical_description", b"physical_description", "type", b"type"]) -> None: ...
 
 global___AvailableDeviceInfo = AvailableDeviceInfo
 
-@typing_extensions.final
+@typing.final
 class MachineConfiguration(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     HOSTNAME_FIELD_NUMBER: builtins.int
     SERIAL_IDENTIFIER_FIELD_NUMBER: builtins.int
     PLATFORM_INFO_FIELD_NUMBER: builtins.int
     CPU_INFO_FIELD_NUMBER: builtins.int
@@ -397,81 +405,86 @@
     hostname: builtins.str
     """Host name of machine that ran the benchmark."""
     serial_identifier: builtins.str
     """Unique serial number of the machine."""
     @property
     def platform_info(self) -> global___PlatformInfo:
         """Additional platform information."""
+
     @property
     def cpu_info(self) -> global___CPUInfo:
         """CPU Information."""
+
     @property
     def device_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.any_pb2.Any]:
         """Other devices that are attached and relevant (e.g. GPUInfo)."""
+
     @property
     def available_device_info(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AvailableDeviceInfo]:
         """Devices accessible to the test (e.g. as given by list_local_devices)."""
+
     @property
     def memory_info(self) -> global___MemoryInfo: ...
     def __init__(
         self,
         *,
         hostname: builtins.str | None = ...,
         serial_identifier: builtins.str | None = ...,
         platform_info: global___PlatformInfo | None = ...,
         cpu_info: global___CPUInfo | None = ...,
         device_info: collections.abc.Iterable[google.protobuf.any_pb2.Any] | None = ...,
         available_device_info: collections.abc.Iterable[global___AvailableDeviceInfo] | None = ...,
         memory_info: global___MemoryInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cpu_info", b"cpu_info", "memory_info", b"memory_info", "platform_info", b"platform_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["available_device_info", b"available_device_info", "cpu_info", b"cpu_info", "device_info", b"device_info", "hostname", b"hostname", "memory_info", b"memory_info", "platform_info", b"platform_info", "serial_identifier", b"serial_identifier"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cpu_info", b"cpu_info", "memory_info", b"memory_info", "platform_info", b"platform_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["available_device_info", b"available_device_info", "cpu_info", b"cpu_info", "device_info", b"device_info", "hostname", b"hostname", "memory_info", b"memory_info", "platform_info", b"platform_info", "serial_identifier", b"serial_identifier"]) -> None: ...
 
 global___MachineConfiguration = MachineConfiguration
 
-@typing_extensions.final
+@typing.final
 class RunConfiguration(google.protobuf.message.Message):
     """Run-specific items such as arguments to the test / benchmark."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class EnvVarsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: builtins.str | None = ...,
         ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     ARGUMENT_FIELD_NUMBER: builtins.int
     ENV_VARS_FIELD_NUMBER: builtins.int
     @property
     def argument(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def env_vars(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Environment variables used to run the test/benchmark."""
+
     def __init__(
         self,
         *,
         argument: collections.abc.Iterable[builtins.str] | None = ...,
         env_vars: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["argument", b"argument", "env_vars", b"env_vars"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["argument", b"argument", "env_vars", b"env_vars"]) -> None: ...
 
 global___RunConfiguration = RunConfiguration
 
-@typing_extensions.final
+@typing.final
 class TestResults(google.protobuf.message.Message):
     """The output of one benchmark / test run.  Each run contains a list of
     tests or benchmarks, stored as BenchmarkEntry messages.
 
     This message should be emitted by the reporter (which runs the
     test / BM in a subprocess and then reads the emitted BenchmarkEntry messages;
     usually from a serialized json file, finally collecting them along
@@ -517,47 +530,52 @@
     BENCHMARK_TYPE_FIELD_NUMBER: builtins.int
     RUN_MODE_FIELD_NUMBER: builtins.int
     TF_VERSION_FIELD_NUMBER: builtins.int
     target: builtins.str
     """The target of the run, e.g.:
      //tensorflow/core:kernels_adjust_contrast_op_benchmark_test
     """
-    @property
-    def entries(self) -> global___BenchmarkEntries:
-        """The list of tests or benchmarks in this run."""
-    @property
-    def build_configuration(self) -> global___BuildConfiguration:
-        """The configuration of the build (compiled opt? with cuda? any copts?)"""
-    @property
-    def commit_id(self) -> global___CommitId:
-        """The commit id (git hash or changelist)"""
     start_time: builtins.int
     """The time the run started (in seconds of UTC time since Unix epoch)"""
     run_time: builtins.float
     """The amount of time the total run took (wall time in seconds)"""
-    @property
-    def machine_configuration(self) -> global___MachineConfiguration:
-        """Machine-specific parameters (Platform and CPU info)"""
-    @property
-    def run_configuration(self) -> global___RunConfiguration:
-        """Run-specific parameters (arguments, etc)"""
     name: builtins.str
     """Benchmark target identifier."""
     benchmark_type: global___TestResults.BenchmarkType.ValueType
     run_mode: builtins.str
     """Used for differentiating between continuous and debug builds.
     Must be one of:
     * cbuild: results from continuous build.
     * presubmit: results from oneshot requests.
     * culprit: results from culprit finder rerun.
     """
     tf_version: builtins.str
     """TensorFlow version this benchmark runs against.
     This can be either set to full version or just the major version.
     """
+    @property
+    def entries(self) -> global___BenchmarkEntries:
+        """The list of tests or benchmarks in this run."""
+
+    @property
+    def build_configuration(self) -> global___BuildConfiguration:
+        """The configuration of the build (compiled opt? with cuda? any copts?)"""
+
+    @property
+    def commit_id(self) -> global___CommitId:
+        """The commit id (git hash or changelist)"""
+
+    @property
+    def machine_configuration(self) -> global___MachineConfiguration:
+        """Machine-specific parameters (Platform and CPU info)"""
+
+    @property
+    def run_configuration(self) -> global___RunConfiguration:
+        """Run-specific parameters (arguments, etc)"""
+
     def __init__(
         self,
         *,
         target: builtins.str | None = ...,
         entries: global___BenchmarkEntries | None = ...,
         build_configuration: global___BuildConfiguration | None = ...,
         commit_id: global___CommitId | None = ...,
@@ -566,11 +584,11 @@
         machine_configuration: global___MachineConfiguration | None = ...,
         run_configuration: global___RunConfiguration | None = ...,
         name: builtins.str | None = ...,
         benchmark_type: global___TestResults.BenchmarkType.ValueType | None = ...,
         run_mode: builtins.str | None = ...,
         tf_version: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["build_configuration", b"build_configuration", "commit_id", b"commit_id", "entries", b"entries", "machine_configuration", b"machine_configuration", "run_configuration", b"run_configuration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["benchmark_type", b"benchmark_type", "build_configuration", b"build_configuration", "commit_id", b"commit_id", "entries", b"entries", "machine_configuration", b"machine_configuration", "name", b"name", "run_configuration", b"run_configuration", "run_mode", b"run_mode", "run_time", b"run_time", "start_time", b"start_time", "target", b"target", "tf_version", b"tf_version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["build_configuration", b"build_configuration", "commit_id", b"commit_id", "entries", b"entries", "machine_configuration", b"machine_configuration", "run_configuration", b"run_configuration"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["benchmark_type", b"benchmark_type", "build_configuration", b"build_configuration", "commit_id", b"commit_id", "entries", b"entries", "machine_configuration", b"machine_configuration", "name", b"name", "run_configuration", b"run_configuration", "run_mode", b"run_mode", "run_time", b"run_time", "start_time", b"start_time", "target", b"target", "tf_version", b"tf_version"]) -> None: ...
 
 global___TestResults = TestResults
```

### Comparing `types-tensorflow-2.15.0.20240314/tensorflow-stubs/types/experimental.pyi` & `types-tensorflow-2.15.0.20240411/tensorflow-stubs/types/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240314
+Version: 2.15.0.20240411
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,17 +27,17 @@
 
 This version of `types-tensorflow` aims to provide accurate annotations
 for `tensorflow==2.15.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
-Partially generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on tensorflow==2.12.1
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a1bfd65e9fa92e1bb61a475c7622ba0376d936d5` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `fe02cba606d1329afd8b1e28451b390d678305e8` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-tensorflow-2.15.0.20240314/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.15.0.20240411/types_tensorflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,22 +60,20 @@
 tensorflow-stubs/core/framework/versions_pb2.pyi
 tensorflow-stubs/core/protobuf/__init__.pyi
 tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
 tensorflow-stubs/core/protobuf/cluster_pb2.pyi
 tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
 tensorflow-stubs/core/protobuf/config_pb2.pyi
 tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
-tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
 tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
 tensorflow-stubs/core/protobuf/data_service_pb2.pyi
 tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
 tensorflow-stubs/core/protobuf/debug_pb2.pyi
 tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
 tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
-tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
 tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
 tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
 tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
 tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
 tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
 tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
 tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
```

