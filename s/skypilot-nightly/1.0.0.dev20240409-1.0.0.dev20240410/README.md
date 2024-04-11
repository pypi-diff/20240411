# Comparing `tmp/skypilot-nightly-1.0.0.dev20240409.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20240409.tar", last modified: Tue Apr  9 10:40:33 2024, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20240410.tar", last modified: Wed Apr 10 10:40:35 2024, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20240409.tar` & `skypilot-nightly-1.0.0.dev20240410.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.982278 skypilot-nightly-1.0.0.dev20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-09 10:40:28.000000 skypilot-nightly-1.0.0.dev20240409/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-09 10:40:33.982278 skypilot-nightly-1.0.0.dev20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-04-09 10:40:28.000000 skypilot-nightly-1.0.0.dev20240409/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 10:40:33.982278 skypilot-nightly-1.0.0.dev20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-09 10:40:31.000000 skypilot-nightly-1.0.0.dev20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.918277 skypilot-nightly-1.0.0.dev20240409/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.918277 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.922278 skypilot-nightly-1.0.0.dev20240409/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.922278 skypilot-nightly-1.0.0.dev20240409/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.922278 skypilot-nightly-1.0.0.dev20240409/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   186851 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.926277 skypilot-nightly-1.0.0.dev20240409/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    30942 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46892 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.930277 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.930277 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.930277 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    39960 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.934278 skypilot-nightly-1.0.0.dev20240409/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31094 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.934278 skypilot-nightly-1.0.0.dev20240409/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.934278 skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.934278 skypilot-nightly-1.0.0.dev20240409/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.938278 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.938278 skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.938278 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.938278 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52429 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.942278 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.942278 skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.942278 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.946277 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.946277 skypilot-nightly-1.0.0.dev20240409/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.946277 skypilot-nightly-1.0.0.dev20240409/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-09 10:40:31.000000 skypilot-nightly-1.0.0.dev20240409/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.950278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.950278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.950278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.954278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.954278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.954278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.954278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.954278 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.958278 skypilot-nightly-1.0.0.dev20240409/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.958278 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.958278 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.958278 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.962278 skypilot-nightly-1.0.0.dev20240409/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/spot-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.962278 skypilot-nightly-1.0.0.dev20240409/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.966278 skypilot-nightly-1.0.0.dev20240409/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.966278 skypilot-nightly-1.0.0.dev20240409/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.966278 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.970278 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-09 10:40:33.000000 skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 10:40:33.970278 skypilot-nightly-1.0.0.dev20240409/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   211200 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_spot_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-09 10:40:29.000000 skypilot-nightly-1.0.0.dev20240409/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.614659 skypilot-nightly-1.0.0.dev20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-10 10:40:35.614659 skypilot-nightly-1.0.0.dev20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 10:40:35.614659 skypilot-nightly-1.0.0.dev20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-10 10:40:32.000000 skypilot-nightly-1.0.0.dev20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.546659 skypilot-nightly-1.0.0.dev20240410/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.550659 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.550659 skypilot-nightly-1.0.0.dev20240410/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.550659 skypilot-nightly-1.0.0.dev20240410/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.554659 skypilot-nightly-1.0.0.dev20240410/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186851 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.554659 skypilot-nightly-1.0.0.dev20240410/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30942 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46892 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.558659 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.558659 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.562659 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39960 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.562659 skypilot-nightly-1.0.0.dev20240410/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31094 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.562659 skypilot-nightly-1.0.0.dev20240410/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.566659 skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.566659 skypilot-nightly-1.0.0.dev20240410/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.566659 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.566659 skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.566659 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.570659 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52429 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.570659 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.570659 skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.570659 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.574659 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.578659 skypilot-nightly-1.0.0.dev20240410/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.578659 skypilot-nightly-1.0.0.dev20240410/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-10 10:40:32.000000 skypilot-nightly-1.0.0.dev20240410/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.578659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.578659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.582659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.582659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.582659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.582659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.582659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.586659 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.586659 skypilot-nightly-1.0.0.dev20240410/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.586659 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.586659 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.586659 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.590659 skypilot-nightly-1.0.0.dev20240410/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/spot-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.590659 skypilot-nightly-1.0.0.dev20240410/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.594659 skypilot-nightly-1.0.0.dev20240410/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.594659 skypilot-nightly-1.0.0.dev20240410/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.598659 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.602659 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-10 10:40:35.000000 skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 10:40:35.602659 skypilot-nightly-1.0.0.dev20240410/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211200 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_spot_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-10 10:40:29.000000 skypilot-nightly-1.0.0.dev20240410/tests/test_yaml_parser.py
```

### Comparing `skypilot-nightly-1.0.0.dev20240409/LICENSE` & `skypilot-nightly-1.0.0.dev20240410/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20240410/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/PKG-INFO` & `skypilot-nightly-1.0.0.dev20240410/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240409
+Version: 1.0.0.dev20240410
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot-nightly-1.0.0.dev20240409/README.md` & `skypilot-nightly-1.0.0.dev20240410/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/pyproject.toml` & `skypilot-nightly-1.0.0.dev20240410/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/setup.py` & `skypilot-nightly-1.0.0.dev20240410/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240409'
+__version__ = '1.0.0.dev20240410'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/common.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/kubernetes.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/adaptors/vsphere.py` & `skypilot-nightly-1.0.0.dev20240410/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20240410/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20240410/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/check.py` & `skypilot-nightly-1.0.0.dev20240410/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/cli.py` & `skypilot-nightly-1.0.0.dev20240410/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20240410/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/cloud_registry.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/cudo.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/fluidstack.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/kubernetes.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/paperspace.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/runpod.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/gcp_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/oci_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/utils/scp_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/clouds/vsphere.py` & `skypilot-nightly-1.0.0.dev20240410/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/core.py` & `skypilot-nightly-1.0.0.dev20240410/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/dag.py` & `skypilot-nightly-1.0.0.dev20240410/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20240410/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20240410/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20240410/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/execution.py` & `skypilot-nightly-1.0.0.dev20240410/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20240410/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20240410/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/aws/utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/azure/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/common.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/cudo_machine_type.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/cudo_wrapper.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/cudo/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/docker_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/fluidstack/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/instance_setup.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/network.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/network_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/kubernetes/utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/logging.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/metadata_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/paperspace/utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/provisioner.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/runpod/utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/cls_api_client.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/metadata_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/service_manager.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/ssl_helper.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/vapiconnect.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/common/vim_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/instance.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/provision/vsphere/vsphere_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/resources.py` & `skypilot-nightly-1.0.0.dev20240410/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/autoscalers.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/controller.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/core.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/load_balancer.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/load_balancing_policies.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/replica_managers.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/serve_state.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/serve_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/service.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/serve/service_spec.py` & `skypilot-nightly-1.0.0.dev20240410/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20240410/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20240410/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20240410/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/log_lib.pyi` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/command_runner.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20240410/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/task.py` & `skypilot-nightly-1.0.0.dev20240410/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/cudo-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/fluidstack-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ingress.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/paperspace-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/runpod-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/sky-serve-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/templates/vsphere-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240410/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20240410/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20240410/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/cluster_yaml_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/command_runner.pyi` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/controller_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/create_cluster.sh` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/delete_cluster.sh` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/generate_kind_config.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/gpu_labeler.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/kubernetes_enums.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/resources_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/rich_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20240410/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240409
+Version: 1.0.0.dev20240410
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20240410/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_serve_autoscaler.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_spot_serve.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_spot_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240409/tests/test_yaml_parser.py` & `skypilot-nightly-1.0.0.dev20240410/tests/test_yaml_parser.py`

 * *Files identical despite different names*

