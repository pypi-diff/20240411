# Comparing `tmp/openfabric_pysdk-0.2.8.tar.gz` & `tmp/openfabric_pysdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfabric_pysdk-0.2.8.tar", max compression
+gzip compressed data, was "openfabric_pysdk-0.2.9.tar", max compression
```

## Comparing `openfabric_pysdk-0.2.8.tar` & `openfabric_pysdk-0.2.9.tar`

### file list

```diff
@@ -1,78 +1,81 @@
--rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.8/README.md
--rw-r--r--   0        0        0        1 2023-12-02 20:01:49.456768 openfabric_pysdk-0.2.8/openfabric_pysdk/__init__.py
--rw-r--r--   0        0        0      348 2023-12-02 20:02:07.831742 openfabric_pysdk-0.2.8/openfabric_pysdk/api/__init__.py
--rw-r--r--   0        0        0       21 2023-04-30 07:33:24.749243 openfabric_pysdk-0.2.8/openfabric_pysdk/app/__init__.py
--rw-r--r--   0        0        0     7292 2023-12-03 08:34:14.629806 openfabric_pysdk-0.2.8/openfabric_pysdk/app/app.py
--rw-r--r--   0        0        0     4004 2023-12-03 08:34:14.647076 openfabric_pysdk-0.2.8/openfabric_pysdk/app/comm.py
--rwxr-xr-x   0        0        0    11614 2023-12-03 09:00:29.587508 openfabric_pysdk-0.2.8/openfabric_pysdk/app/worker.py
--rw-r--r--   0        0        0       67 2023-04-30 07:33:24.750402 openfabric_pysdk-0.2.8/openfabric_pysdk/benchmark/__init__.py
--rw-r--r--   0        0        0     3606 2023-04-30 07:33:24.751474 openfabric_pysdk-0.2.8/openfabric_pysdk/benchmark/time_benchmark.py
--rw-r--r--   0        0        0      282 2023-04-30 07:33:24.751836 openfabric_pysdk-0.2.8/openfabric_pysdk/context/__init__.py
--rw-r--r--   0        0        0      178 2023-12-02 20:01:49.458730 openfabric_pysdk-0.2.8/openfabric_pysdk/context/bar.py
--rw-r--r--   0        0        0      485 2023-12-02 20:02:07.833178 openfabric_pysdk-0.2.8/openfabric_pysdk/context/bar_schema.py
--rw-r--r--   0        0        0     1224 2023-04-30 07:33:24.753644 openfabric_pysdk-0.2.8/openfabric_pysdk/context/message.py
--rw-r--r--   0        0        0      607 2023-12-02 20:02:07.833889 openfabric_pysdk-0.2.8/openfabric_pysdk/context/message_schema.py
--rw-r--r--   0        0        0     4567 2023-12-02 20:02:07.834173 openfabric_pysdk-0.2.8/openfabric_pysdk/context/ray.py
--rw-r--r--   0        0        0      933 2023-12-02 20:02:07.834363 openfabric_pysdk-0.2.8/openfabric_pysdk/context/ray_schema.py
--rw-r--r--   0        0        0      861 2023-04-30 07:33:24.755605 openfabric_pysdk-0.2.8/openfabric_pysdk/context/state.py
--rw-r--r--   0        0        0      313 2023-04-30 07:33:24.755983 openfabric_pysdk-0.2.8/openfabric_pysdk/context/state_schema.py
--rw-r--r--   0        0        0       27 2023-12-02 20:02:07.834560 openfabric_pysdk-0.2.8/openfabric_pysdk/engine/__init__.py
--rw-r--r--   0        0        0     6085 2023-12-02 20:02:07.834931 openfabric_pysdk-0.2.8/openfabric_pysdk/engine/engine.py
--rw-r--r--   0        0        0       62 2023-04-30 07:33:24.758547 openfabric_pysdk-0.2.8/openfabric_pysdk/execution/__init__.py
--rw-r--r--   0        0        0     4745 2023-12-02 20:01:49.462437 openfabric_pysdk-0.2.8/openfabric_pysdk/execution/container.py
--rw-r--r--   0        0        0      522 2023-12-02 20:01:49.462774 openfabric_pysdk-0.2.8/openfabric_pysdk/execution/profile.py
--rw-r--r--   0        0        0       49 2023-04-30 07:33:24.761730 openfabric_pysdk-0.2.8/openfabric_pysdk/fields/__init__.py
--rw-r--r--   0        0        0       62 2023-04-30 07:33:24.762486 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/__init__.py
--rw-r--r--   0        0        0      908 2023-12-02 20:02:07.835169 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/core/__init__.py
--rw-r--r--   0        0        0      423 2023-04-30 07:33:24.764277 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/rest/__init__.py
--rw-r--r--   0        0        0      131 2023-04-30 07:33:24.764893 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/socket/__init__.py
--rw-r--r--   0        0        0      339 2023-04-30 07:33:24.765183 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/socket/socketio_client.py
--rw-r--r--   0        0        0      703 2023-04-30 07:33:24.765747 openfabric_pysdk-0.2.8/openfabric_pysdk/flask/socket/socketio_server.py
--rw-r--r--   0        0        0       25 2023-12-03 08:27:41.693092 openfabric_pysdk-0.2.8/openfabric_pysdk/helper/__init__.py
--rwxr-xr-x   0        0        0    17722 2024-01-31 15:27:56.027849 openfabric_pysdk-0.2.8/openfabric_pysdk/helper/proxy.py
--rw-r--r--   0        0        0      464 2023-12-02 20:02:07.836434 openfabric_pysdk-0.2.8/openfabric_pysdk/loader/__init__.py
--rw-r--r--   0        0        0      411 2023-04-30 07:33:24.766884 openfabric_pysdk-0.2.8/openfabric_pysdk/loader/config.py
--rw-r--r--   0        0        0      208 2023-12-02 20:01:49.464294 openfabric_pysdk-0.2.8/openfabric_pysdk/service/__init__.py
--rw-r--r--   0        0        0     1840 2023-12-02 20:01:49.464952 openfabric_pysdk-0.2.8/openfabric_pysdk/service/config_service.py
--rw-r--r--   0        0        0     1443 2023-04-30 07:33:24.768243 openfabric_pysdk-0.2.8/openfabric_pysdk/service/remote_service.py
--rw-r--r--   0        0        0     1007 2023-04-30 07:33:24.768766 openfabric_pysdk-0.2.8/openfabric_pysdk/service/rest_service.py
--rw-r--r--   0        0        0     2199 2023-05-21 17:16:05.359939 openfabric_pysdk-0.2.8/openfabric_pysdk/service/socket_service.py
--rw-r--r--   0        0        0     1477 2023-04-30 07:33:24.769946 openfabric_pysdk-0.2.8/openfabric_pysdk/service/swagger_service.py
--rw-r--r--   0        0        0     1436 2023-12-02 20:01:49.465767 openfabric_pysdk-0.2.8/openfabric_pysdk/starter.py
--rw-r--r--   0        0        0       75 2023-12-02 20:01:49.466355 openfabric_pysdk-0.2.8/openfabric_pysdk/store/__init__.py
--rw-r--r--   0        0        0     2814 2023-12-02 20:02:07.836967 openfabric_pysdk-0.2.8/openfabric_pysdk/store/kvdb.py
--rw-r--r--   0        0        0     1438 2023-04-30 07:33:24.771791 openfabric_pysdk-0.2.8/openfabric_pysdk/store/lru.py
--rw-r--r--   0        0        0     2361 2023-12-02 20:02:07.837166 openfabric_pysdk-0.2.8/openfabric_pysdk/store/store.py
--rw-r--r--   0        0        0     3114 2023-12-02 20:02:07.837514 openfabric_pysdk-0.2.8/openfabric_pysdk/task.py
--rw-r--r--   0        0        0       52 2023-04-30 07:33:24.772326 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/__init__.py
--rw-r--r--   0        0        0      308 2023-04-30 07:33:24.772612 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/resource_descriptor.py
--rw-r--r--   0        0        0        1 2023-04-30 07:33:24.772728 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/__init__.py
--rw-r--r--   0        0        0      230 2023-04-30 07:33:24.773153 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/__init__.py
--rw-r--r--   0        0        0      933 2023-12-02 20:01:49.467940 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/benchmark_api.py
--rw-r--r--   0        0        0     1674 2023-12-02 20:01:49.468501 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/config_api.py
--rw-r--r--   0        0        0     1116 2023-12-02 20:02:07.837728 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/execution_api.py
--rw-r--r--   0        0        0     1040 2023-07-30 06:10:23.989543 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/manifest_api.py
--rw-r--r--   0        0        0     2818 2023-12-02 20:02:07.838038 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/queue_api.py
--rw-r--r--   0        0        0      256 2023-05-20 05:27:06.116771 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/__init__.py
--rw-r--r--   0        0        0      943 2023-04-30 07:33:24.776948 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/benchmark_api.py
--rw-r--r--   0        0        0     1864 2023-04-30 07:33:24.777581 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/config_api.py
--rw-r--r--   0        0        0     1015 2023-04-30 07:33:24.778047 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/execution_api.py
--rw-r--r--   0        0        0      966 2023-04-30 07:33:24.778209 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/manifest_api.py
--rw-r--r--   0        0        0     3036 2023-04-30 07:33:24.778366 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/queue_api.py
--rw-r--r--   0        0        0      135 2023-04-30 07:33:24.778771 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/__init__.py
--rw-r--r--   0        0        0      529 2023-04-30 07:33:24.779464 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/benchmark_schema.py
--rw-r--r--   0        0        0      852 2023-04-30 07:33:24.779824 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/manifest_schema.py
--rw-r--r--   0        0        0      453 2023-04-30 07:33:24.780025 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/uid_schema.py
--rw-r--r--   0        0        0        0 2023-04-30 07:33:24.780094 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/__init__.py
--rw-r--r--   0        0        0       45 2023-04-30 07:33:24.780365 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/local/__init__.py
--rw-r--r--   0        0        0     7786 2023-12-08 14:00:37.194347 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/local/execution_socket.py
--rw-r--r--   0        0        0       71 2023-05-20 05:27:06.117732 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/remote/__init__.py
--rw-r--r--   0        0        0     3954 2023-04-30 07:33:24.780960 openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/remote/execution_socket.py
--rw-r--r--   0        0        0      138 2023-04-30 07:33:24.781197 openfabric_pysdk-0.2.8/openfabric_pysdk/utility/__init__.py
--rw-r--r--   0        0        0      679 2023-04-30 07:33:24.781459 openfabric_pysdk-0.2.8/openfabric_pysdk/utility/change_util.py
--rw-r--r--   0        0        0     1874 2023-12-02 20:02:07.838519 openfabric_pysdk-0.2.8/openfabric_pysdk/utility/loader_util.py
--rw-r--r--   0        0        0      345 2023-04-30 07:33:24.782179 openfabric_pysdk-0.2.8/openfabric_pysdk/utility/schema_util.py
--rw-r--r--   0        0        0      890 2023-04-30 07:33:24.782442 openfabric_pysdk-0.2.8/openfabric_pysdk/utility/zip_util.py
--rw-r--r--   0        0        0    13433 2023-04-30 07:33:24.783125 openfabric_pysdk-0.2.8/openfabric_pysdk/view/index.html
--rw-r--r--   0        0        0      962 2024-01-31 15:31:39.489174 openfabric_pysdk-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-07 14:53:56.463341 openfabric_pysdk-0.2.9/README.md
+-rw-r--r--   0        0        0        1 2024-02-02 06:09:55.276615 openfabric_pysdk-0.2.9/openfabric_pysdk/__init__.py
+-rw-r--r--   0        0        0      348 2024-02-02 06:09:55.276897 openfabric_pysdk-0.2.9/openfabric_pysdk/api/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-30 07:33:24.749243 openfabric_pysdk-0.2.9/openfabric_pysdk/app/__init__.py
+-rw-r--r--   0        0        0     7312 2024-02-27 15:14:15.128810 openfabric_pysdk-0.2.9/openfabric_pysdk/app/app.py
+-rw-r--r--   0        0        0     4004 2024-02-27 15:13:50.782570 openfabric_pysdk-0.2.9/openfabric_pysdk/app/comm.py
+-rwxr-xr-x   0        0        0    11632 2024-03-06 17:04:25.174179 openfabric_pysdk-0.2.9/openfabric_pysdk/app/worker.py
+-rw-r--r--   0        0        0       67 2023-04-30 07:33:24.750402 openfabric_pysdk-0.2.9/openfabric_pysdk/benchmark/__init__.py
+-rw-r--r--   0        0        0     3606 2023-04-30 07:33:24.751474 openfabric_pysdk-0.2.9/openfabric_pysdk/benchmark/time_benchmark.py
+-rw-r--r--   0        0        0      282 2023-04-30 07:33:24.751836 openfabric_pysdk-0.2.9/openfabric_pysdk/context/__init__.py
+-rw-r--r--   0        0        0      178 2024-02-02 06:09:55.277734 openfabric_pysdk-0.2.9/openfabric_pysdk/context/bar.py
+-rw-r--r--   0        0        0      485 2024-02-02 06:09:55.278327 openfabric_pysdk-0.2.9/openfabric_pysdk/context/bar_schema.py
+-rw-r--r--   0        0        0     1224 2024-02-27 15:13:50.784134 openfabric_pysdk-0.2.9/openfabric_pysdk/context/message.py
+-rw-r--r--   0        0        0      607 2024-02-02 06:09:55.278591 openfabric_pysdk-0.2.9/openfabric_pysdk/context/message_schema.py
+-rw-r--r--   0        0        0     4567 2024-02-27 15:13:50.785249 openfabric_pysdk-0.2.9/openfabric_pysdk/context/ray.py
+-rw-r--r--   0        0        0      933 2024-02-02 06:09:55.279610 openfabric_pysdk-0.2.9/openfabric_pysdk/context/ray_schema.py
+-rw-r--r--   0        0        0      861 2023-04-30 07:33:24.755605 openfabric_pysdk-0.2.9/openfabric_pysdk/context/state.py
+-rw-r--r--   0        0        0      313 2023-04-30 07:33:24.755983 openfabric_pysdk-0.2.9/openfabric_pysdk/context/state_schema.py
+-rw-r--r--   0        0        0       27 2024-02-02 06:09:55.279902 openfabric_pysdk-0.2.9/openfabric_pysdk/engine/__init__.py
+-rw-r--r--   0        0        0     6085 2024-02-02 06:09:55.280177 openfabric_pysdk-0.2.9/openfabric_pysdk/engine/engine.py
+-rw-r--r--   0        0        0       62 2023-04-30 07:33:24.758547 openfabric_pysdk-0.2.9/openfabric_pysdk/execution/__init__.py
+-rw-r--r--   0        0        0     4745 2024-04-11 10:14:12.069745 openfabric_pysdk-0.2.9/openfabric_pysdk/execution/container.py
+-rw-r--r--   0        0        0      522 2024-02-02 06:09:55.281480 openfabric_pysdk-0.2.9/openfabric_pysdk/execution/profile.py
+-rw-r--r--   0        0        0      124 2024-04-11 08:44:00.539176 openfabric_pysdk-0.2.9/openfabric_pysdk/fields/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-30 07:33:24.762486 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/__init__.py
+-rw-r--r--   0        0        0      908 2024-02-02 06:09:55.281702 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/core/__init__.py
+-rw-r--r--   0        0        0      423 2023-04-30 07:33:24.764277 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/rest/__init__.py
+-rw-r--r--   0        0        0      131 2023-04-30 07:33:24.764893 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/socket/__init__.py
+-rw-r--r--   0        0        0      339 2023-04-30 07:33:24.765183 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/socket/socketio_client.py
+-rw-r--r--   0        0        0      703 2023-04-30 07:33:24.765747 openfabric_pysdk-0.2.9/openfabric_pysdk/flask/socket/socketio_server.py
+-rw-r--r--   0        0        0       25 2023-12-03 08:27:41.693092 openfabric_pysdk-0.2.9/openfabric_pysdk/helper/__init__.py
+-rwxr-xr-x   0        0        0    17722 2024-02-02 06:09:55.282492 openfabric_pysdk-0.2.9/openfabric_pysdk/helper/proxy.py
+-rw-r--r--   0        0        0      464 2024-02-01 15:30:18.808593 openfabric_pysdk-0.2.9/openfabric_pysdk/loader/__init__.py
+-rw-r--r--   0        0        0      411 2024-02-01 15:30:18.808745 openfabric_pysdk-0.2.9/openfabric_pysdk/loader/config.py
+-rw-r--r--   0        0        0      306 2024-04-11 10:21:45.242841 openfabric_pysdk-0.2.9/openfabric_pysdk/service/__init__.py
+-rw-r--r--   0        0        0     1840 2024-02-02 06:09:55.283304 openfabric_pysdk-0.2.9/openfabric_pysdk/service/config_service.py
+-rw-r--r--   0        0        0      347 2024-04-11 10:16:05.532339 openfabric_pysdk-0.2.9/openfabric_pysdk/service/environment_service.py
+-rw-r--r--   0        0        0     1861 2024-04-11 10:43:49.941480 openfabric_pysdk-0.2.9/openfabric_pysdk/service/property_service.py
+-rw-r--r--   0        0        0     2177 2024-04-11 09:13:39.724005 openfabric_pysdk-0.2.9/openfabric_pysdk/service/remote_service.py
+-rw-r--r--   0        0        0     1007 2023-04-30 07:33:24.768766 openfabric_pysdk-0.2.9/openfabric_pysdk/service/rest_service.py
+-rw-r--r--   0        0        0     2199 2023-05-21 17:16:05.359939 openfabric_pysdk-0.2.9/openfabric_pysdk/service/socket_service.py
+-rw-r--r--   0        0        0     1477 2023-04-30 07:33:24.769946 openfabric_pysdk-0.2.9/openfabric_pysdk/service/swagger_service.py
+-rw-r--r--   0        0        0     1436 2024-02-02 06:09:55.283727 openfabric_pysdk-0.2.9/openfabric_pysdk/starter.py
+-rw-r--r--   0        0        0       75 2024-02-02 06:09:55.284206 openfabric_pysdk-0.2.9/openfabric_pysdk/store/__init__.py
+-rw-r--r--   0        0        0     2814 2024-02-02 06:09:55.284774 openfabric_pysdk-0.2.9/openfabric_pysdk/store/kvdb.py
+-rw-r--r--   0        0        0     1438 2023-04-30 07:33:24.771791 openfabric_pysdk-0.2.9/openfabric_pysdk/store/lru.py
+-rw-r--r--   0        0        0     2361 2024-02-02 06:09:55.285097 openfabric_pysdk-0.2.9/openfabric_pysdk/store/store.py
+-rw-r--r--   0        0        0     3114 2024-02-27 15:13:50.785839 openfabric_pysdk-0.2.9/openfabric_pysdk/task.py
+-rw-r--r--   0        0        0       52 2023-04-30 07:33:24.772326 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-30 07:33:24.772612 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/resource_descriptor.py
+-rw-r--r--   0        0        0        1 2023-04-30 07:33:24.772728 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-11 10:22:18.047343 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/__init__.py
+-rw-r--r--   0        0        0      933 2024-02-02 06:09:55.285839 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/benchmark_api.py
+-rw-r--r--   0        0        0     1662 2024-04-10 09:54:10.603223 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/config_api.py
+-rw-r--r--   0        0        0     1110 2024-04-10 09:54:10.611040 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/execution_api.py
+-rw-r--r--   0        0        0     1202 2024-04-11 10:37:20.148464 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/manifest_api.py
+-rw-r--r--   0        0        0     2818 2024-02-02 06:09:55.286626 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/queue_api.py
+-rw-r--r--   0        0        0      256 2024-04-11 10:22:16.295955 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/__init__.py
+-rw-r--r--   0        0        0      943 2023-04-30 07:33:24.776948 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/benchmark_api.py
+-rw-r--r--   0        0        0     1852 2024-04-10 09:54:10.605344 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/config_api.py
+-rw-r--r--   0        0        0     1009 2024-04-10 09:54:10.600169 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/execution_api.py
+-rw-r--r--   0        0        0      966 2023-04-30 07:33:24.778209 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/manifest_api.py
+-rw-r--r--   0        0        0     3036 2024-02-01 15:30:18.811330 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/queue_api.py
+-rw-r--r--   0        0        0      189 2024-04-11 10:35:17.704707 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/__init__.py
+-rw-r--r--   0        0        0      529 2023-04-30 07:33:24.779464 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/benchmark_schema.py
+-rw-r--r--   0        0        0      919 2024-04-11 10:37:20.152987 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/manifest_schema.py
+-rw-r--r--   0        0        0     1040 2024-04-11 08:44:00.534615 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/property_schema.py
+-rw-r--r--   0        0        0      453 2023-04-30 07:33:24.780025 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/uid_schema.py
+-rw-r--r--   0        0        0        0 2023-04-30 07:33:24.780094 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/__init__.py
+-rw-r--r--   0        0        0       45 2023-04-30 07:33:24.780365 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/local/__init__.py
+-rw-r--r--   0        0        0     7786 2024-02-27 15:13:50.786480 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/local/execution_socket.py
+-rw-r--r--   0        0        0       71 2023-05-20 05:27:06.117732 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/remote/__init__.py
+-rw-r--r--   0        0        0     3954 2023-04-30 07:33:24.780960 openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/remote/execution_socket.py
+-rw-r--r--   0        0        0      138 2024-02-01 14:18:30.995987 openfabric_pysdk-0.2.9/openfabric_pysdk/utility/__init__.py
+-rw-r--r--   0        0        0      679 2023-04-30 07:33:24.781459 openfabric_pysdk-0.2.9/openfabric_pysdk/utility/change_util.py
+-rw-r--r--   0        0        0     1874 2024-02-02 06:09:55.287185 openfabric_pysdk-0.2.9/openfabric_pysdk/utility/loader_util.py
+-rw-r--r--   0        0        0      345 2023-04-30 07:33:24.782179 openfabric_pysdk-0.2.9/openfabric_pysdk/utility/schema_util.py
+-rw-r--r--   0        0        0      890 2023-04-30 07:33:24.782442 openfabric_pysdk-0.2.9/openfabric_pysdk/utility/zip_util.py
+-rw-r--r--   0        0        0    13433 2023-04-30 07:33:24.783125 openfabric_pysdk-0.2.9/openfabric_pysdk/view/index.html
+-rw-r--r--   0        0        0      994 2024-04-11 07:19:47.562529 openfabric_pysdk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1468 1970-01-01 00:00:00.000000 openfabric_pysdk-0.2.9/PKG-INFO
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/app/app.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/app/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from openfabric_pysdk.context import Ray, State, StateStatus, RaySchema, RayStatus, StateSchema
 from openfabric_pysdk.loader import ConfigClass, InputClass, OutputClass
 from openfabric_pysdk.loader.config import manifest, state_config
 from openfabric_pysdk.store import KeyValueDB
 
-from .comm import Subscriber, Publisher, DispatchMessage, DispatchActions
+from openfabric_pysdk.app.comm import Subscriber, Publisher, DispatchMessage, DispatchActions
 
 my_env = os.environ.copy()
 if "PYTHONPATH" in my_env:
     my_env["PYTHONPATH"] = f"{os.getcwd()}:{my_env['PYTHONPATH']}"
 else:
     my_env["PYTHONPATH"] = os.getcwd()
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/app/comm.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/app/comm.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/app/worker.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/app/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         except (KeyboardInterrupt, SystemExit):
             raise
         except:
             self.handleError(record)
 
 
 class Worker:
-    __db__path: KeyValueDB = f"{os.getcwd()}/datastore"
+    __db__path: str = f"{os.getcwd()}/datastore"
 
     def __init__(self):
         self.state = State()
 
     # ------------------------------------------------------------------------
     def process(self, qid):
 
@@ -189,15 +189,15 @@
         if current_qid is not None:
             working = True
             try:
                 worker.process(current_qid)
             except:
                 # TODO: fix this.
                 # try catch should be in process, but it's relating to reading the db
-                logging.error(f"Failed to execute {current_qid}")
+                logging.error(f"Failed to execute {current_qid} {traceback.format_exc()}")
                 pass
             retry_counter = 10 * suspend_request_time_s
         else:
             if retry_counter > 0:
                 retry_counter -= 1
             else:
                 working = False
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/benchmark/time_benchmark.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/benchmark/time_benchmark.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/context/message.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/context/message.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/context/message_schema.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/context/message_schema.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/context/ray.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/context/ray.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/context/ray_schema.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/context/ray_schema.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/context/state.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/context/state.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/engine/engine.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/engine/engine.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/execution/container.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/execution/container.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/execution/profile.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/execution/profile.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/flask/core/__init__.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/flask/core/__init__.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/flask/socket/socketio_server.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/flask/socket/socketio_server.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/helper/proxy.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/helper/proxy.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/service/config_service.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/service/config_service.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/service/rest_service.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/service/rest_service.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/service/socket_service.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/service/socket_service.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/service/swagger_service.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/service/swagger_service.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/starter.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/starter.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/store/kvdb.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/store/kvdb.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/store/lru.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/store/lru.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/store/store.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/store/store.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/task.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/task.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/benchmark_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/benchmark_api.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/config_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/config_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
     # ------------------------------------------------------------------------
-    @doc(description="Get APP configuration", tags=["Developer"])
+    @doc(description="Get APP configuration", tags=["App"])
     @use_kwargs(UserIdSchema, location='query')
     @marshal_with(ConfigSchema)
     def get(self, uid: UserId) -> ConfigClass:
         with MeasureBlockTime("ConfigRestApi::get"):
             app = self.__descriptor.app
             return ConfigService.read(app, uid)
 
     # ------------------------------------------------------------------------
-    @doc(description="Set APP configuration", tags=["Developer"])
+    @doc(description="Set APP configuration", tags=["App"])
     @use_kwargs(UserIdSchema, location='query')
     @use_kwargs(ConfigSchema, location='json')
     @marshal_with(ConfigSchema)
     def post(self, uid: UserId, config: Union[ConfigClass, List[ConfigClass]]) -> ConfigClass:
         with MeasureBlockTime("ConfigRestApi::post"):
             app = self.__descriptor.app
             return ConfigService.write(app, uid, config)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/execution_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/execution_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
     # ------------------------------------------------------------------------
-    @doc(description="Execute execution and get response", tags=["Execution"])
+    @doc(description="Execute execution and get response", tags=["App"])
     @use_kwargs(InputSchema, location='json')
     @marshal_with(OutputSchema)
     def post(self, *args) -> OutputClass:
         sid = uuid.uuid4().hex
         data = InputSchema().dump(list(args) if InputSchema().many is True else args[0])
         app = self.__descriptor.app
         qid = engine.prepare(app, data, sid=sid)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/manifest_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/benchmark_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from typing import Any, Dict
-
-from openfabric_pysdk.loader import *
-from openfabric_pysdk.flask.rest import *
-from openfabric_pysdk.context import State
-from openfabric_pysdk.benchmark import MeasureBlockTime
+from openfabric_pysdk.flask import *
+from openfabric_pysdk.service import RemoteService
 from openfabric_pysdk.transport import ResourceDescriptor
-from openfabric_pysdk.transport.schema import ManifestSchema
+from openfabric_pysdk.transport.schema import BenchmarkSchema
 
 
 #######################################################
-#  Manifest API
+#  Benchmark API
 #######################################################
-class ManifestApi(MethodResource, Resource):
+class BenchmarkApi(MethodResource, Resource):
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
     # ------------------------------------------------------------------------
-    @doc(description="Get APP manifest", tags=["Developer"])
-    @marshal_with(ManifestSchema)
+    @doc(description="Get APP benchmarks", tags=["Developer"])
+    @marshal_with(BenchmarkSchema)
     def get(self):
-        with MeasureBlockTime("ManifestRestApi::get"):
-            return self.__descriptor.app.get_manifest().all()
+        url = f"{self.__descriptor.remote}/{self.__descriptor.endpoint}"
+        return RemoteService.get(url, BenchmarkSchema().load)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/local/queue_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/local/queue_api.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/benchmark_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/manifest_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Any, Dict
+
 from openfabric_pysdk.flask import *
 from openfabric_pysdk.service import RemoteService
 from openfabric_pysdk.transport import ResourceDescriptor
-from openfabric_pysdk.transport.schema import BenchmarkSchema
+from openfabric_pysdk.transport.schema import ManifestSchema
 
 
 #######################################################
-#  Benchmark API
+#  Manifest API
 #######################################################
-class BenchmarkApi(MethodResource, Resource):
+class ManifestApi(MethodResource, Resource):
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
     # ------------------------------------------------------------------------
-    @doc(description="Get APP benchmarks", tags=["Developer"])
-    @marshal_with(BenchmarkSchema)
+    @doc(description="Get APP manifest", tags=["Developer"])
+    @marshal_with(ManifestSchema)
     def get(self):
         url = f"{self.__descriptor.remote}/{self.__descriptor.endpoint}"
-        return RemoteService.get(url, BenchmarkSchema().load)
+        return RemoteService.get(url, ManifestSchema().load)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/config_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/config_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
     # ------------------------------------------------------------------------
-    @doc(description="Get APP configuration", tags=["Developer"])
+    @doc(description="Get APP configuration", tags=["App"])
     @use_kwargs(UserIdSchema, location='query')
     @marshal_with(ConfigSchema)
     def get(self, uidc: UserId) -> ConfigClass:
         url = f"{self.__descriptor.remote}/{self.__descriptor.endpoint}?uid={uidc.uid}"
         return RemoteService.get(url, ConfigSchema().load)
 
     # ------------------------------------------------------------------------
-    @doc(description="Set APP configuration", tags=["Developer"])
+    @doc(description="Set APP configuration", tags=["App"])
     @use_kwargs(UserIdSchema, location='query')
     @use_kwargs(ConfigSchema, location='json')
     @marshal_with(ConfigSchema)
     def post(self, uidc: UserId, config: Union[ConfigClass, List[ConfigClass]]) -> ConfigClass:
 
         if ConfigSchema().many is True and not isinstance(config, list):
             config = [config]
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/execution_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/execution_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 class ExecutionApi(MethodResource, Resource):
     __descriptor: ResourceDescriptor = None
 
     # ------------------------------------------------------------------------
     def __init__(self, descriptor: ResourceDescriptor = None):
         self.__descriptor = descriptor
 
-    @doc(description="Execute execution and get response", tags=["Execution"])
+    @doc(description="Execute execution and get response", tags=["App"])
     @use_kwargs(InputSchema, location='json')
     @marshal_with(OutputSchema)
     def post(self, *args) -> OutputClass:
         data = InputSchema().dump(list(args) if InputSchema().many is True else args[0])
         url = f"{self.__descriptor.remote}/{self.__descriptor.endpoint}"
         return RemoteService.post(url, data, OutputSchema().load)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/rest/remote/queue_api.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/rest/remote/queue_api.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/benchmark_schema.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/benchmark_schema.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/schema/manifest_schema.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/schema/manifest_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,10 +9,11 @@
     version = fields.String(description="App version", allow_none=True)
     description = fields.String(description="APP description", allow_none=True)
     organization = fields.String(description="APP organization", allow_none=True)
     sdk = fields.String(description="APP sdk", allow_none=True)
     overview = fields.String(description="APP overview", allow_none=True)
     input = fields.String(description="APP input", allow_none=True)
     output = fields.String(description="APP output", allow_none=True)
+    dos = fields.String(description="APP output", allow_none=True)
 
     def __init__(self):
         super().__init__(many=False)
```

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/local/execution_socket.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/local/execution_socket.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/transport/socket/remote/execution_socket.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/transport/socket/remote/execution_socket.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/utility/change_util.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/utility/change_util.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/utility/loader_util.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/utility/loader_util.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/utility/zip_util.py` & `openfabric_pysdk-0.2.9/openfabric_pysdk/utility/zip_util.py`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/openfabric_pysdk/view/index.html` & `openfabric_pysdk-0.2.9/openfabric_pysdk/view/index.html`

 * *Files identical despite different names*

### Comparing `openfabric_pysdk-0.2.8/pyproject.toml` & `openfabric_pysdk-0.2.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "openfabric-pysdk"
-version = "0.2.8"
+version = "0.2.9"
 description = "Openfabric Python SDK"
 authors = ["Andrei Tara <andrei@openfabric.ai>"]
 readme = "README.md"
 homepage = "https://openfabric.ai"
 repository = "https://github.com/Openfabric/openfabic-pysdk"
-keywords = ["openfabric", "SDK", "IoAI"]
+keywords = ["Openfabric", "SDK", "IoAI"]
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
@@ -25,14 +25,15 @@
 tqdm = "^4.62.3"
 Werkzeug = ">=2.0.3"
 marshmallow-enum = "^1.5.1"
 gevent = "^22.10.2"
 gevent-websocket = "^0.10.1"
 socketio-client = "^0.7.2"
 pyzmq = "^25.1.1"
+marshmallow-jsonapi = "^0.24.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openfabric_pysdk-0.2.8/PKG-INFO` & `openfabric_pysdk-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: openfabric-pysdk
-Version: 0.2.8
+Version: 0.2.9
 Summary: Openfabric Python SDK
 Home-page: https://openfabric.ai
-Keywords: openfabric,SDK,IoAI
+Keywords: Openfabric,SDK,IoAI
 Author: Andrei Tara
 Author-email: andrei@openfabric.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2.0.1,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-RESTful (>=0.3.9,<0.4.0)
 Requires-Dist: Flask-SocketIO (>=5.3.6,<6.0.0)
 Requires-Dist: Werkzeug (>=2.0.3)
 Requires-Dist: flask-apispec (>=0.11.0,<0.12.0)
 Requires-Dist: gevent (>=22.10.2,<23.0.0)
 Requires-Dist: gevent-websocket (>=0.10.1,<0.11.0)
 Requires-Dist: marshmallow-enum (>=1.5.1,<2.0.0)
+Requires-Dist: marshmallow-jsonapi (>=0.24.0,<0.25.0)
 Requires-Dist: pickleDB (>=0.9.2,<0.10.0)
 Requires-Dist: pyzmq (>=25.1.1,<26.0.0)
 Requires-Dist: runstats (>=2.0.0,<3.0.0)
 Requires-Dist: socketio-client (>=0.7.2,<0.8.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Project-URL: Repository, https://github.com/Openfabric/openfabic-pysdk
 Description-Content-Type: text/markdown
```

