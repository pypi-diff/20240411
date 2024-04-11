# Comparing `tmp/aws-parallelcluster-3.9.0.tar.gz` & `tmp/aws-parallelcluster-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-3.9.0.tar", last modified: Tue Mar 12 01:17:41 2024, max compression
+gzip compressed data, was "aws-parallelcluster-3.9.1.tar", last modified: Thu Apr 11 10:38:43 2024, max compression
```

## Comparing `aws-parallelcluster-3.9.0.tar` & `aws-parallelcluster-3.9.1.tar`

### file list

```diff
@@ -1,272 +1,272 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.649145 aws-parallelcluster-3.9.0/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      114 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/MANIFEST.in
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2003 2024-03-12 01:17:41.649145 aws-parallelcluster-3.9.0/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      787 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/README
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2024-03-12 01:17:41.649145 aws-parallelcluster-3.9.0/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.605145 aws-parallelcluster-3.9.0/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.605145 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2003 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10956 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      147 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      659 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       36 2024-03-12 01:17:41.000000 aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.605145 aws-parallelcluster-3.9.0/src/pcluster/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.609145 aws-parallelcluster-3.9.0/src/pcluster/api/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.609145 aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2643 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11260 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/serverless_wsgi.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.609145 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      548 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4019 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4326 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_instances_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7167 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20246 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7697 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6289 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/image_logs_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15354 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/controllers/image_operations_controller.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4218 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/converters.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1536 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/encoder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5812 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/errors.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7657 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/flask_app.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.621145 aws-parallelcluster-3.9.0/src/pcluster/api/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6251 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4682 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2128 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2428 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/base_model_.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3757 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3652 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3639 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/change.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1717 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cloud_formation_resource_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1775 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cloud_formation_stack_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2103 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9207 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8637 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1879 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1630 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4053 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/config_validation_message.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/conflict_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3813 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3875 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3751 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/delete_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2220 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/delete_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3397 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_cluster_instances_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18397 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3802 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19464 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_image_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4859 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/dryrun_operation_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6209 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_info.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2185 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1488 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6566 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_instance.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2451 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/failure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3660 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/get_cluster_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2791 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/get_cluster_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/get_image_log_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2759 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/get_image_stack_events_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1576 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/image_build_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1678 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/image_builder_image_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2053 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/image_configuration_structure.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8609 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/image_info_summary.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1615 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/image_status_filtering_option.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1484 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/instance_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2183 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/internal_service_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2161 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/limit_exceeded_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3024 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/list_cluster_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3200 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/list_clusters_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2992 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/list_image_log_streams_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3108 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/list_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2315 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/list_official_images_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2373 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/log_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8592 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/log_stream.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5231 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/login_nodes_pool.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1537 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/login_nodes_state.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2418 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/metadata.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1376 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/node_type.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/not_found_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1532 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/requested_compute_fleet_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/scheduler.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12343 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/stack_event.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2286 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/tag.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2172 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/unauthorized_client_error_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6155 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2594 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4944 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2377 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_compute_fleet_request_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3274 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_compute_fleet_response_content.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4087 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/update_error.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1394 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/models/validation_level.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.621145 aws-parallelcluster-3.9.0/src/pcluster/api/openapi/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/openapi/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   115718 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/openapi/openapi.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1388 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/typing_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8594 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/api/util.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.625145 aws-parallelcluster-3.9.0/src/pcluster/aws/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6159 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/aws_api.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    21932 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/aws_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5430 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/batch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7832 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/cfn.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8514 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2234 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/dynamo.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    24218 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/ec2.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3313 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/efs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2879 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/elb.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5416 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/fsx.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1351 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/iam.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      949 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      907 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/kms.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5687 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1801 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/resource_groups.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2097 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/route53.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7491 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/s3.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/s3_resource.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1369 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/secretsmanager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1003 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/ssm.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      959 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/aws/sts.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.629145 aws-parallelcluster-3.9.0/src/pcluster/cli/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/__init__.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.629145 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4355 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/cluster_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      975 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5346 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/common.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.629145 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1477 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/command.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20483 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/easyconfig.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10146 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/networking.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5959 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/subnet_computation.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8376 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6742 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/dcv_connect.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      911 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/dcv_util.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3571 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/image_logs.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3972 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/ssh.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1434 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/commands/version.py
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)    11370 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/entrypoint.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1116 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/exceptions.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3002 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4586 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/middleware.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7730 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/cli/model.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.633145 aws-parallelcluster-3.9.0/src/pcluster/config/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)   134626 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/cluster_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17316 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13054 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/config_patch.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12720 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/imagebuilder_config.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    29091 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/update_policy.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1186 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/config/update_policy_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12553 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/constants.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2624 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/imagebuilder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2574 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/launch_template_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.633145 aws-parallelcluster-3.9.0/src/pcluster/lib/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      963 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/lib/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3558 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/lib/lib.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.633145 aws-parallelcluster-3.9.0/src/pcluster/models/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51878 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/cluster.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12259 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/cluster_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13929 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12565 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/compute_fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    35259 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/imagebuilder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5037 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/imagebuilder_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6294 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/login_nodes_status.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16902 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/models/s3_bucket.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.633145 aws-parallelcluster-3.9.0/src/pcluster/networking/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/networking/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3769 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/networking/vpc_factory.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.601145 aws-parallelcluster-3.9.0/src/pcluster/resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.601145 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.633145 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/alinux2/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1816 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/alinux2/Dockerfile
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1162 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/build-docker-images.sh
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      535 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/buildspec.yml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1573 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     5466 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1954 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2882 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2457 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
--rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)      879 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/upload-docker-images.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/compute_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7727 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/compute_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.601145 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7610 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10142 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       96 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)       81 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2701 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13195 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1842 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3545 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2763 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.637145 aws-parallelcluster-3.9.0/src/pcluster/resources/head_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6306 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/head_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.641146 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1919 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/custom_script.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11069 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9027 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6729 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16855 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13499 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.641146 aws-parallelcluster-3.9.0/src/pcluster/resources/login_node/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7686 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/resources/login_node/user_data.sh
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.641146 aws-parallelcluster-3.9.0/src/pcluster/schemas/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/schemas/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    76502 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/schemas/cluster_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11046 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/schemas/common_schema.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8453 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/schemas/imagebuilder_schema.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.645146 aws-parallelcluster-3.9.0/src/pcluster/templates/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    38701 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/awsbatch_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5999 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_artifacts_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3232 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    45548 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_builder_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    70801 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/cluster_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5926 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/compute_fleet_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    37794 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/cw_dashboard_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    44641 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/imagebuilder_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      682 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/import_cdk.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    22368 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/login_nodes_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    23692 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/queues_stack.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13602 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/templates/slurm_builder.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19631 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.649145 aws-parallelcluster-3.9.0/src/pcluster/validators/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8783 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/awsbatch_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    68488 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/cluster_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6601 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3528 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/database_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6757 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/directory_service_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12873 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/ebs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    32583 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/ec2_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1212 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/efs_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1202 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/feature_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9990 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/fsx_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4000 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/iam_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2361 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/imagebuilder_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    14335 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/instances_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1414 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/kms_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1858 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/monitoring_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9288 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/networking_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6760 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/s3_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3869 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/secret_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7463 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/slurm_settings_validator.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4081 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/tags_validators.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      825 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster/validators/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-03-12 01:17:41.649145 aws-parallelcluster-3.9.0/src/pcluster3_config_converter/
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster3_config_converter/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (2000)    53018 2024-03-11 21:02:55.000000 aws-parallelcluster-3.9.0/src/pcluster3_config_converter/pcluster3_config_converter.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.579415 aws-parallelcluster-3.9.1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      114 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2003 2024-04-11 10:38:43.579415 aws-parallelcluster-3.9.1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      787 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/README
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       38 2024-04-11 10:38:43.579415 aws-parallelcluster-3.9.1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.535415 aws-parallelcluster-3.9.1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.535415 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2003 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10956 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      147 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        1 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      659 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       36 2024-04-11 10:38:43.000000 aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.535415 aws-parallelcluster-3.9.1/src/pcluster/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.539415 aws-parallelcluster-3.9.1/src/pcluster/api/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.539415 aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2643 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11260 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/serverless_wsgi.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.539415 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      548 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4019 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4326 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_instances_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7167 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20246 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7697 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6289 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/image_logs_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    15354 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/controllers/image_operations_controller.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4218 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/converters.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1536 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/encoder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5812 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/errors.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7657 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/flask_app.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.551415 aws-parallelcluster-3.9.1/src/pcluster/api/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6251 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4682 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2128 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2428 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/base_model_.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3757 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3652 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3639 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/change.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1717 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cloud_formation_resource_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1775 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cloud_formation_stack_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2103 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9207 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8637 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1879 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1630 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4053 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/config_validation_message.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/conflict_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3813 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3875 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3751 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2302 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/delete_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2220 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/delete_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3397 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_cluster_instances_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    18397 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3802 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19464 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_image_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4859 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6209 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_info.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2185 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1488 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6566 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_instance.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2451 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/failure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3660 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/get_cluster_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2791 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3618 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/get_image_log_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2759 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/get_image_stack_events_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1576 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/image_build_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1678 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/image_builder_image_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2053 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/image_configuration_structure.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8609 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/image_info_summary.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1615 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/image_status_filtering_option.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1484 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/instance_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2183 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/internal_service_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2161 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3024 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3200 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/list_clusters_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2992 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/list_image_log_streams_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3108 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/list_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2315 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/list_official_images_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2373 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/log_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8592 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/log_stream.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5231 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/login_nodes_pool.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1537 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/login_nodes_state.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2418 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/metadata.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1376 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/node_type.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2106 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/not_found_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1532 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/requested_compute_fleet_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/scheduler.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12343 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/stack_event.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2286 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/tag.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2172 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/unauthorized_client_error_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6155 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2594 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4944 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2377 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_compute_fleet_request_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3274 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_compute_fleet_response_content.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4087 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/update_error.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1394 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/models/validation_level.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.555415 aws-parallelcluster-3.9.1/src/pcluster/api/openapi/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/openapi/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   115718 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/openapi/openapi.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1388 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/typing_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8594 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/api/util.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.559415 aws-parallelcluster-3.9.1/src/pcluster/aws/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6159 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/aws_api.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    21932 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/aws_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5430 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/batch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7832 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/cfn.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8514 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2234 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/dynamo.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    24218 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/ec2.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3313 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/efs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2879 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/elb.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5416 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/fsx.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1351 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/iam.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      949 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      907 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/kms.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5687 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1801 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/resource_groups.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2097 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/route53.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7491 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/s3.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2656 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/s3_resource.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1369 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/secretsmanager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1003 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/ssm.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      959 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/aws/sts.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.559415 aws-parallelcluster-3.9.1/src/pcluster/cli/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/__init__.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.559415 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4355 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/cluster_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      975 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5346 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/common.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.563415 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1477 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/command.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    20483 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/easyconfig.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10146 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/networking.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5959 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/subnet_computation.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8376 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6742 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/dcv_connect.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      911 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/dcv_util.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3571 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/image_logs.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3972 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/ssh.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1434 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/commands/version.py
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)    11370 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/entrypoint.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1116 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/exceptions.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3002 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4586 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/middleware.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7730 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/cli/model.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.563415 aws-parallelcluster-3.9.1/src/pcluster/config/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)   134626 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/cluster_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    17316 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13054 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/config_patch.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12720 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/imagebuilder_config.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    29091 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/update_policy.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1186 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/config/update_policy_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12553 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/constants.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2624 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/imagebuilder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2574 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/launch_template_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.563415 aws-parallelcluster-3.9.1/src/pcluster/lib/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      963 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/lib/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3558 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/lib/lib.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.563415 aws-parallelcluster-3.9.1/src/pcluster/models/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    51878 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/cluster.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12259 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/cluster_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13929 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12565 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/compute_fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    35259 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/imagebuilder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5037 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/imagebuilder_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6294 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/login_nodes_status.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16902 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/models/s3_bucket.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/networking/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      559 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/networking/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3769 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/networking/vpc_factory.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.535415 aws-parallelcluster-3.9.1/src/pcluster/resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.531415 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/alinux2/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1816 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1162 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/build-docker-images.sh
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      535 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/buildspec.yml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1573 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     5466 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     1954 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2882 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)     2457 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh
+-rwxr-xr-x   0 jenkins   (2000) jenkins   (2000)      879 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/upload-docker-images.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/compute_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7727 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/compute_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.535415 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7610 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.567415 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    10142 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       96 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/NOTICE
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)       81 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2701 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13195 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1842 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3545 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3369 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2763 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.571415 aws-parallelcluster-3.9.1/src/pcluster/resources/head_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6306 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/head_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.571415 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1919 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/custom_script.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11069 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9027 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6729 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    16855 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13499 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.571415 aws-parallelcluster-3.9.1/src/pcluster/resources/login_node/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7686 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/resources/login_node/user_data.sh
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.571415 aws-parallelcluster-3.9.1/src/pcluster/schemas/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/schemas/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    76502 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/schemas/cluster_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    11046 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/schemas/common_schema.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8453 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/schemas/imagebuilder_schema.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.575415 aws-parallelcluster-3.9.1/src/pcluster/templates/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    38701 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/awsbatch_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5999 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_artifacts_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3232 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    45548 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_builder_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    70801 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/cluster_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     5926 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/compute_fleet_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    37794 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/cw_dashboard_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    44641 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/imagebuilder_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      682 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/import_cdk.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    22368 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/login_nodes_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    23692 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/queues_stack.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    13602 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/templates/slurm_builder.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    19631 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.579415 aws-parallelcluster-3.9.1/src/pcluster/validators/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     8783 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/awsbatch_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    68488 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/cluster_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6601 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3528 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/database_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6757 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/directory_service_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    12873 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/ebs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    32583 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/ec2_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1212 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/efs_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1202 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/feature_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9990 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/fsx_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4000 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/iam_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     2361 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/imagebuilder_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    14335 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/instances_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1414 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/kms_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     1858 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/monitoring_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     9288 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/networking_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     6760 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/s3_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     3869 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/secret_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     7463 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/slurm_settings_validator.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)     4081 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/tags_validators.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      825 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster/validators/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (2000)        0 2024-04-11 10:38:43.579415 aws-parallelcluster-3.9.1/src/pcluster3_config_converter/
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)      554 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster3_config_converter/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (2000)    53018 2024-04-11 06:43:49.000000 aws-parallelcluster-3.9.1/src/pcluster3_config_converter/pcluster3_config_converter.py
```

### Comparing `aws-parallelcluster-3.9.0/PKG-INFO` & `aws-parallelcluster-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.9.0
+Version: 3.9.1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.9.0/README` & `aws-parallelcluster-3.9.1/README`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/setup.py` & `aws-parallelcluster-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def readme():
     """Read the README file and use it as long description."""
     with open(os.path.join(os.path.dirname(__file__), "README"), encoding="utf-8") as f:
         return f.read()
 
 
-VERSION = "3.9.0"
+VERSION = "3.9.1"
 CDK_VERSION = "1.164"
 REQUIRES = [
     "setuptools",
     "boto3>=1.16.14",
     "tabulate>=0.8.8,<=0.8.10",
     "PyYAML>=5.3.1,!=5.4",
     "jinja2~=3.0",
```

### Comparing `aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/PKG-INFO` & `aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster
-Version: 3.9.0
+Version: 3.9.1
 Summary: AWS ParallelCluster is an AWS supported Open Source cluster management tool to deploy and manage HPC clusters in the AWS cloud.
 Home-page: https://github.com/aws/aws-parallelcluster
 Author: Amazon Web Services
 License: Apache License 2.0
 Project-URL: Changelog, https://github.com/aws/aws-parallelcluster/blob/develop/CHANGELOG.md
 Project-URL: Issue Tracker, https://github.com/aws/aws-parallelcluster/issues
 Project-URL: Documentation, https://docs.aws.amazon.com/parallelcluster/
```

### Comparing `aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/SOURCES.txt` & `aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/aws_parallelcluster.egg-info/requires.txt` & `aws-parallelcluster-3.9.1/src/aws_parallelcluster.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/entrypoint.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/awslambda/serverless_wsgi.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/awslambda/serverless_wsgi.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_compute_fleet_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_compute_fleet_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_instances_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_instances_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_logs_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/cluster_operations_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/cluster_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/image_logs_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/image_logs_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/controllers/image_operations_controller.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/controllers/image_operations_controller.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/converters.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/converters.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/encoder.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/encoder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/errors.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/errors.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/flask_app.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/flask_app.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/ami_info.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/bad_request_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/base_model_.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_bad_request_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_request_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/build_image_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/build_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/change.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/change.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cloud_formation_resource_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cloud_formation_resource_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cloud_formation_stack_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cloud_formation_stack_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_configuration_structure.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_info_summary.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_instance.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/cluster_status_filtering_option.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/cluster_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/compute_fleet_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/config_validation_message.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/config_validation_message.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/conflict_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/conflict_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_request_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/create_cluster_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/create_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/delete_cluster_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/delete_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/delete_image_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/delete_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_cluster_instances_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_cluster_instances_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_cluster_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_compute_fleet_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/describe_image_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/describe_image_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/dryrun_operation_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/dryrun_operation_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_info.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_info.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_info_summary.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_ami_state.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_ami_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/ec2_instance.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/ec2_instance.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/failure.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/failure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/get_cluster_log_events_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/get_cluster_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/get_cluster_stack_events_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/get_cluster_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/get_image_log_events_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/get_image_log_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/get_image_stack_events_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/get_image_stack_events_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/image_build_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/image_build_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/image_builder_image_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/image_builder_image_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/image_configuration_structure.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/image_configuration_structure.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/image_info_summary.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/image_info_summary.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/image_status_filtering_option.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/image_status_filtering_option.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/instance_state.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/instance_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/internal_service_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/internal_service_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/limit_exceeded_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/limit_exceeded_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/list_cluster_log_streams_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/list_cluster_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/list_clusters_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/list_clusters_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/list_image_log_streams_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/list_image_log_streams_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/list_images_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/list_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/list_official_images_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/list_official_images_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/log_event.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/log_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/log_stream.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/log_stream.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/login_nodes_pool.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/login_nodes_pool.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/login_nodes_state.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/login_nodes_state.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/metadata.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/metadata.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/node_type.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/node_type.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/not_found_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/not_found_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/requested_compute_fleet_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/requested_compute_fleet_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/scheduler.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/scheduler.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/stack_event.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/stack_event.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/tag.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/tag.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/unauthorized_client_error_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/unauthorized_client_error_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_bad_request_exception_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_request_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_cluster_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_cluster_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_compute_fleet_request_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_compute_fleet_request_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_compute_fleet_response_content.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_compute_fleet_response_content.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/update_error.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/update_error.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/models/validation_level.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/models/validation_level.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/openapi/openapi.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/api/openapi/openapi.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 openapi: 3.0.2
 info:
   description: ParallelCluster API
   title: ParallelCluster
-  version: 3.9.0
+  version: 3.9.1
 servers:
 - url: /
 # override: auth is defined the the API GW level
 # security:
 # - aws.auth.sigv4: []
 paths:
   /v3/clusters:
```

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/typing_utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/typing_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/api/util.py` & `aws-parallelcluster-3.9.1/src/pcluster/api/util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/aws_api.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/aws_api.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/aws_resources.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/aws_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/batch.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/batch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/cfn.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/cfn.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/dynamo.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/dynamo.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/ec2.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/efs.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/efs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/elb.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/fsx.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/fsx.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/iam.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/iam.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/imagebuilder.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/kms.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/kms.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/logs.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/resource_groups.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/resource_groups.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/route53.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/route53.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/s3.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/s3.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/s3_resource.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/s3_resource.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/secretsmanager.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/ssm.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/aws/sts.py` & `aws-parallelcluster-3.9.1/src/pcluster/aws/sts.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/cluster_logs.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/commands.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/command.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/command.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/easyconfig.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/easyconfig.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/networking.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/networking.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/subnet_computation.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/subnet_computation.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/configure/utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/configure/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/dcv_connect.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/dcv_connect.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/dcv_util.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/dcv_util.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/image_logs.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/image_logs.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/ssh.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/ssh.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/commands/version.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/entrypoint.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/exceptions.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/logger.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/middleware.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/middleware.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/cli/model.py` & `aws-parallelcluster-3.9.1/src/pcluster/cli/model.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/cluster_config.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/cluster_config.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/config_patch.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/config_patch.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/imagebuilder_config.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/imagebuilder_config.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/update_policy.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/update_policy.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/config/update_policy_utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/config/update_policy_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/constants.py` & `aws-parallelcluster-3.9.1/src/pcluster/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,16 @@
 MIN_MEMORY_PRECENTAGE_DIFFERENCE = 0.20
 
 MAX_EBS_COUNT = 5
 MAX_NEW_STORAGE_COUNT = {"efs": 1, "fsx": 1, "raid": 1}
 MAX_EXISTING_STORAGE_COUNT = {"efs": 20, "fsx": 20, "raid": 0}
 
 COOKBOOK_PACKAGES_VERSIONS = {
-    "parallelcluster": "3.9.0",
-    "cookbook": "aws-parallelcluster-cookbook-3.9.0",
+    "parallelcluster": "3.9.1",
+    "cookbook": "aws-parallelcluster-cookbook-3.9.1",
     "chef": "18.2.7",
     "berkshelf": "8.0.7",
     "ami": "dev",
 }
 
 CW_DASHBOARD_ENABLED_DEFAULT = True
 CW_ALARMS_ENABLED_DEFAULT = True
```

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/imagebuilder_utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/imagebuilder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/launch_template_utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/launch_template_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/lib/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/lib/lib.py` & `aws-parallelcluster-3.9.1/src/pcluster/lib/lib.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/cluster.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/cluster.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/cluster_resources.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/cluster_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/compute_fleet_status_manager.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/compute_fleet_status_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/imagebuilder.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/imagebuilder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/imagebuilder_resources.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/imagebuilder_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/login_nodes_status.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/login_nodes_status.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/models/s3_bucket.py` & `aws-parallelcluster-3.9.1/src/pcluster/models/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/networking/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/networking/vpc_factory.py` & `aws-parallelcluster-3.9.1/src/pcluster/networking/vpc_factory.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/alinux2/Dockerfile` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/alinux2/Dockerfile`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/build-docker-images.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/build-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/buildspec.yml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/buildspec.yml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/entrypoint.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/generate_hostfile.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/modify_yum_vars.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/mount_efs.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/mount_efs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/scripts/mount_nfs.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/batch/docker/upload-docker-images.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/batch/docker/upload-docker-images.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/compute_node/user_data.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/compute_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/cleanup_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/log_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/resource_helper.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/crhelper/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/delete_image_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/manage_docker_images.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py` & `aws-parallelcluster-3.9.1/src/pcluster/resources/custom_resources/custom_resources_code/send_build_notification.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/head_node/user_data.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/head_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/custom_script.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/custom_script.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_tag.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_test.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/parallelcluster_validate.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/imagebuilder/update_and_reboot.yaml` & `aws-parallelcluster-3.9.1/src/pcluster/resources/imagebuilder/update_and_reboot.yaml`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/resources/login_node/user_data.sh` & `aws-parallelcluster-3.9.1/src/pcluster/resources/login_node/user_data.sh`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/schemas/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/schemas/cluster_schema.py` & `aws-parallelcluster-3.9.1/src/pcluster/schemas/cluster_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/schemas/common_schema.py` & `aws-parallelcluster-3.9.1/src/pcluster/schemas/common_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/schemas/imagebuilder_schema.py` & `aws-parallelcluster-3.9.1/src/pcluster/schemas/imagebuilder_schema.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/awsbatch_builder.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/awsbatch_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_artifacts_manager.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_artifacts_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_builder.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/cdk_builder_utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/cdk_builder_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/cluster_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/cluster_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/compute_fleet_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/compute_fleet_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/cw_dashboard_builder.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/cw_dashboard_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/imagebuilder_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/imagebuilder_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/import_cdk.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/import_cdk.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/login_nodes_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/login_nodes_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/queues_stack.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/queues_stack.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/templates/slurm_builder.py` & `aws-parallelcluster-3.9.1/src/pcluster/templates/slurm_builder.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/awsbatch_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/awsbatch_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/cluster_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/cluster_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/common.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/database_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/database_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/directory_service_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/directory_service_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/ebs_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/ebs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/ec2_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/ec2_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/efs_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/efs_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/feature_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/feature_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/fsx_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/fsx_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/iam_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/iam_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/imagebuilder_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/imagebuilder_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/instances_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/instances_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/kms_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/kms_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/monitoring_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/monitoring_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/networking_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/networking_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/s3_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/s3_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/secret_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/secret_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/slurm_settings_validator.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/slurm_settings_validator.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/tags_validators.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/tags_validators.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster/validators/utils.py` & `aws-parallelcluster-3.9.1/src/pcluster/validators/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster3_config_converter/__init__.py` & `aws-parallelcluster-3.9.1/src/pcluster3_config_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-3.9.0/src/pcluster3_config_converter/pcluster3_config_converter.py` & `aws-parallelcluster-3.9.1/src/pcluster3_config_converter/pcluster3_config_converter.py`

 * *Files identical despite different names*

