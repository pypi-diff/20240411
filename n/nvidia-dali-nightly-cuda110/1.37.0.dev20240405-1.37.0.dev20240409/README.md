# Comparing `tmp/nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar.gz` & `tmp/nvidia_dali_nightly_cuda110-1.37.0.dev20240409.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda110-1.37.0.dev20240409.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda110-1.37.0.dev20240405.tar` & `nvidia_dali_nightly_cuda110-1.37.0.dev20240409.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda110
-Version: 1.37.0.dev20240405
-Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: d28d6cbfc665781c5f3ab4ba28602374c48da31b
+Version: 1.37.0.dev20240409
+Summary: NVIDIA DALI nightly  for CUDA 11.0. Git SHA: fb5786c82c162af3f2120e8ab8cbb8d5d5cdbf12
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

