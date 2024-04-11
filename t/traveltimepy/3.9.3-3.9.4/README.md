# Comparing `tmp/traveltimepy-3.9.3.tar.gz` & `tmp/traveltimepy-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traveltimepy-3.9.3.tar", last modified: Mon Mar  4 18:20:07 2024, max compression
+gzip compressed data, was "traveltimepy-3.9.4.tar", last modified: Thu Apr 11 15:45:25 2024, max compression
```

## Comparing `traveltimepy-3.9.3.tar` & `traveltimepy-3.9.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.221625 traveltimepy-3.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-03-04 18:20:07.221625 traveltimepy-3.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29216 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.213625 traveltimepy-3.9.3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/benchmarks/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/benchmarks/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/benchmarks/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-04 18:20:07.225625 traveltimepy-3.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.213625 traveltimepy-3.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/geocoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/map_info_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/postcodes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/routes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/time_filter_fast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/time_filter_proto_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/time_filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/time_map_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/wkt_parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/wkt_pretty_print_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/tests/wkt_validate_objects_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.217625 traveltimepy-3.9.3/traveltimepy/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-03-04 18:19:45.000000 traveltimepy-3.9.3/traveltimepy/TimeFilterFastRequest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-04 18:19:45.000000 traveltimepy-3.9.3/traveltimepy/TimeFilterFastResponse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/accept_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.217625 traveltimepy-3.9.3/traveltimepy/dto/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.221625 traveltimepy-3.9.3/traveltimepy/dto/requests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/postcodes_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_map_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/requests/time_map_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.221625 traveltimepy-3.9.3/traveltimepy/dto/responses/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/map_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/time_map_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/responses/zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/dto/transportation.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)    24873 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/proto_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    20368 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.221625 traveltimepy-3.9.3/traveltimepy/wkt/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/geometries.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-03-04 18:19:41.000000 traveltimepy-3.9.3/traveltimepy/wkt/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 18:20:07.217625 traveltimepy-3.9.3/traveltimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-04 18:20:07.000000 traveltimepy-3.9.3/traveltimepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29216 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.013324 traveltimepy-3.9.4/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/benchmarks/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.013324 traveltimepy-3.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/geocoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/map_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/postcodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/routes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_fast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_proto_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/time_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_pretty_print_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/tests/wkt_validate_objects_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-11 15:45:16.000000 traveltimepy-3.9.4/traveltimepy/TimeFilterFastRequest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-11 15:45:16.000000 traveltimepy-3.9.4/traveltimepy/TimeFilterFastResponse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/accept_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy/dto/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/traveltimepy/dto/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/time_map_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/responses/zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/dto/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24873 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/proto_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20368 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.021324 traveltimepy-3.9.4/traveltimepy/wkt/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-11 15:45:12.000000 traveltimepy-3.9.4/traveltimepy/wkt/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:45:25.017324 traveltimepy-3.9.4/traveltimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 15:45:24.000000 traveltimepy-3.9.4/traveltimepy.egg-info/top_level.txt
```

### Comparing `traveltimepy-3.9.3/LICENSE` & `traveltimepy-3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/PKG-INFO` & `traveltimepy-3.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.3
+Version: 3.9.4
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `traveltimepy-3.9.3/README.md` & `traveltimepy-3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/benchmarks/common.py` & `traveltimepy-3.9.4/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/benchmarks/time_filter.py` & `traveltimepy-3.9.4/benchmarks/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/benchmarks/time_filter_fast.py` & `traveltimepy-3.9.4/benchmarks/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/benchmarks/time_map.py` & `traveltimepy-3.9.4/benchmarks/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/setup.cfg` & `traveltimepy-3.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/conftest.py` & `traveltimepy-3.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/postcodes_test.py` & `traveltimepy-3.9.4/tests/postcodes_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/routes_test.py` & `traveltimepy-3.9.4/tests/routes_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/supported_locations.py` & `traveltimepy-3.9.4/tests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/time_filter_fast_test.py` & `traveltimepy-3.9.4/tests/time_filter_fast_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/time_filter_proto_test.py` & `traveltimepy-3.9.4/tests/time_filter_proto_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/time_filter_test.py` & `traveltimepy-3.9.4/tests/time_filter_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/time_map_test.py` & `traveltimepy-3.9.4/tests/time_map_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/wkt_parsing_test.py` & `traveltimepy-3.9.4/tests/wkt_parsing_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/wkt_pretty_print_test.py` & `traveltimepy-3.9.4/tests/wkt_pretty_print_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/tests/wkt_validate_objects_test.py` & `traveltimepy-3.9.4/tests/wkt_validate_objects_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/TimeFilterFastRequest_pb2.py` & `traveltimepy-3.9.4/traveltimepy/TimeFilterFastRequest_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/TimeFilterFastResponse_pb2.py` & `traveltimepy-3.9.4/traveltimepy/TimeFilterFastResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/__init__.py` & `traveltimepy-3.9.4/traveltimepy/__init__.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/common.py` & `traveltimepy-3.9.4/traveltimepy/dto/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/postcodes.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/postcodes_zones.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/postcodes_zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/routes.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/supported_locations.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter_fast.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_filter_proto.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_filter_proto.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_map.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_map_geojson.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_geojson.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/requests/time_map_wkt.py` & `traveltimepy-3.9.4/traveltimepy/dto/requests/time_map_wkt.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/responses/routes.py` & `traveltimepy-3.9.4/traveltimepy/dto/responses/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/responses/time_filter.py` & `traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/responses/time_filter_fast.py` & `traveltimepy-3.9.4/traveltimepy/dto/responses/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/responses/time_map_wkt.py` & `traveltimepy-3.9.4/traveltimepy/dto/responses/time_map_wkt.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/responses/zones.py` & `traveltimepy-3.9.4/traveltimepy/dto/responses/zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/dto/transportation.py` & `traveltimepy-3.9.4/traveltimepy/dto/transportation.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/http.py` & `traveltimepy-3.9.4/traveltimepy/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                 return await _process_response(response_class, resp)
 
 
 async def _process_response(response_class: Type[T], response: ClientResponse) -> T:
     text = await response.text()
     json_data = json.loads(text)
     if response.status != 200:
-        parsed = ResponseError.model_validate_json(json_data)
+        parsed = ResponseError.model_validate_json(json.dumps(json_data))
         msg = (
             f"Travel Time API request failed: {parsed.description}\n"
             f"Error code: {parsed.error_code}\n"
             f"Additional info: {parsed.additional_info}\n"
             f"<{parsed.documentation_link}>\n"
         )
         raise ApiError(msg)
```

### Comparing `traveltimepy-3.9.3/traveltimepy/itertools.py` & `traveltimepy-3.9.4/traveltimepy/itertools.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/mapper.py` & `traveltimepy-3.9.4/traveltimepy/mapper.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/proto_http.py` & `traveltimepy-3.9.4/traveltimepy/proto_http.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/sdk.py` & `traveltimepy-3.9.4/traveltimepy/sdk.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/wkt/error.py` & `traveltimepy-3.9.4/traveltimepy/wkt/error.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/wkt/geometries.py` & `traveltimepy-3.9.4/traveltimepy/wkt/geometries.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy/wkt/parsing.py` & `traveltimepy-3.9.4/traveltimepy/wkt/parsing.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.3/traveltimepy.egg-info/PKG-INFO` & `traveltimepy-3.9.4/traveltimepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.3
+Version: 3.9.4
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `traveltimepy-3.9.3/traveltimepy.egg-info/SOURCES.txt` & `traveltimepy-3.9.4/traveltimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

