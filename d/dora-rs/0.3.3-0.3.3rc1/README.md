# Comparing `tmp/dora_rs-0.3.3.tar.gz` & `tmp/dora_rs-0.3.3rc1.tar.gz`

## Comparing `dora_rs-0.3.3.tar` & `dora_rs-0.3.3rc1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0     1001      127      665 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/Cargo.toml
--rw-r--r--   0     1001      127     9127 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/config.rs
--rw-r--r--   0     1001      127      957 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/coordinator_messages.rs
--rw-r--r--   0     1001      127     6944 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/daemon_messages.rs
--rw-r--r--   0     1001      127    11528 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/descriptor/mod.rs
--rw-r--r--   0     1001      127     7332 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/descriptor/validate.rs
--rw-r--r--   0     1001      127     7349 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      127     2397 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/lib.rs
--rw-r--r--   0     1001      127     2066 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/core/src/topics.rs
--rw-r--r--   0     1001      127      424 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/Cargo.toml
--rw-r--r--   0     1001      127     9105 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/lib.rs
--rw-r--r--   0     1001      127     3515 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/qos.rs
--rw-r--r--   0     1001      127      729 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
--rw-r--r--   0     1001      127     6330 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
--rw-r--r--   0     1001      127     4726 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
--rw-r--r--   0     1001      127     6326 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
--rw-r--r--   0     1001      127     1154 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
--rw-r--r--   0     1001      127     4263 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
--rw-r--r--   0     1001      127     9390 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
--rw-r--r--   0     1001      127     9481 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
--rw-r--r--   0     1001      127     7776 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
--rw-r--r--   0     1001      127     3086 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
--rw-r--r--   0     1001      127     9552 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
--rw-r--r--   0     1001      127    11898 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/test_utils.py
--rw-r--r--   0     1001      127      461 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/operator/types/Cargo.toml
--rw-r--r--   0     1001      127     4911 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/operator/types/src/lib.rs
--rw-r--r--   0     1001      127      549 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/python/operator/Cargo.toml
--rw-r--r--   0     1001      127     7968 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/python/operator/src/lib.rs
--rw-r--r--   0     1001      127      452 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/download/Cargo.toml
--rw-r--r--   0     1001      127     1285 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/download/src/lib.rs
--rw-r--r--   0     1001      127      583 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/telemetry/tracing/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/telemetry/tracing/src/lib.rs
--rw-r--r--   0     1001      127     2388 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/telemetry/tracing/src/telemetry.rs
--rw-r--r--   0     1001      127      733 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/Cargo.toml
--rw-r--r--   0     1001      127     2429 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      127     2149 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      127     3457 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/event_stream/event.rs
--rw-r--r--   0     1001      127     3100 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/event_stream/merged.rs
--rw-r--r--   0     1001      127     8375 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/event_stream/mod.rs
--rw-r--r--   0     1001      127     9280 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/event_stream/thread.rs
--rw-r--r--   0     1001      127      764 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/lib.rs
--rw-r--r--   0     1001      127     2553 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/node/arrow_utils.rs
--rw-r--r--   0     1001      127     3654 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/node/control_channel.rs
--rw-r--r--   0     1001      127     5795 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/node/drop_stream.rs
--rw-r--r--   0     1001      127    14352 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/rust/node/src/node/mod.rs
--rw-r--r--   0     1001      127     1364 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/Cargo.toml
--rw-r--r--   0     1001      127     1493 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/build.rs
--rw-r--r--   0     1001      127      276 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/mod.rs
--rw-r--r--   0     1001      127     4114 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/sequence.rs
--rw-r--r--   0     1001      127     5495 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/string.rs
--rw-r--r--   0     1001      127     2337 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/traits.rs
--rw-r--r--   0     1001      127      223 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/lib.rs
--rw-r--r--   0     1001      127      451 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/message/Cargo.toml
--rw-r--r--   0     1001      127     4223 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/message/src/lib.rs
--rw-r--r--   0     1001      127      561 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/telemetry/metrics/Cargo.toml
--rw-r--r--   0     1001      127     1836 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/telemetry/metrics/src/lib.rs
--rw-r--r--   0     1001      127     1431 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/Cargo.toml
--rw-r--r--   0     1001      127    13120 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/src/lib.rs
--rw-r--r--   0     1001      127     4296 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/src/operator/channel.rs
--rw-r--r--   0     1001      127     2639 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/src/operator/mod.rs
--rw-r--r--   0     1001      127    15244 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/src/operator/python.rs
--rw-r--r--   0     1001      127    10280 2024-04-11 13:45:58.000000 dora_rs-0.3.3/binaries/runtime/src/operator/shared_lib.rs
--rw-r--r--   0     1001      127      323 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/arrow-convert/Cargo.toml
--rw-r--r--   0     1001      127     5495 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/arrow-convert/src/from_impls.rs
--rw-r--r--   0     1001      127     3744 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/arrow-convert/src/into_impls.rs
--rw-r--r--   0     1001      127      485 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/arrow-convert/src/lib.rs
--rw-r--r--   0     1001      127      288 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
--rw-r--r--   0     1001      127      787 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/build.rs
--rw-r--r--   0     1001      127    10910 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
--rw-r--r--   0     1001      127     3703 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
--rw-r--r--   0     1001      127     2848 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
--rw-r--r--   0     1001      127      776 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
--rw-r--r--   0     1001      127     2257 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
--rw-r--r--   0     1001      127     9363 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
--rw-r--r--   0     1001      127     4376 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
--rw-r--r--   0     1001      127     4024 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
--rw-r--r--   0     1001      127      191 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
--rw-r--r--   0     1001      127     4327 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
--rw-r--r--   0     1001      127     2607 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
--rw-r--r--   0     1001      127    10849 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
--rw-r--r--   0     1001      127     7208 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
--rw-r--r--   0     1001      127     1942 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
--rw-r--r--   0     1001      127     4429 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
--rw-r--r--   0     1001      127    20805 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
--rw-r--r--   0     1001      127      299 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
--rw-r--r--   0     1001      127     3789 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
--rw-r--r--   0     1001      127    12158 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
--rw-r--r--   0     1001      127     3382 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
--rw-r--r--   0     1001      127    11907 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
--rw-r--r--   0     1001      127      100 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
--rw-r--r--   0     1001      127     1271 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
--rw-r--r--   0     1001      127      240 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
--rw-r--r--   0     1001      127     1346 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
--rw-r--r--   0     1001      127      315 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
--rw-r--r--   0     1001      127      315 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
--rw-r--r--   0     1001      127        0 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
--rw-r--r--   0     1001      127      484 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
--rw-r--r--   0     1001      127       29 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
--rw-r--r--   0     1001      127      591 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
--rw-r--r--   0     1001      127     1255 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
--rw-r--r--   0     1001      127      415 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
--rw-r--r--   0     1001      127     2282 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
--rw-r--r--   0     1001      127      524 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
--rw-r--r--   0     1001      127        4 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
--rw-r--r--   0     1001      127      593 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      127     3249 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      127     7343 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      127     2019 2024-04-11 13:45:58.000000 dora_rs-0.3.3/libraries/shared-memory-server/src/lib.rs
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.3/apis/python/node/Cargo.toml
--rw-r--r--   0     1001      127      201 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/python/node/README.md
--rw-r--r--   0     1001      127      514 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/python/node/dora/__init__.py
--rw-r--r--   0     1001      127     6852 2024-04-11 13:45:58.000000 dora_rs-0.3.3/apis/python/node/src/lib.rs
--rw-r--r--   0     1001      127   169802 2024-04-11 13:45:58.000000 dora_rs-0.3.3/Cargo.lock
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 dora_rs-0.3.3/Cargo.toml
--rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.3/pyproject.toml
--rw-r--r--   0     1001      127      514 2024-04-11 13:45:58.000000 dora_rs-0.3.3/dora/__init__.py
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 dora_rs-0.3.3/PKG-INFO
+-rw-r--r--   0     1001      127      323 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/Cargo.toml
+-rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs
+-rw-r--r--   0     1001      127     3744 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs
+-rw-r--r--   0     1001      127      485 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/arrow-convert/src/lib.rs
+-rw-r--r--   0     1001      127      452 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/Cargo.toml
+-rw-r--r--   0     1001      127     1285 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs
+-rw-r--r--   0     1001      127      461 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/Cargo.toml
+-rw-r--r--   0     1001      127     4911 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs
+-rw-r--r--   0     1001      127      288 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
+-rw-r--r--   0     1001      127      787 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs
+-rw-r--r--   0     1001      127    10910 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
+-rw-r--r--   0     1001      127     3703 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
+-rw-r--r--   0     1001      127     2848 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
+-rw-r--r--   0     1001      127      776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
+-rw-r--r--   0     1001      127     2257 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
+-rw-r--r--   0     1001      127     9363 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
+-rw-r--r--   0     1001      127     4376 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
+-rw-r--r--   0     1001      127     4024 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
+-rw-r--r--   0     1001      127      191 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
+-rw-r--r--   0     1001      127     4327 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
+-rw-r--r--   0     1001      127     2607 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
+-rw-r--r--   0     1001      127    10849 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
+-rw-r--r--   0     1001      127     7208 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
+-rw-r--r--   0     1001      127     1942 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
+-rw-r--r--   0     1001      127     4429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
+-rw-r--r--   0     1001      127    20805 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
+-rw-r--r--   0     1001      127      299 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
+-rw-r--r--   0     1001      127     3789 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
+-rw-r--r--   0     1001      127    12158 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
+-rw-r--r--   0     1001      127     3382 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
+-rw-r--r--   0     1001      127    11907 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
+-rw-r--r--   0     1001      127      100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
+-rw-r--r--   0     1001      127     1271 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
+-rw-r--r--   0     1001      127      240 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
+-rw-r--r--   0     1001      127     1346 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
+-rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
+-rw-r--r--   0     1001      127      315 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
+-rw-r--r--   0     1001      127        0 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
+-rw-r--r--   0     1001      127      484 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
+-rw-r--r--   0     1001      127       29 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
+-rw-r--r--   0     1001      127      591 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
+-rw-r--r--   0     1001      127     1255 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
+-rw-r--r--   0     1001      127      415 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
+-rw-r--r--   0     1001      127     2282 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
+-rw-r--r--   0     1001      127      524 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
+-rw-r--r--   0     1001      127        4 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
+-rw-r--r--   0     1001      127      593 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      127     3249 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      127     7343 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      127     2019 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs
+-rw-r--r--   0     1001      127      733 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml
+-rw-r--r--   0     1001      127     2429 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      127     2149 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      127     3457 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs
+-rw-r--r--   0     1001      127     3100 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs
+-rw-r--r--   0     1001      127     8375 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs
+-rw-r--r--   0     1001      127     9280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs
+-rw-r--r--   0     1001      127      764 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs
+-rw-r--r--   0     1001      127     2553 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs
+-rw-r--r--   0     1001      127     3654 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs
+-rw-r--r--   0     1001      127     5795 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs
+-rw-r--r--   0     1001      127    14352 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs
+-rw-r--r--   0     1001      127      561 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/Cargo.toml
+-rw-r--r--   0     1001      127     1836 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs
+-rw-r--r--   0     1001      127      424 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/Cargo.toml
+-rw-r--r--   0     1001      127     9105 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/lib.rs
+-rw-r--r--   0     1001      127     3515 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs
+-rw-r--r--   0     1001      127      729 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
+-rw-r--r--   0     1001      127     6330 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
+-rw-r--r--   0     1001      127     4726 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
+-rw-r--r--   0     1001      127     6326 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
+-rw-r--r--   0     1001      127     1154 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
+-rw-r--r--   0     1001      127     4263 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
+-rw-r--r--   0     1001      127     9390 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
+-rw-r--r--   0     1001      127     9481 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
+-rw-r--r--   0     1001      127     7776 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
+-rw-r--r--   0     1001      127     3086 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
+-rw-r--r--   0     1001      127     9552 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
+-rw-r--r--   0     1001      127    11898 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py
+-rw-r--r--   0     1001      127      451 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/Cargo.toml
+-rw-r--r--   0     1001      127     4223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/message/src/lib.rs
+-rw-r--r--   0     1001      127      549 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml
+-rw-r--r--   0     1001      127     7968 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs
+-rw-r--r--   0     1001      127      665 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/Cargo.toml
+-rw-r--r--   0     1001      127     9127 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/config.rs
+-rw-r--r--   0     1001      127      957 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      127     6944 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs
+-rw-r--r--   0     1001      127    10351 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      127     7260 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      127     7349 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      127     2397 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/lib.rs
+-rw-r--r--   0     1001      127     2066 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/core/src/topics.rs
+-rw-r--r--   0     1001      127     1431 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml
+-rw-r--r--   0     1001      127    13120 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs
+-rw-r--r--   0     1001      127     4296 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      127     2639 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      127    15169 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs
+-rw-r--r--   0     1001      127    10280 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs
+-rw-r--r--   0     1001      127      583 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs
+-rw-r--r--   0     1001      127     2388 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs
+-rw-r--r--   0     1001      127     1364 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml
+-rw-r--r--   0     1001      127     1493 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/build.rs
+-rw-r--r--   0     1001      127      276 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/mod.rs
+-rw-r--r--   0     1001      127     4114 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs
+-rw-r--r--   0     1001      127     5495 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs
+-rw-r--r--   0     1001      127     2337 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs
+-rw-r--r--   0     1001      127      223 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/lib.rs
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/apis/python/node/Cargo.toml
+-rw-r--r--   0     1001      127      201 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/README.md
+-rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/dora/__init__.py
+-rw-r--r--   0     1001      127     6852 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/apis/python/node/src/lib.rs
+-rw-r--r--   0     1001      127   169924 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/Cargo.lock
+-rw-r--r--   0        0        0     3959 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/Cargo.toml
+-rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/pyproject.toml
+-rw-r--r--   0     1001      127      518 2024-04-08 07:45:19.000000 dora_rs-0.3.3rc1/dora/__init__.py
+-rw-r--r--   0        0        0      452 1970-01-01 00:00:00.000000 dora_rs-0.3.3rc1/PKG-INFO
```

### Comparing `dora_rs-0.3.3/libraries/core/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/config.rs` & `dora_rs-0.3.3rc1/libraries/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/coordinator_messages.rs` & `dora_rs-0.3.3rc1/libraries/core/src/coordinator_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/daemon_messages.rs` & `dora_rs-0.3.3rc1/libraries/core/src/daemon_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/descriptor/mod.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -256,61 +256,17 @@
     pub send_stdout_as: Option<String>,
 }
 
 #[derive(Debug, Serialize, Deserialize, Clone)]
 #[serde(rename_all = "kebab-case")]
 pub enum OperatorSource {
     SharedLibrary(String),
-    Python(PythonSource),
+    Python(String),
     Wasm(String),
 }
-#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
-#[serde(
-    deny_unknown_fields,
-    from = "PythonSourceDef",
-    into = "PythonSourceDef"
-)]
-pub struct PythonSource {
-    pub source: String,
-    pub conda_env: Option<String>,
-}
-
-#[derive(Debug, Clone, PartialEq, Eq, Serialize, Deserialize)]
-#[serde(untagged)]
-pub enum PythonSourceDef {
-    SourceOnly(String),
-    WithOptions {
-        source: String,
-        conda_env: Option<String>,
-    },
-}
-
-impl From<PythonSource> for PythonSourceDef {
-    fn from(input: PythonSource) -> Self {
-        match input {
-            PythonSource {
-                source,
-                conda_env: None,
-            } => Self::SourceOnly(source),
-            PythonSource { source, conda_env } => Self::WithOptions { source, conda_env },
-        }
-    }
-}
-
-impl From<PythonSourceDef> for PythonSource {
-    fn from(value: PythonSourceDef) -> Self {
-        match value {
-            PythonSourceDef::SourceOnly(source) => Self {
-                source,
-                conda_env: None,
-            },
-            PythonSourceDef::WithOptions { source, conda_env } => Self { source, conda_env },
-        }
-    }
-}
 
 pub fn source_is_url(source: &str) -> bool {
     source.contains("://")
 }
 
 pub fn resolve_path(source: &str, working_dir: &Path) -> Result<PathBuf> {
     let path = Path::new(&source);
```

### Comparing `dora_rs-0.3.3/libraries/core/src/descriptor/validate.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/validate.rs`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,17 @@
                             } else {
                                 let path = adjust_shared_library_path(Path::new(&path))?;
                                 if !working_dir.join(&path).exists() {
                                     bail!("no shared library at `{}`", path.display());
                                 }
                             }
                         }
-                        OperatorSource::Python(python_source) => {
+                        OperatorSource::Python(path) => {
                             has_python_operator = true;
-                            let path = &python_source.source;
-                            if source_is_url(&path) {
+                            if source_is_url(path) {
                                 info!("{path} is a URL."); // TODO: Implement url check.
                             } else if !working_dir.join(path).exists() {
                                 bail!("no Python library at `{path}`");
                             }
                         }
                         OperatorSource::Wasm(path) => {
                             if source_is_url(path) {
```

### Comparing `dora_rs-0.3.3/libraries/core/src/descriptor/visualize.rs` & `dora_rs-0.3.3rc1/libraries/core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/core/src/topics.rs` & `dora_rs-0.3.3rc1/libraries/core/src/topics.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/qos.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/qos.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/python/test_utils.py` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/operator/types/src/lib.rs` & `dora_rs-0.3.3rc1/apis/rust/operator/types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/python/operator/Cargo.toml` & `dora_rs-0.3.3rc1/apis/python/operator/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/python/operator/src/lib.rs` & `dora_rs-0.3.3rc1/apis/python/operator/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/download/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/telemetry/tracing/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/telemetry/tracing/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/telemetry/tracing/src/telemetry.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/Cargo.toml` & `dora_rs-0.3.3rc1/apis/rust/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/daemon_connection/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/daemon_connection/tcp.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/event_stream/event.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/event_stream/merged.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/merged.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/event_stream/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/event_stream/thread.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/lib.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/node/arrow_utils.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/arrow_utils.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/node/control_channel.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/node/drop_stream.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/drop_stream.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/rust/node/src/node/mod.rs` & `dora_rs-0.3.3rc1/apis/rust/node/src/node/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/build.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/sequence.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/string.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/src/_core/traits.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/src/_core/traits.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/message/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/telemetry/metrics/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/telemetry/metrics/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/telemetry/metrics/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/binaries/runtime/Cargo.toml` & `dora_rs-0.3.3rc1/binaries/runtime/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/binaries/runtime/src/lib.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/binaries/runtime/src/operator/channel.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/binaries/runtime/src/operator/mod.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/binaries/runtime/src/operator/python.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/python.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #![allow(clippy::borrow_deref_ref)] // clippy warns about code generated by #[pymethods]
 
 use super::{OperatorEvent, StopReason};
 use dora_core::{
     config::{NodeId, OperatorId},
-    descriptor::{source_is_url, Descriptor, PythonSource},
+    descriptor::{source_is_url, Descriptor},
 };
 use dora_download::download_file;
 use dora_node_api::Event;
 use dora_operator_api_python::PyEvent;
 use dora_operator_api_types::DoraStatus;
 use eyre::{bail, eyre, Context, Result};
 use pyo3::{
@@ -31,33 +31,33 @@
     }
 }
 
 #[tracing::instrument(skip(events_tx, incoming_events), level = "trace")]
 pub fn run(
     node_id: &NodeId,
     operator_id: &OperatorId,
-    python_source: &PythonSource,
+    source: &str,
     events_tx: Sender<OperatorEvent>,
     incoming_events: flume::Receiver<Event>,
     init_done: oneshot::Sender<Result<()>>,
     dataflow_descriptor: &Descriptor,
 ) -> eyre::Result<()> {
-    let path = if source_is_url(&python_source.source) {
+    let path = if source_is_url(source) {
         let target_path = Path::new("build")
             .join(node_id.to_string())
             .join(format!("{}.py", operator_id));
         // try to download the shared library
         let rt = tokio::runtime::Builder::new_current_thread()
             .enable_all()
             .build()?;
-        rt.block_on(download_file(&python_source.source, &target_path))
+        rt.block_on(download_file(source, &target_path))
             .wrap_err("failed to download Python operator")?;
         target_path
     } else {
-        Path::new(&python_source.source).to_owned()
+        Path::new(source).to_owned()
     };
 
     if !path.exists() {
         bail!("No python file exists at {}", path.display());
     }
     let path = path
         .canonicalize()
```

### Comparing `dora_rs-0.3.3/binaries/runtime/src/operator/shared_lib.rs` & `dora_rs-0.3.3rc1/binaries/runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/arrow-convert/src/from_impls.rs` & `dora_rs-0.3.3rc1/libraries/arrow-convert/src/from_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/arrow-convert/src/into_impls.rs` & `dora_rs-0.3.3rc1/libraries/arrow-convert/src/into_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/build.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv` & `dora_rs-0.3.3rc1/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/shared-memory-server/Cargo.toml` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/shared-memory-server/src/channel.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/libraries/shared-memory-server/src/lib.rs` & `dora_rs-0.3.3rc1/libraries/shared-memory-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/python/node/Cargo.toml` & `dora_rs-0.3.3rc1/apis/python/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/apis/python/node/dora/__init__.py` & `dora_rs-0.3.3rc1/apis/python/node/dora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from enum import Enum
 
 from .dora import *
 
 __author__ = "Dora-rs Authors"
-__version__ = "0.3.3"
+__version__ = "0.3.3-rc1"
 
 
 class DoraStatus(Enum):
     """Dora status to indicate if operator `on_input` loop
      should be stopped.
 
     Args:
```

### Comparing `dora_rs-0.3.3/apis/python/node/src/lib.rs` & `dora_rs-0.3.3rc1/apis/python/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.3/Cargo.lock` & `dora_rs-0.3.3rc1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -707,28 +707,28 @@
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -1067,23 +1067,23 @@
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "flume 0.10.14",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.3.3"
+version = "0.3.3-rc1"
 
 [[package]]
 name = "concurrent-queue"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f057a694a54f12365049b0958a1685bb52d567f5593b355fbf685838e873d400"
 dependencies = [
@@ -1457,23 +1457,23 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dora-arrow-convert"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "eyre",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "bat",
  "clap 4.4.6",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-coordinator",
  "dora-core",
@@ -1495,15 +1495,15 @@
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
  "futures-concurrency",
@@ -1513,15 +1513,15 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
@@ -1530,15 +1530,15 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "async-trait",
  "bincode",
  "ctrlc",
  "dora-arrow-convert",
  "dora-core",
@@ -1553,20 +1553,19 @@
  "serde_yaml 0.8.26",
  "shared-memory-server",
  "tokio",
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
  "uuid",
- "which",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -1586,37 +1585,37 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow-data",
  "arrow-schema",
  "eyre",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "eyre",
  "opentelemetry 0.22.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "opentelemetry_sdk 0.22.1",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "bincode",
  "dora-arrow-convert",
  "dora-core",
  "dora-tracing",
@@ -1630,25 +1629,25 @@
  "shared_memory_extended",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow-array",
  "dora-node-api",
  "eyre",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "dora-ros2-bridge",
  "dora-ros2-bridge-msg-gen",
  "eyre",
@@ -1657,15 +1656,15 @@
  "rust-format",
  "serde",
  "serde-big-array",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-ros2-bridge-python",
  "dora-runtime",
  "eyre",
@@ -1674,72 +1673,72 @@
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-arrow-convert",
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "arrow-schema",
  "dora-node-api",
  "eyre",
  "flume 0.10.14",
  "pyo3",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "arrow",
  "dora-arrow-convert",
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-record"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "chrono",
  "dora-node-api",
  "dora-tracing",
  "eyre",
  "parquet",
  "tokio",
@@ -1794,15 +1793,15 @@
  "pyo3",
  "serde",
  "serde_assert",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "aligned-vec",
  "arrow",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
@@ -1821,15 +1820,15 @@
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
@@ -3281,33 +3280,33 @@
  "net2",
  "winapi 0.2.8",
  "ws2_32-sys",
 ]
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "names"
@@ -4738,33 +4737,33 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-operator"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rust-format"
@@ -4775,15 +4774,15 @@
  "prettyplease",
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust-ros2-dataflow-example-node"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "dora-node-api",
  "dora-ros2-bridge",
  "eyre",
  "futures",
  "futures-timer",
  "rand",
@@ -5186,15 +5185,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.3.3"
+version = "0.3.3-rc1"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory_extended",
  "tracing",
```

### Comparing `dora_rs-0.3.3/Cargo.toml` & `dora_rs-0.3.3rc1/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [workspace]
 members = ["apis/python/node", "apis/rust/*", "libraries/extensions/telemetry/*"]
 
 [workspace.package]
 # Make sure to also bump `apis/node/python/__init__.py` version.
-version = "0.3.3"
+version = "0.3.3-rc1"
 description = "`dora` goal is to be a low latency, composable, and distributed data flow."
 documentation = "https://dora.carsmos.ai"
 license = "Apache-2.0"
 
 [workspace.dependencies]
-dora-node-api = { version = "0.3.3", path = "apis/rust/node", default-features = false }
-dora-node-api-python = { version = "0.3.3", path = "apis/python/node", default-features = false }
-dora-operator-api = { version = "0.3.3", path = "apis/rust/operator", default-features = false }
-dora-operator-api-macros = { version = "0.3.3", path = "apis/rust/operator/macros" }
-dora-operator-api-types = { version = "0.3.3", path = "apis/rust/operator/types" }
-dora-operator-api-python = { version = "0.3.3", path = "apis/python/operator" }
-dora-operator-api-c = { version = "0.3.3", path = "apis/c/operator" }
-dora-node-api-c = { version = "0.3.3", path = "apis/c/node" }
-dora-core = { version = "0.3.3", path = "libraries/core" }
-dora-arrow-convert = { version = "0.3.3", path = "libraries/arrow-convert" }
-dora-tracing = { version = "0.3.3", path = "libraries/extensions/telemetry/tracing" }
-dora-metrics = { version = "0.3.3", path = "libraries/extensions/telemetry/metrics" }
-dora-download = { version = "0.3.3", path = "libraries/extensions/download" }
-shared-memory-server = { version = "0.3.3", path = "libraries/shared-memory-server" }
-communication-layer-request-reply = { version = "0.3.3", path = "libraries/communication-layer/request-reply" }
-dora-message = { version = "0.3.3", path = "libraries/message" }
-dora-runtime = { version = "0.3.3", path = "binaries/runtime" }
-dora-daemon = { version = "0.3.3", path = "binaries/daemon" }
-dora-coordinator = { version = "0.3.3", path = "binaries/coordinator" }
+dora-node-api = { version = "0.3.3-rc1", path = "apis/rust/node", default-features = false }
+dora-node-api-python = { version = "0.3.3-rc1", path = "apis/python/node", default-features = false }
+dora-operator-api = { version = "0.3.3-rc1", path = "apis/rust/operator", default-features = false }
+dora-operator-api-macros = { version = "0.3.3-rc1", path = "apis/rust/operator/macros" }
+dora-operator-api-types = { version = "0.3.3-rc1", path = "apis/rust/operator/types" }
+dora-operator-api-python = { version = "0.3.3-rc1", path = "apis/python/operator" }
+dora-operator-api-c = { version = "0.3.3-rc1", path = "apis/c/operator" }
+dora-node-api-c = { version = "0.3.3-rc1", path = "apis/c/node" }
+dora-core = { version = "0.3.3-rc1", path = "libraries/core" }
+dora-arrow-convert = { version = "0.3.3-rc1", path = "libraries/arrow-convert" }
+dora-tracing = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/tracing" }
+dora-metrics = { version = "0.3.3-rc1", path = "libraries/extensions/telemetry/metrics" }
+dora-download = { version = "0.3.3-rc1", path = "libraries/extensions/download" }
+shared-memory-server = { version = "0.3.3-rc1", path = "libraries/shared-memory-server" }
+communication-layer-request-reply = { version = "0.3.3-rc1", path = "libraries/communication-layer/request-reply" }
+dora-message = { version = "0.3.3-rc1", path = "libraries/message" }
+dora-runtime = { version = "0.3.3-rc1", path = "binaries/runtime" }
+dora-daemon = { version = "0.3.3-rc1", path = "binaries/daemon" }
+dora-coordinator = { version = "0.3.3-rc1", path = "binaries/coordinator" }
 dora-ros2-bridge = { path = "libraries/extensions/ros2-bridge" }
 dora-ros2-bridge-msg-gen = { path = "libraries/extensions/ros2-bridge/msg-gen" }
 dora-ros2-bridge-python = { path = "libraries/extensions/ros2-bridge/python" }
 arrow = "48.0.0"
 arrow-schema = "48.0.0"
 arrow-data = "48.0.0"
 arrow-array = "48.0.0"
@@ -56,15 +56,15 @@
 dora-core = { workspace = true }
 dora-tracing = { workspace = true }
 dora-download = { workspace = true }
 dunce = "1.0.2"
 serde_yaml = "0.8.23"
 uuid = { version = "1.7", features = ["v7", "serde"] }
 tracing = "0.1.36"
-futures = "0.3.25"
+futures = "0.3.3-rc15"
 tokio-stream = "0.1.11"
 
 [[example]]
 name = "c-dataflow"
 path = "examples/c-dataflow/run.rs"
 
 [[example]]
```

### Comparing `dora_rs-0.3.3/dora/__init__.py` & `dora_rs-0.3.3rc1/dora/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 from enum import Enum
 
 from .dora import *
 
 __author__ = "Dora-rs Authors"
-__version__ = "0.3.3"
+__version__ = "0.3.3-rc1"
 
 
 class DoraStatus(Enum):
     """Dora status to indicate if operator `on_input` loop
      should be stopped.
 
     Args:
```

