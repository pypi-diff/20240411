# Comparing `tmp/whylogs-1.3.9.tar.gz` & `tmp/whylogs-1.3.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs-1.3.9.tar", max compression
+gzip compressed data, was "whylogs-1.3.9.dev0.tar", max compression
```

## Comparing `whylogs-1.3.9.tar` & `whylogs-1.3.9.dev0.tar`

### file list

```diff
@@ -1,242 +1,242 @@
--rw-r--r--   0        0        0     3166 2023-10-10 21:00:04.731292 whylogs-1.3.9/DESCRIPTION.md
--rw-r--r--   0        0        0     6420 2023-10-10 21:00:41.479796 whylogs-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     1801 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/__init__.py
--rw-r--r--   0        0        0      347 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/__init__.py
--rw-r--r--   0        0        0      590 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/annotations.py
--rw-r--r--   0        0        0      120 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/fugue/__init__.py
--rw-r--r--   0        0        0     4840 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/fugue/profiler.py
--rw-r--r--   0        0        0     1997 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/fugue/registry.py
--rw-r--r--   0        0        0    10067 2023-10-10 21:00:04.799293 whylogs-1.3.9/whylogs/api/logger/__init__.py
--rw-r--r--   0        0        0      101 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/events/__init__.py
--rw-r--r--   0        0        0     5599 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/events/event.py
--rw-r--r--   0        0        0      750 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/events/file_name.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/__init__.py
--rw-r--r--   0        0        0     7857 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/actor.py
--rw-r--r--   0        0        0     2102 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/data_logger.py
--rw-r--r--   0        0        0     1539 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
--rw-r--r--   0        0        0      530 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/future_util.py
--rw-r--r--   0        0        0      650 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/list_util.py
--rw-r--r--   0        0        0     1628 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
--rw-r--r--   0        0        0      282 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
--rw-r--r--   0        0        0     2756 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_actor.py
--rw-r--r--   0        0        0    20221 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
--rw-r--r--   0        0        0     8364 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
--rw-r--r--   0        0        0      358 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/signal_util.py
--rw-r--r--   0        0        0      579 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/string_util.py
--rw-r--r--   0        0        0     2971 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/thread_actor.py
--rw-r--r--   0        0        0    17715 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
--rw-r--r--   0        0        0     4008 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/time_util.py
--rw-r--r--   0        0        0     5458 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/logger.py
--rw-r--r--   0        0        0    20448 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/result_set.py
--rw-r--r--   0        0        0     9549 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/rolling.py
--rw-r--r--   0        0        0     2113 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/segment_cache.py
--rw-r--r--   0        0        0     6462 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/segment_processing.py
--rw-r--r--   0        0        0      687 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/logger/transient.py
--rw-r--r--   0        0        0      406 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/pyspark/experimental/__init__.py
--rw-r--r--   0        0        0     6168 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/pyspark/experimental/profiler.py
--rw-r--r--   0        0        0     7663 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/pyspark/experimental/segmented_profiler.py
--rw-r--r--   0        0        0      465 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/reader/__init__.py
--rw-r--r--   0        0        0      645 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/reader/local.py
--rw-r--r--   0        0        0      617 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/reader/reader.py
--rw-r--r--   0        0        0     2073 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/reader/s3.py
--rw-r--r--   0        0        0      237 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/store/__init__.py
--rw-r--r--   0        0        0     4566 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/store/local_store.py
--rw-r--r--   0        0        0     1208 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/store/profile_store.py
--rw-r--r--   0        0        0      672 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/store/query.py
--rw-r--r--   0        0        0     5350 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/store/sqlite_store.py
--rw-r--r--   0        0        0     6128 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/usage_stats/__init__.py
--rw-r--r--   0        0        0       79 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/__init__.py
--rw-r--r--   0        0        0    17933 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/config.py
--rw-r--r--   0        0        0      354 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/lazy.py
--rw-r--r--   0        0        0      442 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/notebook_check.py
--rw-r--r--   0        0        0     3893 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/notebook_logger.py
--rw-r--r--   0        0        0     2823 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/prompts.py
--rw-r--r--   0        0        0    13188 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/session.py
--rw-r--r--   0        0        0     7029 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/session_manager.py
--rw-r--r--   0        0        0     5095 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/session_types.py
--rw-r--r--   0        0        0      278 2023-10-10 21:00:04.803293 whylogs-1.3.9/whylogs/api/whylabs/session/why_init.py
--rw-r--r--   0        0        0     6586 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/whylabs/session/whylabs_client_cache.py
--rw-r--r--   0        0        0      947 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/__init__.py
--rw-r--r--   0        0        0     2726 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/gcs.py
--rw-r--r--   0        0        0     1169 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/local.py
--rw-r--r--   0        0        0     2084 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/mlflow.py
--rw-r--r--   0        0        0     3408 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/s3.py
--rw-r--r--   0        0        0    42227 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/whylabs.py
--rw-r--r--   0        0        0     1211 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/api/writer/writer.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/context/__init__.py
--rw-r--r--   0        0        0      302 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/context/environ.py
--rw-r--r--   0        0        0      516 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/context/version.py
--rw-r--r--   0        0        0     1090 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/__init__.py
--rw-r--r--   0        0        0     3575 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/column_profile.py
--rw-r--r--   0        0        0      208 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/common.py
--rw-r--r--   0        0        0     1589 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/configs.py
--rw-r--r--   0        0        0      455 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/__init__.py
--rw-r--r--   0        0        0     1798 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/__init__.py
--rw-r--r--   0        0        0     1103 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/cardinality_metrics.py
--rw-r--r--   0        0        0     2049 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/condition_counts.py
--rw-r--r--   0        0        0     2601 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/count_metrics.py
--rw-r--r--   0        0        0     7063 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/distribution_metrics.py
--rw-r--r--   0        0        0     2083 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/frequent_items.py
--rw-r--r--   0        0        0      737 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/multi_metrics.py
--rw-r--r--   0        0        0     3199 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/factories/types_metrics.py
--rw-r--r--   0        0        0    30661 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/constraints/metric_constraints.py
--rw-r--r--   0        0        0    11337 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/dataset_profile.py
--rw-r--r--   0        0        0     4230 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/datatypes.py
--rw-r--r--   0        0        0      518 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/errors.py
--rw-r--r--   0        0        0     2560 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/feature_weights.py
--rw-r--r--   0        0        0      806 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/input_resolver.py
--rw-r--r--   0        0        0     2238 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metadata.py
--rw-r--r--   0        0        0     1740 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metric_getters.py
--rw-r--r--   0        0        0      984 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/__init__.py
--rw-r--r--   0        0        0     4085 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/aggregators.py
--rw-r--r--   0        0        0     5031 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/column_metrics.py
--rw-r--r--   0        0        0     6481 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/compound_metric.py
--rw-r--r--   0        0        0     7615 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/condition_count_metric.py
--rw-r--r--   0        0        0     1597 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/decorators.py
--rw-r--r--   0        0        0     4840 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/deserializers.py
--rw-r--r--   0        0        0     1361 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/maths.py
--rw-r--r--   0        0        0     6053 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/metric_components.py
--rw-r--r--   0        0        0    21749 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/metrics.py
--rw-r--r--   0        0        0     8016 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/multimetric.py
--rw-r--r--   0        0        0     4517 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/serializers.py
--rw-r--r--   0        0        0     5504 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/metrics/unicode_range.py
--rw-r--r--   0        0        0      107 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/model_performance_metrics/__init__.py
--rw-r--r--   0        0        0    10663 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/model_performance_metrics/confusion_matrix.py
--rw-r--r--   0        0        0     7445 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/model_performance_metrics/model_performance_metrics.py
--rw-r--r--   0        0        0     2837 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/model_performance_metrics/regression_metrics.py
--rw-r--r--   0        0        0     5499 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/predicate_parser.py
--rw-r--r--   0        0        0    14608 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/preprocessing.py
--rw-r--r--   0        0        0      335 2023-10-10 21:00:04.807293 whylogs-1.3.9/whylogs/core/projectors.py
--rw-r--r--   0        0        0      183 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/proto/__init__.py
--rw-r--r--   0        0        0      242 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/proto/v0/__init__.py
--rw-r--r--   0        0        0    12534 2023-10-10 21:00:46.367860 whylogs-1.3.9/whylogs/core/proto/v0/v0_constraints_pb2.py
--rw-r--r--   0        0        0    20212 2023-10-10 21:00:44.875841 whylogs-1.3.9/whylogs/core/proto/v0/v0_constraints_pb2.pyi
--rw-r--r--   0        0        0    21343 2023-10-10 21:00:44.875841 whylogs-1.3.9/whylogs/core/proto/v0/v0_messages_pb2.py
--rw-r--r--   0        0        0    29724 2023-10-10 21:00:44.875841 whylogs-1.3.9/whylogs/core/proto/v0/v0_messages_pb2.pyi
--rw-r--r--   0        0        0    18521 2023-10-10 21:00:46.535863 whylogs-1.3.9/whylogs/core/proto/v0/v0_summaries_pb2.py
--rw-r--r--   0        0        0    24739 2023-10-10 21:00:44.875841 whylogs-1.3.9/whylogs/core/proto/v0/v0_summaries_pb2.pyi
--rw-r--r--   0        0        0    18571 2023-10-10 21:00:44.747839 whylogs-1.3.9/whylogs/core/proto/whylogs_messages_pb2.py
--rw-r--r--   0        0        0    21840 2023-10-10 21:00:44.747839 whylogs-1.3.9/whylogs/core/proto/whylogs_messages_pb2.pyi
--rw-r--r--   0        0        0     7350 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/relations.py
--rw-r--r--   0        0        0    11357 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/resolvers.py
--rw-r--r--   0        0        0    10061 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/schema.py
--rw-r--r--   0        0        0      144 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/segment.py
--rw-r--r--   0        0        0     2343 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/segmentation_partition.py
--rw-r--r--   0        0        0      826 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/specialized_resolvers.py
--rw-r--r--   0        0        0     2118 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/stubs.py
--rw-r--r--   0        0        0      486 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/utils/__init__.py
--rw-r--r--   0        0        0     3603 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2569 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/utils/stats_calculations.py
--rw-r--r--   0        0        0      130 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/utils/timestamp_calculations.py
--rw-r--r--   0        0        0     2004 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/utils/utils.py
--rw-r--r--   0        0        0      281 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/validators/__init__.py
--rw-r--r--   0        0        0     4823 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1329 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/validators/validator.py
--rw-r--r--   0        0        0      214 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/view/__init__.py
--rw-r--r--   0        0        0     6157 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/view/column_profile_view.py
--rw-r--r--   0        0        0    17867 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/view/dataset_profile_view.py
--rw-r--r--   0        0        0     9457 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/core/view/segmented_dataset_profile_view.py
--rw-r--r--   0        0        0      211 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/__init__.py
--rw-r--r--   0        0        0     5813 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/base.py
--rw-r--r--   0        0        0     6087 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/configs.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/descr/__init__.py
--rw-r--r--   0        0        0     6397 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/descr/ecommerce.rst
--rw-r--r--   0        0        0     3506 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/descr/employee.rst
--rw-r--r--   0        0        0    11285 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/descr/weather.rst
--rw-r--r--   0        0        0    10688 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/ecommerce.py
--rw-r--r--   0        0        0    10981 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/employee.py
--rw-r--r--   0        0        0     2349 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/utils.py
--rw-r--r--   0        0        0    11476 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/datasets/weather.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/experimental/__init__.py
--rw-r--r--   0        0        0     3530 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/experimental/api/logger/__init__.py
--rw-r--r--   0        0        0     3770 2023-10-10 21:00:04.811293 whylogs-1.3.9/whylogs/experimental/constraints_generation/__init__.py
--rw-r--r--   0        0        0     1105 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/condition_counts.py
--rw-r--r--   0        0        0      846 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/count_metrics.py
--rw-r--r--   0        0        0     1554 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/distribution_metrics.py
--rw-r--r--   0        0        0     1011 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/frequent_items.py
--rw-r--r--   0        0        0      685 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/multi_metrics.py
--rw-r--r--   0        0        0      973 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/constraints_generation/types_metrics.py
--rw-r--r--   0        0        0    19692 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/core/metrics/udf_metric.py
--rw-r--r--   0        0        0    14428 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/core/udf_schema.py
--rw-r--r--   0        0        0      299 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/core/validators/__init__.py
--rw-r--r--   0        0        0     1218 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/core/validators/condition_validator.py
--rw-r--r--   0        0        0     1262 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/core/validators/validator.py
--rw-r--r--   0        0        0     8861 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/extras/embedding_metric.py
--rw-r--r--   0        0        0      939 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/extras/matrix_component.py
--rwxr-xr-x   0        0        0    16737 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/extras/nlp_metric.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/performance_estimation/__init__.py
--rw-r--r--   0        0        0     1554 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/performance_estimation/estimation_results.py
--rw-r--r--   0        0        0     8872 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/performance_estimation/estimators.py
--rw-r--r--   0        0        0     3777 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/experimental/preprocess/embeddings/selectors.py
--rw-r--r--   0        0        0    11126 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/extras/image_metric.py
--rw-r--r--   0        0        0       52 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/migration/__init__.py
--rw-r--r--   0        0        0    15564 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/migration/converters.py
--rw-r--r--   0        0        0     6992 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/migration/uncompound.py
--rw-r--r--   0        0        0      296 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/__init__.py
--rw-r--r--   0        0        0      168 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/configs.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/drift/__init__.py
--rw-r--r--   0        0        0    21751 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/drift/column_drift_algorithms.py
--rw-r--r--   0        0        0     1366 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/drift/configs.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/enums/__init__.py
--rw-r--r--   0        0        0      901 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/enums/enums.py
--rw-r--r--   0        0        0        0 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/__init__.py
--rw-r--r--   0        0        0      114 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/reports/constraints.py
--rw-r--r--   0        0        0      272 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/reports/histograms.py
--rw-r--r--   0        0        0     2502 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/reports/html_report.py
--rw-r--r--   0        0        0      975 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/reports/profile_summary.py
--rw-r--r--   0        0        0     3218 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/extensions/reports/summary_drift.py
--rw-r--r--   0        0        0       38 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/html/.prettierignore
--rw-r--r--   0        0        0      135 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/html/.prettierrc.yaml
--rw-r--r--   0        0        0   155568 2023-10-10 21:00:04.815293 whylogs-1.3.9/whylogs/viz/html/css/bootstrap.min.css
--rw-r--r--   0        0        0    22747 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/css/whylogs-styles.css
--rw-r--r--   0        0        0   160788 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.ttf
--rw-r--r--   0        0        0    50888 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.woff
--rw-r--r--   0        0        0    32180 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.woff2
--rw-r--r--   0        0        0   172144 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
--rw-r--r--   0        0        0    55560 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff
--rw-r--r--   0        0        0    35476 2023-10-10 21:00:04.819293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
--rw-r--r--   0        0        0   172188 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.ttf
--rw-r--r--   0        0        0    55728 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.woff
--rw-r--r--   0        0        0    35144 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.woff2
--rw-r--r--   0        0        0   161212 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.ttf
--rw-r--r--   0        0        0    53244 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.woff
--rw-r--r--   0        0        0    34516 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.woff2
--rw-r--r--   0        0        0   172380 2023-10-10 21:00:04.823293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
--rw-r--r--   0        0        0    59012 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff
--rw-r--r--   0        0        0    38404 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
--rw-r--r--   0        0        0   161220 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.ttf
--rw-r--r--   0        0        0    50936 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.woff
--rw-r--r--   0        0        0    32192 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.woff2
--rw-r--r--   0        0        0   161152 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.ttf
--rw-r--r--   0        0        0    53296 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.woff
--rw-r--r--   0        0        0    34744 2023-10-10 21:00:04.827293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.woff2
--rw-r--r--   0        0        0   172396 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
--rw-r--r--   0        0        0    58892 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
--rw-r--r--   0        0        0    38500 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
--rw-r--r--   0        0        0     3156 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/images/placement-chart.png
--rw-r--r--   0        0        0     9649 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/images/whylabs-favicon.png
--rw-r--r--   0        0        0   270687 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/js/d3.min.js
--rw-r--r--   0        0        0    12606 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/js/handlebars.js
--rw-r--r--   0        0        0    89501 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    55927 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/js/whylogs-script.js
--rw-r--r--   0        0        0    52663 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
--rw-r--r--   0        0        0    14235 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
--rw-r--r--   0        0        0    26825 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
--rw-r--r--   0        0        0    14144 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
--rw-r--r--   0        0        0    15177 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
--rw-r--r--   0        0        0    18298 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
--rw-r--r--   0        0        0    41933 2023-10-10 21:00:04.831293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
--rw-r--r--   0        0        0    98500 2023-10-10 21:00:04.835293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
--rw-r--r--   0        0        0   752494 2023-10-10 21:00:04.835293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-library-all-in.html
--rw-r--r--   0        0        0    25371 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/html/templates/index-hbs.html
--rw-r--r--   0        0        0    26014 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/html/templates/index.html
--rw-r--r--   0        0        0    22429 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/notebook_profile_viz.py
--rw-r--r--   0        0        0      410 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/__init__.py
--rw-r--r--   0        0        0     2466 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/descriptive_stats.py
--rw-r--r--   0        0        0    12576 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/drift_calculations.py
--rw-r--r--   0        0        0     3561 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/frequent_items_calculations.py
--rw-r--r--   0        0        0     2747 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/histogram_calculations.py
--rw-r--r--   0        0        0     1060 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/html_template_utils.py
--rw-r--r--   0        0        0    14298 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/profile_viz_calculations.py
--rw-r--r--   0        0        0     3581 2023-10-10 21:00:04.839293 whylogs-1.3.9/whylogs/viz/utils/quantile_stats.py
--rw-r--r--   0        0        0     7004 1970-01-01 00:00:00.000000 whylogs-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     3166 2023-06-27 17:33:07.264805 whylogs-1.3.9.dev0/DESCRIPTION.md
+-rw-r--r--   0        0        0     6425 2023-10-04 20:19:08.594477 whylogs-1.3.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1801 2023-10-04 20:07:03.827570 whylogs-1.3.9.dev0/whylogs/__init__.py
+-rw-r--r--   0        0        0      347 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-08 01:23:07.097906 whylogs-1.3.9.dev0/whylogs/api/annotations.py
+-rw-r--r--   0        0        0      120 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/fugue/__init__.py
+-rw-r--r--   0        0        0     4840 2023-06-16 15:50:21.999413 whylogs-1.3.9.dev0/whylogs/api/fugue/profiler.py
+-rw-r--r--   0        0        0     1997 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/api/fugue/registry.py
+-rw-r--r--   0        0        0    10067 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/__init__.py
+-rw-r--r--   0        0        0      101 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/__init__.py
+-rw-r--r--   0        0        0     5599 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/event.py
+-rw-r--r--   0        0        0      750 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/events/file_name.py
+-rw-r--r--   0        0        0        0 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/__init__.py
+-rw-r--r--   0        0        0     7857 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/actor.py
+-rw-r--r--   0        0        0     2102 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/data_logger.py
+-rw-r--r--   0        0        0     1539 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py
+-rw-r--r--   0        0        0      530 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/future_util.py
+-rw-r--r--   0        0        0      650 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/list_util.py
+-rw-r--r--   0        0        0     1628 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py
+-rw-r--r--   0        0        0      282 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/proc_error_message.py
+-rw-r--r--   0        0        0     2756 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_actor.py
+-rw-r--r--   0        0        0    20221 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py
+-rw-r--r--   0        0        0     8364 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py
+-rw-r--r--   0        0        0      358 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/signal_util.py
+-rw-r--r--   0        0        0      579 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/string_util.py
+-rw-r--r--   0        0        0     2971 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_actor.py
+-rw-r--r--   0        0        0    17715 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py
+-rw-r--r--   0        0        0     4008 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py
+-rw-r--r--   0        0        0     5458 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/logger.py
+-rw-r--r--   0        0        0    20448 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/result_set.py
+-rw-r--r--   0        0        0     9549 2023-10-02 21:55:43.763605 whylogs-1.3.9.dev0/whylogs/api/logger/rolling.py
+-rw-r--r--   0        0        0     2113 2023-09-14 13:45:35.715676 whylogs-1.3.9.dev0/whylogs/api/logger/segment_cache.py
+-rw-r--r--   0        0        0     6462 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/logger/segment_processing.py
+-rw-r--r--   0        0        0      687 2023-05-31 17:44:36.663303 whylogs-1.3.9.dev0/whylogs/api/logger/transient.py
+-rw-r--r--   0        0        0      406 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/__init__.py
+-rw-r--r--   0        0        0     6168 2023-08-16 17:11:22.596804 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/profiler.py
+-rw-r--r--   0        0        0     7663 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py
+-rw-r--r--   0        0        0      465 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/__init__.py
+-rw-r--r--   0        0        0      645 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/local.py
+-rw-r--r--   0        0        0      617 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/reader.py
+-rw-r--r--   0        0        0     2073 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/reader/s3.py
+-rw-r--r--   0        0        0      237 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/__init__.py
+-rw-r--r--   0        0        0     4566 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/local_store.py
+-rw-r--r--   0        0        0     1208 2023-03-03 16:21:20.616995 whylogs-1.3.9.dev0/whylogs/api/store/profile_store.py
+-rw-r--r--   0        0        0      672 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/query.py
+-rw-r--r--   0        0        0     5350 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/store/sqlite_store.py
+-rw-r--r--   0        0        0     6128 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/usage_stats/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/whylabs/__init__.py
+-rw-r--r--   0        0        0    17933 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/config.py
+-rw-r--r--   0        0        0      354 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/lazy.py
+-rw-r--r--   0        0        0      442 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_check.py
+-rw-r--r--   0        0        0     3893 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_logger.py
+-rw-r--r--   0        0        0     2823 2023-10-02 22:34:26.613605 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/prompts.py
+-rw-r--r--   0        0        0    13188 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session.py
+-rw-r--r--   0        0        0     7029 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_manager.py
+-rw-r--r--   0        0        0     5095 2023-09-22 16:11:43.930291 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_types.py
+-rw-r--r--   0        0        0      278 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/why_init.py
+-rw-r--r--   0        0        0     6586 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/api/whylabs/session/whylabs_client_cache.py
+-rw-r--r--   0        0        0      947 2023-01-30 20:46:41.225482 whylogs-1.3.9.dev0/whylogs/api/writer/__init__.py
+-rw-r--r--   0        0        0     2726 2023-06-16 15:50:22.009413 whylogs-1.3.9.dev0/whylogs/api/writer/gcs.py
+-rw-r--r--   0        0        0     1169 2023-06-16 15:50:22.009413 whylogs-1.3.9.dev0/whylogs/api/writer/local.py
+-rw-r--r--   0        0        0     2084 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/writer/mlflow.py
+-rw-r--r--   0        0        0     3408 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/api/writer/s3.py
+-rw-r--r--   0        0        0    42227 2023-10-04 20:17:38.537768 whylogs-1.3.9.dev0/whylogs/api/writer/whylabs.py
+-rw-r--r--   0        0        0     1211 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/api/writer/writer.py
+-rw-r--r--   0        0        0        0 2023-10-04 20:06:57.677570 whylogs-1.3.9.dev0/whylogs/context/__init__.py
+-rw-r--r--   0        0        0      302 2023-10-04 20:17:37.837768 whylogs-1.3.9.dev0/whylogs/context/environ.py
+-rw-r--r--   0        0        0      502 2023-10-04 20:07:00.617570 whylogs-1.3.9.dev0/whylogs/context/version.py
+-rw-r--r--   0        0        0     1090 2023-08-31 15:56:24.908582 whylogs-1.3.9.dev0/whylogs/core/__init__.py
+-rw-r--r--   0        0        0     3575 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/column_profile.py
+-rw-r--r--   0        0        0      208 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/common.py
+-rw-r--r--   0        0        0     1589 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/configs.py
+-rw-r--r--   0        0        0      455 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/core/constraints/__init__.py
+-rw-r--r--   0        0        0     1798 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/__init__.py
+-rw-r--r--   0        0        0     1103 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py
+-rw-r--r--   0        0        0     2049 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/condition_counts.py
+-rw-r--r--   0        0        0     2601 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/count_metrics.py
+-rw-r--r--   0        0        0     7063 2023-05-25 19:20:19.422537 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py
+-rw-r--r--   0        0        0     2083 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/frequent_items.py
+-rw-r--r--   0        0        0      737 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/multi_metrics.py
+-rw-r--r--   0        0        0     3199 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/constraints/factories/types_metrics.py
+-rw-r--r--   0        0        0    30661 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/constraints/metric_constraints.py
+-rw-r--r--   0        0        0    11337 2023-09-22 19:58:53.969842 whylogs-1.3.9.dev0/whylogs/core/dataset_profile.py
+-rw-r--r--   0        0        0     4230 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/datatypes.py
+-rw-r--r--   0        0        0      518 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/errors.py
+-rw-r--r--   0        0        0     2560 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/feature_weights.py
+-rw-r--r--   0        0        0      806 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/input_resolver.py
+-rw-r--r--   0        0        0     2045 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/core/metadata.py
+-rw-r--r--   0        0        0     1740 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/metric_getters.py
+-rw-r--r--   0        0        0      984 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/__init__.py
+-rw-r--r--   0        0        0     4085 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/aggregators.py
+-rw-r--r--   0        0        0     5031 2023-04-20 13:28:02.613992 whylogs-1.3.9.dev0/whylogs/core/metrics/column_metrics.py
+-rw-r--r--   0        0        0     6481 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/compound_metric.py
+-rw-r--r--   0        0        0     7615 2023-06-27 17:33:07.364805 whylogs-1.3.9.dev0/whylogs/core/metrics/condition_count_metric.py
+-rw-r--r--   0        0        0     1597 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/decorators.py
+-rw-r--r--   0        0        0     4840 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/deserializers.py
+-rw-r--r--   0        0        0     1361 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/maths.py
+-rw-r--r--   0        0        0     6053 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/metric_components.py
+-rw-r--r--   0        0        0    21749 2023-07-04 17:04:07.025540 whylogs-1.3.9.dev0/whylogs/core/metrics/metrics.py
+-rw-r--r--   0        0        0     8016 2023-06-06 15:22:27.487907 whylogs-1.3.9.dev0/whylogs/core/metrics/multimetric.py
+-rw-r--r--   0        0        0     4517 2023-04-11 19:13:37.824666 whylogs-1.3.9.dev0/whylogs/core/metrics/serializers.py
+-rw-r--r--   0        0        0     5504 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/metrics/unicode_range.py
+-rw-r--r--   0        0        0      107 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/__init__.py
+-rw-r--r--   0        0        0    10663 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py
+-rw-r--r--   0        0        0     7445 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py
+-rw-r--r--   0        0        0     2837 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py
+-rw-r--r--   0        0        0     5499 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/predicate_parser.py
+-rw-r--r--   0        0        0    14608 2023-08-25 20:03:25.598581 whylogs-1.3.9.dev0/whylogs/core/preprocessing.py
+-rw-r--r--   0        0        0      335 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/projectors.py
+-rw-r--r--   0        0        0      183 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/proto/__init__.py
+-rw-r--r--   0        0        0      242 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/proto/v0/__init__.py
+-rw-r--r--   0        0        0    12534 2023-10-04 20:35:56.255776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py
+-rw-r--r--   0        0        0    20212 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi
+-rw-r--r--   0        0        0    21343 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py
+-rw-r--r--   0        0        0    29724 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi
+-rw-r--r--   0        0        0    18521 2023-10-04 20:35:56.365776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py
+-rw-r--r--   0        0        0    24739 2023-10-04 20:35:55.705776 whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi
+-rw-r--r--   0        0        0    18571 2023-10-04 20:35:55.575776 whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py
+-rw-r--r--   0        0        0    21840 2023-10-04 20:35:55.575776 whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi
+-rw-r--r--   0        0        0     7350 2023-02-24 20:07:49.042231 whylogs-1.3.9.dev0/whylogs/core/relations.py
+-rw-r--r--   0        0        0    11357 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/core/resolvers.py
+-rw-r--r--   0        0        0    10061 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/schema.py
+-rw-r--r--   0        0        0      144 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/segment.py
+-rw-r--r--   0        0        0     2343 2023-03-22 21:08:17.851744 whylogs-1.3.9.dev0/whylogs/core/segmentation_partition.py
+-rw-r--r--   0        0        0      826 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/core/specialized_resolvers.py
+-rw-r--r--   0        0        0     2118 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/stubs.py
+-rw-r--r--   0        0        0      486 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/utils/__init__.py
+-rw-r--r--   0        0        0     3603 2023-06-23 19:18:55.967672 whylogs-1.3.9.dev0/whylogs/core/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2569 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/utils/stats_calculations.py
+-rw-r--r--   0        0        0      130 2023-01-30 20:46:41.235482 whylogs-1.3.9.dev0/whylogs/core/utils/timestamp_calculations.py
+-rw-r--r--   0        0        0     2004 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/core/utils/utils.py
+-rw-r--r--   0        0        0      281 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/__init__.py
+-rw-r--r--   0        0        0     4823 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1329 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/core/validators/validator.py
+-rw-r--r--   0        0        0      214 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/core/view/__init__.py
+-rw-r--r--   0        0        0     6157 2023-06-27 17:33:07.374805 whylogs-1.3.9.dev0/whylogs/core/view/column_profile_view.py
+-rw-r--r--   0        0        0    17867 2023-09-06 16:54:55.052065 whylogs-1.3.9.dev0/whylogs/core/view/dataset_profile_view.py
+-rw-r--r--   0        0        0     9457 2023-10-04 14:11:26.367936 whylogs-1.3.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py
+-rw-r--r--   0        0        0      211 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/__init__.py
+-rw-r--r--   0        0        0     5813 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/base.py
+-rw-r--r--   0        0        0     6087 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/descr/__init__.py
+-rw-r--r--   0        0        0     6397 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/descr/ecommerce.rst
+-rw-r--r--   0        0        0     3506 2023-02-22 16:52:30.792231 whylogs-1.3.9.dev0/whylogs/datasets/descr/employee.rst
+-rw-r--r--   0        0        0    11285 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/descr/weather.rst
+-rw-r--r--   0        0        0    10688 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/ecommerce.py
+-rw-r--r--   0        0        0    10981 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/employee.py
+-rw-r--r--   0        0        0     2349 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/datasets/utils.py
+-rw-r--r--   0        0        0    11476 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/datasets/weather.py
+-rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/__init__.py
+-rw-r--r--   0        0        0     3530 2023-07-19 19:51:34.012366 whylogs-1.3.9.dev0/whylogs/experimental/api/logger/__init__.py
+-rw-r--r--   0        0        0     3770 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/condition_counts.py
+-rw-r--r--   0        0        0      846 2023-03-28 21:40:50.417571 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/count_metrics.py
+-rw-r--r--   0        0        0     1554 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py
+-rw-r--r--   0        0        0     1011 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/frequent_items.py
+-rw-r--r--   0        0        0      685 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/multi_metrics.py
+-rw-r--r--   0        0        0      973 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/types_metrics.py
+-rw-r--r--   0        0        0    19692 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/experimental/core/metrics/udf_metric.py
+-rw-r--r--   0        0        0    14428 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/udf_schema.py
+-rw-r--r--   0        0        0      299 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/__init__.py
+-rw-r--r--   0        0        0     1218 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/condition_validator.py
+-rw-r--r--   0        0        0     1262 2023-08-25 20:03:25.608581 whylogs-1.3.9.dev0/whylogs/experimental/core/validators/validator.py
+-rw-r--r--   0        0        0     8861 2023-06-27 17:33:07.384805 whylogs-1.3.9.dev0/whylogs/experimental/extras/embedding_metric.py
+-rw-r--r--   0        0        0      939 2023-02-14 19:22:29.792231 whylogs-1.3.9.dev0/whylogs/experimental/extras/matrix_component.py
+-rwxr-xr-x   0        0        0    16737 2023-07-03 16:02:37.106297 whylogs-1.3.9.dev0/whylogs/experimental/extras/nlp_metric.py
+-rw-r--r--   0        0        0        0 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/__init__.py
+-rw-r--r--   0        0        0     1554 2023-04-11 19:13:37.834666 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimation_results.py
+-rw-r--r--   0        0        0     8872 2023-03-03 16:19:17.576995 whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimators.py
+-rw-r--r--   0        0        0     3777 2023-06-27 17:33:07.394805 whylogs-1.3.9.dev0/whylogs/experimental/preprocess/embeddings/selectors.py
+-rw-r--r--   0        0        0    11126 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/extras/image_metric.py
+-rw-r--r--   0        0        0       52 2023-02-27 17:39:54.122231 whylogs-1.3.9.dev0/whylogs/migration/__init__.py
+-rw-r--r--   0        0        0    15564 2023-09-12 18:45:06.905676 whylogs-1.3.9.dev0/whylogs/migration/converters.py
+-rw-r--r--   0        0        0     6992 2023-08-28 14:42:47.838581 whylogs-1.3.9.dev0/whylogs/migration/uncompound.py
+-rw-r--r--   0        0        0      296 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/__init__.py
+-rw-r--r--   0        0        0      168 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/drift/__init__.py
+-rw-r--r--   0        0        0    21751 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/drift/column_drift_algorithms.py
+-rw-r--r--   0        0        0     1366 2023-03-24 22:58:37.321744 whylogs-1.3.9.dev0/whylogs/viz/drift/configs.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/enums/__init__.py
+-rw-r--r--   0        0        0      901 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/enums/enums.py
+-rw-r--r--   0        0        0        0 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/__init__.py
+-rw-r--r--   0        0        0      114 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/constraints.py
+-rw-r--r--   0        0        0      272 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/histograms.py
+-rw-r--r--   0        0        0     2502 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/html_report.py
+-rw-r--r--   0        0        0      975 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/profile_summary.py
+-rw-r--r--   0        0        0     3218 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/summary_drift.py
+-rw-r--r--   0        0        0       38 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/.prettierignore
+-rw-r--r--   0        0        0      135 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/.prettierrc.yaml
+-rw-r--r--   0        0        0   155568 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/css/bootstrap.min.css
+-rw-r--r--   0        0        0    22747 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/css/whylogs-styles.css
+-rw-r--r--   0        0        0   160788 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf
+-rw-r--r--   0        0        0    50888 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff
+-rw-r--r--   0        0        0    32180 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2
+-rw-r--r--   0        0        0   172144 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf
+-rw-r--r--   0        0        0    55560 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff
+-rw-r--r--   0        0        0    35476 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2
+-rw-r--r--   0        0        0   172188 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf
+-rw-r--r--   0        0        0    55728 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff
+-rw-r--r--   0        0        0    35144 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2
+-rw-r--r--   0        0        0   161212 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf
+-rw-r--r--   0        0        0    53244 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff
+-rw-r--r--   0        0        0    34516 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2
+-rw-r--r--   0        0        0   172380 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf
+-rw-r--r--   0        0        0    59012 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff
+-rw-r--r--   0        0        0    38404 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2
+-rw-r--r--   0        0        0   161220 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf
+-rw-r--r--   0        0        0    50936 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff
+-rw-r--r--   0        0        0    32192 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2
+-rw-r--r--   0        0        0   161152 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf
+-rw-r--r--   0        0        0    53296 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff
+-rw-r--r--   0        0        0    34744 2023-01-30 20:46:41.245482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2
+-rw-r--r--   0        0        0   172396 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0        0        0    58892 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff
+-rw-r--r--   0        0        0    38500 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2
+-rw-r--r--   0        0        0     3156 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/images/placement-chart.png
+-rw-r--r--   0        0        0     9649 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/images/whylabs-favicon.png
+-rw-r--r--   0        0        0   270687 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/d3.min.js
+-rw-r--r--   0        0        0    12606 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/handlebars.js
+-rw-r--r--   0        0        0    89501 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0    55927 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/js/whylogs-script.js
+-rw-r--r--   0        0        0    52663 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html
+-rw-r--r--   0        0        0    14235 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html
+-rw-r--r--   0        0        0    26825 2023-05-25 19:20:19.432537 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html
+-rw-r--r--   0        0        0    14144 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html
+-rw-r--r--   0        0        0    15177 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html
+-rw-r--r--   0        0        0    18298 2023-01-30 20:46:41.255482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html
+-rw-r--r--   0        0        0    41933 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html
+-rw-r--r--   0        0        0    98500 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html
+-rw-r--r--   0        0        0   752494 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html
+-rw-r--r--   0        0        0    25371 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs.html
+-rw-r--r--   0        0        0    26014 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/html/templates/index.html
+-rw-r--r--   0        0        0    22429 2023-10-03 20:09:49.137598 whylogs-1.3.9.dev0/whylogs/viz/notebook_profile_viz.py
+-rw-r--r--   0        0        0      410 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/__init__.py
+-rw-r--r--   0        0        0     2466 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/descriptive_stats.py
+-rw-r--r--   0        0        0    12576 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/drift_calculations.py
+-rw-r--r--   0        0        0     3561 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/utils/frequent_items_calculations.py
+-rw-r--r--   0        0        0     2747 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/histogram_calculations.py
+-rw-r--r--   0        0        0     1060 2023-04-20 13:28:02.623992 whylogs-1.3.9.dev0/whylogs/viz/utils/html_template_utils.py
+-rw-r--r--   0        0        0    14298 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/profile_viz_calculations.py
+-rw-r--r--   0        0        0     3581 2023-01-30 20:46:41.265482 whylogs-1.3.9.dev0/whylogs/viz/utils/quantile_stats.py
+-rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 whylogs-1.3.9.dev0/PKG-INFO
```

### Comparing `whylogs-1.3.9/DESCRIPTION.md` & `whylogs-1.3.9.dev0/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/pyproject.toml` & `whylogs-1.3.9.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylogs"
-version = "1.3.9"
+version = "1.3.9-dev0"
 description = "Profile and monitor your ML data pipeline end-to-end"
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 homepage = "https://docs.whylabs.ai"
 readme = "DESCRIPTION.md"
 include = ["whylogs/core/proto/v0/*.py*", "whylogs/core/proto/*.py*"]
```

### Comparing `whylogs-1.3.9/whylogs/__init__.py` & `whylogs-1.3.9.dev0/whylogs/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/annotations.py` & `whylogs-1.3.9.dev0/whylogs/api/annotations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/fugue/profiler.py` & `whylogs-1.3.9.dev0/whylogs/api/fugue/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/fugue/registry.py` & `whylogs-1.3.9.dev0/whylogs/api/fugue/registry.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/__init__.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/events/event.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/events/event.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/events/file_name.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/events/file_name.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/actor.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/data_logger.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/data_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/faster_fifo_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/future_util.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/future_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/list_util.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/list_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/mp_queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_actor.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/process_rolling_logger_messages.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/string_util.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/string_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/thread_actor.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_actor.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/thread_rolling_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/experimental/logger/actor/time_util.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/experimental/logger/actor/time_util.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/logger.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/result_set.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/result_set.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/rolling.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/rolling.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/segment_cache.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/segment_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/segment_processing.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/segment_processing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/logger/transient.py` & `whylogs-1.3.9.dev0/whylogs/api/logger/transient.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/pyspark/experimental/profiler.py` & `whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/pyspark/experimental/segmented_profiler.py` & `whylogs-1.3.9.dev0/whylogs/api/pyspark/experimental/segmented_profiler.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/reader/local.py` & `whylogs-1.3.9.dev0/whylogs/api/reader/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/reader/reader.py` & `whylogs-1.3.9.dev0/whylogs/api/reader/reader.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/reader/s3.py` & `whylogs-1.3.9.dev0/whylogs/api/reader/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/store/local_store.py` & `whylogs-1.3.9.dev0/whylogs/api/store/local_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/store/profile_store.py` & `whylogs-1.3.9.dev0/whylogs/api/store/profile_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/store/query.py` & `whylogs-1.3.9.dev0/whylogs/api/store/query.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/store/sqlite_store.py` & `whylogs-1.3.9.dev0/whylogs/api/store/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/usage_stats/__init__.py` & `whylogs-1.3.9.dev0/whylogs/api/usage_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/config.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/config.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/notebook_logger.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/notebook_logger.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/prompts.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/prompts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/session.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/session_manager.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_manager.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/session_types.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/session_types.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/whylabs/session/whylabs_client_cache.py` & `whylogs-1.3.9.dev0/whylogs/api/whylabs/session/whylabs_client_cache.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/__init__.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/gcs.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/gcs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/local.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/local.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/mlflow.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/mlflow.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/s3.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/s3.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/whylabs.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/whylabs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/api/writer/writer.py` & `whylogs-1.3.9.dev0/whylogs/api/writer/writer.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/__init__.py` & `whylogs-1.3.9.dev0/whylogs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/column_profile.py` & `whylogs-1.3.9.dev0/whylogs/core/column_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/configs.py` & `whylogs-1.3.9.dev0/whylogs/core/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/__init__.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/cardinality_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/cardinality_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/condition_counts.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/count_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/distribution_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/frequent_items.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/multi_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/factories/types_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/factories/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/constraints/metric_constraints.py` & `whylogs-1.3.9.dev0/whylogs/core/constraints/metric_constraints.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/dataset_profile.py` & `whylogs-1.3.9.dev0/whylogs/core/dataset_profile.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/datatypes.py` & `whylogs-1.3.9.dev0/whylogs/core/datatypes.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/errors.py` & `whylogs-1.3.9.dev0/whylogs/core/errors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/feature_weights.py` & `whylogs-1.3.9.dev0/whylogs/core/feature_weights.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/input_resolver.py` & `whylogs-1.3.9.dev0/whylogs/core/input_resolver.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metadata.py` & `whylogs-1.3.9.dev0/whylogs/core/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import json
 import logging
 from datetime import datetime, timezone
 from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
-from whylogs.context.version import whylogs_version
 from whylogs.core.utils.timestamp_calculations import to_utc_milliseconds
 
 diagnostic_logger = logging.getLogger(__name__)
 
 WHYLABS_TRACE_ID_KEY = "whylabs.traceId"
 CREATION_TIMESTAMP_KEY = "whylogs.creationTimestamp"
 DATASET_TIMESTAMP_KEY = "whylogs.datasetTimestamp"
 USER_TAGS_KEY = "whylogs.user.tags"
 NAME_KEY = "whylogs.name"
-WHYLOGS_VERSION_KEY = "whylogs.version"
 
 
 def _populate_common_profile_metadata(
     metadata: Optional[Dict[str, str]] = None,
     *,
     name: Optional[str] = None,
     trace_id: Optional[str] = None,
@@ -51,11 +49,8 @@
         metadata[DATASET_TIMESTAMP_KEY] = str(timestamp)
 
     if name and NAME_KEY not in metadata:
         metadata[NAME_KEY] = name
     if tags and USER_TAGS_KEY not in metadata:
         metadata[USER_TAGS_KEY] = json.dumps(sorted(set(tags)))
 
-    if WHYLOGS_VERSION_KEY not in metadata:
-        metadata[WHYLOGS_VERSION_KEY] = whylogs_version
-
     return metadata
```

### Comparing `whylogs-1.3.9/whylogs/core/metric_getters.py` & `whylogs-1.3.9.dev0/whylogs/core/metric_getters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/__init__.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/aggregators.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/aggregators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/column_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/column_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/compound_metric.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/compound_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/condition_count_metric.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/condition_count_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/decorators.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/decorators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/deserializers.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/deserializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/maths.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/maths.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/metric_components.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/metric_components.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/multimetric.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/multimetric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/serializers.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/serializers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/metrics/unicode_range.py` & `whylogs-1.3.9.dev0/whylogs/core/metrics/unicode_range.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/model_performance_metrics/confusion_matrix.py` & `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/model_performance_metrics/model_performance_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/model_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/model_performance_metrics/regression_metrics.py` & `whylogs-1.3.9.dev0/whylogs/core/model_performance_metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/predicate_parser.py` & `whylogs-1.3.9.dev0/whylogs/core/predicate_parser.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/preprocessing.py` & `whylogs-1.3.9.dev0/whylogs/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_constraints_pb2.py` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_constraints_pb2.pyi` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_constraints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_messages_pb2.py` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_messages_pb2.pyi` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_summaries_pb2.py` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/v0/v0_summaries_pb2.pyi` & `whylogs-1.3.9.dev0/whylogs/core/proto/v0/v0_summaries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/whylogs_messages_pb2.py` & `whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/proto/whylogs_messages_pb2.pyi` & `whylogs-1.3.9.dev0/whylogs/core/proto/whylogs_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/relations.py` & `whylogs-1.3.9.dev0/whylogs/core/relations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/resolvers.py` & `whylogs-1.3.9.dev0/whylogs/core/resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/schema.py` & `whylogs-1.3.9.dev0/whylogs/core/schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/segmentation_partition.py` & `whylogs-1.3.9.dev0/whylogs/core/segmentation_partition.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/specialized_resolvers.py` & `whylogs-1.3.9.dev0/whylogs/core/specialized_resolvers.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/stubs.py` & `whylogs-1.3.9.dev0/whylogs/core/stubs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/utils/protobuf_utils.py` & `whylogs-1.3.9.dev0/whylogs/core/utils/protobuf_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/utils/stats_calculations.py` & `whylogs-1.3.9.dev0/whylogs/core/utils/stats_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/utils/utils.py` & `whylogs-1.3.9.dev0/whylogs/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/validators/condition_validator.py` & `whylogs-1.3.9.dev0/whylogs/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/validators/validator.py` & `whylogs-1.3.9.dev0/whylogs/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/view/column_profile_view.py` & `whylogs-1.3.9.dev0/whylogs/core/view/column_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/view/dataset_profile_view.py` & `whylogs-1.3.9.dev0/whylogs/core/view/dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/core/view/segmented_dataset_profile_view.py` & `whylogs-1.3.9.dev0/whylogs/core/view/segmented_dataset_profile_view.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/base.py` & `whylogs-1.3.9.dev0/whylogs/datasets/base.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/configs.py` & `whylogs-1.3.9.dev0/whylogs/datasets/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/descr/ecommerce.rst` & `whylogs-1.3.9.dev0/whylogs/datasets/descr/ecommerce.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/descr/employee.rst` & `whylogs-1.3.9.dev0/whylogs/datasets/descr/employee.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/descr/weather.rst` & `whylogs-1.3.9.dev0/whylogs/datasets/descr/weather.rst`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/ecommerce.py` & `whylogs-1.3.9.dev0/whylogs/datasets/ecommerce.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/employee.py` & `whylogs-1.3.9.dev0/whylogs/datasets/employee.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/utils.py` & `whylogs-1.3.9.dev0/whylogs/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/datasets/weather.py` & `whylogs-1.3.9.dev0/whylogs/datasets/weather.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/api/logger/__init__.py` & `whylogs-1.3.9.dev0/whylogs/experimental/api/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/__init__.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/condition_counts.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/condition_counts.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/count_metrics.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/count_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/distribution_metrics.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/distribution_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/frequent_items.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/frequent_items.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/multi_metrics.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/multi_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/constraints_generation/types_metrics.py` & `whylogs-1.3.9.dev0/whylogs/experimental/constraints_generation/types_metrics.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/core/metrics/udf_metric.py` & `whylogs-1.3.9.dev0/whylogs/experimental/core/metrics/udf_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/core/udf_schema.py` & `whylogs-1.3.9.dev0/whylogs/experimental/core/udf_schema.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/core/validators/condition_validator.py` & `whylogs-1.3.9.dev0/whylogs/experimental/core/validators/condition_validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/core/validators/validator.py` & `whylogs-1.3.9.dev0/whylogs/experimental/core/validators/validator.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/extras/embedding_metric.py` & `whylogs-1.3.9.dev0/whylogs/experimental/extras/embedding_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/extras/matrix_component.py` & `whylogs-1.3.9.dev0/whylogs/experimental/extras/matrix_component.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/extras/nlp_metric.py` & `whylogs-1.3.9.dev0/whylogs/experimental/extras/nlp_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/performance_estimation/estimation_results.py` & `whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimation_results.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/performance_estimation/estimators.py` & `whylogs-1.3.9.dev0/whylogs/experimental/performance_estimation/estimators.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/experimental/preprocess/embeddings/selectors.py` & `whylogs-1.3.9.dev0/whylogs/experimental/preprocess/embeddings/selectors.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/extras/image_metric.py` & `whylogs-1.3.9.dev0/whylogs/extras/image_metric.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/migration/converters.py` & `whylogs-1.3.9.dev0/whylogs/migration/converters.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/migration/uncompound.py` & `whylogs-1.3.9.dev0/whylogs/migration/uncompound.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/drift/column_drift_algorithms.py` & `whylogs-1.3.9.dev0/whylogs/viz/drift/column_drift_algorithms.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/drift/configs.py` & `whylogs-1.3.9.dev0/whylogs/viz/drift/configs.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/enums/enums.py` & `whylogs-1.3.9.dev0/whylogs/viz/enums/enums.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/extensions/reports/html_report.py` & `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/html_report.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/extensions/reports/profile_summary.py` & `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/profile_summary.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/extensions/reports/summary_drift.py` & `whylogs-1.3.9.dev0/whylogs/viz/extensions/reports/summary_drift.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/css/bootstrap.min.css` & `whylogs-1.3.9.dev0/whylogs/viz/html/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/css/whylogs-styles.css` & `whylogs-1.3.9.dev0/whylogs/viz/html/css/whylogs-styles.css`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Bold.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Bold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-BoldItalic.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Italic.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Italic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Medium.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Medium.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-MediumItalic.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-MediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-Regular.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-Regular.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBold.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2` & `whylogs-1.3.9.dev0/whylogs/viz/html/fonts/Asap-SemiBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/images/placement-chart.png` & `whylogs-1.3.9.dev0/whylogs/viz/html/images/placement-chart.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/images/whylabs-favicon.png` & `whylogs-1.3.9.dev0/whylogs/viz/html/images/whylabs-favicon.png`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/js/d3.min.js` & `whylogs-1.3.9.dev0/whylogs/viz/html/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/js/handlebars.js` & `whylogs-1.3.9.dev0/whylogs/viz/html/js/handlebars.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/js/jquery-3.6.0.min.js` & `whylogs-1.3.9.dev0/whylogs/viz/html/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/js/whylogs-script.js` & `whylogs-1.3.9.dev0/whylogs/viz/html/js/whylogs-script.js`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-for-jupyter-notebook.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-bar-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-constraints-report.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-differenced-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-distribution-chart.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-feature-summary-statistics.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in-jupyter-profile-summary.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-cdn-all-in.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-cdn-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs-library-all-in.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs-library-all-in.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index-hbs.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index-hbs.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/html/templates/index.html` & `whylogs-1.3.9.dev0/whylogs/viz/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/notebook_profile_viz.py` & `whylogs-1.3.9.dev0/whylogs/viz/notebook_profile_viz.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/descriptive_stats.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/drift_calculations.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/drift_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/frequent_items_calculations.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/frequent_items_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/histogram_calculations.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/histogram_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/html_template_utils.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/html_template_utils.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/profile_viz_calculations.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/profile_viz_calculations.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/whylogs/viz/utils/quantile_stats.py` & `whylogs-1.3.9.dev0/whylogs/viz/utils/quantile_stats.py`

 * *Files identical despite different names*

### Comparing `whylogs-1.3.9/PKG-INFO` & `whylogs-1.3.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,438 +1,439 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7768 796c  : 2.1.Name: whyl
 00000020: 6f67 730a 5665 7273 696f 6e3a 2031 2e33  ogs.Version: 1.3
-00000030: 2e39 0a53 756d 6d61 7279 3a20 5072 6f66  .9.Summary: Prof
-00000040: 696c 6520 616e 6420 6d6f 6e69 746f 7220  ile and monitor 
-00000050: 796f 7572 204d 4c20 6461 7461 2070 6970  your ML data pip
-00000060: 656c 696e 6520 656e 642d 746f 2d65 6e64  eline end-to-end
-00000070: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000080: 733a 2f2f 646f 6373 2e77 6879 6c61 6273  s://docs.whylabs
-00000090: 2e61 690a 4c69 6365 6e73 653a 2041 7061  .ai.License: Apa
-000000a0: 6368 652d 322e 300a 4175 7468 6f72 3a20  che-2.0.Author: 
-000000b0: 5768 794c 6162 732e 6169 0a41 7574 686f  WhyLabs.ai.Autho
-000000c0: 722d 656d 6169 6c3a 2073 7570 706f 7274  r-email: support
-000000d0: 4077 6879 6c61 6273 2e61 690a 5265 7175  @whylabs.ai.Requ
-000000e0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000000f0: 2e37 2e31 2c3c 340a 436c 6173 7369 6669  .7.1,<4.Classifi
-00000100: 6572 3a20 4c69 6365 6e73 6520 3a3a 204f  er: License :: O
-00000110: 5349 2041 7070 726f 7665 6420 3a3a 2041  SI Approved :: A
-00000120: 7061 6368 6520 536f 6674 7761 7265 204c  pache Software L
-00000130: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
-00000140: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000150: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000160: 6e20 3a3a 2033 0a43 6c61 7373 6966 6965  n :: 3.Classifie
-00000170: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000180: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000190: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-000001a0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000001b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001c0: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-000001d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000001f0: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000200: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000210: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000220: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000230: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000240: 2061 6c6c 0a50 726f 7669 6465 732d 4578   all.Provides-Ex
-00000250: 7472 613a 2064 6174 6173 6574 730a 5072  tra: datasets.Pr
-00000260: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
-00000270: 6373 0a50 726f 7669 6465 732d 4578 7472  cs.Provides-Extr
-00000280: 613a 2065 6d62 6564 6469 6e67 730a 5072  a: embeddings.Pr
-00000290: 6f76 6964 6573 2d45 7874 7261 3a20 6675  ovides-Extra: fu
-000002a0: 6775 650a 5072 6f76 6964 6573 2d45 7874  gue.Provides-Ext
-000002b0: 7261 3a20 6763 730a 5072 6f76 6964 6573  ra: gcs.Provides
-000002c0: 2d45 7874 7261 3a20 696d 6167 650a 5072  -Extra: image.Pr
-000002d0: 6f76 6964 6573 2d45 7874 7261 3a20 6d6c  ovides-Extra: ml
-000002e0: 666c 6f77 0a50 726f 7669 6465 732d 4578  flow.Provides-Ex
-000002f0: 7472 613a 2070 726f 630a 5072 6f76 6964  tra: proc.Provid
-00000300: 6573 2d45 7874 7261 3a20 7072 6f63 2d6d  es-Extra: proc-m
-00000310: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
-00000320: 3a20 7333 0a50 726f 7669 6465 732d 4578  : s3.Provides-Ex
-00000330: 7472 613a 2073 7061 726b 0a50 726f 7669  tra: spark.Provi
-00000340: 6465 732d 4578 7472 613a 2076 697a 0a52  des-Extra: viz.R
-00000350: 6571 7569 7265 732d 4469 7374 3a20 5069  equires-Dist: Pi
-00000360: 6c6c 6f77 2028 3e3d 392e 322e 302c 3c31  llow (>=9.2.0,<1
-00000370: 302e 302e 3029 203b 2065 7874 7261 203d  0.0.0) ; extra =
-00000380: 3d20 2276 697a 2220 6f72 2065 7874 7261  = "viz" or extra
-00000390: 203d 3d20 2269 6d61 6765 2220 6f72 2065   == "image" or e
-000003a0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-000003b0: 7175 6972 6573 2d44 6973 743a 2062 6f74  quires-Dist: bot
-000003c0: 6f33 2028 3e3d 312e 3232 2e31 332c 3c32  o3 (>=1.22.13,<2
-000003d0: 2e30 2e30 2920 3b20 6578 7472 6120 3d3d  .0.0) ; extra ==
-000003e0: 2022 7333 2220 6f72 2065 7874 7261 203d   "s3" or extra =
-000003f0: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000400: 2d44 6973 743a 2066 6173 7465 722d 6669  -Dist: faster-fi
-00000410: 666f 2028 3e3d 312e 342e 352c 3c32 2e30  fo (>=1.4.5,<2.0
-00000420: 2e30 2920 3b20 6578 7472 6120 3d3d 2022  .0) ; extra == "
-00000430: 7072 6f63 2220 6f72 2065 7874 7261 203d  proc" or extra =
-00000440: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000450: 2d44 6973 743a 2066 7567 7565 2028 3e3d  -Dist: fugue (>=
-00000460: 302e 382e 312c 3c30 2e39 2e30 2920 3b20  0.8.1,<0.9.0) ; 
-00000470: 6578 7472 6120 3d3d 2022 6675 6775 6522  extra == "fugue"
-00000480: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000490: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-000004a0: 3a20 6675 726f 2028 3e3d 3230 3232 2e33  : furo (>=2022.3
-000004b0: 2e34 2c3c 3230 3233 2e30 2e30 2920 3b20  .4,<2023.0.0) ; 
-000004c0: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
-000004d0: 5265 7175 6972 6573 2d44 6973 743a 2067  Requires-Dist: g
-000004e0: 6f6f 676c 652d 636c 6f75 642d 7374 6f72  oogle-cloud-stor
-000004f0: 6167 6520 283e 3d32 2e35 2e30 2c3c 332e  age (>=2.5.0,<3.
-00000500: 302e 3029 203b 2065 7874 7261 203d 3d20  0.0) ; extra == 
-00000510: 2267 6373 2220 6f72 2065 7874 7261 203d  "gcs" or extra =
-00000520: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
-00000530: 2d44 6973 743a 2069 6d70 6f72 746c 6962  -Dist: importlib
-00000540: 2d6d 6574 6164 6174 6120 283c 342e 3329  -metadata (<4.3)
-00000550: 203b 2070 7974 686f 6e5f 7665 7273 696f   ; python_versio
-00000560: 6e20 3c20 2233 2e38 220a 5265 7175 6972  n < "3.8".Requir
-00000570: 6573 2d44 6973 743a 2069 7079 7468 6f6e  es-Dist: ipython
-00000580: 203b 2065 7874 7261 203d 3d20 2276 697a   ; extra == "viz
-00000590: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
-000005a0: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
-000005b0: 743a 2069 7079 7468 6f6e 5f67 656e 7574  t: ipython_genut
-000005c0: 696c 7320 283e 3d30 2e32 2e30 2c3c 302e  ils (>=0.2.0,<0.
-000005d0: 332e 3029 203b 2065 7874 7261 203d 3d20  3.0) ; extra == 
-000005e0: 2264 6f63 7322 0a52 6571 7569 7265 732d  "docs".Requires-
-000005f0: 4469 7374 3a20 6d6c 666c 6f77 2d73 6b69  Dist: mlflow-ski
-00000600: 6e6e 7920 283c 322e 302e 3129 203b 2028  nny (<2.0.1) ; (
-00000610: 7079 7468 6f6e 5f76 6572 7369 6f6e 203c  python_version <
-00000620: 2022 332e 3822 2920 616e 6420 2865 7874   "3.8") and (ext
-00000630: 7261 203d 3d20 226d 6c66 6c6f 7722 206f  ra == "mlflow" o
-00000640: 7220 6578 7472 6120 3d3d 2022 616c 6c22  r extra == "all"
-00000650: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000660: 206d 6c66 6c6f 772d 736b 696e 6e79 2028   mlflow-skinny (
-00000670: 3e3d 322e 352e 302c 3c33 2e30 2e30 2920  >=2.5.0,<3.0.0) 
-00000680: 3b20 2870 7974 686f 6e5f 7665 7273 696f  ; (python_versio
-00000690: 6e20 3e3d 2022 332e 3822 2920 616e 6420  n >= "3.8") and 
-000006a0: 2865 7874 7261 203d 3d20 226d 6c66 6c6f  (extra == "mlflo
-000006b0: 7722 206f 7220 6578 7472 6120 3d3d 2022  w" or extra == "
-000006c0: 616c 6c22 290a 5265 7175 6972 6573 2d44  all").Requires-D
-000006d0: 6973 743a 206d 7973 742d 7061 7273 6572  ist: myst-parser
-000006e0: 5b73 7068 696e 785d 2028 3e3d 302e 3137  [sphinx] (>=0.17
-000006f0: 2e32 2c3c 302e 3138 2e30 2920 3b20 6578  .2,<0.18.0) ; ex
-00000700: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
-00000710: 7175 6972 6573 2d44 6973 743a 206e 6263  quires-Dist: nbc
-00000720: 6f6e 7665 7274 2028 3e3d 372e 302e 302c  onvert (>=7.0.0,
-00000730: 3c38 2e30 2e30 2920 3b20 6578 7472 6120  <8.0.0) ; extra 
-00000740: 3d3d 2022 646f 6373 220a 5265 7175 6972  == "docs".Requir
-00000750: 6573 2d44 6973 743a 206e 6273 7068 696e  es-Dist: nbsphin
-00000760: 7820 283e 3d30 2e38 2e39 2c3c 302e 392e  x (>=0.8.9,<0.9.
-00000770: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
-00000780: 6f63 7322 0a52 6571 7569 7265 732d 4469  ocs".Requires-Di
-00000790: 7374 3a20 6e75 6d70 7920 283e 3d31 2e32  st: numpy (>=1.2
-000007a0: 332e 3229 203b 2028 7079 7468 6f6e 5f76  3.2) ; (python_v
-000007b0: 6572 7369 6f6e 203e 3d20 2233 2e31 3122  ersion >= "3.11"
-000007c0: 2920 616e 6420 2865 7874 7261 203d 3d20  ) and (extra == 
-000007d0: 2276 697a 2220 6f72 2065 7874 7261 203d  "viz" or extra =
-000007e0: 3d20 2269 6d61 6765 2220 6f72 2065 7874  = "image" or ext
-000007f0: 7261 203d 3d20 2265 6d62 6564 6469 6e67  ra == "embedding
-00000800: 7322 206f 7220 6578 7472 6120 3d3d 2022  s" or extra == "
-00000810: 616c 6c22 290a 5265 7175 6972 6573 2d44  all").Requires-D
-00000820: 6973 743a 206e 756d 7079 203b 2028 7079  ist: numpy ; (py
-00000830: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
-00000840: 332e 3131 2229 2061 6e64 2028 6578 7472  3.11") and (extr
-00000850: 6120 3d3d 2022 7669 7a22 206f 7220 6578  a == "viz" or ex
-00000860: 7472 6120 3d3d 2022 696d 6167 6522 206f  tra == "image" o
-00000870: 7220 6578 7472 6120 3d3d 2022 656d 6265  r extra == "embe
-00000880: 6464 696e 6773 2220 6f72 2065 7874 7261  ddings" or extra
-00000890: 203d 3d20 2261 6c6c 2229 0a52 6571 7569   == "all").Requi
-000008a0: 7265 732d 4469 7374 3a20 6f72 6a73 6f6e  res-Dist: orjson
-000008b0: 2028 3e3d 332e 382e 3130 2c3c 342e 302e   (>=3.8.10,<4.0.
-000008c0: 3029 203b 2065 7874 7261 203d 3d20 2270  0) ; extra == "p
-000008d0: 726f 6322 206f 7220 6578 7472 6120 3d3d  roc" or extra ==
-000008e0: 2022 7072 6f63 2d6d 7022 206f 7220 6578   "proc-mp" or ex
-000008f0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
-00000900: 7569 7265 732d 4469 7374 3a20 7061 6e64  uires-Dist: pand
-00000910: 6173 203b 2065 7874 7261 203d 3d20 2264  as ; extra == "d
-00000920: 6174 6173 6574 7322 206f 7220 6578 7472  atasets" or extr
-00000930: 6120 3d3d 2022 7072 6f63 2220 6f72 2065  a == "proc" or e
-00000940: 7874 7261 203d 3d20 2270 726f 632d 6d70  xtra == "proc-mp
-00000950: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
-00000960: 6c6c 220a 5265 7175 6972 6573 2d44 6973  ll".Requires-Dis
-00000970: 743a 2070 6c61 7466 6f72 6d64 6972 7320  t: platformdirs 
-00000980: 283e 3d33 2e35 2e30 2c3c 342e 302e 3029  (>=3.5.0,<4.0.0)
-00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009a0: 7072 6f74 6f62 7566 2028 3e3d 332e 3139  protobuf (>=3.19
-000009b0: 2e34 290a 5265 7175 6972 6573 2d44 6973  .4).Requires-Dis
-000009c0: 743a 2070 7961 7272 6f77 2028 3e3d 382e  t: pyarrow (>=8.
-000009d0: 302e 302c 3c31 3329 203b 2065 7874 7261  0.0,<13) ; extra
-000009e0: 203d 3d20 2273 7061 726b 2220 6f72 2065   == "spark" or e
-000009f0: 7874 7261 203d 3d20 2261 6c6c 220a 5265  xtra == "all".Re
-00000a00: 7175 6972 6573 2d44 6973 743a 2070 7962  quires-Dist: pyb
-00000a10: 6172 7333 2028 3e3d 302e 392c 3c30 2e31  ars3 (>=0.9,<0.1
-00000a20: 3029 203b 2065 7874 7261 203d 3d20 2276  0) ; extra == "v
-00000a30: 697a 2220 6f72 2065 7874 7261 203d 3d20  iz" or extra == 
-00000a40: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
-00000a50: 6973 743a 2070 7973 7061 726b 2028 3e3d  ist: pyspark (>=
-00000a60: 332e 302e 302c 3c34 2e30 2e30 2920 3b20  3.0.0,<4.0.0) ; 
-00000a70: 6578 7472 6120 3d3d 2022 7370 6172 6b22  extra == "spark"
-00000a80: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000a90: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
-00000aa0: 3a20 7265 7175 6573 7473 2028 3e3d 322e  : requests (>=2.
-00000ab0: 3237 2c3c 332e 3029 0a52 6571 7569 7265  27,<3.0).Require
-00000ac0: 732d 4469 7374 3a20 7363 696b 6974 2d6c  s-Dist: scikit-l
-00000ad0: 6561 726e 2028 3e3d 312e 302e 322c 3c32  earn (>=1.0.2,<2
-00000ae0: 2e30 2e30 2920 3b20 2870 7974 686f 6e5f  .0.0) ; (python_
-00000af0: 7665 7273 696f 6e20 3c20 2233 2e31 3122  version < "3.11"
-00000b00: 2920 616e 6420 2865 7874 7261 203d 3d20  ) and (extra == 
-00000b10: 2265 6d62 6564 6469 6e67 7322 206f 7220  "embeddings" or 
-00000b20: 6578 7472 6120 3d3d 2022 616c 6c22 290a  extra == "all").
-00000b30: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
-00000b40: 6369 6b69 742d 6c65 6172 6e20 283e 3d31  cikit-learn (>=1
-00000b50: 2e31 2e32 2c3c 3229 203b 2028 7079 7468  .1.2,<2) ; (pyth
-00000b60: 6f6e 5f76 6572 7369 6f6e 203e 3d20 2233  on_version >= "3
-00000b70: 2e31 3122 2920 616e 6420 2865 7874 7261  .11") and (extra
-00000b80: 203d 3d20 2265 6d62 6564 6469 6e67 7322   == "embeddings"
-00000b90: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000ba0: 6c22 290a 5265 7175 6972 6573 2d44 6973  l").Requires-Dis
-00000bb0: 743a 2073 6369 7079 2028 3e3d 312e 3529  t: scipy (>=1.5)
-00000bc0: 203b 2028 7079 7468 6f6e 5f76 6572 7369   ; (python_versi
-00000bd0: 6f6e 203c 2022 332e 3131 2229 2061 6e64  on < "3.11") and
-00000be0: 2028 6578 7472 6120 3d3d 2022 7669 7a22   (extra == "viz"
-00000bf0: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
-00000c00: 6c22 290a 5265 7175 6972 6573 2d44 6973  l").Requires-Dis
-00000c10: 743a 2073 6369 7079 2028 3e3d 312e 392e  t: scipy (>=1.9.
-00000c20: 3229 203b 2028 7079 7468 6f6e 5f76 6572  2) ; (python_ver
-00000c30: 7369 6f6e 203e 3d20 2233 2e31 3122 2920  sion >= "3.11") 
-00000c40: 616e 6420 2865 7874 7261 203d 3d20 2276  and (extra == "v
-00000c50: 697a 2220 6f72 2065 7874 7261 203d 3d20  iz" or extra == 
-00000c60: 2261 6c6c 2229 0a52 6571 7569 7265 732d  "all").Requires-
-00000c70: 4469 7374 3a20 7370 6869 6e78 203b 2065  Dist: sphinx ; e
-00000c80: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000c90: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000ca0: 6869 6e78 2d61 7574 6f61 7069 203b 2065  hinx-autoapi ; e
-00000cb0: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000cc0: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
-00000cd0: 6869 6e78 2d61 7574 6f62 7569 6c64 2028  hinx-autobuild (
-00000ce0: 3e3d 3230 3231 2e33 2e31 342c 3c32 3032  >=2021.3.14,<202
-00000cf0: 322e 302e 3029 203b 2065 7874 7261 203d  2.0.0) ; extra =
-00000d00: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
-00000d10: 732d 4469 7374 3a20 7370 6869 6e78 2d63  s-Dist: sphinx-c
-00000d20: 6f70 7962 7574 746f 6e20 283e 3d30 2e35  opybutton (>=0.5
-00000d30: 2e30 2c3c 302e 362e 3029 203b 2065 7874  .0,<0.6.0) ; ext
-00000d40: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
-00000d50: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
-00000d60: 6e78 2d69 6e6c 696e 652d 7461 6273 203b  nx-inline-tabs ;
-00000d70: 2028 7079 7468 6f6e 5f76 6572 7369 6f6e   (python_version
-00000d80: 203e 3d20 2233 2e38 2220 616e 6420 7079   >= "3.8" and py
-00000d90: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
-00000da0: 3422 2920 616e 6420 2865 7874 7261 203d  4") and (extra =
-00000db0: 3d20 2264 6f63 7322 290a 5265 7175 6972  = "docs").Requir
-00000dc0: 6573 2d44 6973 743a 2073 7068 696e 7865  es-Dist: sphinxe
-00000dd0: 7874 2d6f 7065 6e67 7261 7068 2028 3e3d  xt-opengraph (>=
-00000de0: 302e 362e 332c 3c30 2e37 2e30 2920 3b20  0.6.3,<0.7.0) ; 
-00000df0: 6578 7472 6120 3d3d 2022 646f 6373 220a  extra == "docs".
-00000e00: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000e10: 7970 6573 2d72 6571 7565 7374 7320 283e  ypes-requests (>
-00000e20: 3d32 2e33 302e 302e 302c 3c33 2e30 2e30  =2.30.0.0,<3.0.0
-00000e30: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000e40: 743a 2074 7970 696e 672d 6578 7465 6e73  t: typing-extens
-00000e50: 696f 6e73 2028 3e3d 332e 3130 2920 3b20  ions (>=3.10) ; 
-00000e60: 7079 7468 6f6e 5f76 6572 7369 6f6e 203c  python_version <
-00000e70: 2022 3422 0a52 6571 7569 7265 732d 4469   "4".Requires-Di
-00000e80: 7374 3a20 7768 796c 6162 732d 636c 6965  st: whylabs-clie
-00000e90: 6e74 2028 3e3d 302e 352e 362c 3c30 2e36  nt (>=0.5.6,<0.6
-00000ea0: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000eb0: 743a 2077 6879 6c6f 6773 2d73 6b65 7463  t: whylogs-sketc
-00000ec0: 6869 6e67 2028 3e3d 332e 342e 312e 6465  hing (>=3.4.1.de
-00000ed0: 7633 290a 4465 7363 7269 7074 696f 6e2d  v3).Description-
-00000ee0: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000ef0: 7874 2f6d 6172 6b64 6f77 6e0a 0a3c 696d  xt/markdown..<im
-00000f00: 6720 7372 633d 2268 7474 7073 3a2f 2f73  g src="https://s
-00000f10: 7461 7469 632e 7363 6172 662e 7368 2f61  tatic.scarf.sh/a
-00000f20: 2e70 6e67 3f78 2d70 7869 643d 6263 3363  .png?x-pxid=bc3c
-00000f30: 3537 6230 2d39 6136 352d 3439 6665 2d62  57b0-9a65-49fe-b
-00000f40: 3865 612d 6637 3131 6334 6433 3562 3832  8ea-f711c4d35b82
-00000f50: 2220 2f3e 3c70 2061 6c69 676e 3d22 6365  " /><p align="ce
-00000f60: 6e74 6572 223e 0a3c 696d 6720 7372 633d  nter">.<img src=
-00000f70: 2268 7474 7073 3a2f 2f69 2e69 6d67 7572  "https://i.imgur
-00000f80: 2e63 6f6d 2f6e 7633 3367 6f56 2e70 6e67  .com/nv33goV.png
-00000f90: 2220 7769 6474 683d 2233 3525 222f 3e0a  " width="35%"/>.
-00000fa0: 3c2f 6272 3e0a 0a3c 6831 2061 6c69 676e  </br>..<h1 align
-00000fb0: 3d22 6365 6e74 6572 223e 5468 6520 6f70  ="center">The op
-00000fc0: 656e 2073 7461 6e64 6172 6420 666f 7220  en standard for 
-00000fd0: 6461 7461 206c 6f67 6769 6e67 0a0a 203c  data logging.. <
-00000fe0: 2f68 313e 0a20 203c 6833 2061 6c69 676e  /h1>.  <h3 align
-00000ff0: 3d22 6365 6e74 6572 223e 0a20 2020 3c61  ="center">.   <a
-00001000: 2068 7265 663d 2268 7474 7073 3a2f 2f77   href="https://w
-00001010: 6879 6c6f 6773 2e72 6561 6474 6865 646f  hylogs.readthedo
-00001020: 6373 2e69 6f2f 223e 3c62 3e44 6f63 756d  cs.io/"><b>Docum
-00001030: 656e 7461 7469 6f6e 3c2f 623e 3c2f 613e  entation</b></a>
-00001040: 2026 6275 6c6c 3b0a 2020 203c 6120 6872   &bull;.   <a hr
-00001050: 6566 3d22 6874 7470 733a 2f2f 6269 742e  ef="https://bit.
-00001060: 6c79 2f77 6879 6c6f 6773 736c 6163 6b22  ly/whylogsslack"
-00001070: 3e3c 623e 536c 6163 6b20 436f 6d6d 756e  ><b>Slack Commun
-00001080: 6974 793c 2f62 3e3c 2f61 3e20 2662 756c  ity</b></a> &bul
-00001090: 6c3b 0a20 2020 3c61 2068 7265 663d 2268  l;.   <a href="h
-000010a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000010b0: 6d2f 7768 796c 6162 732f 7768 796c 6f67  m/whylabs/whylog
-000010c0: 7323 7079 7468 6f6e 2d71 7569 636b 7374  s#python-quickst
-000010d0: 6172 7422 3e3c 623e 5079 7468 6f6e 2051  art"><b>Python Q
-000010e0: 7569 636b 7374 6172 743c 2f62 3e3c 2f61  uickstart</b></a
-000010f0: 3e20 2662 756c 6c3b 0a20 2020 3c61 2068  > &bull;.   <a h
-00001100: 7265 663d 2268 7474 7073 3a2f 2f77 6879  ref="https://why
-00001110: 6c6f 6773 2e72 6561 6474 6865 646f 6373  logs.readthedocs
-00001120: 2e69 6f2f 656e 2f6c 6174 6573 742f 6578  .io/en/latest/ex
-00001130: 616d 706c 6573 2f69 6e74 6567 7261 7469  amples/integrati
-00001140: 6f6e 732f 7772 6974 6572 732f 5772 6974  ons/writers/Writ
-00001150: 696e 675f 746f 5f57 6879 4c61 6273 2e68  ing_to_WhyLabs.h
-00001160: 746d 6c22 3e3c 623e 5768 794c 6162 7320  tml"><b>WhyLabs 
-00001170: 5175 6963 6b73 7461 7274 3c2f 623e 3c2f  Quickstart</b></
-00001180: 613e 0a20 3c2f 6833 3e0a 0a3c 7020 616c  a>. </h3>..<p al
-00001190: 6967 6e3d 2263 656e 7465 7222 3e0a 3c61  ign="center">.<a
-000011a0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
-000011b0: 6974 6875 622e 636f 6d2f 7768 796c 6162  ithub.com/whylab
-000011c0: 732f 7768 796c 6f67 732d 7079 7468 6f6e  s/whylogs-python
-000011d0: 2f62 6c6f 622f 6d61 696e 6c69 6e65 2f4c  /blob/mainline/L
-000011e0: 4943 454e 5345 2220 7461 7267 6574 3d22  ICENSE" target="
-000011f0: 5f62 6c61 6e6b 223e 0a20 2020 203c 696d  _blank">.    <im
-00001200: 6720 7372 633d 2268 7474 703a 2f2f 696d  g src="http://im
-00001210: 672e 7368 6965 6c64 732e 696f 2f3a 6c69  g.shields.io/:li
-00001220: 6365 6e73 652d 4170 6163 6865 2532 3032  cense-Apache%202
-00001230: 2d62 6c75 652e 7376 6722 2061 6c74 3d22  -blue.svg" alt="
-00001240: 4c69 6365 6e73 6522 3e0a 3c2f 613e 0a3c  License">.</a>.<
-00001250: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001260: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-00001270: 2f77 6879 6c6f 6773 2220 7461 7267 6574  /whylogs" target
-00001280: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
-00001290: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000012a0: 2f62 6164 6765 2e66 7572 792e 696f 2f70  /badge.fury.io/p
-000012b0: 792f 7768 796c 6f67 732e 7376 6722 2061  y/whylogs.svg" a
-000012c0: 6c74 3d22 5079 5069 2056 6572 7369 6f6e  lt="PyPi Version
-000012d0: 223e 0a3c 2f61 3e0a 3c61 2068 7265 663d  ">.</a>.<a href=
-000012e0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000012f0: 636f 6d2f 7079 7468 6f6e 2f62 6c61 636b  com/python/black
-00001300: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
-00001310: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
-00001320: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00001330: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-00001340: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-00001350: 2d30 3030 3030 302e 7376 6722 2061 6c74  -000000.svg" alt
-00001360: 3d22 436f 6465 2073 7479 6c65 3a20 626c  ="Code style: bl
-00001370: 6163 6b22 3e0a 3c2f 613e 0a3c 6120 6872  ack">.</a>.<a hr
-00001380: 6566 3d22 6874 7470 733a 2f2f 7065 7079  ef="https://pepy
-00001390: 2e74 6563 682f 7072 6f6a 6563 742f 7768  .tech/project/wh
-000013a0: 796c 6f67 7322 2074 6172 6765 743d 225f  ylogs" target="_
-000013b0: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-000013c0: 2073 7263 3d22 6874 7470 733a 2f2f 7065   src="https://pe
-000013d0: 7079 2e74 6563 682f 6261 6467 652f 7768  py.tech/badge/wh
-000013e0: 796c 6f67 7322 2061 6c74 3d22 5079 5069  ylogs" alt="PyPi
-000013f0: 2044 6f77 6e6c 6f61 6473 223e 0a3c 2f61   Downloads">.</a
-00001400: 3e0a 3c61 2068 7265 663d 2262 6974 2e6c  >.<a href="bit.l
-00001410: 792f 7768 796c 6f67 7322 2074 6172 6765  y/whylogs" targe
-00001420: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
-00001430: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00001440: 2f2f 6769 7468 7562 2e63 6f6d 2f77 6879  //github.com/why
-00001450: 6c61 6273 2f77 6879 6c6f 6773 2d70 7974  labs/whylogs-pyt
-00001460: 686f 6e2f 776f 726b 666c 6f77 732f 7768  hon/workflows/wh
-00001470: 796c 6f67 7325 3230 4349 2f62 6164 6765  ylogs%20CI/badge
-00001480: 2e73 7667 2220 616c 743d 2243 4922 3e0a  .svg" alt="CI">.
-00001490: 3c2f 613e 0a3c 6120 6872 6566 3d22 6874  </a>.<a href="ht
-000014a0: 7470 733a 2f2f 636f 6465 636c 696d 6174  tps://codeclimat
-000014b0: 652e 636f 6d2f 6769 7468 7562 2f77 6879  e.com/github/why
-000014c0: 6c61 6273 2f77 6879 6c6f 6773 2d70 7974  labs/whylogs-pyt
-000014d0: 686f 6e2f 6d61 696e 7461 696e 6162 696c  hon/maintainabil
-000014e0: 6974 7922 2074 6172 6765 743d 225f 626c  ity" target="_bl
-000014f0: 616e 6b22 3e0a 2020 2020 3c69 6d67 2073  ank">.    <img s
-00001500: 7263 3d22 6874 7470 733a 2f2f 6170 692e  rc="https://api.
-00001510: 636f 6465 636c 696d 6174 652e 636f 6d2f  codeclimate.com/
-00001520: 7631 2f62 6164 6765 732f 3434 3266 3663  v1/badges/442f6c
-00001530: 6133 6463 6131 6535 3833 6134 3838 2f6d  a3dca1e583a488/m
-00001540: 6169 6e74 6169 6e61 6269 6c69 7479 2220  aintainability" 
-00001550: 616c 743d 224d 6169 6e74 6169 6e61 6269  alt="Maintainabi
-00001560: 6c69 7479 223e 0a3c 2f61 3e0a 3c2f 703e  lity">.</a>.</p>
-00001570: 0a0a 2323 2057 6861 7420 6973 2077 6879  ..## What is why
-00001580: 6c6f 6773 0a0a 7768 796c 6f67 7320 6973  logs..whylogs is
-00001590: 2061 6e20 6f70 656e 2073 6f75 7263 6520   an open source 
-000015a0: 6c69 6272 6172 7920 666f 7220 6c6f 6767  library for logg
-000015b0: 696e 6720 616e 7920 6b69 6e64 206f 6620  ing any kind of 
-000015c0: 6461 7461 2e20 5769 7468 2077 6879 6c6f  data. With whylo
-000015d0: 6773 2c20 7573 6572 7320 6172 6520 6162  gs, users are ab
-000015e0: 6c65 2074 6f20 6765 6e65 7261 7465 2073  le to generate s
-000015f0: 756d 6d61 7269 6573 206f 6620 7468 6569  ummaries of thei
-00001600: 7220 6461 7461 7365 7473 2028 6361 6c6c  r datasets (call
-00001610: 6564 205f 7768 796c 6f67 7320 7072 6f66  ed _whylogs prof
-00001620: 696c 6573 5f29 2077 6869 6368 2074 6865  iles_) which the
-00001630: 7920 6361 6e20 7573 6520 746f 3a0a 0a31  y can use to:..1
-00001640: 2e20 5472 6163 6b20 6368 616e 6765 7320  . Track changes 
-00001650: 696e 2074 6865 6972 2064 6174 6173 6574  in their dataset
-00001660: 0a32 2e20 4372 6561 7465 205f 6461 7461  .2. Create _data
-00001670: 2063 6f6e 7374 7261 696e 7473 5f20 746f   constraints_ to
-00001680: 206b 6e6f 7720 7768 6574 6865 7220 7468   know whether th
-00001690: 6569 7220 6461 7461 206c 6f6f 6b73 2074  eir data looks t
-000016a0: 6865 2077 6179 2069 7420 7368 6f75 6c64  he way it should
-000016b0: 0a33 2e20 5175 6963 6b6c 7920 7669 7375  .3. Quickly visu
-000016c0: 616c 697a 6520 6b65 7920 7375 6d6d 6172  alize key summar
-000016d0: 7920 7374 6174 6973 7469 6373 2061 626f  y statistics abo
-000016e0: 7574 2074 6865 6972 2064 6174 6173 6574  ut their dataset
-000016f0: 730a 0a54 6865 7365 2074 6872 6565 2066  s..These three f
-00001700: 756e 6374 696f 6e61 6c69 7469 6573 2065  unctionalities e
-00001710: 6e61 626c 6520 6120 7661 7269 6574 7920  nable a variety 
-00001720: 6f66 2075 7365 2063 6173 6573 2066 6f72  of use cases for
-00001730: 2064 6174 6120 7363 6965 6e74 6973 7473   data scientists
-00001740: 2c20 6d61 6368 696e 6520 6c65 6172 6e69  , machine learni
-00001750: 6e67 2065 6e67 696e 6565 7273 2c20 616e  ng engineers, an
-00001760: 6420 6461 7461 2065 6e67 696e 6565 7273  d data engineers
-00001770: 3a0a 0a2d 2044 6574 6563 7420 6461 7461  :..- Detect data
-00001780: 2064 7269 6674 2069 6e20 6d6f 6465 6c20   drift in model 
-00001790: 696e 7075 7420 6665 6174 7572 6573 0a2d  input features.-
-000017a0: 2044 6574 6563 7420 7472 6169 6e69 6e67   Detect training
-000017b0: 2d73 6572 7669 6e67 2073 6b65 772c 2063  -serving skew, c
-000017c0: 6f6e 6365 7074 2064 7269 6674 2c20 616e  oncept drift, an
-000017d0: 6420 6d6f 6465 6c20 7065 7266 6f72 6d61  d model performa
-000017e0: 6e63 6520 6465 6772 6164 6174 696f 6e0a  nce degradation.
-000017f0: 2d20 5661 6c69 6461 7465 2064 6174 6120  - Validate data 
-00001800: 7175 616c 6974 7920 696e 206d 6f64 656c  quality in model
-00001810: 2069 6e70 7574 7320 6f72 2069 6e20 6120   inputs or in a 
-00001820: 6461 7461 2070 6970 656c 696e 650a 2d20  data pipeline.- 
-00001830: 5065 7266 6f72 6d20 6578 706c 6f72 6174  Perform explorat
-00001840: 6f72 7920 6461 7461 2061 6e61 6c79 7369  ory data analysi
-00001850: 7320 6f66 206d 6173 7369 7665 2064 6174  s of massive dat
-00001860: 6173 6574 730a 2d20 5472 6163 6b20 6461  asets.- Track da
-00001870: 7461 2064 6973 7472 6962 7574 696f 6e73  ta distributions
-00001880: 2026 2064 6174 6120 7175 616c 6974 7920   & data quality 
-00001890: 666f 7220 4d4c 2065 7870 6572 696d 656e  for ML experimen
-000018a0: 7473 0a2d 2045 6e61 626c 6520 6461 7461  ts.- Enable data
-000018b0: 2061 7564 6974 696e 6720 616e 6420 676f   auditing and go
-000018c0: 7665 726e 616e 6365 2061 6372 6f73 7320  vernance across 
-000018d0: 7468 6520 6f72 6761 6e69 7a61 7469 6f6e  the organization
-000018e0: 0a2d 2053 7461 6e64 6172 6469 7a65 2064  .- Standardize d
-000018f0: 6174 6120 646f 6375 6d65 6e74 6174 696f  ata documentatio
-00001900: 6e20 7072 6163 7469 6365 7320 6163 726f  n practices acro
-00001910: 7373 2074 6865 206f 7267 616e 697a 6174  ss the organizat
-00001920: 696f 6e0a 2d20 416e 6420 6d6f 7265 0a0a  ion.- And more..
-00001930: 2323 2051 7569 636b 7374 6172 740a 0a49  ## Quickstart..I
-00001940: 6e73 7461 6c6c 2077 6879 6c6f 6773 2075  nstall whylogs u
-00001950: 7369 6e67 2074 6865 2070 6970 2070 6163  sing the pip pac
-00001960: 6b61 6765 206d 616e 6167 6572 2069 6e20  kage manager in 
-00001970: 6120 7465 726d 696e 616c 2062 7920 7275  a terminal by ru
-00001980: 6e6e 696e 673a 0a0a 6060 600a 7069 7020  nning:..```.pip 
-00001990: 696e 7374 616c 6c20 7768 796c 6f67 730a  install whylogs.
-000019a0: 6060 600a 0a54 6865 6e20 796f 7520 6361  ```..Then you ca
-000019b0: 6e20 6c6f 6720 6461 7461 2069 6e20 7079  n log data in py
-000019c0: 7468 6f6e 2061 7320 7369 6d70 6c79 2061  thon as simply a
-000019d0: 7320 7468 6973 3a0a 0a60 6060 7079 7468  s this:..```pyth
-000019e0: 6f6e 0a69 6d70 6f72 7420 7768 796c 6f67  on.import whylog
-000019f0: 7320 6173 2077 6879 0a69 6d70 6f72 7420  s as why.import 
-00001a00: 7061 6e64 6173 2061 7320 7064 0a0a 6466  pandas as pd..df
-00001a10: 203d 2070 642e 7265 6164 5f63 7376 2822   = pd.read_csv("
-00001a20: 7061 7468 2f74 6f2f 6669 6c65 2e63 7376  path/to/file.csv
-00001a30: 2229 0a72 6573 756c 7473 203d 2077 6879  ").results = why
-00001a40: 2e6c 6f67 2864 6629 0a60 6060 0a0a 416e  .log(df).```..An
-00001a50: 6420 766f 696c c3a0 2c20 796f 7520 6e6f  d voil.., you no
-00001a60: 7720 6861 7665 2061 2077 6879 6c6f 6773  w have a whylogs
-00001a70: 2070 726f 6669 6c65 2e20 546f 206c 6561   profile. To lea
-00001a80: 726e 206d 6f72 6520 6162 6f75 7420 7768  rn more about wh
-00001a90: 6174 2061 2077 6879 6c6f 6773 2070 726f  at a whylogs pro
-00001aa0: 6669 6c65 2069 7320 616e 6420 7768 6174  file is and what
-00001ab0: 2079 6f75 2063 616e 2064 6f20 7769 7468   you can do with
-00001ac0: 2069 742c 2063 6865 636b 206f 7574 206f   it, check out o
-00001ad0: 7572 205b 646f 6373 5d28 6874 7470 733a  ur [docs](https:
-00001ae0: 2f2f 7768 796c 6f67 732e 7265 6164 7468  //whylogs.readth
-00001af0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00001b00: 7374 2f29 2061 6e64 206f 7572 205b 6578  st/) and our [ex
-00001b10: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
-00001b20: 6769 7468 7562 2e63 6f6d 2f77 6879 6c61  github.com/whyla
-00001b30: 6273 2f77 6879 6c6f 6773 2f74 7265 652f  bs/whylogs/tree/
-00001b40: 6d61 696e 6c69 6e65 2f70 7974 686f 6e2f  mainline/python/
-00001b50: 6578 616d 706c 6573 292e 0a0a            examples)...
+00000030: 2e39 2e64 6576 300a 5375 6d6d 6172 793a  .9.dev0.Summary:
+00000040: 2050 726f 6669 6c65 2061 6e64 206d 6f6e   Profile and mon
+00000050: 6974 6f72 2079 6f75 7220 4d4c 2064 6174  itor your ML dat
+00000060: 6120 7069 7065 6c69 6e65 2065 6e64 2d74  a pipeline end-t
+00000070: 6f2d 656e 640a 486f 6d65 2d70 6167 653a  o-end.Home-page:
+00000080: 2068 7474 7073 3a2f 2f64 6f63 732e 7768   https://docs.wh
+00000090: 796c 6162 732e 6169 0a4c 6963 656e 7365  ylabs.ai.License
+000000a0: 3a20 4170 6163 6865 2d32 2e30 0a41 7574  : Apache-2.0.Aut
+000000b0: 686f 723a 2057 6879 4c61 6273 2e61 690a  hor: WhyLabs.ai.
+000000c0: 4175 7468 6f72 2d65 6d61 696c 3a20 7375  Author-email: su
+000000d0: 7070 6f72 7440 7768 796c 6162 732e 6169  pport@whylabs.ai
+000000e0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
+000000f0: 3a20 3e3d 332e 372e 312c 3c34 0a43 6c61  : >=3.7.1,<4.Cla
+00000100: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00000110: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000120: 203a 3a20 4170 6163 6865 2053 6f66 7477   :: Apache Softw
+00000130: 6172 6520 4c69 6365 6e73 650a 436c 6173  are License.Clas
+00000140: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000150: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000160: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
+00000170: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000190: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+000001a0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000001b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001c0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+000001d0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000001e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000001f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000200: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000210: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000220: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000230: 2033 2e31 310a 5072 6f76 6964 6573 2d45   3.11.Provides-E
+00000240: 7874 7261 3a20 616c 6c0a 5072 6f76 6964  xtra: all.Provid
+00000250: 6573 2d45 7874 7261 3a20 6461 7461 7365  es-Extra: datase
+00000260: 7473 0a50 726f 7669 6465 732d 4578 7472  ts.Provides-Extr
+00000270: 613a 2064 6f63 730a 5072 6f76 6964 6573  a: docs.Provides
+00000280: 2d45 7874 7261 3a20 656d 6265 6464 696e  -Extra: embeddin
+00000290: 6773 0a50 726f 7669 6465 732d 4578 7472  gs.Provides-Extr
+000002a0: 613a 2066 7567 7565 0a50 726f 7669 6465  a: fugue.Provide
+000002b0: 732d 4578 7472 613a 2067 6373 0a50 726f  s-Extra: gcs.Pro
+000002c0: 7669 6465 732d 4578 7472 613a 2069 6d61  vides-Extra: ima
+000002d0: 6765 0a50 726f 7669 6465 732d 4578 7472  ge.Provides-Extr
+000002e0: 613a 206d 6c66 6c6f 770a 5072 6f76 6964  a: mlflow.Provid
+000002f0: 6573 2d45 7874 7261 3a20 7072 6f63 0a50  es-Extra: proc.P
+00000300: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
+00000310: 726f 632d 6d70 0a50 726f 7669 6465 732d  roc-mp.Provides-
+00000320: 4578 7472 613a 2073 330a 5072 6f76 6964  Extra: s3.Provid
+00000330: 6573 2d45 7874 7261 3a20 7370 6172 6b0a  es-Extra: spark.
+00000340: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000350: 7669 7a0a 5265 7175 6972 6573 2d44 6973  viz.Requires-Dis
+00000360: 743a 2050 696c 6c6f 7720 283e 3d39 2e32  t: Pillow (>=9.2
+00000370: 2e30 2c3c 3130 2e30 2e30 2920 3b20 6578  .0,<10.0.0) ; ex
+00000380: 7472 6120 3d3d 2022 7669 7a22 206f 7220  tra == "viz" or 
+00000390: 6578 7472 6120 3d3d 2022 696d 6167 6522  extra == "image"
+000003a0: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
+000003b0: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+000003c0: 3a20 626f 746f 3320 283e 3d31 2e32 322e  : boto3 (>=1.22.
+000003d0: 3133 2c3c 322e 302e 3029 203b 2065 7874  13,<2.0.0) ; ext
+000003e0: 7261 203d 3d20 2273 3322 206f 7220 6578  ra == "s3" or ex
+000003f0: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
+00000400: 7569 7265 732d 4469 7374 3a20 6661 7374  uires-Dist: fast
+00000410: 6572 2d66 6966 6f20 283e 3d31 2e34 2e35  er-fifo (>=1.4.5
+00000420: 2c3c 322e 302e 3029 203b 2065 7874 7261  ,<2.0.0) ; extra
+00000430: 203d 3d20 2270 726f 6322 206f 7220 6578   == "proc" or ex
+00000440: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
+00000450: 7569 7265 732d 4469 7374 3a20 6675 6775  uires-Dist: fugu
+00000460: 6520 283e 3d30 2e38 2e31 2c3c 302e 392e  e (>=0.8.1,<0.9.
+00000470: 3029 203b 2065 7874 7261 203d 3d20 2266  0) ; extra == "f
+00000480: 7567 7565 2220 6f72 2065 7874 7261 203d  ugue" or extra =
+00000490: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
+000004a0: 2d44 6973 743a 2066 7572 6f20 283e 3d32  -Dist: furo (>=2
+000004b0: 3032 322e 332e 342c 3c32 3032 332e 302e  022.3.4,<2023.0.
+000004c0: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+000004d0: 6f63 7322 0a52 6571 7569 7265 732d 4469  ocs".Requires-Di
+000004e0: 7374 3a20 676f 6f67 6c65 2d63 6c6f 7564  st: google-cloud
+000004f0: 2d73 746f 7261 6765 2028 3e3d 322e 352e  -storage (>=2.5.
+00000500: 302c 3c33 2e30 2e30 2920 3b20 6578 7472  0,<3.0.0) ; extr
+00000510: 6120 3d3d 2022 6763 7322 206f 7220 6578  a == "gcs" or ex
+00000520: 7472 6120 3d3d 2022 616c 6c22 0a52 6571  tra == "all".Req
+00000530: 7569 7265 732d 4469 7374 3a20 696d 706f  uires-Dist: impo
+00000540: 7274 6c69 622d 6d65 7461 6461 7461 2028  rtlib-metadata (
+00000550: 3c34 2e33 2920 3b20 7079 7468 6f6e 5f76  <4.3) ; python_v
+00000560: 6572 7369 6f6e 203c 2022 332e 3822 0a52  ersion < "3.8".R
+00000570: 6571 7569 7265 732d 4469 7374 3a20 6970  equires-Dist: ip
+00000580: 7974 686f 6e20 3b20 6578 7472 6120 3d3d  ython ; extra ==
+00000590: 2022 7669 7a22 206f 7220 6578 7472 6120   "viz" or extra 
+000005a0: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
+000005b0: 732d 4469 7374 3a20 6970 7974 686f 6e5f  s-Dist: ipython_
+000005c0: 6765 6e75 7469 6c73 2028 3e3d 302e 322e  genutils (>=0.2.
+000005d0: 302c 3c30 2e33 2e30 2920 3b20 6578 7472  0,<0.3.0) ; extr
+000005e0: 6120 3d3d 2022 646f 6373 220a 5265 7175  a == "docs".Requ
+000005f0: 6972 6573 2d44 6973 743a 206d 6c66 6c6f  ires-Dist: mlflo
+00000600: 772d 736b 696e 6e79 2028 3c32 2e30 2e31  w-skinny (<2.0.1
+00000610: 2920 3b20 2870 7974 686f 6e5f 7665 7273  ) ; (python_vers
+00000620: 696f 6e20 3c20 2233 2e38 2229 2061 6e64  ion < "3.8") and
+00000630: 2028 6578 7472 6120 3d3d 2022 6d6c 666c   (extra == "mlfl
+00000640: 6f77 2220 6f72 2065 7874 7261 203d 3d20  ow" or extra == 
+00000650: 2261 6c6c 2229 0a52 6571 7569 7265 732d  "all").Requires-
+00000660: 4469 7374 3a20 6d6c 666c 6f77 2d73 6b69  Dist: mlflow-ski
+00000670: 6e6e 7920 283e 3d32 2e35 2e30 2c3c 332e  nny (>=2.5.0,<3.
+00000680: 302e 3029 203b 2028 7079 7468 6f6e 5f76  0.0) ; (python_v
+00000690: 6572 7369 6f6e 203e 3d20 2233 2e38 2229  ersion >= "3.8")
+000006a0: 2061 6e64 2028 6578 7472 6120 3d3d 2022   and (extra == "
+000006b0: 6d6c 666c 6f77 2220 6f72 2065 7874 7261  mlflow" or extra
+000006c0: 203d 3d20 2261 6c6c 2229 0a52 6571 7569   == "all").Requi
+000006d0: 7265 732d 4469 7374 3a20 6d79 7374 2d70  res-Dist: myst-p
+000006e0: 6172 7365 725b 7370 6869 6e78 5d20 283e  arser[sphinx] (>
+000006f0: 3d30 2e31 372e 322c 3c30 2e31 382e 3029  =0.17.2,<0.18.0)
+00000700: 203b 2065 7874 7261 203d 3d20 2264 6f63   ; extra == "doc
+00000710: 7322 0a52 6571 7569 7265 732d 4469 7374  s".Requires-Dist
+00000720: 3a20 6e62 636f 6e76 6572 7420 283e 3d37  : nbconvert (>=7
+00000730: 2e30 2e30 2c3c 382e 302e 3029 203b 2065  .0.0,<8.0.0) ; e
+00000740: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
+00000750: 6571 7569 7265 732d 4469 7374 3a20 6e62  equires-Dist: nb
+00000760: 7370 6869 6e78 2028 3e3d 302e 382e 392c  sphinx (>=0.8.9,
+00000770: 3c30 2e39 2e30 2920 3b20 6578 7472 6120  <0.9.0) ; extra 
+00000780: 3d3d 2022 646f 6373 220a 5265 7175 6972  == "docs".Requir
+00000790: 6573 2d44 6973 743a 206e 756d 7079 2028  es-Dist: numpy (
+000007a0: 3e3d 312e 3233 2e32 2920 3b20 2870 7974  >=1.23.2) ; (pyt
+000007b0: 686f 6e5f 7665 7273 696f 6e20 3e3d 2022  hon_version >= "
+000007c0: 332e 3131 2229 2061 6e64 2028 6578 7472  3.11") and (extr
+000007d0: 6120 3d3d 2022 7669 7a22 206f 7220 6578  a == "viz" or ex
+000007e0: 7472 6120 3d3d 2022 696d 6167 6522 206f  tra == "image" o
+000007f0: 7220 6578 7472 6120 3d3d 2022 656d 6265  r extra == "embe
+00000800: 6464 696e 6773 2220 6f72 2065 7874 7261  ddings" or extra
+00000810: 203d 3d20 2261 6c6c 2229 0a52 6571 7569   == "all").Requi
+00000820: 7265 732d 4469 7374 3a20 6e75 6d70 7920  res-Dist: numpy 
+00000830: 3b20 2870 7974 686f 6e5f 7665 7273 696f  ; (python_versio
+00000840: 6e20 3c20 2233 2e31 3122 2920 616e 6420  n < "3.11") and 
+00000850: 2865 7874 7261 203d 3d20 2276 697a 2220  (extra == "viz" 
+00000860: 6f72 2065 7874 7261 203d 3d20 2269 6d61  or extra == "ima
+00000870: 6765 2220 6f72 2065 7874 7261 203d 3d20  ge" or extra == 
+00000880: 2265 6d62 6564 6469 6e67 7322 206f 7220  "embeddings" or 
+00000890: 6578 7472 6120 3d3d 2022 616c 6c22 290a  extra == "all").
+000008a0: 5265 7175 6972 6573 2d44 6973 743a 206f  Requires-Dist: o
+000008b0: 726a 736f 6e20 283e 3d33 2e38 2e31 302c  rjson (>=3.8.10,
+000008c0: 3c34 2e30 2e30 2920 3b20 6578 7472 6120  <4.0.0) ; extra 
+000008d0: 3d3d 2022 7072 6f63 2220 6f72 2065 7874  == "proc" or ext
+000008e0: 7261 203d 3d20 2270 726f 632d 6d70 2220  ra == "proc-mp" 
+000008f0: 6f72 2065 7874 7261 203d 3d20 2261 6c6c  or extra == "all
+00000900: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000910: 2070 616e 6461 7320 3b20 6578 7472 6120   pandas ; extra 
+00000920: 3d3d 2022 6461 7461 7365 7473 2220 6f72  == "datasets" or
+00000930: 2065 7874 7261 203d 3d20 2270 726f 6322   extra == "proc"
+00000940: 206f 7220 6578 7472 6120 3d3d 2022 7072   or extra == "pr
+00000950: 6f63 2d6d 7022 206f 7220 6578 7472 6120  oc-mp" or extra 
+00000960: 3d3d 2022 616c 6c22 0a52 6571 7569 7265  == "all".Require
+00000970: 732d 4469 7374 3a20 706c 6174 666f 726d  s-Dist: platform
+00000980: 6469 7273 2028 3e3d 332e 352e 302c 3c34  dirs (>=3.5.0,<4
+00000990: 2e30 2e30 290a 5265 7175 6972 6573 2d44  .0.0).Requires-D
+000009a0: 6973 743a 2070 726f 746f 6275 6620 283e  ist: protobuf (>
+000009b0: 3d33 2e31 392e 3429 0a52 6571 7569 7265  =3.19.4).Require
+000009c0: 732d 4469 7374 3a20 7079 6172 726f 7720  s-Dist: pyarrow 
+000009d0: 283e 3d38 2e30 2e30 2c3c 3133 2920 3b20  (>=8.0.0,<13) ; 
+000009e0: 6578 7472 6120 3d3d 2022 7370 6172 6b22  extra == "spark"
+000009f0: 206f 7220 6578 7472 6120 3d3d 2022 616c   or extra == "al
+00000a00: 6c22 0a52 6571 7569 7265 732d 4469 7374  l".Requires-Dist
+00000a10: 3a20 7079 6261 7273 3320 283e 3d30 2e39  : pybars3 (>=0.9
+00000a20: 2c3c 302e 3130 2920 3b20 6578 7472 6120  ,<0.10) ; extra 
+00000a30: 3d3d 2022 7669 7a22 206f 7220 6578 7472  == "viz" or extr
+00000a40: 6120 3d3d 2022 616c 6c22 0a52 6571 7569  a == "all".Requi
+00000a50: 7265 732d 4469 7374 3a20 7079 7370 6172  res-Dist: pyspar
+00000a60: 6b20 283e 3d33 2e30 2e30 2c3c 342e 302e  k (>=3.0.0,<4.0.
+00000a70: 3029 203b 2065 7874 7261 203d 3d20 2273  0) ; extra == "s
+00000a80: 7061 726b 2220 6f72 2065 7874 7261 203d  park" or extra =
+00000a90: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
+00000aa0: 2d44 6973 743a 2072 6571 7565 7374 7320  -Dist: requests 
+00000ab0: 283e 3d32 2e32 372c 3c33 2e30 290a 5265  (>=2.27,<3.0).Re
+00000ac0: 7175 6972 6573 2d44 6973 743a 2073 6369  quires-Dist: sci
+00000ad0: 6b69 742d 6c65 6172 6e20 283e 3d31 2e30  kit-learn (>=1.0
+00000ae0: 2e32 2c3c 322e 302e 3029 203b 2028 7079  .2,<2.0.0) ; (py
+00000af0: 7468 6f6e 5f76 6572 7369 6f6e 203c 2022  thon_version < "
+00000b00: 332e 3131 2229 2061 6e64 2028 6578 7472  3.11") and (extr
+00000b10: 6120 3d3d 2022 656d 6265 6464 696e 6773  a == "embeddings
+00000b20: 2220 6f72 2065 7874 7261 203d 3d20 2261  " or extra == "a
+00000b30: 6c6c 2229 0a52 6571 7569 7265 732d 4469  ll").Requires-Di
+00000b40: 7374 3a20 7363 696b 6974 2d6c 6561 726e  st: scikit-learn
+00000b50: 2028 3e3d 312e 312e 322c 3c32 2920 3b20   (>=1.1.2,<2) ; 
+00000b60: 2870 7974 686f 6e5f 7665 7273 696f 6e20  (python_version 
+00000b70: 3e3d 2022 332e 3131 2229 2061 6e64 2028  >= "3.11") and (
+00000b80: 6578 7472 6120 3d3d 2022 656d 6265 6464  extra == "embedd
+00000b90: 696e 6773 2220 6f72 2065 7874 7261 203d  ings" or extra =
+00000ba0: 3d20 2261 6c6c 2229 0a52 6571 7569 7265  = "all").Require
+00000bb0: 732d 4469 7374 3a20 7363 6970 7920 283e  s-Dist: scipy (>
+00000bc0: 3d31 2e35 2920 3b20 2870 7974 686f 6e5f  =1.5) ; (python_
+00000bd0: 7665 7273 696f 6e20 3c20 2233 2e31 3122  version < "3.11"
+00000be0: 2920 616e 6420 2865 7874 7261 203d 3d20  ) and (extra == 
+00000bf0: 2276 697a 2220 6f72 2065 7874 7261 203d  "viz" or extra =
+00000c00: 3d20 2261 6c6c 2229 0a52 6571 7569 7265  = "all").Require
+00000c10: 732d 4469 7374 3a20 7363 6970 7920 283e  s-Dist: scipy (>
+00000c20: 3d31 2e39 2e32 2920 3b20 2870 7974 686f  =1.9.2) ; (pytho
+00000c30: 6e5f 7665 7273 696f 6e20 3e3d 2022 332e  n_version >= "3.
+00000c40: 3131 2229 2061 6e64 2028 6578 7472 6120  11") and (extra 
+00000c50: 3d3d 2022 7669 7a22 206f 7220 6578 7472  == "viz" or extr
+00000c60: 6120 3d3d 2022 616c 6c22 290a 5265 7175  a == "all").Requ
+00000c70: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
+00000c80: 7820 3b20 6578 7472 6120 3d3d 2022 646f  x ; extra == "do
+00000c90: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000ca0: 743a 2073 7068 696e 782d 6175 746f 6170  t: sphinx-autoap
+00000cb0: 6920 3b20 6578 7472 6120 3d3d 2022 646f  i ; extra == "do
+00000cc0: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000cd0: 743a 2073 7068 696e 782d 6175 746f 6275  t: sphinx-autobu
+00000ce0: 696c 6420 283e 3d32 3032 312e 332e 3134  ild (>=2021.3.14
+00000cf0: 2c3c 3230 3232 2e30 2e30 2920 3b20 6578  ,<2022.0.0) ; ex
+00000d00: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
+00000d10: 7175 6972 6573 2d44 6973 743a 2073 7068  quires-Dist: sph
+00000d20: 696e 782d 636f 7079 6275 7474 6f6e 2028  inx-copybutton (
+00000d30: 3e3d 302e 352e 302c 3c30 2e36 2e30 2920  >=0.5.0,<0.6.0) 
+00000d40: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
+00000d50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000d60: 2073 7068 696e 782d 696e 6c69 6e65 2d74   sphinx-inline-t
+00000d70: 6162 7320 3b20 2870 7974 686f 6e5f 7665  abs ; (python_ve
+00000d80: 7273 696f 6e20 3e3d 2022 332e 3822 2061  rsion >= "3.8" a
+00000d90: 6e64 2070 7974 686f 6e5f 7665 7273 696f  nd python_versio
+00000da0: 6e20 3c20 2234 2229 2061 6e64 2028 6578  n < "4") and (ex
+00000db0: 7472 6120 3d3d 2022 646f 6373 2229 0a52  tra == "docs").R
+00000dc0: 6571 7569 7265 732d 4469 7374 3a20 7370  equires-Dist: sp
+00000dd0: 6869 6e78 6578 742d 6f70 656e 6772 6170  hinxext-opengrap
+00000de0: 6820 283e 3d30 2e36 2e33 2c3c 302e 372e  h (>=0.6.3,<0.7.
+00000df0: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+00000e00: 6f63 7322 0a52 6571 7569 7265 732d 4469  ocs".Requires-Di
+00000e10: 7374 3a20 7479 7065 732d 7265 7175 6573  st: types-reques
+00000e20: 7473 2028 3e3d 322e 3330 2e30 2e30 2c3c  ts (>=2.30.0.0,<
+00000e30: 332e 302e 302e 3029 0a52 6571 7569 7265  3.0.0.0).Require
+00000e40: 732d 4469 7374 3a20 7479 7069 6e67 2d65  s-Dist: typing-e
+00000e50: 7874 656e 7369 6f6e 7320 283e 3d33 2e31  xtensions (>=3.1
+00000e60: 3029 203b 2070 7974 686f 6e5f 7665 7273  0) ; python_vers
+00000e70: 696f 6e20 3c20 2234 220a 5265 7175 6972  ion < "4".Requir
+00000e80: 6573 2d44 6973 743a 2077 6879 6c61 6273  es-Dist: whylabs
+00000e90: 2d63 6c69 656e 7420 283e 3d30 2e35 2e36  -client (>=0.5.6
+00000ea0: 2c3c 302e 362e 3029 0a52 6571 7569 7265  ,<0.6.0).Require
+00000eb0: 732d 4469 7374 3a20 7768 796c 6f67 732d  s-Dist: whylogs-
+00000ec0: 736b 6574 6368 696e 6720 283e 3d33 2e34  sketching (>=3.4
+00000ed0: 2e31 2e64 6576 3329 0a44 6573 6372 6970  .1.dev3).Descrip
+00000ee0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
+00000ef0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
+00000f00: 0a0a 3c69 6d67 2073 7263 3d22 6874 7470  ..<img src="http
+00000f10: 733a 2f2f 7374 6174 6963 2e73 6361 7266  s://static.scarf
+00000f20: 2e73 682f 612e 706e 673f 782d 7078 6964  .sh/a.png?x-pxid
+00000f30: 3d62 6333 6335 3762 302d 3961 3635 2d34  =bc3c57b0-9a65-4
+00000f40: 3966 652d 6238 6561 2d66 3731 3163 3464  9fe-b8ea-f711c4d
+00000f50: 3335 6238 3222 202f 3e3c 7020 616c 6967  35b82" /><p alig
+00000f60: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
+00000f70: 2073 7263 3d22 6874 7470 733a 2f2f 692e   src="https://i.
+00000f80: 696d 6775 722e 636f 6d2f 6e76 3333 676f  imgur.com/nv33go
+00000f90: 562e 706e 6722 2077 6964 7468 3d22 3335  V.png" width="35
+00000fa0: 2522 2f3e 0a3c 2f62 723e 0a0a 3c68 3120  %"/>.</br>..<h1 
+00000fb0: 616c 6967 6e3d 2263 656e 7465 7222 3e54  align="center">T
+00000fc0: 6865 206f 7065 6e20 7374 616e 6461 7264  he open standard
+00000fd0: 2066 6f72 2064 6174 6120 6c6f 6767 696e   for data loggin
+00000fe0: 670a 0a20 3c2f 6831 3e0a 2020 3c68 3320  g.. </h1>.  <h3 
+00000ff0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00001000: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00001010: 733a 2f2f 7768 796c 6f67 732e 7265 6164  s://whylogs.read
+00001020: 7468 6564 6f63 732e 696f 2f22 3e3c 623e  thedocs.io/"><b>
+00001030: 446f 6375 6d65 6e74 6174 696f 6e3c 2f62  Documentation</b
+00001040: 3e3c 2f61 3e20 2662 756c 6c3b 0a20 2020  ></a> &bull;.   
+00001050: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001060: 2f62 6974 2e6c 792f 7768 796c 6f67 7373  /bit.ly/whylogss
+00001070: 6c61 636b 223e 3c62 3e53 6c61 636b 2043  lack"><b>Slack C
+00001080: 6f6d 6d75 6e69 7479 3c2f 623e 3c2f 613e  ommunity</b></a>
+00001090: 2026 6275 6c6c 3b0a 2020 203c 6120 6872   &bull;.   <a hr
+000010a0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000010b0: 7562 2e63 6f6d 2f77 6879 6c61 6273 2f77  ub.com/whylabs/w
+000010c0: 6879 6c6f 6773 2370 7974 686f 6e2d 7175  hylogs#python-qu
+000010d0: 6963 6b73 7461 7274 223e 3c62 3e50 7974  ickstart"><b>Pyt
+000010e0: 686f 6e20 5175 6963 6b73 7461 7274 3c2f  hon Quickstart</
+000010f0: 623e 3c2f 613e 2026 6275 6c6c 3b0a 2020  b></a> &bull;.  
+00001100: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00001110: 2f2f 7768 796c 6f67 732e 7265 6164 7468  //whylogs.readth
+00001120: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001130: 7374 2f65 7861 6d70 6c65 732f 696e 7465  st/examples/inte
+00001140: 6772 6174 696f 6e73 2f77 7269 7465 7273  grations/writers
+00001150: 2f57 7269 7469 6e67 5f74 6f5f 5768 794c  /Writing_to_WhyL
+00001160: 6162 732e 6874 6d6c 223e 3c62 3e57 6879  abs.html"><b>Why
+00001170: 4c61 6273 2051 7569 636b 7374 6172 743c  Labs Quickstart<
+00001180: 2f62 3e3c 2f61 3e0a 203c 2f68 333e 0a0a  /b></a>. </h3>..
+00001190: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000011a0: 223e 0a3c 6120 6872 6566 3d22 6874 7470  ">.<a href="http
+000011b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f77  s://github.com/w
+000011c0: 6879 6c61 6273 2f77 6879 6c6f 6773 2d70  hylabs/whylogs-p
+000011d0: 7974 686f 6e2f 626c 6f62 2f6d 6169 6e6c  ython/blob/mainl
+000011e0: 696e 652f 4c49 4345 4e53 4522 2074 6172  ine/LICENSE" tar
+000011f0: 6765 743d 225f 626c 616e 6b22 3e0a 2020  get="_blank">.  
+00001200: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00001210: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00001220: 6f2f 3a6c 6963 656e 7365 2d41 7061 6368  o/:license-Apach
+00001230: 6525 3230 322d 626c 7565 2e73 7667 2220  e%202-blue.svg" 
+00001240: 616c 743d 224c 6963 656e 7365 223e 0a3c  alt="License">.<
+00001250: 2f61 3e0a 3c61 2068 7265 663d 2268 7474  /a>.<a href="htt
+00001260: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+00001270: 696f 2f70 792f 7768 796c 6f67 7322 2074  io/py/whylogs" t
+00001280: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
+00001290: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000012a0: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
+000012b0: 2e69 6f2f 7079 2f77 6879 6c6f 6773 2e73  .io/py/whylogs.s
+000012c0: 7667 2220 616c 743d 2250 7950 6920 5665  vg" alt="PyPi Ve
+000012d0: 7273 696f 6e22 3e0a 3c2f 613e 0a3c 6120  rsion">.</a>.<a 
+000012e0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+000012f0: 7468 7562 2e63 6f6d 2f70 7974 686f 6e2f  thub.com/python/
+00001300: 626c 6163 6b22 2074 6172 6765 743d 225f  black" target="_
+00001310: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
+00001320: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00001330: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00001340: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
+00001350: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
+00001360: 2220 616c 743d 2243 6f64 6520 7374 796c  " alt="Code styl
+00001370: 653a 2062 6c61 636b 223e 0a3c 2f61 3e0a  e: black">.</a>.
+00001380: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001390: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
+000013a0: 6374 2f77 6879 6c6f 6773 2220 7461 7267  ct/whylogs" targ
+000013b0: 6574 3d22 5f62 6c61 6e6b 223e 0a20 2020  et="_blank">.   
+000013c0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+000013d0: 3a2f 2f70 6570 792e 7465 6368 2f62 6164  ://pepy.tech/bad
+000013e0: 6765 2f77 6879 6c6f 6773 2220 616c 743d  ge/whylogs" alt=
+000013f0: 2250 7950 6920 446f 776e 6c6f 6164 7322  "PyPi Downloads"
+00001400: 3e0a 3c2f 613e 0a3c 6120 6872 6566 3d22  >.</a>.<a href="
+00001410: 6269 742e 6c79 2f77 6879 6c6f 6773 2220  bit.ly/whylogs" 
+00001420: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00001430: 0a20 2020 203c 696d 6720 7372 633d 2268  .    <img src="h
+00001440: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001450: 6d2f 7768 796c 6162 732f 7768 796c 6f67  m/whylabs/whylog
+00001460: 732d 7079 7468 6f6e 2f77 6f72 6b66 6c6f  s-python/workflo
+00001470: 7773 2f77 6879 6c6f 6773 2532 3043 492f  ws/whylogs%20CI/
+00001480: 6261 6467 652e 7376 6722 2061 6c74 3d22  badge.svg" alt="
+00001490: 4349 223e 0a3c 2f61 3e0a 3c61 2068 7265  CI">.</a>.<a hre
+000014a0: 663d 2268 7474 7073 3a2f 2f63 6f64 6563  f="https://codec
+000014b0: 6c69 6d61 7465 2e63 6f6d 2f67 6974 6875  limate.com/githu
+000014c0: 622f 7768 796c 6162 732f 7768 796c 6f67  b/whylabs/whylog
+000014d0: 732d 7079 7468 6f6e 2f6d 6169 6e74 6169  s-python/maintai
+000014e0: 6e61 6269 6c69 7479 2220 7461 7267 6574  nability" target
+000014f0: 3d22 5f62 6c61 6e6b 223e 0a20 2020 203c  ="_blank">.    <
+00001500: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00001510: 2f61 7069 2e63 6f64 6563 6c69 6d61 7465  /api.codeclimate
+00001520: 2e63 6f6d 2f76 312f 6261 6467 6573 2f34  .com/v1/badges/4
+00001530: 3432 6636 6361 3364 6361 3165 3538 3361  42f6ca3dca1e583a
+00001540: 3438 382f 6d61 696e 7461 696e 6162 696c  488/maintainabil
+00001550: 6974 7922 2061 6c74 3d22 4d61 696e 7461  ity" alt="Mainta
+00001560: 696e 6162 696c 6974 7922 3e0a 3c2f 613e  inability">.</a>
+00001570: 0a3c 2f70 3e0a 0a23 2320 5768 6174 2069  .</p>..## What i
+00001580: 7320 7768 796c 6f67 730a 0a77 6879 6c6f  s whylogs..whylo
+00001590: 6773 2069 7320 616e 206f 7065 6e20 736f  gs is an open so
+000015a0: 7572 6365 206c 6962 7261 7279 2066 6f72  urce library for
+000015b0: 206c 6f67 6769 6e67 2061 6e79 206b 696e   logging any kin
+000015c0: 6420 6f66 2064 6174 612e 2057 6974 6820  d of data. With 
+000015d0: 7768 796c 6f67 732c 2075 7365 7273 2061  whylogs, users a
+000015e0: 7265 2061 626c 6520 746f 2067 656e 6572  re able to gener
+000015f0: 6174 6520 7375 6d6d 6172 6965 7320 6f66  ate summaries of
+00001600: 2074 6865 6972 2064 6174 6173 6574 7320   their datasets 
+00001610: 2863 616c 6c65 6420 5f77 6879 6c6f 6773  (called _whylogs
+00001620: 2070 726f 6669 6c65 735f 2920 7768 6963   profiles_) whic
+00001630: 6820 7468 6579 2063 616e 2075 7365 2074  h they can use t
+00001640: 6f3a 0a0a 312e 2054 7261 636b 2063 6861  o:..1. Track cha
+00001650: 6e67 6573 2069 6e20 7468 6569 7220 6461  nges in their da
+00001660: 7461 7365 740a 322e 2043 7265 6174 6520  taset.2. Create 
+00001670: 5f64 6174 6120 636f 6e73 7472 6169 6e74  _data constraint
+00001680: 735f 2074 6f20 6b6e 6f77 2077 6865 7468  s_ to know wheth
+00001690: 6572 2074 6865 6972 2064 6174 6120 6c6f  er their data lo
+000016a0: 6f6b 7320 7468 6520 7761 7920 6974 2073  oks the way it s
+000016b0: 686f 756c 640a 332e 2051 7569 636b 6c79  hould.3. Quickly
+000016c0: 2076 6973 7561 6c69 7a65 206b 6579 2073   visualize key s
+000016d0: 756d 6d61 7279 2073 7461 7469 7374 6963  ummary statistic
+000016e0: 7320 6162 6f75 7420 7468 6569 7220 6461  s about their da
+000016f0: 7461 7365 7473 0a0a 5468 6573 6520 7468  tasets..These th
+00001700: 7265 6520 6675 6e63 7469 6f6e 616c 6974  ree functionalit
+00001710: 6965 7320 656e 6162 6c65 2061 2076 6172  ies enable a var
+00001720: 6965 7479 206f 6620 7573 6520 6361 7365  iety of use case
+00001730: 7320 666f 7220 6461 7461 2073 6369 656e  s for data scien
+00001740: 7469 7374 732c 206d 6163 6869 6e65 206c  tists, machine l
+00001750: 6561 726e 696e 6720 656e 6769 6e65 6572  earning engineer
+00001760: 732c 2061 6e64 2064 6174 6120 656e 6769  s, and data engi
+00001770: 6e65 6572 733a 0a0a 2d20 4465 7465 6374  neers:..- Detect
+00001780: 2064 6174 6120 6472 6966 7420 696e 206d   data drift in m
+00001790: 6f64 656c 2069 6e70 7574 2066 6561 7475  odel input featu
+000017a0: 7265 730a 2d20 4465 7465 6374 2074 7261  res.- Detect tra
+000017b0: 696e 696e 672d 7365 7276 696e 6720 736b  ining-serving sk
+000017c0: 6577 2c20 636f 6e63 6570 7420 6472 6966  ew, concept drif
+000017d0: 742c 2061 6e64 206d 6f64 656c 2070 6572  t, and model per
+000017e0: 666f 726d 616e 6365 2064 6567 7261 6461  formance degrada
+000017f0: 7469 6f6e 0a2d 2056 616c 6964 6174 6520  tion.- Validate 
+00001800: 6461 7461 2071 7561 6c69 7479 2069 6e20  data quality in 
+00001810: 6d6f 6465 6c20 696e 7075 7473 206f 7220  model inputs or 
+00001820: 696e 2061 2064 6174 6120 7069 7065 6c69  in a data pipeli
+00001830: 6e65 0a2d 2050 6572 666f 726d 2065 7870  ne.- Perform exp
+00001840: 6c6f 7261 746f 7279 2064 6174 6120 616e  loratory data an
+00001850: 616c 7973 6973 206f 6620 6d61 7373 6976  alysis of massiv
+00001860: 6520 6461 7461 7365 7473 0a2d 2054 7261  e datasets.- Tra
+00001870: 636b 2064 6174 6120 6469 7374 7269 6275  ck data distribu
+00001880: 7469 6f6e 7320 2620 6461 7461 2071 7561  tions & data qua
+00001890: 6c69 7479 2066 6f72 204d 4c20 6578 7065  lity for ML expe
+000018a0: 7269 6d65 6e74 730a 2d20 456e 6162 6c65  riments.- Enable
+000018b0: 2064 6174 6120 6175 6469 7469 6e67 2061   data auditing a
+000018c0: 6e64 2067 6f76 6572 6e61 6e63 6520 6163  nd governance ac
+000018d0: 726f 7373 2074 6865 206f 7267 616e 697a  ross the organiz
+000018e0: 6174 696f 6e0a 2d20 5374 616e 6461 7264  ation.- Standard
+000018f0: 697a 6520 6461 7461 2064 6f63 756d 656e  ize data documen
+00001900: 7461 7469 6f6e 2070 7261 6374 6963 6573  tation practices
+00001910: 2061 6372 6f73 7320 7468 6520 6f72 6761   across the orga
+00001920: 6e69 7a61 7469 6f6e 0a2d 2041 6e64 206d  nization.- And m
+00001930: 6f72 650a 0a23 2320 5175 6963 6b73 7461  ore..## Quicksta
+00001940: 7274 0a0a 496e 7374 616c 6c20 7768 796c  rt..Install whyl
+00001950: 6f67 7320 7573 696e 6720 7468 6520 7069  ogs using the pi
+00001960: 7020 7061 636b 6167 6520 6d61 6e61 6765  p package manage
+00001970: 7220 696e 2061 2074 6572 6d69 6e61 6c20  r in a terminal 
+00001980: 6279 2072 756e 6e69 6e67 3a0a 0a60 6060  by running:..```
+00001990: 0a70 6970 2069 6e73 7461 6c6c 2077 6879  .pip install why
+000019a0: 6c6f 6773 0a60 6060 0a0a 5468 656e 2079  logs.```..Then y
+000019b0: 6f75 2063 616e 206c 6f67 2064 6174 6120  ou can log data 
+000019c0: 696e 2070 7974 686f 6e20 6173 2073 696d  in python as sim
+000019d0: 706c 7920 6173 2074 6869 733a 0a0a 6060  ply as this:..``
+000019e0: 6070 7974 686f 6e0a 696d 706f 7274 2077  `python.import w
+000019f0: 6879 6c6f 6773 2061 7320 7768 790a 696d  hylogs as why.im
+00001a00: 706f 7274 2070 616e 6461 7320 6173 2070  port pandas as p
+00001a10: 640a 0a64 6620 3d20 7064 2e72 6561 645f  d..df = pd.read_
+00001a20: 6373 7628 2270 6174 682f 746f 2f66 696c  csv("path/to/fil
+00001a30: 652e 6373 7622 290a 7265 7375 6c74 7320  e.csv").results 
+00001a40: 3d20 7768 792e 6c6f 6728 6466 290a 6060  = why.log(df).``
+00001a50: 600a 0a41 6e64 2076 6f69 6cc3 a02c 2079  `..And voil.., y
+00001a60: 6f75 206e 6f77 2068 6176 6520 6120 7768  ou now have a wh
+00001a70: 796c 6f67 7320 7072 6f66 696c 652e 2054  ylogs profile. T
+00001a80: 6f20 6c65 6172 6e20 6d6f 7265 2061 626f  o learn more abo
+00001a90: 7574 2077 6861 7420 6120 7768 796c 6f67  ut what a whylog
+00001aa0: 7320 7072 6f66 696c 6520 6973 2061 6e64  s profile is and
+00001ab0: 2077 6861 7420 796f 7520 6361 6e20 646f   what you can do
+00001ac0: 2077 6974 6820 6974 2c20 6368 6563 6b20   with it, check 
+00001ad0: 6f75 7420 6f75 7220 5b64 6f63 735d 2868  out our [docs](h
+00001ae0: 7474 7073 3a2f 2f77 6879 6c6f 6773 2e72  ttps://whylogs.r
+00001af0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001b00: 2f6c 6174 6573 742f 2920 616e 6420 6f75  /latest/) and ou
+00001b10: 7220 5b65 7861 6d70 6c65 735d 2868 7474  r [examples](htt
+00001b20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001b30: 7768 796c 6162 732f 7768 796c 6f67 732f  whylabs/whylogs/
+00001b40: 7472 6565 2f6d 6169 6e6c 696e 652f 7079  tree/mainline/py
+00001b50: 7468 6f6e 2f65 7861 6d70 6c65 7329 2e0a  thon/examples)..
+00001b60: 0a                                       .
```

